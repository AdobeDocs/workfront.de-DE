---
content-type: api
navigation-topic: api-navigation-topic
title: Verwenden des PKCE-Flusses für OAuth 2-Anwendungen
description: Verwenden des PKCE-Flusses für OAuth 2-Anwendungen
author: Becky
feature: Workfront API
role: Developer
exl-id: 61fe77b6-c6d7-4f23-bfb6-617bccaa1989
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---

# Konfigurieren und verwenden Sie die benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des PKCE-Flusses

PKCE ist ein sicherer Autorisierungsfluss, der gut mit dynamisch aktualisierten Programmen wie mobilen Apps funktioniert, aber für alle OAuth2-Clients nützlich ist. Anstelle eines statischen Client-Geheimnisses verwendet PKCE eine dynamisch generierte Zeichenfolge, wodurch das Risiko eines Lecks des Client-Geheimnisses vermieden wird.

## PKCE - Übersicht

Ein PKCE-Fluss umfasst die folgenden Schritte. Die Schritte in diesem Abschnitt dienen nur informativen Zwecken. Informationen zum Ausführen dieser Verfahren finden Sie in anderen Abschnitten dieses Artikels.

1. Der Client erstellt die `code_challenge`, indem er die `code_verifier` mit `S256` Verschlüsselung umwandelt.

1. Der Client leitet den Browser zusammen mit dem generierten `code_challenge` zur OAuth2-Anmeldeseite weiter. Sie müssen Ihre App (Client) registrieren, damit OAuth2 die Autorisierungsanfrage akzeptieren kann. Nach der Registrierung kann Ihre App den Browser zu OAuth2 umleiten.

1. Der OAuth2-Autorisierungs-Server leitet die Authentifizierungsaufforderung an den Benutzer weiter.

1. Der Benutzer authentifiziert sich mit einer der konfigurierten Anmeldeoptionen und sieht möglicherweise eine Einverständnisseite, auf der die Berechtigungen aufgeführt sind, die OAuth2 der Anwendung erteilt.

1. OAuth2 leitet mit einem `authorization code` zurück zu Ihrem Programm.

1. Ihre Anwendung sendet diesen Code zusammen mit dem `code_verifier` an OAuth2.

1. OAuth2-Autorisierungs-Server wandelt die `code_verifier` mithilfe der `code_challenge_method` der ursprünglichen Autorisierungsanfrage um und vergleicht das Ergebnis mit der `code_challenge`. Wenn der Wert beider Zeichenfolgen übereinstimmt, hat der Server überprüft, ob die Anfragen vom selben Client stammen, und gibt einen `access token` aus.

1. OAuth2 gibt die `access token` und optional eine `refresh token` zurück.

1. Ihre Anwendung kann diese Token jetzt verwenden, um den Ressourcen-Server aufzurufen, z. B. eine API im Namen der Benutzerin oder des Benutzers.

1. Der Ressourcen-Server validiert das Token, bevor er auf die Anfrage antwortet.


## Konfigurieren des Programms

Bevor Sie die Autorisierung implementieren können, müssen Sie Ihre App in OAuth2 registrieren, indem Sie eine App-Integration von Workfront aus erstellen.

Anweisungen zum Erstellen der OAuth2-Anwendung finden Sie unter [Erstellen einer einseitigen OAuth2-Web-Anwendung mit PKCE](../../administration-and-setup/configure-integrations/create-oauth-application.md#create-an-oauth2-single-page-web-application-using-pkce) in [Erstellen von OAuth2-Anwendungen für Workfront-Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md)

>[!NOTE]
>
>Sie können bis zu zehn OAuth2-Anwendungen gleichzeitig haben.


## Erstellen des Proof-Schlüssels für den Code-Austausch

Ähnlich wie beim standardmäßigen Autorisierungs-Code-Fluss leitet Ihre App den Browser des Benutzers zum `/authorize`-Endpunkt Ihres Autorisierungs-Servers um. In diesem Fall müssen Sie jedoch auch eine Code Challenge weitergeben.

Als Erstes generieren Sie einen Code Verifier und eine Challenge.

<table>
  <col/>
  <col/>
    <tbody>
      <tr>
        <td role="rowheader">Code Verifier</td>
        <td>
          <p>Zufällige URL-sichere Zeichenfolge mit einer Mindestlänge von 43 Zeichen</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Code Challenge</td>
        <td>
          <p>Base64-URL-kodierter SHA-256-Hash des Code Verifier</p>
        </td>
      </tr>
    </tbody>
</table>


Sie müssen Code in Ihrer Client-Anwendung hinzufügen, um den Code Verifier und die Code Challenge zu erstellen.

Der PKCE-Generatorcode erstellt eine Ausgabe ähnlich der folgenden:

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

Ihre App speichert die `code_verifier` für später und sendet die `code_challenge` zusammen mit der Autorisierungsanfrage an die `/authorize` URL Ihres Autorisierungsservers.

## Autorisierungs-Code anfordern

Wenn Sie den standardmäßigen benutzerdefinierten Autorisierungs-Server verwenden, würde Ihre Anfrage-URL in etwa wie folgt aussehen:

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

  Anweisungen finden Sie unter Erstellen einer einseitigen OAuth2-Web-Anwendung mit PKCE in Erstellen von OAuth2-Anwendungen für Workfront-Integrationen.

* `response_type` ist `code`, da die Anwendung den Gewährungstyp Autorisierungs-Code verwendet.
* `redirect_uri` ist der Callback-Speicherort, an den der Benutzeragent zusammen mit dem `code` weitergeleitet wird. Diese muss mit einer der Umleitungs-URLs übereinstimmen, die Sie beim Erstellen Ihrer OAuth2-Anwendung angegeben haben.
* `code_challenge_method` ist die Hash-Methode, die zum Generieren der Challenge verwendet wird, was für Workfront Oauth2-Anwendungen, die PKCE verwenden, immer `S256` ist.
* `code_challenge` ist die Code Challenge, die für PKCE verwendet wird.


## Code gegen Token austauschen

Um den Autorisierungs-Code gegen ein Zugriffstoken einzutauschen, übergeben Sie ihn zusammen mit dem `/token` an den `code_verifier`-Endpunkt Ihres Autorisierungsservers.

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
> Im Gegensatz zum regulären Autorisierungs-Code-Fluss ist für diesen Aufruf keine Autorisierungs-Kopfzeile mit der Client-ID und dem Geheimnis erforderlich. Daher eignet sich diese Version des Autorisierungs-Code-Flusses für native Apps wie Mobile Apps oder Single Page Applications, die kein Backend haben.

Beachten Sie die Parameter, die übergeben werden:

* `grant_type` ist `authorization_code`, da die App den Gewährungstyp Autorisierungs-Code verwendet.

* `redirect_uri` muss mit dem URI übereinstimmen, der zum Abrufen des Autorisierungscodes verwendet wurde.

* `code` ist der Autorisierungs-Code, den Sie vom Endpunkt /authorize erhalten haben.

* `code_verifier` ist der PKCE-Code Verifier, den Ihre App in &quot;[&#x200B; des Korrekturabzugsschlüssels für den Code-Austausch“ &#x200B;](#Create).

* `client_id` identifiziert Ihren Client und muss mit dem in OAuth2 vorregistrierten Wert übereinstimmen.


Wenn der Code weiterhin gültig ist und der Code Verifier übereinstimmt, erhält Ihre Anwendung ein Zugriffstoken.

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

## Validieren des Zugriffstokens

Wenn Ihre Anwendung eine Anfrage mit einem Zugriffstoken übergibt, muss der Ressourcen-Server sie validieren.

Sie können Ihr Zugriffs-Token mit einem API-Aufruf ähnlich dem folgenden validieren:

>[!INFO]
>
>**Beispiel:**
>
>```
>/attask/api/<api version>/proj/search \\
>  --header 'sessionID: <access\_token>' \\
>```

## Aktualisierungstoken anfordern

Um ein Aktualisierungs-Token anzufordern, können Sie einen POST-Aufruf an die API durchführen, ähnlich dem folgenden:

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
