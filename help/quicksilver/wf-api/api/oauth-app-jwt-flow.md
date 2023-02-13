---
content-type: api
navigation-topic: api-navigation-topic
title: Verwenden des JWT-Flusses für benutzerdefinierte OAuth 2-Anwendungen
description: Verwenden des JWT-Flusses für benutzerdefinierte OAuth 2-Anwendungen
author: John
feature: Workfront API
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
source-git-commit: 38e957253775f73cee7fe0c0d31bfeedb58ebf53
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Benutzerdefinierte OAuth 2-Anwendungen Ihres Unternehmens mithilfe des JWT-Flusses konfigurieren und verwenden

Um in Workfront integriert zu werden und die Kommunikation Ihrer Client-App mit Workfront im Namen des Benutzers zu ermöglichen, müssen Sie:

* Erstellen einer OAuth2-Anwendung
* Zertifikat mit öffentlichem Schlüssel erstellen
* JSON-Web-Token (JWT) erstellen

## Erstellen einer OAuth2-Anwendung

Anweisungen zum Erstellen der OAuth2-Anwendung finden Sie unter [Erstellen einer OAuth2-Anwendung mithilfe der Serverauthentifizierung (JWT-Fluss)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2) in [OAuth2-Anwendungen für Workfront-Integrationen erstellen](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Zertifikat mit öffentlichem Schlüssel erstellen

Das JWT muss signiert und base-64-kodiert sein, damit es in die Zugriffsanfrage aufgenommen werden kann. Die JWT-Bibliotheken bieten Funktionen zum Ausführen dieser Aufgaben.

Das Token muss mit dem privaten Schlüssel für ein digitales Signaturzertifikat signiert werden. Wenn Sie dies tun, können Sie den privaten Schlüssel jedes zugehörigen Zertifikats verwenden, um Ihr JWT zu signieren.

Der verwendete Algorithmus ist RS256 (RSA Signature with SHA-256). Dies ist ein asymmetrischer Algorithmus, der ein Schlüsselpaar aus öffentlichem/privatem Schlüssel verwendet. Der Identitätsanbieter verfügt über einen privaten (geheimen) Schlüssel, mit dem die Signatur generiert wird, und der Verbraucher des JWT erhält einen öffentlichen Schlüssel, um die Signatur zu validieren.

Um den öffentlichen Schlüssel zu generieren, führen Sie folgende Schritte aus: **one** des Folgenden.

* Öffnen Sie Ihr MacOS/Linux-Terminal und führen Sie den folgenden Befehl aus. Laden Sie dann `certificate_pub.crt` mithilfe der **Hinzufügen eines öffentlichen Schlüssels** in der OAuth2-Anwendungseinrichtung in Workfront.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* Verwenden Sie die **Generieren eines öffentlichen/privaten Keypairs** in der OAuth2-Anwendungseinrichtung in Workfront, um den RSA zu generieren.

## JSON-Web-Token erstellen

Ein JSON-Web-Token für die Authentifizierung von Dienstkonten erfordert einen bestimmten Satz von Ansprüchen und muss mit einem gültigen digitalen Signaturzertifikat signiert werden. Es wird empfohlen, eine der öffentlich verfügbaren Bibliotheken oder Tools zum Erstellen Ihres JWT zu verwenden.

Die folgende Tabelle enthält Informationen zu Feldern, die bei der Konfiguration des JWT-Tokens erforderlich sein können.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">exp</td> 
   <td> <p>Erforderlich. Der Ablaufparameter ist ein erforderlicher Parameter, der die absolute Zeit seit dem 1.1.1970 GMT misst. Sie müssen sicherstellen, dass die Ablaufzeit nach dem Zeitpunkt des Problems liegt. Danach ist das JWT nicht mehr gültig. </p> <p>Hinweis: Es wird empfohlen, ein sehr kurzlebiges Token (einige Minuten) zu verwenden, damit es bald abläuft, nachdem es gegen ein Zugriffstoken ausgetauscht wurde. Jedes Mal, wenn ein neues Zugriffstoken erforderlich ist, wird ein JWT signiert und ausgetauscht. Dies ist ein sichererer Ansatz. Wir empfehlen keine langlebigen Token, die bei Bedarf wiederverwendet werden, um Zugriffstoken zu erhalten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">is</td> 
   <td>Erforderlich. Der Emittent ist Ihre Kunden-ID aus den OAuth2-App-Details.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">sub</td> 
   <td>Erforderlich. Der Betreff ist Ihre Benutzer-ID, mit der der öffentliche Schlüssel bei der Einrichtung erstellt wurde.</td> 
  </tr> 
 </tbody> 
</table>

## JWT ersetzen, um ein Zugriffstoken abzurufen

1. Senden Sie eine POST-Anfrage an:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. Der Hauptteil der Anfrage sollte URL-kodierte Parameter mit Ihrer Client-ID, dem Client-Geheimnis und JWT enthalten:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

 
