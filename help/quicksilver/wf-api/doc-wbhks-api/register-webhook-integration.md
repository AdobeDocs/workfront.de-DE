---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Webhook-Integration registrieren
description: Webhook-Integration registrieren
author: Becky
feature: Workfront API
exl-id: 9a4f8dbe-967f-4a41-a42c-8e3acb604972
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 11%

---


# Webhook-Integration registrieren

Adobe Workfront-Administratoren können eine benutzerdefinierte Webhook-Integration für ihr Unternehmen hinzufügen, indem sie zu Einrichtung > Dokumente > Benutzerdefinierte Integrationen in Workfront navigieren. Auf der Seite Benutzerspezifische Integration unter Einrichtung können Administratoren eine Liste der vorhandenen Dokument-Webhook-Integrationen anzeigen. Auf dieser Seite können Integrationen hinzugefügt, bearbeitet, aktiviert und deaktiviert werden.

Um eine Integration hinzuzufügen, klicken Sie auf **Benutzerspezifische Integration hinzufügen**.

![](assets/webhooks-integration-350x230.png)

![](assets/webhooks-integration-2-350x220.png)

## Verfügbare Felder

Beim Hinzufügen einer Integration gibt der Administrator Werte für die folgenden Felder ein.

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
   <td>Basis-API URL</td> 
   <td> <p>Der Speicherort der Callback-API. Bei Aufrufen an das externe System hängt Workfront einfach den Endpunktnamen an diese Adresse an. Wenn der Administrator beispielsweise die Basis-API-URL "https://www.mycompany.com/api/v1"eingegeben hat, verwendet Workfront die folgende URL, um die Metadaten eines Dokuments zu erhalten: https://www.mycompany.com/api/v1/metadata?id=1234</p> </td> 
  </tr> 
  <tr> 
   <td>Anforderungsparameter</td> 
   <td> <p>Optionale Werte, die an die Abfragezeichenfolge eines jeden API-Aufrufs anzuhängen sind. Beispiel: access_type=offline. </p> </td> 
  </tr> 
  <tr> 
   <td>Authentifizierungstyp</td> 
   <td>OAuth2 oder ApiKey</td> 
  </tr> 
  <tr> 
   <td>Authentifizierungs-URL</td> 
   <td> <p>(Nur OAuth2) Die vollständige URL, die für die Benutzerauthentifizierung verwendet wird. Workfront navigiert Benutzer im Rahmen der OAuth-Bereitstellung zu dieser Adresse. Hinweis: Workfront hängt einen "state"-Parameter an die Abfragezeichenfolge an. Der Provider muss dies zurück an Workfront übergeben, indem er es an den Workfront-Weiterleitungs-URI anhängt.</p> </td> 
  </tr> 
  <tr> 
   <td>Token Endpoint URL</td> 
   <td> <p>(Nur OAuth2) Die vollständige API-URL, die zum Abrufen von OAuth2-Token verwendet wird. Dies wird vom Webhook-Provider oder externen Dokumentenanbieter gehostet</p> </td> 
  </tr> 
  <tr> 
   <td>Client-ID</td> 
   <td>(Nur OAuth2) Die OAuth2-Client-ID für diese Integration</td> 
  </tr> 
  <tr> 
   <td>Geheimer Client-Schlüssel</td> 
   <td> <p>(Nur OAuth2) Das OAuth2-Client-Geheimnis für diese Integration</p> </td> 
  </tr> 
  <tr> 
   <td>Workfront Redirect-URI</td> 
   <td>(Nur OAuth2) Dies ist ein schreibgeschütztes Feld, das von Workfront generiert wird. Dieser Wert wird verwendet, um diese Integration beim externen Dokumentenanbieter zu registrieren. Hinweis: Wie oben für die Authentifizierungs-URL beschrieben, muss der Provider den Parameter "state"und seinen Wert bei der Durchführung der Umleitung an den Abfragezeichenfolgen anhängen.</td> 
  </tr> 
  <tr> 
   <td>ApiKey</td> 
   <td> <p>(Nur APIKey) Wird verwendet, um autorisierte API-Aufrufe an den Webhook-Provider durchzuführen. Der vom Webhook-Provider ausgegebene API-Schlüssel.</p> </td> 
  </tr> 
 </tbody> 
</table>
