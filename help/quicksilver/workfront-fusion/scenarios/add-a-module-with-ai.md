---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Generieren eines Moduls mit AI
description: Sie können eine Textaufforderung eingeben, um ein für die Eingabeaufforderung konfiguriertes HTTP-Modul zu erstellen.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
source-git-commit: fe096ba36da9b56e0e38f6061481b66cfbeee5c6
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 1%

---

# Generieren eines Moduls mit AI

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>Da sich diese Funktion noch in der Anfangsphase ihrer Entwicklung befindet, steht sie nur internen Workfront-Benutzern zur Verfügung.

Sie können mithilfe von KI eine Textaufforderung eingeben, in der Sie beschreiben, was Sie mit einem Modul tun müssen. Fusion generiert dann ein HTTP-Modul, das eine Verbindung zum richtigen Endpunkt der gewünschten API herstellt.

Wie bei allen aus AI generierten Elementen empfehlen wir, das generierte Modul zu überprüfen und zu testen, um sicherzustellen, dass es die gewünschte Leistung erzielt.

## Derzeit unterstützte AI-Modulanwendungen

Die Fusion AI kann derzeit Module generieren, die eine Verbindung zu den folgenden Anwendungen herstellen:

* Adobe Firefly
* Azure OpenAI
* Microsoft-Diagramm
* Adobe Workfront-Planung
* Adobe Analytics
* Adobe PDF Services
* Adobe Marketo
* Adobe Frame.io
* Dropbox
* NetSuite
* Google-Kalendar
* Atlassian Jira
* GitLab
* Spotify
* Bitbucket
* OpenAI
* Slack

## Modul generieren

1. Fügen Sie ein Modul hinzu und wählen Sie in der Liste der Anwendungen die Option **Mit KI generieren** aus.

   Oder

   Klicken Sie mit der rechten Maustaste auf einen leeren Bereich des Szenario-Editors und wählen Sie dann **Mit AI generieren** aus.
1. Geben Sie eine Textaufforderung in das Feld ein.

   Tipps zu Eingabeaufforderungen finden Sie in diesem Artikel unter [Tipps zum Erstellen von Textaufforderungen](#tips-for-creating-text-prompts).
1. Fügen Sie Ihr API-Token für die Anwendung zum -Modul hinzu.
1. Überprüfen Sie das Modul, um sicherzustellen, dass es für die entsprechende Anwendung und Aktion konfiguriert zu sein scheint.
1. (Bedingt) Wenn das Modul nicht an Ihr Szenario angehängt ist, ziehen Sie es an die gewünschte Position.

Wir empfehlen, das Modul zu testen, um sicherzustellen, dass das generierte Modul die gewünschte Leistung erzielt.

## Tipps zum Erstellen von Textanforderungen

Textaufforderungen sollten mindestens die folgenden Informationen enthalten:

* Die Anwendung, mit der Sie eine Verbindung herstellen
* Die Aktion, die Sie ausführen möchten

>[!INFO]
>
>**Beispiele**:
>
>* `Retrieve a list of my calendars from Google Calendar`
>
>   Dazu gehören die Anwendung `Google Calendar` und die Aktion `Retrieve a list of my calendars`.
>
>* `Retrieve popular songs from Spotify`
>
>   Dazu gehören die Anwendung `Spotify` und die Aktion `Retrieve popular songs`.

Beachten Sie beim Erstellen von Textanforderungen Folgendes:

* Da jedes Fusion-Modul eine einzelne Aktion ausführt, sollte Ihre Textaufforderung eine bestimmte Aktion beschreiben.
* Verwenden Sie eine direkte, einfache Sprache.
* Prüfen und testen Sie Ihr Modul. Wenn die Ausführung nicht wie erwartet erfolgt, verfeinern Sie die Eingabeaufforderung und versuchen Sie es erneut.
