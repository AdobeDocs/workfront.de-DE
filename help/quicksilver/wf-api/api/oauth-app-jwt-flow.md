---
content-type: api
navigation-topic: api-navigation-topic
title: Verwenden des JWT-Flusses für benutzerdefinierte OAuth 2-Anwendungen
description: Verwenden des JWT-Flusses für benutzerdefinierte OAuth 2-Anwendungen
author: Becky
feature: Workfront API
role: Developer
exl-id: 4bd56fe6-1f36-4c36-82cd-96de748ad680
source-git-commit: 6f041459caf040846ffdec5bc75e9d74c99e318b
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Konfigurieren und verwenden Sie die benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des JWT-Flusses

Um mit Workfront zu integrieren und Ihrer Client-Anwendung zu ermöglichen, im Namen der Benutzerin bzw. des Benutzers mit Workfront zu kommunizieren, ist Folgendes erforderlich:

* Erstellen eines OAuth2-Programms
* Erstellen eines Zertifikats mit öffentlichem Schlüssel
* Erstellen eines JSON Web Token (JWT)

## Erstellen einer OAuth2-Anwendung

Anweisungen zum Erstellen der OAuth2-Anwendung finden Sie unter [Erstellen einer OAuth2-Anwendung mit Serverauthentifizierung (JWT-Fluss)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create2) in [Erstellen von OAuth2-Anwendungen für Workfront-Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md)

>[!NOTE]
>
>Sie können bis zu zehn OAuth2-Anwendungen gleichzeitig haben.

## Erstellen eines Zertifikats mit öffentlichem Schlüssel

Das JWT muss signiert und Base-64-codiert sein, damit es in die Zugriffsanfrage aufgenommen werden kann. Die JWT-Bibliotheken bieten Funktionen zum Ausführen dieser Aufgaben.

Das Token muss mit dem privaten Schlüssel für ein digitales Signaturzertifikat signiert werden. In diesem Fall können Sie den privaten Schlüssel eines beliebigen zugehörigen Zertifikats verwenden, um Ihr JWT zu signieren.

Der verwendete Algorithmus ist RS256 (RSA Signature with SHA-256). Dies ist ein asymmetrischer Algorithmus, der ein Schlüsselpaar aus öffentlichem/privatem Schlüssel verwendet. Der Identitätsanbieter verfügt über einen privaten (geheimen) Schlüssel zum Generieren der Signatur, und der Benutzer des JWT erhält einen öffentlichen Schlüssel zum Validieren der Signatur.

Um den öffentlichen Schlüssel zu generieren **führen Sie** der folgenden Schritte aus.

* Öffnen Sie Ihr MacOS/Linux-Terminal und führen Sie den folgenden Befehl aus und laden Sie dann `certificate_pub.crt` mithilfe der Schaltfläche **Öffentlichen Schlüssel hinzufügen** im Setup der OAuth2-Anwendung in Workfront hoch.

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>openssl req -x509 -sha256 -nodes -newkey rsa:2048 -keyout private.key -out certificate_pub.crt</code></pre>

* Verwenden Sie die Schaltfläche **Schlüsselpaar aus öffentlichem/privatem Schlüssel generieren** im OAuth2-Programm-Setup in Workfront, um die RSA zu generieren.

## Erstellen eines JSON-Web-Tokens

Ein JSON-Web-Token für die Authentifizierung des Service-Kontos erfordert einen bestimmten Satz von Ansprüchen und muss mit einem gültigen digitalen Signaturzertifikat signiert werden. Es wird empfohlen, eine der öffentlich verfügbaren Bibliotheken oder Tools zum Erstellen des JWT zu verwenden.

Die folgende Tabelle enthält Informationen zu Feldern, die möglicherweise erforderlich sind, wenn Sie das JWT-Token konfigurieren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Exp</td> 
   <td> <p>Erforderlich. Der Parameter Ablauf ist ein erforderlicher Parameter, der die absolute Zeit seit dem 01/01/1970 GMT misst. Sie müssen sicherstellen, dass die Ablaufzeit nach dem Zeitpunkt der Anfrage liegt. Nach dieser Zeit ist der JWT nicht mehr gültig. </p> <p>Hinweis: Es wird empfohlen, über ein Token mit sehr kurzer Lebensdauer (einige Minuten) zu verfügen, damit es bald abläuft, nachdem es gegen ein Zugriffs-Token eingetauscht wurde. Jedes Mal, wenn ein neues Zugriffstoken erforderlich ist, wird ein JWT signiert und ausgetauscht. Dies ist ein sichererer Ansatz. Wir empfehlen nicht länger laufende Token, die wiederverwendet werden, um bei Bedarf Zugriffs-Token zu erhalten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ISS</td> 
   <td>Erforderlich. Aussteller ist Ihre Kunden-ID aus den OAuth2-App-Details.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Untergruppe</td> 
   <td>Erforderlich. Der Betreff ist Ihre Benutzer-ID, die den öffentlichen Schlüssel bei der Einrichtung erstellt hat.</td> 
  </tr> 
 </tbody> 
</table>

## Austauschen des JWT zum Abrufen eines Zugriffs-Tokens

1. Anforderung einer POST senden an:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>https://yourdomain.my.workfront.com/integrations/oauth2/api/v1/jwt/exchange</code></pre>

1. Der Text der Anfrage sollte URL-kodierte Parameter mit Ihrer Client-ID, Ihrem Client-Geheimnis und JWT enthalten:

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>client_id={client_id_value}&client_secret={client_secret_value}&jwt_token={base64_encoded_JWT}</code></pre>

 
