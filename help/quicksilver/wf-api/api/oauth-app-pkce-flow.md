---
content-type: api
navigation-topic: api-navigation-topic
title: PKCE-Fluss für OAuth 2-Anwendungen verwenden
description: PKCE-Fluss für OAuth 2-Anwendungen verwenden
author: Becky
feature: Workfront API
role: Developer
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
source-git-commit: 6f041459caf040846ffdec5bc75e9d74c99e318b
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---

# Benutzerdefinierte OAuth 2-Anwendungen Ihres Unternehmens mithilfe des PKCE-Flusses konfigurieren und verwenden

PKCE ist ein sicherer Autorisierungsfluss, der gut mit dynamisch aktualisierten Anwendungen wie Apps funktioniert, aber für alle OAuth2-Clients nützlich ist. Statt eines statischen Client-Geheimnisses verwendet PKCE eine dynamisch generierte Zeichenfolge, wodurch das Risiko eines durchgesickerten Client-Geheimnisses entfällt.

## PKCE - Übersicht

Ein PKCE-Fluss umfasst die folgenden Schritte. Die Schritte in diesem Abschnitt werden nur zu Informationszwecken beschrieben. Weitere Informationen zur Durchführung dieser Verfahren finden Sie in anderen Abschnitten dieses Artikels.

1. Der Client erstellt die `code_challenge`, indem er die `code_verifier` mit der `S256`-Verschlüsselung transformiert.

1. Der Client leitet den Browser zusammen mit dem generierten `code_challenge` zur OAuth2-Anmeldeseite. Sie müssen Ihre App (den Client) registrieren, damit OAuth2 die Autorisierungsanforderung annehmen kann. Nach der Registrierung kann Ihre App den Browser zu OAuth2 umleiten.

1. Der OAuth2-Autorisierungsserver leitet die Authentifizierungsaufforderung an den Benutzer weiter.

1. Der Benutzer authentifiziert sich mit einer der konfigurierten Anmeldeoptionen und kann eine Einverständnisseite sehen, auf der die Berechtigungen aufgelistet werden, die OAuth2 der Anwendung erteilt.

1. OAuth2 leitet mit einem `authorization code` zurück zu Ihrer Anwendung.

1. Ihre Anwendung sendet diesen Code zusammen mit dem `code_verifier` an OAuth2.

1. Der OAuth2-Autorisierungsserver transformiert die `code_verifier` mit dem `code_challenge_method` aus der ursprünglichen Autorisierungsanfrage und überprüft das Ergebnis mit dem `code_challenge`. Wenn der Wert beider Zeichenfolgen übereinstimmt, hat der Server überprüft, ob die Anforderungen von demselben Client stammen, und gibt einen `access token` aus.

1. OAuth2 gibt die `access token` und optional eine `refresh token` zurück.

1. Ihre Anwendung kann diese Token jetzt verwenden, um den Ressourcenserver, z. B. eine API, im Namen des Benutzers aufzurufen.

1. Der Ressourcenserver validiert das Token, bevor er auf die Anfrage antwortet.


## Anwendung konfigurieren

Bevor Sie die Autorisierung implementieren können, müssen Sie Ihre App in OAuth2 registrieren, indem Sie eine App-Integration aus Workfront erstellen.

Anweisungen zum Erstellen der OAuth2-Anwendung finden Sie unter [Erstellen einer OAuth2-Single-Page-Webanwendung mit PKCE](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce) in [Erstellen von OAuth2-Anwendungen für Workfront-Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md) .

>[!NOTE]
>
>Sie können bis zu zehn OAuth2-Anwendungen gleichzeitig haben.


## Erstellen des Testschlüssels für den Code Exchange

Ähnlich wie beim standardmäßigen Autorisierungscode-Fluss leitet Ihre App den Browser des Benutzers an den `/authorize` -Endpunkt Ihres Autorisierungsservers weiter. In diesem Fall müssen Sie jedoch auch eine Code-Herausforderung weitergeben.

Ihr erster Schritt besteht darin, einen Code-Prüfer und eine Herausforderung zu erstellen.

<table>
  <col/>
  <col/>
    <tbody>
      <tr>
        <td role="rowheader">Code-Prüfer</td>
        <td>
          <p>Zufällige URL-sichere Zeichenfolge mit mindestens 43 Zeichen</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Code-Herausforderung</td>
        <td>
          <p>Base64 URL-kodierter SHA-256-Hash des Code-Verifikators</p>
        </td>
      </tr>
    </tbody>
</table>


Sie müssen Code in Ihrer Client-App hinzufügen, um die Codeüberprüfung und die Codeherausforderung zu erstellen.

Der PKCE Generator-Code erstellt eine Ausgabe ähnlich der folgenden:

>[!INFO]
>
>**Beispiel:**
>
>```
>{
>  "code\_verifier":"N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat",
>  "code\_challenge":"wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>}
>```

Ihre App speichert den `code_verifier` für später und sendet den `code_challenge` zusammen mit der Autorisierungsanfrage an die `/authorize` -URL Ihres Autorisierungsservers.

## Autorisierungscode anfordern

Wenn Sie den standardmäßigen benutzerdefinierten Autorisierungsserver verwenden, ähnelt Ihre Anforderungs-URL der folgenden:

>[!INFO]
>
>**Beispiel:**
>
>
>```
>/authorize?client\_id=<clientID>&response\_type=code&redirect\_uri=<redirectURL>
>&code\_challenge\_method=S256&code\_challenge=wzgjYF9qEiWep-CwqgrTE78-2ghjwCtRO3vj23o4W\_fw"
>```

Beachten Sie die Parameter, die übergeben werden:

* `client_id` entspricht der Client-ID der OAuth2-Anwendung, die Sie beim Konfigurieren der Anwendung in der erstellt haben.

  Anweisungen finden Sie unter Erstellen einer OAuth2-Single-Page-Webanwendung mit PKCE in OAuth2-Anwendungen für Workfront-Integrationen erstellen .

* `response_type` ist `code`, da die Anwendung die Art der Gewährung des Autorisierungscodes verwendet.

* `redirect_uri` ist der Callback-Speicherort, an den der Benutzeragent zusammen mit dem `code` weitergeleitet wird. Dies muss mit einer der Umleitungs-URLs übereinstimmen, die Sie beim Erstellen Ihrer OAuth2-Anwendung angegeben haben.

* `code_challenge_method` ist die Hash-Methode, mit der die Herausforderung generiert wird. Sie ist immer `S256` für Workfront Oauth2-Anwendungen, die PKCE verwenden.

* `code_challenge` ist die Code-Herausforderung, die für PKCE verwendet wird.


## Code für Token austauschen

Um den Autorisierungscode gegen ein Zugriffstoken auszutauschen, übergeben Sie ihn zusammen mit dem `code_verifier` an den `/token` -Endpunkt Ihres Autorisierungsservers.

>[!INFO]
>
>**Beispiel:**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=authorization\_code&client\_id=<clientID>&redirect\_uri=<redirectURL>&code=<code>&code\_verifier=N28zVMsKU6ptUjHaYWg3T1NFTDQqcW1R4BU5NXywapNac4hhfkxjwfhZQat
>```

>[!IMPORTANT]
>
> Im Gegensatz zum normalen Autorisierungscode-Fluss erfordert dieser Aufruf nicht den Autorisierungs-Header mit der Client-ID und dem geheimen Schlüssel. Aus diesem Grund eignet sich diese Version des Autorisierungscode-Flusses für native Apps wie Apps oder Einzelseitenanwendungen, die kein Backend haben.

Beachten Sie die Parameter, die übergeben werden:

* `grant_type` ist `authorization_code`, da die App den Grant-Typ &quot;Autorisierungscode&quot;verwendet.

* `redirect_uri` muss mit dem URI übereinstimmen, der zum Abrufen des Autorisierungscodes verwendet wurde.

* `code` ist der Autorisierungscode, den Sie vom /authorize -Endpunkt erhalten haben.

* `code_verifier` ist der PKCE-Code-Prüfer, den Ihre App in [Erstellen des Testschlüssels für Code Exchange](#Create) generiert hat.

* `client_id` identifiziert Ihren Client und muss mit dem in OAuth2 registrierten Wert übereinstimmen.


Wenn der Code weiterhin gültig ist und die Codeüberprüfung übereinstimmt, erhält Ihre Anwendung ein Zugriffstoken.

>[!INFO]
>
>**Beispiel:**
>
>```
>{
>    "access\_token": "eyJhd\[...\]Yozv",
>    "expires\_in": 3600,
>    "token\_type": "Bearer"
>}
>```

## Zugriffstoken überprüfen

Wenn Ihre Anwendung eine Anforderung mit einem Zugriffstoken übergibt, muss der Ressourcenserver sie überprüfen.

Sie können Ihr Zugriffstoken mit einem API-Aufruf wie dem folgenden validieren:

>[!INFO]
>
>**Beispiel:**
>
>```
>/attask/api/<api version>/proj/search \\
>  --header 'sessionID: <access\_token>' \\
>```

## Aktualisierungs-Token anfordern

Um ein Aktualisierungstoken anzufordern, können Sie einen POST-Aufruf an die -API ausführen, ähnlich wie im Folgenden:

>[!INFO]
>
>**Beispiel:**
>
>```
>/token \\
>  --header 'accept: application/json' \\
>  --header 'cache-control: no-cache' \\
>  --header 'content-type: application/x-www-form-urlencoded' \\
>  --data 'grant\_type=refresh\_token&client\_id=<clientID>&redirect\_uri=<redirectURL>&refresh\_token=<refresh\_token>
>```
