---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 'Workfront Fusion-Veröffentlichungsaktivität: Woche vom 16. November 2020'
description: Auf dieser Seite werden alle Verbesserungen beschrieben, die in Adobe Workfront Fusion in der Woche vom 16. November 2020 vorgenommen wurden.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 9221a69e-2482-478b-95a9-f62dd28538d6
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# Workfront Fusion-Veröffentlichungsaktivität: Woche vom 16. November 2020

Auf dieser Seite werden alle Verbesserungen beschrieben, die in Adobe Workfront Fusion in der Woche vom 16. November 2020 vorgenommen wurden.

Eine Liste aller aktuellen Änderungen finden Sie unter [Adobe Workfront Fusion-Versionsaktivität](../../../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Eine Liste der letzten Fehlerbehebungen in Workfront Fusion finden Sie auf der Seite [Workfront-Wartungs-Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) und suchen Sie nach Updates mit der Bezeichnung Workfront Fusion-Wartungs-Update.

## Aktualisierungen des Jira-Cloud-Connectors

Um die Möglichkeiten zur Verwendung des Jira Cloud-Connectors zu erweitern, haben wir drei neue Module hinzugefügt:

* Problem zum Sprint hinzufügen
* Einträge auflisten
* Nach Datensätzen suchen

Wir haben auch vorhandene Module aktualisiert, um den Objekttyp „Sprint“ zu unterstützen. Zuvor war der Zugriff auf das „Sprint“-Objekt nur über das Modul für benutzerdefinierte API-Aufrufe möglich.

Weitere Informationen finden Sie unter [Jira Software-Module](../../../../../workfront-fusion/apps-and-their-modules/jira-software-modules.md).

## Die Ausführungs-ID ist jetzt für die Zuordnung in Szenarien verfügbar

Die Ausführungs-ID für ein Szenario ist jetzt im Zuordnungsbereich verfügbar. Diese ID stellt eine bestimmte Ausführung des Szenarios dar und kann als Metadaten verwendet werden. Beispielsweise kann die Ausführungs-ID mit einem von Fusion erstellten Datensatz gespeichert werden, sodass Sie später feststellen können, mit welcher Fusion-Ausführung der Datensatz erstellt wurde. Die Ausführungs-ID finden Sie im Zuordnungsbereich unter Allgemeine Funktionen.

Weitere Informationen zu Szenario-Ausführungen finden Sie unter [Szenario-Ausführung, Zyklen und Phasen in Adobe Workfront Fusion](../../../../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Tastaturbefehle für Workfront Fusion 2.0-Szenarien

Um die Erstellung von Szenarien zu vereinfachen, wurden einige Tastaturbefehle hinzugefügt:

* Strg/Befehl+Umschalt+Eingabe: Ein Szenario einmal ausführen
* Strg/Befehl + Umsch + S: Szenario speichern

Weitere Informationen zum Erstellen von Workfront Fusion 2.0-Szenarien finden Sie unter [Erstellen eines Szenarios in Adobe Workfront Fusion](../../../../../workfront-fusion/scenarios/create-a-scenario.md).

## Aktualisierungen des Office 365 Excel-Connectors

Um die Möglichkeiten zur Verwendung des Office 365 Excel-Connectors zu erweitern, haben wir einige neue Module hinzugefügt. Jetzt können Sie:

* Trigger eines Moduls aus Änderungen in Arbeitsmappen
* Arbeitsmappen suchen oder herunterladen
* Auflisten von Arbeitsblättern, Arbeitsblattzeilen, Tabellen oder Tabellenzeilen
* Aktualisieren einer Tabelle oder Arbeitsblattzeile
* Löschen einer Tabelle oder Arbeitsblattzeile
* Abrufen von Metadaten für eine Tabelle
* Erstellen eines benutzerdefinierten API-Aufrufs

Zuvor verfügbare Module sind weiterhin in der App vorhanden.

Weitere Informationen finden Sie unter [Microsoft Office 365 Excel-Module](../../../../../workfront-fusion/apps-and-their-modules/microsoft-365-excel-modules.md).

## Verwenden von OAuth 2.0 in Verbindungen Ihrer Workfront-App

Wir haben den Workfront-Connector aktualisiert, um OAuth 2.0 verwenden zu können. Durch dieses Update ist es einfacher, Änderungen an den Verbindungen Ihrer Workfront-App vorzunehmen. Wenn sich beispielsweise etwas an Ihrer Verbindung ändert (z. B. ein Kennwort), müssen Sie in Ihren Szenarien nicht mehr jede einzelne Verbindung aktualisieren. Darüber hinaus bietet OAuth2 weitere Vorteile, z. B. verbesserte Sicherheit und die Möglichkeit, Single Sign-on (SSO) zu verwenden.

Für bestehende Verbindungen sind derzeit keine Änderungen erforderlich. Sie können jedoch vorhandene Verbindungen erneut autorisieren, wenn Sie die Vorteile von OAuth 2.0 nutzen möchten.

Weitere Informationen finden Sie unter [Adobe Workfront-Module](../../../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).
