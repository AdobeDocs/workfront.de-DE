---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Erstellen eines Szenariosegments mit KI
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# Erstellen eines Szenariosegments mit KI

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Generieren eines Szenario-Segments mithilfe von KI](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/add-a-module-with-ai.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>Da sich diese Funktion in Beta befindet, steht sie nur einigen Workfront-Benutzenden zur Verfügung.

Sie können KI verwenden, um eine Textaufforderung einzugeben, die beschreibt, was Sie für einen Abschnitt Ihres Szenarios tun müssen. Fusion generiert dann Module, die diese Aktionen ausführen, die Sie in Ihrem Szenario verwenden können.

Wie bei allen aus KI generierten Modulen empfehlen wir, die generierten Module zweimal zu überprüfen und zu testen, um sicherzustellen, dass sie die beabsichtigte Leistung erbringen.

## Derzeit unterstützte KI-Modulanwendungen

Die Fusion-KI kann derzeit Module generieren, die eine Verbindung zu den folgenden Anwendungen herstellen:

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
* Atlassischer Jira
* GitLab
* Spotify
* Bitbucket
* OpenAI
* Slack

## Module generieren

1. Beginnen Sie mit dem Hinzufügen eines Moduls und wählen **Mit KI generieren** aus der Liste der Programme aus.

   Oder

   Klicken Sie auf das Symbol ![Mit KI generieren](assets/generate-with-ai-icon-beta.png) unten auf der Seite des Szenario-Editors.

   Das Bedienfeld KI-Assistent wird geöffnet.
1. Geben Sie in das Feld eine Eingabeaufforderung ein.

   Tipps zu Eingabeaufforderungen finden Sie unter [Tipps zum Erstellen von Eingabeaufforderungen](#tips-for-creating-text-prompts) in diesem Artikel.

   Der KI-Assistent generiert das Modul oder den Satz von Modulen.
1. (Bedingt) Fügen Sie bei Bedarf Ihr API-Token für die Anwendung in die Module ein.
1. Überprüfen Sie die Module, um sicherzustellen, dass sie für das entsprechende Programm und die entsprechende Aktion konfiguriert sind.
1. (Bedingt) Wenn der Abschnitt Erzeugtes Szenario nicht mit Ihrem Szenario verbunden ist, ziehen Sie ihn an die gewünschte Position.

Es wird empfohlen, die Module zu testen, um sicherzustellen, dass sie die beabsichtigte Leistung erzielen.

## Tipps zum Erstellen von Eingabeaufforderungen

Textaufforderungen sollten mindestens die folgenden Informationen enthalten:

* Die Anwendung, mit der Sie eine Verbindung herstellen
* Die Aktion(en), die Sie ausführen möchten

>[!IMPORTANT]
>
>Sie können mehr als ein Modul gleichzeitig generieren, können aber nur Module für jeweils ein Programm generieren.

>[!INFO]
>
>**Beispiele**:
>
>* `Delete the records 'xyz-123', 'xyz-456', 'xyz-789' from Adobe Workfront Planning`
>Dazu gehören die `Workfront Planning` und die `delete records`. Bei dieser Eingabeaufforderung werden drei Module erstellt, eines für jeden zu löschenden Datensatz.
>* `Change campaign summary of the record 'xyz-123' from Adobe Workfront Planning`
>Dazu gehören die `Workfront Planning` und die `change campaign summary`.
>* `Get all field details in the record type with ID 'test-record' from Adobe Workfront Planning`
>Dazu gehören die `Workfront Planning` und die `get field details`.
>
>Das folgende Beispiel ist NICHT korrekt:
>
>* `Generate an image in Adobe Firefly and upload it to Dropbox`
>
>    Dieses Beispiel ist falsch, da es mehr als ein Programm enthält

Beachten Sie beim Erstellen von Textaufforderungen Folgendes:

* Verwenden Sie eine direkte, einfache Sprache.
* Überprüfen und testen Sie Ihre Module. Wenn die Eingabeaufforderung nicht die erwartete Leistung zeigt, verfeinern Sie sie und versuchen Sie es erneut.
