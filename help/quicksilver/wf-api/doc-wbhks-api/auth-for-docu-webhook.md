---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Authentifizierung für Document Webhooks
description: Authentifizierung für Document Webhooks
author: Becky
feature: Workfront API
role: Developer
exl-id: 2303c202-27c7-4922-a613-e9824910504c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Authentifizierung für Document Webhooks

## Authentifizierung

Adobe Workfront Document Webhooks unterstützt zwei verschiedene Authentifizierungsformen: OAuth2 und ApiKey. In beiden Fällen übergibt Workfront beim Ausführen eines API-Aufrufs Authentifizierungstoken in der Kopfzeile.

### OAuth2

Mit OAuth2 kann Workfront im Auftrag eines Benutzers autorisierte API-Aufrufe an einen Webhook-Provider senden. Dazu muss der Benutzer sein externes Document Provider-Konto mit Workfront verbinden und Workfront gewähren

Zugang zu Handlungen in ihrem Namen. Dieser Handshaking-Prozess erfolgt nur einmal für jeden Benutzer. So funktioniert es:

1. Der Benutzer beginnt damit, die Webhook-Integration mit seinem Konto zu verbinden. Dies geschieht derzeit durch Klicken auf das Dropdown-Menü &quot;Dokument hinzufügen&quot;> &quot;Dienst hinzufügen&quot;> &quot;Name der benutzerdefinierten Integration&quot;.
1. Workfront navigiert zum Benutzer über die Authentifizierungs-URL, die ihn auffordern kann, sich beim externen Dokumentenanbieter anzumelden. Diese Seite wird vom Webhook Provider oder vom externen Dokumentenverwaltungssystem gehostet. Dadurch fügt Workfront der Authentifizierungs-URL einen &quot;state&quot;-Parameter hinzu. Dieser Wert muss zurück an Workfront übergeben werden, indem der gleiche Wert im folgenden Schritt an den Workfront-URI angehängt wird.
1. Nach der Anmeldung beim externen System (oder wenn der Benutzer bereits angemeldet ist) wird der Benutzer zu einer &quot;Authentifizierungsseite&quot;geleitet, auf der erklärt wird, dass Workfront Zugriff anfordert, um eine Reihe von Aktionen im Namen des Benutzers durchzuführen.
1. Wenn der Benutzer auf die Schaltfläche &quot;Zulassen&quot;klickt, leitet der Browser zum Workfront-Weiterleitungs-URI um und fügt &quot;code=`<code>`&quot; zum Querystring hinzu. Gemäß der OAuth2-Spezifikation ist dieses Token kurzlebig. Die Abfragezeichenfolge muss auch die folgende sein: &quot;state=`<sent_by_workfront>`&quot;.
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
