---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 'Workfront Fusion-Release-Aktivität: Woche vom 3. Mai 2021'''
description: Auf dieser Seite werden alle Verbesserungen beschrieben, die in der Adobe Workfront Fusion-Woche vom 3. Mai 2021 vorgenommen wurden.
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: af3312c5-3416-4c03-8528-6a2c0240110e
hidefromtoc: true
source-git-commit: 9c2321794c5ba773bfda1d6e9dfda6b8de1a1449
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# Workfront Fusion-Release-Aktivität: Woche vom 3. Mai 2021

Auf dieser Seite werden alle Verbesserungen beschrieben, die in der Adobe Workfront Fusion-Woche vom 3. Mai 2021 vorgenommen wurden.

Eine Liste aller letzten Änderungen finden Sie unter [Adobe Workfront Fusion-Release-Aktivität](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Eine Liste der letzten Fehlerkorrekturen in Workfront Fusion finden Sie unter [Workfront-Wartungs-Updates](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) und suchen Sie nach Aktualisierungen mit der Bezeichnung Workfront Fusion Maintenance Update .

## Salesforce-Connector kann jetzt mit SOQL suchen

Das Modul Salesforce > Suche nach Datensätzen bietet jetzt die Möglichkeit, mithilfe von SOQL (Salesforce Object Query Language) zu suchen. Sie können auch mit den zuvor verfügbaren Optionen (SOSL und einfache Suchen) suchen.

Weitere Informationen finden Sie unter [Salesforce-Module](../../../workfront-fusion/apps-and-their-modules/salesforce-modules.md).

## Neuer Verbindungstyp im Azure DevOps-Connector erfordert weniger Bereiche

Um die Sicherheit zu erhöhen, haben wir dem Workfront Fusion Azure DevOps Connector einen neuen Connector-Typ hinzugefügt. Wenn Sie jetzt eine Verbindung in einem Azure DevOps-Modul erstellen, können Sie aus zwei Arten von Verbindungen auswählen:

* Azure DevOps

   Dieser neue Verbindungstyp beschränkt die Bereiche auf die speziell von Workfront Fusion benötigten.

* Azure DevOps (alle Bereiche anfordern)

   Dies ist der veraltete Verbindungstyp, der alle in einer Verbindung zu Azure DevOps verfügbaren Bereiche anfordert.

Wir empfehlen Ihnen, den Azure DevOps-Verbindungstyp in allen Ihren neuen Szenarien zu verwenden, die Azure DevOps verwenden. Wir empfehlen Ihnen außerdem, alle Azure DevOps-Module in Ihren vorhandenen Szenarien zu ändern, um den neuen Verbindungstyp zu verwenden. Der veraltete Verbindungstyp Azure DevOps (Alle Bereiche anfordern) wird in naher Zukunft nicht mehr unterstützt.

Weitere Informationen finden Sie unter [Azure DevOps-Module](../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md).
