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
source-wordcount: '3646'
ht-degree: 3%

---


# Document Webhooks-API

Adobe Workfront Document Webhooks definiert eine Reihe von API-Endpunkten, über die Workfront autorisierte API-Aufrufe an einen externen Dokumentanbieter sendet. Dadurch kann jeder ein Middleware-Plugin für jeden Dokumentenspeicher erstellen.

Das Benutzererlebnis für webhook-basierte Integrationen ähnelt dem von vorhandenen Dokumentenintegrationen wie Google Drive, Box und Dropbox. Ein Workfront-Benutzer kann beispielsweise die folgenden Aktionen durchführen:

* Navigieren zur Ordnerstruktur des externen Dokumentanbieters
* Suchdateien
* Verknüpfen von Dateien in Workfront
* Hochladen von Dateien in den externen Dokumentanbieter
* Anzeigen einer Miniaturansicht für das Dokument

## Referenzimplementierung

Um die Entwicklung einer neuen Webhooks-Implementierung zu beschleunigen, stellt Workfront eine Referenzimplementierung bereit. Der Code dafür finden Sie unter [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). Diese Implementierung ist Java-basiert und ermöglicht es Workfront, Dokumente in einem Netzwerkdateisystem zu verbinden.

## Registrieren einer Webhook-Integration

Workfront-Administratoren können eine benutzerdefinierte Webhook-Integration für ihr Unternehmen hinzufügen, indem sie zu Einrichtung > Dokumente > Benutzerdefinierte Integrationen in Workfront navigieren. Auf der Seite Benutzerspezifische Integration unter Einrichtung können Administratoren eine Liste der vorhandenen Dokument-Webhook-Integrationen anzeigen. Auf dieser Seite können Integrationen hinzugefügt, bearbeitet, aktiviert und deaktiviert werden. Um eine Integration hinzuzufügen, klicken Sie auf die Schaltfläche &quot;Integration hinzufügen&quot;.

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
   <td> <p>Der Speicherort der Callback-API. Bei Aufrufen an das externe System hängt Workfront einfach den Endpunktnamen an diese Adresse an. Wenn der Administrator beispielsweise die Basis-API-URL " https://www.mycompany.com/api/v1 "eingegeben hat, verwendet Workfront die folgende URL, um die Metadaten eines Dokuments zu erhalten: https://www.mycompany.com/api/v1/metadata?id=1234.</p> </td> 
  </tr> 
  <tr> 
   <td>Anforderungsparameter</td> 
   <td> <p>Optionale Werte, die an die Abfragezeichenfolge eines jeden API-Aufrufs anzuhängen sind. Beispiel: access_type=offline.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Authentifizierungstyp</td> 
   <td>OAuth2 oder ApiKey</td> 
  </tr> 
  <tr> 
   <td>Authentifizierungs-URL</td> 
   <td> <p>(Nur OAuth2) Die vollständige URL, die für die Benutzerauthentifizierung verwendet wird. Workfront navigiert Benutzer im Rahmen des OAuth-Bereitstellungsprozesses zu dieser Adresse. Hinweis: Workfront hängt einen "state"-Parameter an die Abfragezeichenfolge an. Der Provider muss dies zurück an Workfront übergeben, indem er es an den Workfront-Weiterleitungs-URI anhängt.</p> </td> 
  </tr> 
  <tr> 
   <td>Token Endpoint URL</td> 
   <td> <p>(Nur OAuth2) Die vollständige API-URL, mit der OAuth2-Token abgerufen werden. Dies wird vom Webhook-Provider oder externen Dokumentenanbieter gehostet</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Client-ID</td> 
   <td>(Nur OAuth2) Die OAuth2-Client-ID für diese Integration</td> 
  </tr> 
  <tr> 
   <td>Geheimer Client-Schlüssel</td> 
   <td> <p>(Nur OAuth2) Das OAuth2 Client Secret für diese Integration</p> </td> 
  </tr> 
  <tr> 
   <td>Workfront Redirect-URI</td> 
   <td>  <p>(Nur OAuth2) Dies ist ein schreibgeschütztes Feld, das von Workfront generiert wird. Dieser Wert wird verwendet, um diese Integration beim externen Dokumentenanbieter zu registrieren. Hinweis: Wie oben für die Authentifizierungs-URL beschrieben, muss der Provider den Parameter "state"und seinen Wert beim Ausführen der Umleitung an den Abfragezeichenfolgen anhängen.</p></td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td>  <p>(Nur APIKey) Wird verwendet, um autorisierte API-Aufrufe an den Webhook-Provider durchzuführen. Der vom Webhook-Provider ausgegebene API-Schlüssel.</p></td> 
  </tr> 
 </tbody> 
</table>

 

## Authentifizierung

Workfront Document Webhooks unterstützt zwei verschiedene Authentifizierungsformen: OAuth2 und ApiKey. In beiden Fällen übergibt Workfront beim Ausführen eines API-Aufrufs Authentifizierungstoken in der Kopfzeile.

### OAuth2

Mit OAuth2 kann Workfront im Auftrag eines Benutzers autorisierte API-Aufrufe an einen Webhook-Provider senden. Dazu muss der Benutzer sein externes Document Provider-Konto mit Workfront verbinden und Workfront gewähren

Zugang zu Handlungen in ihrem Namen. Dieser Handshaking-Prozess erfolgt nur einmal für jeden Benutzer. So funktioniert es:

1. Der Benutzer beginnt damit, die Webhook-Integration mit seinem Konto zu verbinden. Dies geschieht derzeit durch Klicken auf das Dropdown-Menü &quot;Dokument hinzufügen&quot;> &quot;Dienst hinzufügen&quot;> &quot;Name der benutzerdefinierten Integration&quot;.
1. Workfront navigiert zum Benutzer über die Authentifizierungs-URL, die ihn auffordern kann, sich beim externen Dokumentenanbieter anzumelden. Diese Seite wird vom Webhook Provider oder vom externen Dokumentenverwaltungssystem gehostet. Dadurch fügt Workfront der Authentifizierungs-URL einen &quot;state&quot;-Parameter hinzu. Dieser Wert muss zurück an Workfront übergeben werden, indem der gleiche Wert im folgenden Schritt an den Workfront-URI angehängt wird.
1. Nach der Anmeldung beim externen System (oder wenn der Benutzer bereits angemeldet ist) wird der Benutzer zu einer &quot;Authentifizierungsseite&quot;geleitet, auf der erklärt wird, dass Workfront Zugriff anfordert, um eine Reihe von Aktionen im Namen des Benutzers durchzuführen.
1. Wenn der Benutzer auf die Schaltfläche &quot;Zulassen&quot;klickt, leitet der Browser zum Workfront-Weiterleitungs-URI um und fügt &quot;code=&quot;hinzu`<code>`&quot; auf den Querystring. Gemäß der OAuth2-Spezifikation ist dieses Token kurzlebig. Die Abfragezeichenfolge muss auch die folgende sein: &quot;state=`<sent_by_workfront>`&quot;.
1. Workfront verarbeitet diese Anforderung und führt einen API-Aufruf an die Token-Endpunkt-URL mit dem Autorisierungscode aus.
1. Die Token-Endpunkt-URL gibt ein Aktualisierungstoken und Zugriffstoken zurück.
1. Workfront speichert diese Token und stellt die Webhook-Integration für diesen Benutzer vollständig bereit.
1. Ab diesem Zeitpunkt kann Workfront autorisierte API-Aufrufe an den Webhook-Provider senden. Beim Ausführen dieser Aufrufe sendet Workfront das Zugriffstoken im HTTP-Anforderungsheader, wie unten dargestellt:

   ```
   -------------------------------  
   Authorization: Bearer [access_token] ­­­­­­­­­­­­­­­­­­­­­­­­­­  
   -------------------------------
   ```

1. Wenn das Zugriffstoken abgelaufen ist, führt Workfront einen Aufruf an die Token-Endpunkt-URL durch, um ein neues Zugriffstoken abzurufen, und versucht dann erneut, den autorisierten API-Aufruf mit dem neuen Zugriffstoken durchzuführen.

### ApiKey

Autorisierte API-Aufrufe an einen Webhook-Provider mithilfe eines APIKey durchzuführen, ist viel einfacher als OAuth2. Beim Ausführen eines API-Aufrufs übergibt Workfront einfach den ApiKey- und Workfront-Benutzernamen im HTTP-Anforderungsheader:

```
-------------------------------

apiKey: 12345

username: johndoe@foo.com

-------------------------------
```

Der Webhook-Provider kann den Benutzernamen verwenden, um benutzerspezifische Berechtigungen anzuwenden. Dies funktioniert am besten, wenn beide Systeme über Single Sign On (SSO) eine Verbindung zu LDAP herstellen.

### Hinzufügen von Anforderungsheadern (optional)

Zusätzlich zur Verwendung von OAuth2-Token oder einem ApiKey zur Authentifizierung kann Workfront für jeden API-Aufruf einen vordefinierten Header-Satz an den Webhook-Provider senden. Ein Workfront-Administrator kann diese Einrichtung bei der Registrierung oder Bearbeitung einer Webook-Integration einrichten, wie im obigen Abschnitt beschrieben. Siehe Registrieren einer Webhook-Integration .

Dies kann beispielsweise für die einfache Authentifizierung verwendet werden. Dazu fügt der Workfront-Administrator die folgenden Request Header-Informationen im Dialogfeld &quot;Benutzerdefinierte Integration&quot;hinzu:

   Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ===

wobei QWxhZGRpbjpvcGVuIHNlc2FtZQ== eine Base-64-kodierte Zeichenfolge von &quot;username:password&quot;ist. Siehe Grundlegende Authentifizierung . Sofern dies hinzugefügt wurde, übergibt Workfront dies zusätzlich zu anderen Anforderungsheadern im HTTP-Anforderungsheader:

```
­­­­­­­­­­­­­­­­­­­­­­­­­­-------------------------------

apiKey: 12345

username: johndoe@foo.com

Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

## API-Spezifikation

Im Folgenden finden Sie eine Liste der APIs, die der Webhook-Provider implementieren sollte, damit Dokument-Webhooks funktionieren.

### Abrufen von OAuth2-Token (nur OAuth2-Authentifizierung erforderlich)

Gibt das OAuth2-Aktualisierungstoken und Zugriffstoken für einen authentifizierten Benutzer zurück. Dies wird einmal aufgerufen, wenn der Benutzer einen Dokumentanbieter bereitstellt. Nachfolgende Aufrufe werden durchgeführt, um ein aktualisiertes Zugriffstoken zu erhalten.

HTTP-Anforderungs-POST /any/url

Die URL kann konfiguriert werden und entspricht dem URL-Wert des Token-Endpunkts auf der Setup-Seite der benutzerdefinierten Integration.

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
   <td>yes</td> 
   <td> <p>Zu den Werten gehören "authorization_code"oder "refresh_token". Der angegebene Wert gibt an, welcher der beiden Parameter an diesen API-Aufruf übergeben wird: code oder refresh_token.</p> </td> 
  </tr> 
  <tr> 
   <td>code</td> 
   <td>abhängig</td> 
   <td> <p>Der Autorisierungscode, der an Workfront gesendet wird, nachdem der Benutzer auf die Schaltfläche "Grant" geklickt hat. Dies ist nur erforderlich, wenn der Fördertyp "authorization_code"ist. Der Autorisierungscode sollte kurzlebig sein und in der Regel innerhalb von 10 Minuten oder weniger ablaufen.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token</td> 
   <td>abhängig</td> 
   <td> <p>Dies ist nur erforderlich, wenn nachfolgende Aufrufe durchgeführt werden, um ein neues access_token abzurufen, da das vorherige access_token abgelaufen ist. Setzen Sie beim Senden dieses Werts den Parameter grant_type auf "refresh_token".</p> </td> 
  </tr> 
  <tr> 
   <td>client_id</td> 
   <td>yes</td> 
   <td>Die in Workfront für diese benutzerdefinierte Integration konfigurierte Client-ID.</td> 
  </tr> 
  <tr> 
   <td>client_secret</td> 
   <td>yes</td> 
   <td> Der Client Secret , der in Workfront für diese benutzerdefinierte Integration konfiguriert wurde.</td> 
  </tr> 
 </tbody> 
</table>

 

**Reaktion**

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
   <td> <p>Ein Token, mit dem autorisierte API-Aufrufe im Namen des Benutzers durchgeführt werden. Dies sollte ablaufen, um nicht autorisierte API-Aufrufe zu verhindern.</p> </td> 
  </tr> 
  <tr> 
   <td>refresh_token </td> 
   <td>Zeichenfolge</td> 
   <td> <p>Ein langlebiges Token, das zum Abrufen eines neuen access_token durch Aufruf dieser API-Methode verwendet wird.</p> </td> 
  </tr> 
  <tr> 
   <td>expires_in </td> 
   <td>long</td> 
   <td>  <p>(optional) Die Zeit (in Sekunden) bis zum Ablauf des access_token (im Allgemeinen 3.600).</p></td> 
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


**Reaktion**

```
{
"access_token":"ad8af5ad5ads759", 
"refresh_token":"9a0h5d87d808ads", 
"expires_id":"3600" 
}
```

### Abrufen von Metadaten für Dateien oder Ordner

Gibt Metadaten für die angegebene Datei oder den angegebenen Ordner zurück.

**URL**

GET /metadata?id=[Dokument- oder Ordner-ID]

**Abfrageparameter**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Name </th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>id</td> 
   <td>  <p>Die Kennung der Datei oder des Ordners, auf die der Webhook-Provider verweist. Dies unterscheidet sich von der Dokument-ID von Workfront. Um die Metadaten des Stammverzeichnisses abzurufen, verwenden Sie den Wert '/'.</p><p>Hinweis: Die maximale Länge der ID beträgt 255 Zeichen.</p></td> 
  </tr> 
 </tbody> 
</table>

 

**Reaktion**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Name </th> 
   <th>Typ </th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>title </td> 
   <td>Zeichenfolge </td> 
   <td>Der Name des Dokuments oder Ordners</td> 
  </tr> 
  <tr> 
   <td>kind </td> 
   <td>Zeichenfolge </td> 
   <td>Gibt an, ob es sich bei diesem Element um eine Datei oder einen Ordner handelt ('file' oder 'folder')</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>Zeichenfolge </td> 
   <td>Die ID der Datei oder des Ordners.</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>Zeichenfolge </td> 
   <td> <p>Der URL-Pfad, der von einem Benutzer zum Anzeigen des Dokuments in einem Browserfenster verwendet wird. Die URL kann entweder vom Dokumentenanbieter oder vom nativen externen Speicheranbieter gehostet werden.</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>Zeichenfolge </td> 
   <td> <p>Der URL-Pfad, den ein Benutzer zum Herunterladen des Dokuments in ein Browserfenster verwendet. Die URL kann entweder vom Dokumentenanbieter oder vom nativen externen Speicheranbieter gehostet werden.</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>Zeichenfolge </td> 
   <td>Der MIME-Typ für die Datei. (optional)</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>Zeichenfolge </td> 
   <td>Letzte Änderung dieser Datei (formatierter RFC 3339-Zeitstempel)</td> 
  </tr> 
  <tr> 
   <td>size</td> 
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

**Reaktion**

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
>Die Fehlerbehandlung sollte für alle API-Aufrufe einheitlich sein. Weitere Informationen finden Sie unten im Abschnitt &quot;Umgang mit Fehlern&quot;.

### Abrufen einer Liste von Elementen in einem Ordner

Gibt Metadaten für die Dateien und Ordner eines bestimmten Ordners zurück.

**URL**

GET /files

**Abfrageparameter**

| Name  | Beschreibung |
|---|---|
| parentId  | Die Ordner-ID. Um die Metadaten des Stammverzeichnisses abzurufen, verwenden Sie den Wert &#39;/&#39;. |

{style="table-layout:auto"}

Die Document Webhooks-API unterstützt derzeit keine Paginierung.

**Reaktion**

JSON mit einer Liste von Dateien und Ordnern. Die Metadaten für jedes Element sind mit denen identisch, die vom Endpunkt /metadata zurückgegeben werden.

**Beispiel:** `https://www.acme.com/api/files?parentId=123456`

**Reaktion**

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

### Suchen

Gibt Metadaten für die Dateien und Ordner zurück, die von einer Suche zurückgegeben wurden. Dies kann als Volltextsuche oder als reguläre Datenbankabfrage implementiert werden. Workfront ruft den Endpunkt /search auf, wenn der Benutzer eine Suche über den externen Dateibrowser durchführt.

**URL**

GET /search

**Abfrageparameter**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Name </th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Abfrage</td> 
   <td>Der Suchbegriff oder -ausdruck.</td> 
  </tr> 
  <tr> 
   <td>parentId</td> 
   <td> <p>(optional) Die Ordner-ID, von der aus die Suche ausgeführt wurde. Hinweis: Dies ist ein Platzhalter für eine zukünftige Funktion in Workfront. Derzeit wird dieser Parameter nicht von der Arbeitsfläche übergeben. </p> </td> 
  </tr> 
  </tbody> 
</table>

Die Document Webhooks-API unterstützt derzeit keine Paginierung.

 

**Reaktion**

JSON mit einer Liste von Metadaten für Dateien und Ordner, die der Abfrage entsprechen. Was eine &quot;Übereinstimmung&quot;ausmacht, wird vom Webhook-Provider bestimmt. Idealerweise sollte eine Volltextsuche durchgeführt werden. Eine filename-basierte Suche funktioniert ebenfalls.

**Beispiel:** `https://www.acme.com/api/search?query=test-query`

**Reaktion**

```
[
{ File/Folder Metadata },
{ File/Folder Metadata }
]
```

### Abrufen des Inhalts eines Dokuments

Gibt die unformatierten Bytes für ein Dokument aus

**URL**

GET /download

**Abfrageparameter**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Name </th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>id</p> </td> 
   <td> Die Dokument-ID.</td> 
  </tr> 
 </tbody> 
</table>

 

**Reaktion**

Die rohen Bytes des Dokuments.

**Beispiel:** `https://www.acme.com/api/download?id=123456`

### Miniaturansicht für ein Dokument abrufen

Gibt die unformatierten Miniaturansichten für ein Dokument zurück.

**URL**

GET /thumbnail

**Abfrageparameter**

| Name  | Beschreibung |
|---|---|
| id  | Die Dokument-ID. |
| size  |  Die Breite der Miniaturansicht |

{style="table-layout:auto"}

 

**Reaktion**

Die unformatierten Miniaturansichten.

**Beispiel:** `https://www.acme.com/api/thumbnail?id=123456`

### Datei hochladen - Teil 1 von 2

Das Hochladen einer Datei in einen Dokumentenspeicheranbieter ist ein zweistufiger Prozess, der zwei separate API-Endpunkte erfordert. Workfront startet den Upload-Prozess durch Aufruf von /uploadInit . Dieser Endpunkt gibt eine Dokument-ID zurück, die beim Hochladen der Dokument-Bytes an /upload übergeben wird. Je nach zugrunde liegendem Dokumentenspeicher kann es erforderlich sein, ein Dokument mit einer Länge von null zu erstellen und den Inhalt des Dokuments später zu aktualisieren.

Wird Version 1.1 dieser Spezifikation hinzugefügt, können die Dokument-ID und die Dokumentversions-ID verwendet werden, um zusätzliche Informationen aus Workfront abzurufen. Wenn das Document Management-System beispielsweise zusätzliche Informationen zum Dokument benötigt, kann der Webhook-Implementierungscode die Dokument-ID verwenden, um diese Informationen mithilfe der Workfront-RESTful-API abzurufen. Als Best Practice empfiehlt sich, diese Informationen aus benutzerdefinierten Datenfeldern im Dokument zu erhalten, die Aufgaben, Probleme oder Projekte enthalten.

**URL**

POST /uploadInit

**Abfrageparameter**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Name </th> 
   <th>Beschreibung</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>parentId </td> 
   <td>Die übergeordnete Ordner-ID, wie vom Webhook-Provider referenziert.</td> 
  </tr> 
  <tr> 
   <td>filename </td> 
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

 

**Reaktion**

Die Metadaten für die Datei, wie vom Endpunkt /metadata definiert.

**Beispiel:** `https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&docu mentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b`

**Reaktion**

`[file_metadata]` enthält die neue Dokument-ID, die vom Dokumentanbieter verwendet wird.

### Datei hochladen - Teil 2 von 2

Lädt die Bytes eines Dokuments in den Webhook-Provider hoch.

**URL**

PUT /upload

**Abfrageparameter**

| Name  | Beschreibung |
|---|---|
| id  |  Die Dokument-ID, die gerade erstellt wurde. |


 

**Anfrageinhalt**

Die rohen Inhalts-Bytes für das Dokument.

**Reaktion**

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

**Beispiel:** `https://www.acme.com/api/upload?id=1234` *[Dokument-Bytes, die im Aktualisierungsstream enthalten sind]*

**Reaktion**

```
{
"result":"success"
}
```

### Informationen zum Dienst erhalten 

(Releasedatum - TBD) Gibt Informationen zum Dienst zurück, z. B. Funktionen. Workfront verwendet diese Informationen, um die Benutzeroberfläche in Workfront anzupassen. Wenn die Webhook-Implementierung beispielsweise einige benutzerdefinierte Aktionen enthält, sollte die JSON diese Vorgänge in der JSON auflisten. Benutzer können diese Aktionen dann über Workfront aufrufen.

**URL**

GET /serviceInfo

Abfrageparameter

Keine. Darüber hinaus sollten Aufrufe an diesen Endpunkt keine Authentifizierung erfordern.

**Reaktion**

JSON mit Informationen zu diesem Dienst

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
   <td>Die von diesem Dienst implementierte Webhook-Version. Dies ist die Versionsnummer, die oben in dieser Spezifikation aufgeführt ist.</td> 
  </tr> 
  <tr> 
   <td>version </td> 
   <td>Zeichenfolge </td> 
   <td>Die interne Versionsnummer für diesen Dienst. Diese Nummer wird vom Webhook-Dienstleister bestimmt und nur zu Informationszwecken verwendet.<br><br></td> 
  </tr> 
  <tr> 
   <td>publisher </td> 
   <td>Zeichenfolge </td> 
   <td>Der Name des Unternehmens, das die Webhook-Implementierung bereitstellt.</td> 
  </tr> 
  <tr> 
   <td>availableEndpoints</td> 
   <td>Zeichenfolge </td> 
   <td>Eine Liste mit den von diesem Dienst implementierten API-Endpunkten. Dies kann verwendet werden, um sicherzustellen, dass die Benutzeroberfläche in Workfront die vom Webhook-Provider bereitgestellten Funktionen widerspiegelt. Jedes Element in der Liste muss den Namen des Endpunkts enthalten (z. B. "Suche").</td> 
  </tr> 
  <tr> 
   <td>customActions </td> 
   <td>Zeichenfolge</td> 
   <td>  <p>Eine Liste mit den von diesem Webhook implementierten benutzerdefinierten Vorgängen. Jedes Listenelement enthält einen Namen und einen Anzeigenamen. Der Anzeigename wird im Dropdown-Menü "Dokumentaktionen"in Workfront angezeigt. Durch Klicken auf das Element in der Dropdown-Liste wird die Aktion im Webhook aufgerufen, indem der Endpunkt /customAction aufgerufen wird.</p></td> 
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

(Hinzugefügt in Version 1.2) Erstellt einen Ordner in einem bestimmten Verzeichnis.
URL

POST /createFolder

**Abfrageparameter**

| Name  | Beschreibung |
|---|---|
| parentId  | Die Ordner-ID, in der der Ordner erstellt werden soll |
| name  | Der Name des neuen Ordners |

{style="table-layout:auto"}

 

**Reaktion**

Die Metadaten für den neu erstellten Ordner, wie vom Endpunkt /metadata definiert.

**Beispiel:** `POST https://www.acme.com/api/createFolder`

```
-------------------------------

parentId=1234

name=New Folder ­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­­

-------------------------------
```

return

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

### Löschen eines Dokuments oder Ordners

(Veröffentlichungsdatum - TBD) Löscht ein Dokument oder einen Ordner mit der angegebenen ID im externen System. Durch Löschen eines Ordners werden auch dessen Inhalte gelöscht.

URL

PUT/Löschen

**Abfrageparameter**

| Name  | Beschreibung |
|---|---|
| documentId  | Die zu löschende Dokument-ID |
| folderId  |  Die zu löschende Ordner-ID |

{style="table-layout:auto"}

Antwort Eine JSON-Zeichenfolge, die auf Erfolg oder Fehler hinweist, wie im Abschnitt Umgang mit Fehlern unten angegeben.

**Beispiel:** PUT https://www.acme.com/api/delete id=1234

return

```
{
"status": "success" 
}
```

return

```
{
"status": "failure", "error": "File not found"
}
```


### Umbenennen eines Dokuments oder Ordners

(Veröffentlichungsdatum - TBD) Benennt ein Dokument oder einen Ordner mit der angegebenen ID im externen System um.

URL

PUT /rename

**Abfrageparameter**

| Name  | Beschreibung |
|---|---|
| id | Die umzubenennende Dokument- oder Ordner-ID |
| name  | Der neue Name des Dokuments oder Ordners |

{style="table-layout:auto"}

 

Antwort

Eine JSON-Zeichenfolge, die den Erfolg oder Fehler angibt, wie im Abschnitt Umgang mit Fehlern unten angegeben.

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

(Veröffentlichungsdatum - TBD) Dieser Endpunkt ermöglicht einem Workfront-Benutzer (oder eventuell einem automatisierten Workflow-Ereignis), eine Aktion im externen System durchzuführen. Der Endpunkt /customAction akzeptiert einen Parameter &quot;name&quot;, der es dem Webhook-Provider ermöglicht, mehrere benutzerdefinierte Vorgänge zu implementieren.

Der Webhook-Provider registriert benutzerdefinierte Aktionen bei Workfront, indem er die Aktionen in die Antwort /serviceInfo unter customActions einbezieht. Workfront lädt diese Liste beim Einrichten oder Aktualisieren des Webhook-Providers unter Einrichtung > Dokumente > Benutzerdefinierte Integrationen.\
![](assets/mceclip0-350x262.png)

Benutzer können die benutzerdefinierte Aktion durch Auswahl des Bereichs unter &quot;Dokumentaktionen&quot;Trigger haben.\
![](assets/mceclip1-350x95.png)

**URL**

GET /customAction

**Abfrageparameter**

<table style="table-layout:auto">
 <col>
 <col>
 <thead>
  <tr>
   <th>Name </th>
   <th>Beschreibung</th>
  </tr>
 </thead>
 <tbody>
  <tr>
   <td><p>name</p></td>
   <td><p>Die Kennung, die die Art der auszuführenden Aktion angibt. Dieser Wert entspricht einem der customAction -Werte, die vom Endpunkt /serviceInfo zurückgegeben werden.</p></td>
  </tr>
  <tr>
   <td>documentId </td>
   <td>Die Dokument-ID der Arbeitsfläche, für die die Aktion ausgeführt wird.</td>
  </tr>
  <tr>
   <td>documentVersionId </td>
   <td> Die Kennung der Dokumentversion, für die die Aktion ausgeführt wird.</td>
  </tr>
 </tbody>
</table>

 

**Reaktion**

Eine JSON-Zeichenfolge, die den Erfolg oder Fehler angibt, wie im Abschnitt Umgang mit Fehlern unten angegeben. Bei einem Fehler (d. h. Status = &quot;Fehler&quot;) zeigt Workfront die bereitgestellte Fehlermeldung an.

**Beispiel:** https://sample.com/webhooks/customName?name=archive&amp;documentId=5502082c003a4f30 ddec2fb2b739cb7c&amp;documentVersionId=54b598a700e2342d6971597a5df1a8d3

response

```
{
"status": "success" 
}
```


## Umgang mit Fehlern

Bei der Verarbeitung von API-Anfragen können Probleme auftreten. Dies sollte über alle API-Endpunkte hinweg einheitlich gehandhabt werden. Wenn ein Fehler auftritt, führt der Webhook-Provider die folgenden Schritte aus:

* Fügen Sie einen Fehlercode in die Antwortheader ein. Zu den Fehlercodes gehören:

   * 403 - Verboten. Gibt an, dass entweder die Anfrage-Token fehlen oder ungültig sind oder dass die mit den Token verknüpften Anmeldeinformationen keinen Zugriff auf die angegebene Ressource haben. Bei OAuth-basierten Webhook-Anbietern versucht Workfront, neue Zugriffstoken abzurufen.
   * 404 - Nicht gefunden. Gibt an, dass die angegebene Datei oder der angegebene Ordner nicht vorhanden ist.
   * 500 - Interner Server-Fehler. Jeder andere Fehlertyp.

* Beschreiben Sie den Fehler im Antworttext im folgenden Format:


```
{
"status": "error"
"error": "Sample error message" 
}
```


## Test

Führen Sie die folgenden Tests aus, um sicherzustellen, dass Ihre Dokument-Webhook-Implementierung ordnungsgemäß funktioniert. Hierbei handelt es sich um manuelle Tests, die über die Workfront-Web-Oberfläche durchgeführt werden und indirekt die Endpunkte für Ihre Webhook-Implementierung erreichen.

### Voraussetzungen

Zum Ausführen dieser Tests benötigen Sie Folgendes:

* Ein Workfront-Konto mit aktiviertem Advanced Document Management (ADM)
* Ein Workfront-Benutzer für dieses Konto mit Systemadministratorrechten
* Eine Document Webhook-Instanz, auf die die HTTP-Endpunkte von Workfront zugegriffen werden können

Bei diesen Tests wird außerdem davon ausgegangen, dass Sie Ihre Document Webhook-Instanz bereits in Workfront unter Einrichtung > Dokumente > Benutzerdefinierte Integrationen registriert haben.

### Test 1: Bereitstellung des Document Webhook-Dienstes für einen Benutzer

Testen Sie die Authentifizierungs-URL und die Token-Endpunkt-URL für OAuth-basierte Webhook-Provider.

1. Gehen Sie in Workfront zur Hauptseite &quot;Dokumente&quot;, indem Sie in der oberen Navigationsleiste auf den Link Dokumente klicken.
1. Klicken Sie auf das Dropdown-Menü Dokumente hinzufügen und wählen Sie Ihren Document Webhook-Dienst unter Dienst hinzufügen aus.
1. (Nur OAuth-Dienste) Nach Abschluss des vorherigen Schritts wird die OAuth2-Authentifizierungsseite Ihres Dienstes in einem Popup-Fenster geladen. (Hinweis: Sie werden möglicherweise aufgefordert, sich zuerst bei Ihrem Dienst anzumelden.) Gewähren Sie auf der Authentifizierungsseite Workfront Zugriff auf das Benutzerkonto, indem Sie auf die Schaltfläche Vertrauen oder Zulassen klicken.
1. Vergewissern Sie sich, dass Ihr Dienst zum Dropdown-Menü Dokumente hinzufügen hinzugefügt wurde. Wenn Sie ihn anfangs nicht sehen, versuchen Sie, den Browser zu aktualisieren.

### Test 2: Verknüpfen eines Dokuments mit Workfront Tests die folgenden Endpunkte: /files, /metadata

1. Gehen Sie in Workfront zur Hauptseite &quot;Dokumente&quot;, indem Sie in der oberen Navigationsleiste auf den Link Dokumente klicken.
1. Wählen Sie Ihren Document Webhook-Dienst unter Dokumente hinzufügen aus.
1. Navigieren Sie vom Modal aus durch die Ordnerstruktur.
1. Überprüfen Sie, ob Sie in der Lage sind, ordnungsgemäß in der Ordnerstruktur zu navigieren.
1. Auswählen und Verknüpfen eines Dokuments mit Workfront

### Test 3: Navigieren Sie zu einem Dokument im Content Management System.

Testet die folgenden Endpunkte: /metadata (insbesondere viewLink)

1. Dokument in Workfront verknüpfen
1. Wählen Sie das Dokument aus und klicken Sie auf den Link Öffnen .
1. Überprüfen Sie, ob das Dokument in einer neuen Registerkarte geöffnet wird.

### Test 4: Navigieren Sie zu einem Dokument im Content Management System (mit Anmeldung).

Testet die folgenden Endpunkte: /metadata (insbesondere viewLink)

1. Stellen Sie sicher, dass Sie vom Content Management System abgemeldet wurden.
1. Verknüpfen eines Dokuments mit Workfront
1. Wählen Sie das Dokument aus und klicken Sie auf den Link Öffnen .
1. Vergewissern Sie sich, dass der Anmeldebildschirm des Content Management-Systems in einer neuen Registerkarte geladen wird.
1. Melden Sie sich an und vergewissern Sie sich, dass Sie zum Dokument gelangt sind.

### Test 5: Laden Sie das Dokument aus dem Content Management System herunter

Testet die folgenden Endpunkte: /metadata (insbesondere downloadLink)

1. Verknüpfen eines Dokuments mit Workfront
1. Wählen Sie das Dokument aus und klicken Sie auf den Link Herunterladen .
1. Vergewissern Sie sich, dass der Download beginnt.

### Test 6: Suche nach Inhalt

Testet die folgenden Endpunkte: /search

1. Gehen Sie in Workfront zur Hauptseite &quot;Dokumente&quot;, indem Sie in der oberen Navigationsleiste auf den Link Dokumente klicken.
1. Wählen Sie Ihren Document Webhook-Dienst unter Dokumente hinzufügen aus.
1. Führen Sie im Modal eine Suche durch.
1. Überprüfen Sie, ob die Suchergebnisse korrekt sind.

### Test 7: Versand eines Dokuments von Workfront an das Content Management System

Testet die folgenden Endpunkte: /files, /uploadInit, /upload

1. Gehen Sie in Workfront zur Hauptseite &quot;Dokumente&quot;, indem Sie in der oberen Navigationsleiste auf den Link Dokumente klicken.
1. Hochladen eines Dokuments von Ihrem Computer in Workfront
1. Navigieren Sie zur Seite mit den Dokumentdetails .
1. Wählen Sie im Dropdown-Menü Dokumentaktionen unter Senden an Ihren Document Webhook-Dienst aus.
1. Wechseln Sie zum gewünschten Zielordner und klicken Sie auf die Schaltfläche Speichern .
1. Stellen Sie sicher, dass das Dokument an die richtige Stelle im Content Management System hochgeladen wurde.

### Test 8: Anzeigen von Miniaturansichten in Workfront

Testet die folgenden Endpunkte: /thumbnail

1. Verknüpfen eines Dokuments mit Workfront
1. Wählen Sie das Dokument in der Liste aus.
1. Stellen Sie sicher, dass die Miniaturansicht im rechten Bereich angezeigt wird.

### Test 9: Abrufen der Inhalts-Bytes

Testet die folgenden Endpunkte: /download

1. Verknüpfen eines Dokuments mit Workfront
1. Rufen Sie die Seite mit den Dokumentdetails auf.
1. Senden Sie das Dokument an Workfront, indem Sie &quot;Dokumentaktionen&quot;> &quot;Senden an...&quot;> &quot;Workfront&quot;auswählen. Dadurch wird eine neue Dokumentversion in Workfront erstellt.
1. Laden Sie das Dokument von Workfront herunter, indem Sie auf den Link Herunterladen klicken.

### Test 10: Zugriffstoken aktualisieren (nur OAuth2 Webhook-Anbieter)

Testet die folgenden Endpunkte: Token-Endpunkt-URL

1. Bereitstellen eines Document Webhook-Dienstes für einen Benutzer
1. Invalidierung des Zugriffstokens des Benutzers durch 1) Warten auf eine Zeitüberschreitung oder 2) manuelles Invalidieren des Zugriffs-Tokens im externen System.
1. Aktualisieren Sie das Zugriffstoken in Workfront. Dazu können Sie beispielsweise ein Dokument mit Workfront verknüpfen. Sie wissen, dass das Zugriffstoken erfolgreich aktualisiert wurde, wenn Sie zu einem Dokument navigieren und es verknüpfen konnten.

>[!NOTE]
>
>Zurzeit ist die Option Senden an.. nicht für verknüpfte Dokumente verfügbar. Dieser wird von Workfront hinzugefügt. Sie können den Endpunkt /download testen, indem Sie den Endpunkt manuell mithilfe eines REST-Clients wie Postman aufrufen. Alternativ kann der Endpunkt /download durch Generieren eines digitalen Testversands getestet werden. Wenden Sie sich zur Aktivierung des digitalen Testversands an Workfront.

## Versionen

* Version 1.0 (Veröffentlichungsdatum - Mai 2015)

   * Erstspezifikation

* Version 1.1 (Veröffentlichungsdatum - Juni 2015)

   * Aktualisiert /uploadInit - documentId und documentVersionId hinzugefügt

* Version 1.2 (Veröffentlichungsdatum - Oktober 2015)

   * /createFolder hinzugefügt

