---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Document Webhooks-API
description: Document Webhooks-API
author: Becky
feature: Workfront API
role: Developer
exl-id: 7ac2c6c8-1cb8-49df-8d63-a6b47ad02a13
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '3620'
ht-degree: 2%

---


# Document Webhooks-API

Adobe Workfront Document Webhooks definiert einen Satz von API-Endpunkten, über die Workfront autorisierte API-Aufrufe an einen externen Dokumentanbieter sendet. Dadurch kann jeder ein Middleware-Plug-in für einen beliebigen Dokumentspeicheranbieter erstellen.

Das Benutzererlebnis bei Webhook-basierten Integrationen ähnelt dem von vorhandenen Dokumentenintegrationen, z. B. Google Drive, Box und Dropbox. Beispielsweise kann ein Workfront-Benutzer die folgenden Aktionen ausführen:

* Navigieren in der Ordnerstruktur des externen Dokumentanbieters
* Dateien durchsuchen
* Verknüpfen von Dateien mit Workfront
* Hochladen von Dateien in den externen Dokumentanbieter
* Anzeigen einer Miniaturansicht für das Dokument

## Referenzimplementierung

Um die Entwicklung einer neuen Webhooks-Implementierung zu beschleunigen, stellt Workfront eine Referenzimplementierung bereit. Code dafür finden Sie unter [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). Diese Implementierung basiert auf Java und ermöglicht es Workfront, Dokumente in einem Netzwerk-Dateisystem zu verbinden.

## Registrieren von Webhook-Integrationen

Workfront-Administratoren können eine benutzerdefinierte Webhook-Integration für ihr Unternehmen hinzufügen, indem sie in Workfront zu Einrichtung > Dokumente > Benutzerdefinierte Integrationen navigieren. Auf der Seite „Benutzerdefinierte Integration“ im Setup können Admins eine Liste der vorhandenen Dokument-Webhook-Integrationen anzeigen. Auf dieser Seite können Integrationen hinzugefügt, bearbeitet, aktiviert und deaktiviert werden. Um eine Integration hinzuzufügen, klicken Sie auf die Schaltfläche Integration hinzufügen .

### Verfügbare Felder

Beim Hinzufügen einer Integration gibt der Administrator Werte für die folgenden Felder ein:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Feldname</th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Name</td> 
   <td>Der Name dieser Integration.</td> 
  </tr> 
  <tr> 
   <td>Basis-API-URL</td> 
   <td> <p>Der Speicherort der Callback-API. Wenn Sie das externe System aufrufen, hängt Workfront einfach den Endpunktnamen an diese Adresse an. Wenn der Administrator beispielsweise die Basis-API-URL https://www.mycompany.com/api/v1 eingegeben hat, ruft Workfront die Metadaten eines Dokuments über die folgende URL ab: https://www.mycompany.com/api/v1/metadata?id=1234.</p> </td> 
  </tr> 
  <tr> 
   <td>Anfrageparameter</td> 
   <td> <p>Optionale Werte, die an die Abfragezeichenfolge eines jeden API-Aufrufs anzuhängen sind. Beispiel: access_type=offline.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Authentifizierungstyp</td> 
   <td>OAuth2 oder API-Schlüssel</td> 
  </tr> 
  <tr> 
   <td>Authentifizierungs-URL</td> 
   <td> <p>(Nur OAuth2) Die vollständige URL, die für die Benutzerauthentifizierung verwendet wird. Workfront führt Benutzer im Rahmen des OAuth-Bereitstellungsprozesses zu dieser Adresse. Hinweis: Workfront hängt einen „state“-Parameter an die Abfragezeichenfolge an. Der Anbieter muss dies zurück an Workfront übergeben, indem er es an den Workfront-Umleitungs-URI anhängt.</p> </td> 
  </tr> 
  <tr> 
   <td>Token Endpoint URL</td> 
   <td> <p>(Nur OAuth2) Die vollständige API-URL, die zum Abrufen von OAuth2-Token verwendet wird. Dies wird vom Webhook-Anbieter oder externen Dokumentanbieter gehostet</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Client-ID</td> 
   <td>(Nur OAuth2) Die OAuth2-Client-ID für diese Integration</td> 
  </tr> 
  <tr> 
   <td>Geheimer Client-Schlüssel</td> 
   <td> <p>(Nur OAuth2) Der geheime OAuth2-Client-Schlüssel für diese Integration</p> </td> 
  </tr> 
  <tr> 
   <td>Workfront Redirect-URI</td> 
   <td>  <p>(Nur OAuth2) Dies ist ein schreibgeschütztes Feld, das von Workfront generiert wird. Dieser Wert wird verwendet, um diese Integration beim externen Dokumentanbieter zu registrieren. Hinweis: Wie oben für die Authentifizierungs-URL beschrieben, muss der Anbieter den Parameter „state“ und dessen Wert an die Abfragezeichenfolge anhängen, wenn er die Umleitung durchführt.</p></td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td>  <p>(Nur API-Schlüssel) Wird verwendet, um autorisierte API-Aufrufe an den Webhook-Anbieter durchzuführen. Der vom Webhook-Anbieter ausgegebene API-Schlüssel.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## Authentifizierung

Workfront-Dokument-Webhooks unterstützen zwei verschiedene Authentifizierungsformen: OAuth2 und ApiKey. In beiden Fällen übergibt Workfront bei einem API-Aufruf Authentifizierungs-Token in der -Kopfzeile.

### OAuth2

Mit OAuth2 kann Workfront im Namen eines Benutzers autorisierte API-Aufrufe an einen Webhook-Anbieter durchführen. Zuvor muss der Benutzer sein externes Dokumentenanbieterkonto mit Workfront verbinden und Workfront gewähren

Zugang zu Handlungen in ihrem Namen. Dieser Handshaking-Vorgang erfolgt für jeden Benutzer nur einmal. So funktioniert es:

1. Der Benutzer beginnt mit dem Verbinden der Webhook-Integration mit seinem Konto. Klicken Sie dazu auf das Dropdown-Menü „Dokument hinzufügen“ > „Service hinzufügen“ > „Name der benutzerdefinierten Integration“.
1. Workfront verwendet die Authentifizierungs-URL, wodurch der Benutzer möglicherweise aufgefordert wird, sich beim externen Dokumentanbieter anzumelden. Diese Seite wird vom Webhook-Anbieter oder dem externen Document Management-System gehostet. Dabei fügt Workfront der Authentifizierungs-URL einen Parameter „state“ hinzu. Dieser Wert muss zurück an Workfront übergeben werden, indem im folgenden Schritt derselbe Wert an den Workfront-Rückgabe-URI angehängt wird.
1. Nach der Anmeldung beim externen System (oder wenn der Benutzer bereits angemeldet ist) wird der Benutzer zu einer Seite „Authentifizierung“ weitergeleitet, auf der erklärt wird, dass Workfront Zugriff anfordert, um eine Reihe von Aktionen im Namen des Benutzers auszuführen.
1. Wenn der/die Benutzende auf die Schaltfläche „Zulassen“ klickt, wird der Browser zum Workfront-Umleitungs-URI weitergeleitet und der Abfragezeichenfolge wird „code=`<code>`&quot; hinzugefügt. Gemäß der OAuth2-Spezifikation ist dieses Token kurzlebig. Die Abfragezeichenfolge muss außerdem Folgendes enthalten: „state=`<sent_by_workfront>`&quot;.
1. Workfront verarbeitet diese Anfrage und führt einen API-Aufruf an die Token-Endpunkt-URL mit dem Autorisierungs-Code durch.
1. Die Token-Endpunkt-URL gibt ein Aktualisierungs-Token und ein Zugriffs-Token zurück.
1. Workfront speichert diese Token und stellt die Webhook-Integration für diesen Benutzer bereit.
1. Ab diesem Zeitpunkt kann Workfront autorisierte API-Aufrufe an den Webhook-Anbieter durchführen. Bei diesen Aufrufen sendet Workfront das Zugriffstoken in der HTTP-Anfrage-Kopfzeile wie unten dargestellt:

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. Wenn das Zugriffstoken abgelaufen ist, führt Workfront einen Aufruf an die Token-Endpunkt-URL durch, um ein neues Zugriffstoken abzurufen, und versucht dann den autorisierten API-Aufruf mit dem neuen Zugriffstoken erneut.

### ApiKey

Die Durchführung autorisierter API-Aufrufe an einen Webhook-Anbieter mithilfe eines APIkeys ist viel einfacher als OAuth2. Wenn Sie einen API-Aufruf ausführen, übergibt Workfront einfach den API-Schlüssel und den Workfront-Benutzernamen in der HTTP-Anfrage-Kopfzeile:

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Der Webhook-Anbieter kann den Benutzernamen verwenden, um benutzerspezifische Berechtigungen anzuwenden. Dies funktioniert am besten, wenn beide Systeme über Single Sign-On (SSO) eine Verbindung zu LDAP herstellen.

### Hinzufügen von Anfrage-Headern (optional)

Zusätzlich zur Verwendung von OAuth2-Token oder eines API-Schlüssels zur Authentifizierung kann Workfront für jeden API-Aufruf einen vordefinierten Satz von Kopfzeilen an den Webhook-Anbieter senden. Ein Workfront-Administrator kann dies beim Registrieren oder Bearbeiten einer Webook-Integration einrichten, wie im obigen Abschnitt beschrieben. Siehe Registrieren einer Webhook-Integration.

Dies kann beispielsweise für die Standardauthentifizierung verwendet werden. Dazu fügt der Workfront-Administrator die folgenden Anfrage-Header-Informationen im Dialogfeld für die benutzerdefinierte Integration hinzu:

   Zulassung Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==

wobei QWxhZGRpbjpvcGVuIHNlc2FtZQ== eine base-64-kodierte Zeichenfolge von „username:password“ ist. Siehe Standardauthentifizierung . Sofern dies hinzugefügt wurde, übergibt Workfront dies zusätzlich zu anderen Anfrage-Headern in der HTTP-Anfrage-Kopfzeile:

```
­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------

apiKey: 12345

username: johndoe@foo.com

Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

## API-Spezifikation

Nachfolgend finden Sie eine Liste der APIs, die der Webhook-Anbieter implementieren sollte, damit Dokument-Webhooks funktionieren.

### Abrufen von OAuth2-Token (nur OAuth2-Authentifizierung erforderlich)

Gibt das OAuth2-Aktualisierungs-Token und Zugriffs-Token für einen authentifizierten Benutzer zurück. Dieser wird einmal aufgerufen, wenn der Benutzer einen Dokumentanbieter bereitstellt. Nachfolgende Aufrufe erfolgen, um ein aktualisiertes Zugriffstoken abzurufen.

HTTP-Anfrage-POST /any/url

Die URL ist konfigurierbar und entspricht dem Token-Endpunkt-URL-Wert auf der Seite „Benutzerdefiniertes Integrations-Setup“.

**Abfrageparameter**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Name</th> 
   <th>Erforderlich</th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>grant_type</td> 
   <td>Ja</td> 
   <td> <p>Die Werte umfassen „authorization_code“ oder „refresh_token“. Der angegebene Wert gibt an, welcher der beiden Parameter an diesen API-Aufruf übergeben wird: code oder refresh_token.</p> </td> 
  </tr> 
  <tr> 
   <td>Code</td> 
   <td>Depends</td> 
   <td> <p>Der Autorisierungs-Code wird an Workfront gesendet, unmittelbar nachdem der Benutzer auf die Schaltfläche „Gewähren“ geklickt hat. Dies ist nur erforderlich, wenn der Gewährungstyp „authorization_code“ ist. Der Autorisierungs-Code sollte kurzlebig sein und im Allgemeinen in 10 Minuten oder weniger ablaufen.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token</td> 
   <td>Depends</td> 
   <td> <p>Dies ist nur erforderlich, wenn nachfolgende Aufrufe zum Abrufen eines neuen Zugriffs-Tokens erfolgen, da das vorherige Zugriffs-Token abgelaufen ist. Wenn Sie diesen Wert senden, setzen Sie den Parameter grant_type auf „refresh_token“.</p> </td> 
  </tr> 
  <tr> 
   <td>client_id</td> 
   <td>Ja</td> 
   <td>Die in Workfront für diese benutzerdefinierte Integration konfigurierte Client-ID.</td> 
  </tr> 
  <tr> 
   <td>client_secret</td> 
   <td>Ja</td> 
   <td> Der in Workfront für diese benutzerdefinierte Integration konfigurierte geheime Clientschlüssel.</td> 
  </tr> 
 </tbody> 
</table>

 

**Antwort**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Name</th> 
   <th>Typ </th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>access_token </td> 
   <td>Zeichenfolge</td> 
   <td> <p>Ein Token, das verwendet wird, um autorisierte API-Aufrufe im Namen des Benutzers durchzuführen. Dieser sollte ablaufen, um nicht autorisierte API-Aufrufe zu verhindern.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token </td> 
   <td>Zeichenfolge</td> 
   <td> <p>Ein langlebiges Token, mit dem ein neues Zugriffs-Token abgerufen wird, indem diese API-Methode aufgerufen wird.</p> </td> 
  </tr> 
  <tr> 
   <td>expires_in </td> 
   <td>lang</td> 
   <td>  <p>(Optional) Die Zeit (in Sekunden), bevor das Zugriffs-Token abläuft, im Allgemeinen 3.600.</p></td> 
  </tr> 
 </tbody> 
</table>

 

**Beispiel**

```
POST /oauth2/token
grant_type=authorization_code
code=d9ac7asdf6asdf579d7a8
client_id=123456
client_secret=6asdf7a7a9a4af
```


**Antwort**

```
{
"access_token":"ad8af5ad5ads759", 
"refresh_token":"9a0h5d87d808ads", 
"expires_id":"3600" 
}
```

### Abrufen von Metadaten für Datei oder Ordner

Gibt Metadaten für die angegebene Datei oder den angegebenen Ordner zurück.

**URL**

GET /metadata?id=[document or folder ID]

**Abfrageparameter**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>-Name </th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>ID</td> 
   <td>  <p>Die ID der Datei oder des Ordners, auf die bzw. den der Webhook-Anbieter verweist. Dies unterscheidet sich von der Dokument-ID von Workfront. Um die Metadaten des Stammverzeichnisses abzurufen, verwenden Sie den Wert "/".</p><p>Hinweis: Die maximale Länge für die ID beträgt 255 Zeichen.</p></td> 
  </tr> 
 </tbody> 
</table>

 

**Antwort**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>-Name </th> 
   <th>Typ </th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Anrede </td> 
   <td>Zeichenfolge </td> 
   <td>Der Name des Dokuments oder Ordners</td> 
  </tr> 
  <tr> 
   <td>Art </td> 
   <td>Zeichenfolge </td> 
   <td>Gibt an, ob es sich bei diesem Element um eine Datei oder einen Ordner ('Datei' oder 'Ordner') handelt</td> 
  </tr> 
  <tr> 
   <td>ID</td> 
   <td>Zeichenfolge </td> 
   <td>Die ID der Datei oder des Ordners.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>Zeichenfolge </td> 
   <td> <p>Der URL-Pfad, der von einem Benutzer zum Anzeigen des Dokuments in einem Browser-Fenster verwendet wird. Die URL kann entweder vom Dokumentanbieter oder vom nativen externen Speicheranbieter gehostet werden.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>Zeichenfolge </td> 
   <td> <p>Der URL-Pfad, der von einem Benutzer zum Herunterladen des Dokuments in einem Browser-Fenster verwendet wird. Die URL kann entweder vom Dokumentanbieter oder vom nativen externen Speicheranbieter gehostet werden.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>Zeichenfolge </td> 
   <td>Der MIME-Typ für die Datei. (optional)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>Zeichenfolge </td> 
   <td>Letzter Änderungszeitpunkt dieser Datei (formatierter RFC 3339-Zeitstempel)</td> 
  </tr> 
  <tr> 
   <td>Größe</td> 
   <td>Lang</td> 
   <td>  Die Größe der Datei in Byte. (optional)</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>Boolesch</td> 
   <td>  <p> Gibt an, ob diese Datei oder dieser Ordner für den authentifizierten Benutzer schreibgeschützt ist.(optional)</p><p> </p></td> 
  </tr> 
 </tbody> 
</table>

**Beispiel:** `https://www.acme.com/api/metadata?id=12345`

**Antwort**

```
{
"title":"My Document", 
"kind":"file"
"id":"12345", 
"viewLink":"https://www.acme.com/viewDocument?id=12345", 
"downloadLink":"https://www.acme.com/downloadDocument?id=12345",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size": "32554694"
}
```

>[!NOTE]
>
>Die Fehlerbehandlung sollte bei allen API-Aufrufen konsistent sein. Einzelheiten finden Sie im Abschnitt „Fehlerbehandlung“ weiter unten.

### Abrufen einer Liste von Elementen in einem Ordner

Gibt Metadaten für die Dateien und Ordner für einen bestimmten Ordner zurück.

**URL**

GET /files

**Abfrageparameter**

| -Name  | Beschreibung |
|---|---|
| parentId  | Die Ordner-ID. Um die Metadaten des Stammverzeichnisses abzurufen, verwenden Sie den Wert &quot;/&quot;. |

{style="table-layout:auto"}

Die Document Webhooks-API unterstützt derzeit nicht die Paginierung.

**Antwort**

JSON mit einer Liste von Dateien und Ordnern. Die Metadaten für jedes Element sind mit denen identisch, die vom Endpunkt /metadata zurückgegeben werden.

**Beispiel:** `https://www.acme.com/api/files?parentId=123456`

**Antwort**

```
[
{
"title":"Folder A",
"kind":"folder",
"id":"2lj23lkj",
"viewLink":"https://www.acme.com/viewDocument?id=2lj23lkj",
"downloadLink":"https://www.acme.com/downloadDocument?id=2lj23lkj",
"mimeType":"",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"" 
},
{
"title":"My Document",
"kind":"file",
"id":"da8cj234"
"viewLink":"https://www.acme.com/viewDocument?id=da8cj234",
"downloadLink":"https://www.acme.com/downloadDocument?id=da8cj234",
"mimeType":"image/png",
"dateModified":"2014­06­05T17:39:45.251Z",
"size":"32554694"
},
]
```

### Suche durchführen

Gibt Metadaten für die bei einer Suche zurückgegebenen Dateien und Ordner zurück. Dies kann als Volltextsuche oder als reguläre Datenbankabfrage implementiert werden. Workfront ruft den /search-Endpunkt auf, wenn der Benutzer eine Suche über den externen Dateibrowser durchführt.

**URL**

GET/search

**Abfrageparameter**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>-Name </th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Abfrage</td> 
   <td>Der Suchbegriff oder die Phrase.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(optional) Die Ordner-ID, von der aus die Suche ausgeführt wurde. Hinweis: Dies ist ein Platzhalter für eine zukünftige Funktion in Workfront. Derzeit gibt Workfront diesen Parameter nicht weiter. </p> </td> 
  </tr> 
  </tbody> 
</table>

Die Document Webhooks-API unterstützt derzeit nicht die Paginierung.

 

**Antwort**

JSON mit einer Liste von Metadaten für Dateien und Ordner, die mit der Abfrage übereinstimmen. Was eine „Übereinstimmung“ darstellt, wird vom Webhook-Anbieter bestimmt. Idealerweise sollte dies eine Volltextsuche sein. Eine auf Dateinamen basierende Suche funktioniert ebenfalls.

**Beispiel:** `https://www.acme.com/api/search?query=test-query`

**Antwort**

```
[
{ File/Folder Metadata },
{ File/Folder Metadata }
]
```

### Abrufen des Inhalts eines Dokuments

Gibt die Rohbytes für ein Dokument zurück.

**URL**

GET/Download

**Abfrageparameter**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>-Name </th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>ID</p> </td> 
   <td> Die Dokument-ID.</td> 
  </tr> 
 </tbody> 
</table>

 

**Antwort**

Die Rohbytes des Dokuments.

**Beispiel:** `https://www.acme.com/api/download?id=123456`

### Abrufen einer Miniaturansicht für ein Dokument

Gibt die rohen Miniaturbyte für ein Dokument zurück.

**URL**

GET/Thumbnail

**Abfrageparameter**

| -Name  | Beschreibung |
|---|---|
| ID  | Die Dokument-ID. |
| Größe  |  Die Breite der Miniaturansicht |

{style="table-layout:auto"}

 

**Antwort**

Die rohen Miniaturansichten in Bytes.

**Beispiel:** `https://www.acme.com/api/thumbnail?id=123456`

### Datei hochladen - Teil 1 von 2

Das Hochladen einer Datei in einen Dokumentspeicheranbieter ist ein zweistufiger Prozess, für den zwei separate API-Endpunkte erforderlich sind. Workfront beginnt den Upload-Prozess mit dem Aufruf von /uploadInit . Dieser Endpunkt gibt eine Dokument-ID zurück, die beim Hochladen der Dokument-Bytes an /upload übergeben wird. Je nach dem zugrunde liegenden Dokumentenspeichersystem kann es erforderlich sein, ein Dokument mit einer Länge von null zu erstellen und den Inhalt des Dokuments später zu aktualisieren.

In Version 1.1 dieser Spezifikation können die Dokument-ID und Dokumentversions-ID hinzugefügt werden, um zusätzliche Informationen von Workfront abzurufen. Wenn das Dokumentenverwaltungssystem beispielsweise zusätzliche Informationen zum Dokument benötigt, könnte der Webhook-Implementierungs-Code die Dokument-ID verwenden, um diese Informationen mithilfe der RESTful-API von Workfront abzurufen. Als Best Practice empfiehlt es sich, diese Informationen aus benutzerdefinierten Datenfeldern im Dokument zu generieren, das die Aufgabe, das Problem oder das Projekt enthält.

**URL**

POST /uploadInit

**Abfrageparameter**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>-Name </th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>parentId </td> 
   <td>Die ID des übergeordneten Ordners, wie vom Webhook-Anbieter referenziert.</td> 
  </tr> 
  <tr> 
   <td>Dateiname </td> 
   <td>Der Name des Dokuments</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>Die Workfront-Dokument-ID (in Version 1.1 hinzugefügt)</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>Die Workfront-Dokumentversions-ID (in Version 1.1 hinzugefügt)</td> 
  </tr> 
 </tbody> 
</table>

 

**Antwort**

Die Metadaten für die Datei, wie vom Endpunkt /metadata definiert.

**Beispiel:** `https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&docu mentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b`

**Antwort**

`[file_metadata]` enthält die neue Dokument-ID, die vom Dokumentanbieter verwendet wird.

### Datei hochladen - Teil 2 von 2

Lädt die Bytes eines Dokuments in den Webhook-Anbieter hoch.

**URL**

PUT/Upload

**Abfrageparameter**

| -Name  | Beschreibung |
|---|---|
| ID  |  Die Dokument-ID, die gerade erstellt wurde. |


 

**Anfragetext**

Die Rohdaten-Inhaltsbytes für das Dokument.

**Antwort**

```
{
"result": "success"
}
```

oder

```
{
"result": "fail"
}
```

**Beispiel:** `https://www.acme.com/api/upload?id=1234` *[Dokument-Bytes im Aktualisierungsverlauf enthalten]*

**Antwort**

```
{
"result":"success"
}
```

### Abrufen von Informationen über den Service 

(Veröffentlichungsdatum - wird noch bekannt gegeben) Gibt Informationen zum Service zurück, z. B. Funktionen und Merkmale. Workfront verwendet diese Informationen, um die Benutzeroberfläche in Workfront anzupassen. Wenn die Webhook-Implementierung beispielsweise benutzerdefinierte Aktionen enthält, sollte die JSON diese Vorgänge in der JSON-Datei auflisten. Benutzer können dann diese Aktionen von Workfront aus aufrufen.

**URL**

GET /serviceInfo

Abfrageparameter

Keine. Darüber hinaus sollten Aufrufe an diesen Endpunkt keine Authentifizierung erfordern.

**Antwort**

JSON mit Informationen zu diesem Service

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Name</th> 
   <th>Typ </th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>webhookVersion </td> 
   <td>Zeichenfolge </td> 
   <td>Die Webhook-Version, die von diesem Service implementiert wird. Dies ist die Versionsnummer, die oben in dieser Spezifikation aufgeführt ist.</td> 
  </tr> 
  <tr> 
   <td>Version </td> 
   <td>Zeichenfolge </td> 
   <td>Die interne Versionsnummer für diesen Service. Diese Nummer wird vom Webhook-Dienstleister festgelegt und dient nur zu Informationszwecken.<br><br></td> 
  </tr> 
  <tr> 
   <td>Verleger </td> 
   <td>Zeichenfolge </td> 
   <td>Der Name des Unternehmens, das die Webhook-Implementierung bereitstellt.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>Zeichenfolge </td> 
   <td>Eine Liste mit den API-Endpunkten, die von diesem Service implementiert wurden. Damit kann sichergestellt werden, dass die Benutzeroberfläche in Workfront die vom Webhook-Anbieter bereitgestellten Funktionen widerspiegelt. Jedes Element in der Liste muss den Namen des Endpunkts enthalten (z. B. „Suche„).</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>Zeichenfolge</td> 
   <td>  <p>Eine Liste mit den benutzerdefinierten Vorgängen, die von diesem Webhook implementiert wurden. Jedes Listenelement enthält einen Namen und einen Anzeigenamen. Der Anzeigename wird im Dropdown-Menü „Dokumentaktionen“ in Workfront angezeigt. Durch Klicken auf das Element in der Dropdown-Liste wird die Aktion im Webhook aufgerufen, indem der /customAction-Endpunkt aufgerufen wird.</p></td> 
  </tr> 
 </tbody> 
</table>

**Beispiel:** https://www.acme.com/api/serviceInfo

**Rückgabe**

```
{
"webhook version": "1.2", "version": "1.0", "publisher": "Acme, LLC", "availableEndpoints": ["files", "metadata", "search", "download"

"thumbnail", "uploadInit", "upload" ], "customActions" [
{
"name": "archive", "displayName": "Archive" }, {

"name": "doSomethingElse", "displayName": "Do Something" }, ] }
```

### Erstellen eines Ordners

(In Version 1.2 hinzugefügt) Erstellt einen Ordner in einem bestimmten Verzeichnis.
URL

POST /createFolder

**Abfrageparameter**

| -Name  | Beschreibung |
|---|---|
| parentId  | Die Ordner-ID, in der der Ordner erstellt werden soll |
| -Name  | Der Name des neuen Ordners |

{style="table-layout:auto"}

 

**Antwort**

Die Metadaten für den neu erstellten Ordner, wie vom Endpunkt /metadata definiert.

**Beispiel:** `POST https://www.acme.com/api/createFolder`

```
-------------------------------

parentId=1234

name=New Folder ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

Rückgabe

```
{"title":"New Folder", 
 "kind":"folder""id":"5678",
 "viewLink":"",
 "downloadLink":"",
 "mimeType":"",
 "dateModified":"2014­06­05T17:39:45.251Z" 
 "size": "" 
 }
```

### Dokument oder Ordner löschen

(Veröffentlichungsdatum - wird noch bekannt gegeben) Löscht ein Dokument oder einen Ordner mit der angegebenen ID im externen System. Beim Löschen eines Ordners wird auch dessen Inhalt gelöscht.

URL

PUT/Löschen

**Abfrageparameter**

| -Name  | Beschreibung |
|---|---|
| documentId  | Die zu löschende Dokument-ID |
| folderId  |  Die zu löschende Ordner-ID |

{style="table-layout:auto"}

Antwort Eine JSON-Zeichenfolge, die Erfolg oder Fehler angibt, wie im Abschnitt Fehlerbehandlung unten angegeben.

**Beispiel:** PUT https://www.acme.com/api/delete id=1234

Rückgabe

```
{
"status": "success" 
}
```

Rückgabe

```
{
"status": "failure", "error": "File not found"
}
```


### Dokument oder Ordner umbenennen

(Veröffentlichungsdatum - wird noch bekannt gegeben) Benennt ein Dokument oder einen Ordner mit der angegebenen ID im externen System um.

URL

PUT/Umbenennen

**Abfrageparameter**

| -Name  | Beschreibung |
|---|---|
| ID | Die umzubenennende Dokument- oder Ordner-ID |
| -Name  | Der neue Name des Dokuments oder Ordners |

{style="table-layout:auto"}

 

Antwort

Eine JSON-Zeichenfolge, die Erfolg oder Fehler anzeigt, wie im Abschnitt Fehlerbehandlung unten angegeben.

**Beispiel:**

`PUT https://www.acme.com/api/rename`

```
-------------------------------

id=1234

name=Folder B ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

```
{
"status": "success" 
}returns
{
"status": "failure", error: "Folder cannot be renamed because a folder with that name already exists." 
}
```

### Durchführen einer benutzerdefinierten Aktion

(Veröffentlichungsdatum - wird noch bekannt gegeben) Dieser Endpunkt ermöglicht es einem Workfront-Benutzer (oder vielleicht einem automatisierten Workflow-Ereignis), eine Aktion im externen System durchzuführen. Der /customAction-Endpunkt akzeptiert einen „name“-Parameter, mit dem der Webhook-Anbieter mehrere benutzerdefinierte Vorgänge implementieren kann.

Der Webhook-Anbieter registriert benutzerdefinierte Aktionen bei Workfront, indem er die Aktionen in die /serviceInfo-Antwort unter customActions aufnimmt. Workfront lädt diese Liste, wenn Sie den Webhook-Anbieter unter Einrichtung > Dokumente > Benutzerdefinierte Integrationen einrichten oder aktualisieren.\
![](assets/mceclip0-350x262.png)

Benutzerinnen und Benutzer können die benutzerdefinierte Aktion mit Triggern versehen, indem sie den Abschnitt unter „Dokumentaktionen“ auswählen\
![](assets/mceclip1-350x95.png)

**URL**

GET/customAction

**Abfrageparameter**

<table style="table-layout:auto">
 <col>
 <col>
 <thead>
  <tr>
   <th>-Name </th>
   <th>Beschreibung</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><p>name</p></td>
   <td><p>Die Kennung, die den Typ der auszuführenden Aktion angibt. Dieser Wert entspricht einem der customAction-Werte, die vom Endpunkt /serviceInfo zurückgegeben werden.</p></td>
  </tr>
  <tr>
   <td>documentId </td>
   <td>Die Workfront-Dokument-ID, für die die Aktion ausgeführt wird.</td>
  </tr>
  <tr>
   <td>documentVersionId </td>
   <td> Die ID der Workfront-Dokumentversion, für die die Aktion ausgeführt wird.</td>
  </tr>
 </tbody>
</table>

 

**Antwort**

Eine JSON-Zeichenfolge, die Erfolg oder Fehler anzeigt, wie im Abschnitt Fehlerbehandlung unten angegeben. Bei einem Fehler (d. h. Status = „Fehler„) zeigt Workfront dem Benutzer die bereitgestellte Fehlermeldung an.

**Beispiel:** https://sample.com/webhooks/customName?name=archive&amp;documentId=5502082c003a4f30 ddec2fb2b739cb7c&amp;documentVersionId=54b598a700e2342d6971597a5df1a8d3

Antwort

```
{
"status": "success" 
}
```


## Fehlerbehandlung

Bei der Verarbeitung von API-Anfragen können Probleme auftreten. Dies sollte über alle API-Endpunkte hinweg konsistent gehandhabt werden. Wenn ein Fehler auftritt, führt der Webhook-Anbieter Folgendes aus:

* Fügen Sie einen Fehlercode in die Antwortkopfzeile ein. Zu den Fehlercodes gehören:

   * 403 - Verboten. Gibt an, dass entweder die Anfrage-Token fehlen oder ungültig sind oder dass mit den Token verknüpfte Anmeldeinformationen keinen Zugriff auf die angegebene Ressource haben. Bei OAuth-basierten Webhook-Anbietern versucht Workfront, neue Zugriffstoken abzurufen.
   * 404 - Nicht gefunden. Gibt an, dass die angegebene Datei oder der angegebene Ordner nicht vorhanden ist.
   * 500 - Interner Server-Fehler. Jede andere Fehlerart.

* Beschreiben Sie den Fehler im Antworttext im folgenden Format:


```
{
"status": "error"
"error": "Sample error message" 
}
```


## Testen

Um sicherzustellen, dass die Webhook-Implementierung des Dokuments ordnungsgemäß funktioniert, führen Sie die folgenden Tests aus. Hierbei handelt es sich um manuelle Tests, die die Workfront-Web-Schnittstelle durchlaufen und indirekt die Endpunkte für Ihre Webhook-Implementierung treffen.

### Voraussetzungen

Um diese Tests auszuführen, benötigen Sie Folgendes:

* Ein Workfront-Konto mit aktiviertem Advanced Document Management (ADM)
* Ein Workfront-Benutzer für dieses Konto mit Systemadministratorrechten
* Eine Document Webhook-Instanz, deren HTTP-Endpunkte für Workfront zugänglich sind

Bei diesen Tests wird außerdem davon ausgegangen, dass Sie Ihre Document Webhook-Instanz in Workfront unter Setup > Dokumente > Benutzerdefinierte Integrationen bereits registriert haben.

### Test 1: Bereitstellen des Document Webhook-Service für einen Benutzer

Testet die Authentifizierungs-URL und Token-Endpunkt-URL für OAuth-basierte Webhook-Anbieter.

1. Navigieren Sie in Workfront zur Hauptseite Dokumente , indem Sie in der oberen Navigationsleiste auf den Link Dokumente klicken.
1. Klicken Sie auf das Dropdown-Menü Dokumente hinzufügen und wählen Sie unter Service hinzufügen Ihren Document Webhook-Service aus.
1. (Nur OAuth-Services) Nach Abschluss des vorherigen Schritts wird die OAuth2-Authentifizierungsseite Ihres Services in einem Popup-Fenster geladen. (Hinweis: Sie werden möglicherweise aufgefordert, sich zuerst bei Ihrem Service anzumelden.) Gewähren Sie auf der Authentifizierungsseite Workfront Zugriff auf das Benutzerkonto, indem Sie auf die Schaltfläche Trust oder Allow klicken.
1. Vergewissern Sie sich, dass Ihr Dienst zum Dropdown-Menü Dokumente hinzufügen hinzugefügt wurde. Wenn Sie sie anfangs nicht sehen, versuchen Sie, Ihren Browser zu aktualisieren.

### Test 2: Verknüpfen eines Dokuments mit Workfront Testet die folgenden Endpunkte: /files, /metadata

1. Navigieren Sie in Workfront zur Hauptseite Dokumente , indem Sie in der oberen Navigationsleiste auf den Link Dokumente klicken.
1. Wählen Sie Ihren Document Webhook-Service unter Dokumente hinzufügen aus.
1. Navigieren Sie im Modal durch die Ordnerstruktur.
1. Überprüfen Sie, ob Sie in der Lage sind, ordnungsgemäß in der Ordnerstruktur zu navigieren.
1. Dokument auswählen und mit Workfront verknüpfen

### Test 3: Navigieren zu einem Dokument im Content-Management-System

Testet die folgenden Endpunkte: /metadata (insbesondere den viewLink)

1. Verknüpfen eines Dokuments mit Workfront
1. Wählen Sie das Dokument aus und klicken Sie auf den Link Öffnen .
1. Stellen Sie sicher, dass das Dokument auf einer neuen Registerkarte geöffnet wird.

### Test 4: Navigieren Sie zu einem Dokument im Content Management System (mit Anmeldung)

Testet die folgenden Endpunkte: /metadata (insbesondere den viewLink)

1. Stellen Sie sicher, dass Sie vom Content-Management-System abgemeldet sind.
1. Verknüpfen eines Dokuments mit Workfront.
1. Wählen Sie das Dokument aus und klicken Sie auf den Link Öffnen .
1. Stellen Sie sicher, dass der Anmeldebildschirm des Content Management Systems auf einer neuen Registerkarte geladen wird.
1. Melden Sie sich an und stellen Sie sicher, dass Sie zum Dokument weitergeleitet werden

### Test 5: Herunterladen des Dokuments aus dem Content-Management-System

Testet die folgenden Endpunkte: /metadata (insbesondere den downloadLink)

1. Verknüpfen eines Dokuments mit Workfront.
1. Wählen Sie das Dokument aus und klicken Sie auf den Link Herunterladen .
1. Stellen Sie sicher, dass der Download beginnt.

### Test 6: Suchen nach Inhalten

Testet die folgenden Endpunkte: /search

1. Navigieren Sie in Workfront zur Hauptseite Dokumente , indem Sie in der oberen Navigationsleiste auf den Link Dokumente klicken.
1. Wählen Sie Ihren Document Webhook-Service unter Dokumente hinzufügen aus.
1. Führen Sie über das Modal eine Suche durch.
1. Überprüfen Sie, ob die Suchergebnisse korrekt sind.

### Test 7: Senden eines Dokuments von Workfront an das Content Management System

Testet die folgenden Endpunkte: /files, /uploadInit, /upload

1. Navigieren Sie in Workfront zur Hauptseite Dokumente , indem Sie in der oberen Navigationsleiste auf den Link Dokumente klicken.
1. Dokument von Ihrem Computer in Workfront hochladen
1. Zur Seite mit den Dokumentdetails
1. Wählen Sie im Dropdown-Menü Dokumentaktionen unter Senden an… Ihren Dokument-Webhook-Service aus.
1. Wechseln Sie zum gewünschten Zielordner und klicken Sie auf die Schaltfläche Speichern .
1. Überprüfen Sie, ob das Dokument an den richtigen Speicherort im Content Management System hochgeladen wurde.

### Test 8: Anzeigen von Miniaturansichten in Workfront

Testet die folgenden Endpunkte: /thumbnail

1. Verknüpfen eines Dokuments mit Workfront.
1. Wählen Sie das Dokument in der Liste aus.
1. Stellen Sie sicher, dass die Miniaturansicht im rechten Bedienfeld angezeigt wird.

### Test 9: Abrufen der Inhalts-Bytes

Testet die folgenden Endpunkte: /download

1. Verknüpfen eines Dokuments mit Workfront.
1. Navigieren Sie zur Seite mit den Dokumentdetails.
1. Senden Sie das Dokument an Workfront, indem Sie Dokumentaktionen > Senden an… > Workfront auswählen. Dadurch wird eine neue Dokumentversion in Workfront erstellt.
1. Laden Sie das Dokument von Workfront herunter, indem Sie auf den Download-Link klicken.

### Test 10: Zugriffstoken aktualisieren (nur OAuth2-Webhook-Anbieter)

Testet die folgenden Endpunkte: Token Endpoint URL

1. Bereitstellen des Document Webhook-Services für einen Benutzer
1. Invalidieren Sie das Zugriffs-Token des Benutzers, indem Sie entweder 1 ) auf die Zeitüberschreitung warten oder 2) es im externen System manuell invalidieren.
1. Aktualisieren Sie das Zugriffstoken in Workfront. Dies können Sie beispielsweise tun, indem Sie ein Dokument mit Workfront verknüpfen. Das Zugriffstoken wurde erfolgreich aktualisiert, wenn Sie zu einem Dokument navigieren und es verknüpfen konnten.

>[!NOTE]
>
>Derzeit ist „Senden an…“ nicht für verknüpfte Dokumente verfügbar. Dies wird von Workfront hinzugefügt. Sie können den /download-Endpunkt testen, indem Sie mit einem REST-Client wie Postman manuell auf den Endpunkt klicken. Alternativ kann der Endpunkt /download getestet werden, indem ein digitaler Korrekturabzug generiert wird. Wenden Sie sich zur Aktivierung des digitalen Proofings an Workfront.

## Versionen

* Version 1.0 (Veröffentlichungsdatum - Mai 2015)

   * Erstspezifikation

* Version 1.1 (Veröffentlichungsdatum - Juni 2015)

   * /uploadInit - Dokument-ID und Dokument-Version-ID hinzugefügt

* Version 1.2 (Veröffentlichungsdatum - Oktober 2015)

   * Hinzugefügt /createFolder

