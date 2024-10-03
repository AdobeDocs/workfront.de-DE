---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Generieren eines Szenario-Segments mit AI
description: Sie können eine Textaufforderung eingeben, um ein für die Eingabeaufforderung konfiguriertes HTTP-Modul zu erstellen.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
source-git-commit: 5de5b96bc74ce9b819acfa7b5f16652509ccade1
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Generieren eines Szenario-Segments mit AI

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>Da diese Funktion in Beta verfügbar ist, steht sie nur einigen Workfront-Benutzern zur Verfügung.

Sie können AI verwenden, um eine Textaufforderung einzugeben, die beschreibt, was Sie für einen Abschnitt Ihres Szenarios benötigen. Fusion generiert dann Module, die diese Aktionen ausführen, die Sie in Ihrem Szenario verwenden können.

Wie bei allen aus AI generierten Modulen empfehlen wir, die generierten Module zu überprüfen und zu testen, um sicherzustellen, dass sie die gewünschte Leistung erzielen.

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

## Generieren von Modulen

1. Beginnen Sie mit dem Hinzufügen eines Moduls und wählen Sie in der Liste der Anwendungen die Option **Mit KI generieren** aus.

   Oder

   Klicken Sie unten auf der Seite des Szenario-Editors auf das Symbol Mit KI generieren ![Mit KI generieren](assets/generate-with-ai-icon-beta.png) .

   Das Fenster &quot;KI-Assistent&quot;wird geöffnet.
1. Geben Sie eine Textaufforderung in das Feld ein.

   Tipps zu Eingabeaufforderungen finden Sie in diesem Artikel unter [Tipps zum Erstellen von Textaufforderungen](#tips-for-creating-text-prompts).

   AI Assistant generiert das Modul oder den Satz von Modulen.
1. (Bedingt) Fügen Sie bei Bedarf Ihr API-Token für die Anwendung zu den Modulen hinzu.
1. Überprüfen Sie die Module, um sicherzustellen, dass sie für die entsprechende Anwendung und Aktion konfiguriert sind.
1. (Bedingt) Wenn der Abschnitt zum generierten Szenario nicht an Ihr Szenario angehängt ist, ziehen Sie es an die gewünschte Position.

Es wird empfohlen, die Module zu testen, um sicherzustellen, dass sie die gewünschte Leistung erzielen.

## Tipps zum Erstellen von Textanforderungen

Textaufforderungen sollten mindestens die folgenden Informationen enthalten:

* Die Anwendung, mit der Sie eine Verbindung herstellen
* Die Aktionen, die Sie ausführen möchten

>[!IMPORTANT]
>
>Sie können mehrere Module gleichzeitig generieren, aber nur Module für eine Anwendung gleichzeitig generieren.

>[!INFO]
>
>**Beispiele**:
>
>* `Delete the records 'xyz-123', 'xyz-456', 'xyz-789' from Adobe Workfront Planning`
>Dazu gehören die Anwendung `Workfront Planning` und die Aktion `delete records`. Diese Eingabeaufforderung erstellt drei Module, eines für jeden zu löschenden Datensatz.
>* `Change campaign summary of the record 'xyz-123' from Adobe Workfront Planning`
>Dazu gehören die Anwendung `Workfront Planning` und die Aktion `change campaign summary`.
>* `Get all field details in the record type with ID 'test-record' from Adobe Workfront Planning`
>Dazu gehören die Anwendung `Workfront Planning` und die Aktion `get field details`.
>
>Das folgende Beispiel ist NICHT korrekt:
>
>* `Generate an image in Adobe Firefly and upload it to Dropbox`
>
>    Dieses Beispiel ist falsch, da es mehr als eine Anwendung enthält

Beachten Sie beim Erstellen von Textanforderungen Folgendes:

* Verwenden Sie eine direkte, einfache Sprache.
* Prüfen und testen Sie Ihre Module. Wenn die Ausführung nicht wie erwartet erfolgt, verfeinern Sie die Eingabeaufforderung und versuchen Sie es erneut.
