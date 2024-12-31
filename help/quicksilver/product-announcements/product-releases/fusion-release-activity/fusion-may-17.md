---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 'Workfront Fusion-Veröffentlichungsaktivität: Woche vom 17. Mai 2021'
description: Auf dieser Seite werden alle Verbesserungen beschrieben, die in Adobe Workfront Fusion in der Woche vom 17. Mai 2021 vorgenommen wurden.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 930c335e-2c88-41af-983f-82be790c1a4b
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Workfront Fusion-Veröffentlichungsaktivität: Woche vom 17. Mai 2021

Auf dieser Seite werden alle Verbesserungen beschrieben, die in Adobe Workfront Fusion in der Woche vom 17. Mai 2021 vorgenommen wurden.

Eine Liste aller aktuellen Änderungen finden Sie unter [Adobe Workfront Fusion-Versionsaktivität](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Eine Liste der letzten Fehlerbehebungen in Workfront Fusion finden Sie auf der Seite [Workfront-Wartungs-Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) und suchen Sie nach Updates mit der Bezeichnung Workfront Fusion-Wartungs-Update.

## Kopieren von Modulen in Workfront Fusion-Szenarien

Um die Arbeit mit Ihren Workfront Fusion-Szenarien zu vereinfachen, haben wir das Kopieren und Einfügen von Modulen ermöglicht. Jetzt können Sie ein Modul oder eine Gruppe von Modulen kopieren und in dasselbe oder ein anderes Szenario einfügen. Beim Kopieren von Modulen werden die Feldwerte in diesem Modul beibehalten.

Weitere Informationen finden Sie unter [Module oder Szenarien in Adobe Workfront Fusion kopieren](../../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

## Auswahl mehrerer Module in einem Workfront Fusion-Szenario

Beim Bearbeiten eines Szenarios können jetzt mehrere Module gleichzeitig ausgewählt werden. Sie können dann Massenaktionen für die ausgewählten Module durchführen.

* Kopieren
* Verschieben
* Löschen

Beim Kopieren und Verschieben von Modulen werden die Modulwerte und alle Leitungen, die die Module verbinden, beibehalten.

Weitere Informationen zu Bearbeitungsszenarien finden Sie unter [Erstellen eines Szenarios in Adobe Workfront Fusion](../../../workfront-fusion/scenarios/create-a-scenario.md).

## Module behalten jetzt nicht gespeicherte Informationen bei

Um die Erstellung von Szenarien zu vereinfachen, haben wir es Modulen ermöglicht, Feldwerte beizubehalten, wenn sie nicht im Fokus sind. Wenn Sie nun ein Modul verlassen, ohne es zu speichern, und zu ihm zurückkehren, zeigen die Felder die zuvor eingegebenen Werte an. Wenn das Modul geschlossen ist, wird ein Indikator angezeigt, dass es nicht gespeicherte Felder gibt.

## Der Azure AD-Connector verarbeitet jetzt neue und aktualisierte Datensätze separat

Neue Datensätze und Aktualisierungen vorhandener Datensätze werden jetzt von separaten Modulen verarbeitet.

* Trigger Um nach neuen Datensätzen zu suchen, können Sie das Modul Datensätze überwachen verwenden. Dieses Modul sucht nicht mehr nach aktualisierten Datensätzen.
* Um aktualisierte Datensätze zu erhalten, können Sie das neue Delta-Modul „Benutzer/Gruppen suchen“ verwenden. Dieses Modul gibt neue, aktualisierte und gelöschte Datensätze zurück.

Weitere Informationen finden Sie unter [Azure Active Directory-Module](../../../workfront-fusion/apps-and-their-modules/azure-ad-modules.md).
