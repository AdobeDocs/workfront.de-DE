---
content-type: api
navigation-topic: api-navigation-topic
title: Genehmigungs-Code-Ablauf für benutzerdefinierte OAuth 2-Anwendungen
description: Genehmigungs-Code-Ablauf für benutzerdefinierte OAuth 2-Anwendungen
author: Becky
feature: Workfront API
role: Developer
exl-id: a1ab60c4-4255-4d80-87f1-f36d325254c2
source-git-commit: e41b0df5ee0ce092f0811b18c57f6865bbb3abee
workflow-type: tm+mt
source-wordcount: '717'
ht-degree: 0%

---


# Benutzerdefinierte OAuth 2-Anwendungen Ihres Unternehmens mithilfe des Autorisierungscode-Flusses konfigurieren und verwenden

Um die Integration mit Workfront zu ermöglichen und die Kommunikation Ihrer Client-App mit Workfront im Namen des Benutzers zu ermöglichen, müssen Sie:

* Erstellen einer OAuth2-Anwendung
* Drittanbieteranwendung konfigurieren
* Link zur Autorisierungsseite für Ihre Benutzer
* Einrichten des Autorisierungscodeflusses: Benutzer melden sich bei der Workfront-Instanz an und stimmen zu, dass sie der Client-Anwendung erlauben, in ihrem Namen eine Verbindung zu Workfront herzustellen. Daher erhalten Sie einen Autorisierungscode, den Sie mit Zugriffs- und Aktualisierungstoken austauschen.
* Aktualisierungstoken-Fluss einrichten: In diesem Fluss verwenden Sie das Aktualisierungstoken, um ein neues Zugriffstoken zu erhalten, wenn das alte abgelaufen ist.

## Erstellen einer OAuth2-Anwendung

Anweisungen zum Erstellen der OAuth2-Anwendung finden Sie unter [Erstellen einer OAuth2-Anwendung mit Benutzeranmeldeinformationen (Autorisierungscode-Fluss)](../../administration-and-setup/configure-integrations/create-oauth-application.md#create3) in [Erstellen von OAuth2-Anwendungen für Workfront-Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md) .

>[!NOTE]
>
>Sie können bis zu zehn OAuth2-Anwendungen gleichzeitig haben.

## Link zur Autorisierungsseite für Ihre Benutzer

Ihre Benutzer müssen sich anmelden, um diese Integration in ihrem eigenen Konto zu autorisieren. Die Seite, die sie autorisieren können, hat ein bestimmtes Format, wie hier beschrieben. Verwenden Sie diese Informationen, um die Adresse der Autorisierungsseite für die App zu ermitteln und Ihren Benutzern diese Adresse oder einen Link darauf bereitzustellen.

* Die vollständige URL der Domäne Ihres Unternehmens. Beispiel:

  ```
  https://myorganization.my.workfront.com
  ```


* `client_id`: Dies ist die Client-ID, die beim Erstellen der OAuth2-App in Workfront generiert wurde.

* `redirect_uri`: Diese URL muss mit der Umleitungs-URL übereinstimmen, die Sie beim Erstellen der OAuth2-App in Workfront eingegeben haben. Ihre Benutzer werden zu dieser Seite weitergeleitet, nachdem sie die App für ihr Konto autorisiert haben.

* `response_type`: Dieser Wert muss den Wert `code` haben.

Die URL für die Autorisierungsseite lautet daher:

```
https://<URL of your organization's domain>/integrations/oauth2/authorize?client_id=<Your ClientID>&redirect_uri=<Your redirect URL>&response_type=code
```

>[!NOTE]
>
>Es wird empfohlen, eine Schaltfläche oder einen anderen Link zu erstellen, auf den Ihre Benutzer klicken können, um zu dieser Seite weitergeleitet zu werden.

## Drittanbieteranwendung konfigurieren

Die Drittanbieteranwendung erfordert möglicherweise eine Konfiguration. Die folgende Tabelle enthält Informationen zu Feldern, die bei der Konfiguration der Drittanbieteranwendung erforderlich sein können.

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

## Einrichten des Autorisierungscode-Flusses

![](assets/oauth-2-authorization-code-flow.png)

Um Ihre Benutzer mit OAuth2 anzumelden, gehen Sie wie folgt vor:

1. Wenn der Benutzer die Autorisierungsseite öffnet, wird er zur Workfront-Anmeldeseite weitergeleitet, damit er sich bei Workfront anmelden kann. Wenn der Benutzer über eine SSO-Konfiguration verfügt, wird die Anmeldeseite des Identitäts-Providers geöffnet.

   Wenn der Benutzer bereits im selben Browser bei Workfront angemeldet ist oder sich der Benutzer erfolgreich bei Workfront anmeldet, wird der Benutzer zum Bildschirm für die Zustimmung weitergeleitet:

   ![](assets/consent-screen-350x227.png)

1. Wenn der Benutzer den Zugriff zulässt, wird die Seite zu &quot;`redirect_url`&quot;umgeleitet. Die Umleitung muss die folgenden Abfrageparameter enthalten:

* `code`: Der Autorisierungscode, der zum Abrufen des Zugriffs-/Aktualisierungstokens erforderlich ist.
* `domain`: Die Domäne Ihres Unternehmens. Beispiel: In `myorganization.my.workfront.com` ist die Domäne `myorganization`.
* `lane`: die Spur der Anfrage. Beispiel: In `myorganization.preview.workfront.com` ist die Spur `preview`.

  >[!IMPORTANT]
  >
  >Die `code` ist nur für 2 Minuten gültig. Daher müssen Sie die Aktualisierungs- und Zugriffstoken innerhalb dieser Zeit abrufen.

1. Wenn Sie über einen Code verfügen, können Sie eine Aktualisierung anfordern und auf Token zugreifen, indem Sie den Code zusammen mit den Anmeldeinformationen der Client-App an den Endpunkt `/integrations/oauth2/api/v1/token` senden.

   Die vollständige Token-Anforderungs-URL lautet

   ```
   https://<URL of your organization's domain></span>/integrations/oauth2/api/v1/token
   ```

   **Beispiele:** Beispiel für CURL-Aufruf an Token-Endpunkt:

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
   > Das Client-Geheimnis wurde bei der Registrierung der App in Workfront generiert. Sie sollten ihn an einem sicheren Ort speichern, da er nicht wiederhergestellt werden kann, wenn er verloren geht.

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

   Das Zugriffstoken ist mit ```sessionID``` identisch und läuft genauso ab wie regulärer ```sessionID```

   >[!IMPORTANT]
   >
   > Speichern Sie das Aktualisierungs-Token an einer sicheren Stelle. Sie benötigen es, um ein neues Aktualisierungstoken zu erhalten, wenn das alte abgelaufen ist. Workfront speichert Ihr Aktualisierungstoken nicht.

1. Wenn Sie jetzt über ein Zugriffstoken verfügen, können Sie API-Aufrufe an Workfront durchführen

   ```
   curl --request GET 'https://<workfront host>/attask/api/v14.0/proj/search \
   --header 'sessionID: <access_token>'
   ```

## Zugriffstoken aktualisieren einrichten

![](assets/refresh-access-token-flow-350x142.png)

Um das access_token zu aktualisieren, müssen wir erneut einen &#39;POST&#39;-Aufruf an den Token-Endpunkt durchführen. Diesmal senden wir wie folgt unterschiedliche Formulardaten:

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

Und auch das Zugriffstoken ist der `sessionID` , der verwendet werden kann, um eine API-Anfrage an Workfront zu richten.
