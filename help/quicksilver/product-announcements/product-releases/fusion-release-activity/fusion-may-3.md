---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 'Workfront Fusion-Veröffentlichungsaktivität: Woche vom 3. Mai 2021'
description: Auf dieser Seite werden alle Verbesserungen beschrieben, die in Adobe Workfront Fusion in der Woche vom 3. Mai 2021 vorgenommen wurden.
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: af3312c5-3416-4c03-8528-6a2c0240110e
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Workfront Fusion-Veröffentlichungsaktivität: Woche vom 3. Mai 2021

Auf dieser Seite werden alle Verbesserungen beschrieben, die in Adobe Workfront Fusion in der Woche vom 3. Mai 2021 vorgenommen wurden.

Eine Liste aller aktuellen Änderungen finden Sie unter [Adobe Workfront Fusion-Versionsaktivität](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Eine Liste der letzten Fehlerbehebungen in Workfront Fusion finden Sie auf der Seite [Workfront-Wartungs-Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) und suchen Sie nach Updates mit der Bezeichnung Workfront Fusion-Wartungs-Update.

## Salesforce-Connector kann jetzt mit SOQL suchen

Das Modul Salesforce > Suche nach Datensätzen bietet jetzt die Möglichkeit, mit SOQL (Salesforce Object Query Language) zu suchen. Sie können auch mit den zuvor verfügbaren Optionen suchen (SOSL und einfache Suchen).

Weitere Informationen finden Sie unter [Salesforce-Module](../../../workfront-fusion/apps-and-their-modules/salesforce-modules.md).

## Neuer Verbindungstyp im Azure DevOps-Connector erfordert weniger Bereiche

Zur Verbesserung der Sicherheit haben wir dem Workfront Fusion Azure DevOps-Connector einen neuen Connector-Typ hinzugefügt. Wenn Sie jetzt eine Verbindung in einem Azure DevOps-Modul erstellen, können Sie aus zwei Arten von Verbindungen auswählen:

* Azure DevOps

  Dieser neue Verbindungstyp beschränkt die Bereiche auf die, die speziell von Workfront Fusion benötigt werden.

* Azure DevOps (alle Bereiche anfordern)

  Dies ist der Legacy-Verbindungstyp, der alle in einer Verbindung zu Azure DevOps verfügbaren Bereiche anfordert.

Es wird empfohlen, den Azure DevOps-Verbindungstyp in allen neuen Szenarien zu verwenden, in denen Azure DevOps verwendet wird. Wir empfehlen auch, alle Azure DevOps-Module in Ihren vorhandenen Szenarien zu ändern, um den neuen Verbindungstyp zu verwenden. Der alte Verbindungstyp Azure DevOps (Alle Bereiche anfordern) wird in naher Zukunft nicht mehr unterstützt.

Weitere Informationen finden Sie unter [Azure DevOps-Module](../../../workfront-fusion/apps-and-their-modules/azure-dev-ops.md).
