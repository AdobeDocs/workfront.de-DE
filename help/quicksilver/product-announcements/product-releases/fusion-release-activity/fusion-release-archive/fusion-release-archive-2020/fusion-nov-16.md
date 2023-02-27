---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 'Workfront Fusion-Release-Aktivität: Woche vom 16. November 2020'
description: Auf dieser Seite werden alle Verbesserungen beschrieben, die in der Adobe Workfront Fusion-Woche vom 16. November 2020 vorgenommen wurden.
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: 9221a69e-2482-478b-95a9-f62dd28538d6
hidefromtoc: true
source-git-commit: e6995cd57c4210725d49379df5bcd7e93ce4b02a
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Workfront Fusion-Release-Aktivität: Woche vom 16. November 2020

Auf dieser Seite werden alle Verbesserungen beschrieben, die in der Adobe Workfront Fusion-Woche vom 16. November 2020 vorgenommen wurden.

Eine Liste aller letzten Änderungen finden Sie unter [Adobe Workfront Fusion-Release-Aktivität](../../../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Eine Liste der letzten Fehlerkorrekturen in Workfront Fusion finden Sie unter [Workfront-Wartungs-Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) und suchen Sie nach Aktualisierungen mit der Bezeichnung Workfront Fusion Maintenance Update .

## Aktualisierungen des Jira Cloud-Connectors

Um die Möglichkeiten zur Verwendung des Jira Cloud-Connectors zu erweitern, haben wir drei neue Module hinzugefügt:

* Problem zum Sprint hinzufügen
* Listen-Datensätze
* Datensätze suchen

Wir haben auch vorhandene Module aktualisiert, um den Objekttyp &quot;Sprint&quot;zu unterstützen. Zuvor konnte auf das Objekt &quot;Sprint&quot;nur über das Modul &quot;Benutzerspezifischer API-Aufruf&quot;zugegriffen werden.

Weitere Informationen finden Sie unter [Jira-Softwaremodule](../../../../../workfront-fusion/apps-and-their-modules/jira-software-modules.md).

## Die Ausführungs-ID ist jetzt für die Zuordnung in Szenarien verfügbar.

Die Ausführungs-ID für ein Szenario ist jetzt im Zuordnungsbereich verfügbar. Diese ID stellt eine bestimmte Ausführung des Szenarios dar und kann als Metadaten verwendet werden. Beispielsweise kann die Ausführungs-ID mit einem Datensatz gespeichert werden, den Fusion erstellt, sodass Sie später feststellen können, durch welche Fusion-Ausführung der Datensatz erstellt wurde. Die Ausführungs-ID finden Sie im Zuordnungsbereich unter Allgemeine Funktionen.

Weitere Informationen zu Szenario-Ausführungen finden Sie unter [Ausführung, Zyklen und Phasen eines Szenarios in Adobe Workfront Fusion](../../../../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Tastaturbefehle für Workfront Fusion 2.0-Szenarien

Um das Erstellen eines Szenarios einfacher zu gestalten, haben wir einige Tastaturbefehle hinzugefügt:

* Strg/Befehl+Umschalt+Eingabetaste: Ausführen eines Szenarios einmal
* Strg/Befehl + Umschalt + S: Speichern eines Szenarios

Weitere Informationen zum Erstellen von Workfront Fusion 2.0-Szenarien finden Sie unter [Erstellen eines Szenarios in Adobe Workfront Fusion](../../../../../workfront-fusion/scenarios/create-a-scenario.md).

## Aktualisierungen für Office 365 Excel Connector

Um die Möglichkeiten zur Verwendung des Office 365 Excel Connectors zu erweitern, haben wir einige neue Module hinzugefügt. Jetzt können Sie:

* Trigger eines Moduls von Änderungen in Arbeitsmappen
* Arbeitsmappen suchen oder herunterladen
* Arbeitsblätter, Arbeitsblattzeilen, Tabellen oder Tabellenzeilen auflisten
* Tabellen- oder Arbeitsblattzeilen aktualisieren
* Tabellen- oder Arbeitsblattzeilen löschen
* Abrufen von Metadaten für eine Tabelle
* Benutzerdefinierte API-Aufrufe durchführen

Zuvor verfügbare Module sind weiterhin in der App vorhanden.

Weitere Informationen finden Sie unter [Microsoft Office 365 Excel-Module](../../../../../workfront-fusion/apps-and-their-modules/microsoft-365-excel-modules.md).

## Verwenden von OAuth 2.0 in Ihren Workfront-App-Verbindungen

Wir haben den Workfront-Connector aktualisiert und verwenden nun OAuth 2.0. Dank dieser Aktualisierung ist es einfacher, Änderungen an Ihren Workfront-App-Verbindungen vorzunehmen. Wenn sich beispielsweise etwas an Ihrer Verbindung ändert (z. B. ein Kennwort), müssen Sie nicht mehr jede einzelne Verbindung in Ihren Szenarien aktualisieren. Darüber hinaus bietet OAuth2 weitere Vorteile wie verbesserte Sicherheit und die Möglichkeit, Single Sign-on (SSO) zu verwenden.

Vorhandene Verbindungen erfordern derzeit keine Änderungen. Sie können jedoch vorhandene Verbindungen neu autorisieren, wenn Sie die Vorteile von OAuth 2.0 nutzen möchten.

Weitere Informationen finden Sie unter [Adobe Workfront-Module](../../../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).
