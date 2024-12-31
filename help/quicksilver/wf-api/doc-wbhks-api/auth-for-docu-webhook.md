---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Authentifizierung für Dokument-Webhooks
description: Authentifizierung für Dokument-Webhooks
author: Becky
feature: Workfront API
role: Developer
exl-id: 2303c202-27c7-4922-a613-e9824910504c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Authentifizierung für Dokument-Webhooks

## Authentifizierung

Adobe Workfront-Dokument-Webhooks unterstützen zwei verschiedene Authentifizierungsformen: OAuth2 und ApiKey. In beiden Fällen übergibt Workfront bei einem API-Aufruf Authentifizierungs-Token in der -Kopfzeile.

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

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Adding Request Headers (optional)</h3>
<p>In addition to using either OAuth2 tokens or an ApiKey for authentication, Workfront can send a predefined set of headers to the webhook provider for every API call. A Workfront admin can setup set this up when&nbsp;registering or editing a Webook Integration, as described in the section above. See Registering a Webhook Integration.</p>
<p>For example, this can be used for Basic Authentication. To do this, the Workfront administrator would add the following Request Header information in the Custom Integration dialog:</p>
<p>&nbsp; &nbsp; &nbsp;Authorization Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ==</p>
<p>where QWxhZGRpbjpvcGVuIHNlc2FtZQ== is a base-64 encoded string of "username:password". See Basic Authentication . Provided that this added, Workfront will pass this in the HTTP request header, in addition to other request headers:&nbsp;</p>
<p>-------------------------------</p>
<p>apiKey: 12345</p>
<p>username: johndoe@foo.com</p>
<p>Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ== ­­­­­­­­­­­­­­­­­­­­­­­­­­</p>
<p>-------------------------------</p>
</div>
-->
