---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Generieren eines Moduls mit AI
description: Sie können eine Textaufforderung eingeben, um ein für die Eingabeaufforderung konfiguriertes HTTP-Modul zu erstellen.
author: Becky
feature: Workfront Fusion
source-git-commit: 79b5baf5a9558e07b55fb810aa2d6c772faa51cf
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 1%

---

# Generieren eines Moduls mit AI

Sie können mithilfe von KI eine Textaufforderung eingeben, in der Sie beschreiben, was Sie mit einem Modul tun müssen. Fusion generiert dann ein HTTP-Modul, das eine Verbindung zum richtigen Endpunkt der gewünschten API herstellt.

Wie bei allen aus AI generierten Elementen empfehlen wir, das generierte Modul zu überprüfen und zu testen, um sicherzustellen, dass es die gewünschte Leistung erzielt.

## Derzeit unterstützte AI-Modulanwendungen

Die Fusion AI kann derzeit Module generieren, die eine Verbindung zu den folgenden Anwendungen herstellen:

* Adobe Maestro
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

1. Modul hinzufügen und auswählen **Generieren mit AI** aus der Liste der Anwendungen.

   Oder

   Klicken Sie mit der rechten Maustaste auf einen leeren Bereich des Szenario-Editors und wählen Sie **Generieren mit AI**.
1. Geben Sie eine Textaufforderung in das Feld ein.

   Tipps zu Eingabeaufforderungen finden Sie unter [Tipps zum Erstellen von Textanforderungen](#tips-for-creating-text-prompts) in diesem Artikel.
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
>   Dies schließt die Anwendung ein. `Google Calendar` und die Maßnahmen `Retrieve a list of my calendars`.
>
>* `Retrieve popular songs from Spotify`
>
>   Dies schließt die Anwendung ein. `Spotify` und die Maßnahmen `Retrieve popular songs`.

Beachten Sie beim Erstellen von Textanforderungen Folgendes:

* Da jedes Fusion-Modul eine einzelne Aktion ausführt, sollte Ihre Textaufforderung eine bestimmte Aktion beschreiben.
* Verwenden Sie eine direkte, einfache Sprache.
* Prüfen und testen Sie Ihr Modul. Wenn die Ausführung nicht wie erwartet erfolgt, verfeinern Sie die Eingabeaufforderung und versuchen Sie es erneut.



