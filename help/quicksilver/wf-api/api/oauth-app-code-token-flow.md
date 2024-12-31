---
content-type: api
navigation-topic: api-navigation-topic
title: Autorisierungs-Code-Fluss für benutzerdefinierte OAuth 2-Anwendungen
description: Autorisierungs-Code-Fluss für benutzerdefinierte OAuth 2-Anwendungen
author: Becky
feature: Workfront API
role: Developer
exl-id: a1ab60c4-4255-4d80-87f1-f36d325254c2
source-git-commit: e41b0df5ee0ce092f0811b18c57f6865bbb3abee
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---


# Konfigurieren und verwenden Sie die benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des Autorisierungs-Code-Flusses

Um mit Workfront zu integrieren und Ihrer Client-Anwendung zu ermöglichen, im Namen der Benutzerin bzw. des Benutzers mit Workfront zu kommunizieren, ist Folgendes erforderlich:

* Erstellen eines OAuth2-Programms
* Konfigurieren der Drittanbieteranwendung
* Link zur Autorisierungsseite für Ihre Benutzer
* Einrichten des Autorisierungs-Code-Flusses: Benutzer melden sich bei der Workfront-Instanz an und stimmen zu, dass sie der Client-Anwendung erlauben, in ihrem Namen eine Verbindung zu Workfront herzustellen. Als Ergebnis erhalten Sie einen Autorisierungs-Code, den Sie mit Zugriffs- und Aktualisierungs-Token austauschen.
* Einrichten des Aktualisierungs-Token-Flusses: In diesem Fluss verwenden Sie das Aktualisierungs-Token, um ein neues Zugriffs-Token zu erhalten, wenn das alte abgelaufen ist.

## Erstellen einer OAuth2-Anwendung

Anweisungen zum Erstellen der OAuth2-Anwendung finden Sie unter [Erstellen einer OAuth2-Anwendung mit Benutzeranmeldeinformationen (Autorisierungs-Code-Fluss)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create3) in [Erstellen von OAuth2-Anwendungen für Workfront-Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md)

>[!NOTE]
>
>Sie können bis zu zehn OAuth2-Anwendungen gleichzeitig haben.

## Link zur Autorisierungsseite für Ihre Benutzer

Ihre Benutzer müssen sich anmelden, um diese Integration in ihrem eigenen Konto zu autorisieren. Die Seite, die autorisiert werden soll, weist ein bestimmtes Format auf, das hier beschrieben wird. Verwenden Sie diese Informationen, um die Adresse der Autorisierungsseite für die App zu bestimmen und Ihren Benutzern diese Adresse oder einen Link dazu bereitzustellen.

* Die vollständige URL der Domain Ihres Unternehmens. Beispiel:

  ```
  https://myorganization.my.workfront.com
  ```


* `client_id`: Dies ist die Client-ID, die beim Erstellen der OAuth2-App in Workfront generiert wurde.

* `redirect_uri`: Diese URL muss mit der Umleitungs-URL übereinstimmen, die Sie beim Erstellen der OAuth2-App in Workfront eingegeben haben. Ihre Benutzer werden auf diese Seite weitergeleitet, nachdem sie die App für ihr Konto autorisiert haben.

* `response_type`: Dieser muss den Wert `code` haben.

Die URL für die Autorisierungsseite lautet daher:

```
https://<URL of your organization's domain>/integrations/oauth2/authorize?client_id=<Your ClientID>&redirect_uri=<Your redirect URL>&response_type=code
```

>[!NOTE]
>
>Es wird empfohlen, eine Schaltfläche oder einen anderen Link zu erstellen, auf die bzw. den Ihre Benutzer klicken können, um zu dieser Seite weitergeleitet zu werden.

## Konfigurieren der Drittanbieteranwendung

Die Drittanbieteranwendung muss möglicherweise konfiguriert werden. Die folgende Tabelle enthält Informationen zu den Feldern, die möglicherweise erforderlich sind, wenn Sie die Drittanbieteranwendung konfigurieren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Autorisierungs-URI</td> 
   <td> <p><code>https://&lt;the full URL of your organization's domain&gt;/integrations/oauth2/authorize</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code> https://myorganization.my.workfront.com/integrations/oauth2/authorize</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Token-URL</td> 
   <td> <p><code>https://&lt;the full URL of your organization's domain&gt;/integrations/oauth2/api/v1/token</code> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span><code>https://myorganization.my.workfront.com/integrations/oauth2/api/v1/token</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Bereiche</td> 
   <td>Sie müssen keine Bereiche angeben. </td> 
  </tr> 
 </tbody> 
</table>

## Einrichten des Autorisierungs-Code-Flusses

![](assets/oauth-2-authorization-code-flow.png)

Verwenden Sie den folgenden Prozess, um Ihre Benutzer mit OAuth2 anzumelden:

1. Wenn der/die Benutzende die Autorisierungsseite öffnet, wird sie zur Anmeldeseite von Workfront weitergeleitet, damit der/die Benutzende sich bei Workfront anmelden kann. Wenn der Benutzer über eine SSO-Konfiguration verfügt, wird die Anmeldeseite des Identitätsanbieters geöffnet.

   Wenn der Benutzer bereits mit demselben Browser bei Workfront angemeldet ist oder er sich erfolgreich bei Workfront anmeldet, wird der Benutzer zum Einverständnisbildschirm weitergeleitet:

   ![](assets/consent-screen-350x227.png)

1. Wenn der Benutzer den Zugriff zulässt, wird die Seite zum `redirect_url` umgeleitet. Die Umleitung muss die folgenden Abfrageparameter enthalten:

* `code`: Der Autorisierungs-Code, der zum Abrufen des Zugriffs-/Aktualisierungs-Tokens erforderlich ist.
* `domain`: Die Domain Ihres Unternehmens. Beispiel: In `myorganization.my.workfront.com` ist die Domain `myorganization`.
* `lane`: Die Spur der Anfrage. Beispiel: In `myorganization.preview.workfront.com` ist die Spur `preview`.

  >[!IMPORTANT]
  >
  >Die `code` ist nur 2 Minuten lang gültig. Daher müssen Sie die Aktualisierungs- und Zugriffs-Token innerhalb dieser Zeit erhalten.

1. Wenn Sie über einen Code verfügen, können Sie Aktualisierungs- und Zugriffstoken anfordern, indem Sie den Code zusammen mit den Anmeldeinformationen der Client-Anwendung an den `/integrations/oauth2/api/v1/token`-Endpunkt senden.

   Die vollständige Token-Anforderungs-URL lautet

   ```
   https://<URL of your organization's domain></span>/integrations/oauth2/api/v1/token
   ```

   **Beispiele:** Beispiel für einen CURL-Aufruf an den Token-Endpunkt:

   Beispiel 1

   ```
      curl --location --request POST '**<workfront host>**/integrations/oauth2/api/v1/token' \
      --header 'Authorization: Basic **<base64(client_id:client_secret)>**' \
      --header 'Content-Type: application/json' \
      --data-raw '{
      "code": "**<code>**",
      "grant_type": "**authorization_code**",
      "redirect_uri": "**<redirect_url>**"
      }'
   ```

   Beispiel 2

   ```
      curl --location --request POST '**<workfront host>**/integrations/oauth2/api/v1/token' \
      --header 'Content-Type: application/x-www-form-urlencoded' \
      --data-urlencode 'grant_type=**authorization_code**' \
      --data-urlencode 'redirect_uri=**<redirect_url>**' \
      --data-urlencode 'code=**<code>**' \
      --data-urlencode 'client_id=**<client_id>**' \
      --data-urlencode 'client_secret=**<client_secret>**'  
   ```


   >[!IMPORTANT]
   >
   > Das Client-Geheimnis wurde bei der Registrierung der App in Workfront generiert. Sie sollten sie an einem sicheren Ort aufbewahren, da sie bei Verlust nicht wiederhergestellt werden kann.

   Wenn alle übergebenen Parameter korrekt sind, gibt der Token-Endpunkt die folgende Payload zurück:

   ```
   {
      "token_type": "sessionID",
      "access_token": "string", // the value of sessionID
      "refresh_token": "string",
      "expires_in": 0,
      "wid": "string"
   }
   ```

   Das Zugriffstoken ist dasselbe wie ```sessionID``` und läuft genauso ab wie das normale ```sessionID```

   >[!IMPORTANT]
   >
   > Speichern Sie das Aktualisierungs-Token an einem sicheren Ort. Sie benötigen es, um ein neues Aktualisierungs-Token zu erhalten, wenn das alte abgelaufen ist. Workfront speichert Ihr Aktualisierungs-Token nicht.

1. Wenn Sie jetzt über ein Zugriffstoken verfügen, können Sie API-Aufrufe an Workfront durchführen

   ```
   curl --request GET 'https://<workfront host>/attask/api/v14.0/proj/search \
   --header 'sessionID: <access_token>'
   ```

## Einrichten eines Aktualisierungs-Zugriffstoken

![](assets/refresh-access-token-flow-350x142.png)

Um das Zugriffs-Token zu aktualisieren, müssen wir erneut einen &quot;POST&quot;-Aufruf an den Token-Endpunkt durchführen. Dieses Mal senden wir ein anderes Formular Daten wie folgt:

```
curl --location --request POST '<workfront host>/integrations/oauth2/api/v1/token' \
--header 'Authorization: Basic <base64(client_id:client_secret)>' \
--header 'Content-Type: application/json' \
--data-raw '{
   "grant_type": "refresh_token",
   "refresh_token": "<refresh_token>"
}'

###### OR

curl --location --request POST '<workfront host>/integrations/oauth2/api/v1/token' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--data-urlencode 'grant_type=refresh_token' \
--data-urlencode 'redirect_uri=<redirect_url>' \
--data-urlencode 'refresh_token=<refresh_token>' \
--data-urlencode 'client_id=<client_id>' \
--data-urlencode 'client_secret=<client_secret>'
```

Es wird das folgende Ergebnis zurückgegeben:

```
{
  "token_type": "sessionID",
  "access_token": "string", // the value of sessionID
  "refresh_token": "string",
  "expires_in": 0,
  "wid": "string"
}
```

Auch hier ist das Zugriffstoken der `sessionID`, der für eine API-Anfrage an Workfront verwendet werden kann.
