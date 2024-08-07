---
title: Workfront Fusion-Release-Aktivität:&nbsp;Woche vom 30. August 2021
description: Workfront Fusion-Release-Aktivität:&nbsp;Woche vom 30. August 2021
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 988349f9-aa12-4017-9032-be4d0078959e
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '418'
ht-degree: 0%

---

# Workfront Fusion-Release-Aktivität: Woche vom 30. August 2021

Auf dieser Seite werden alle Verbesserungen beschrieben, die in der Adobe Workfront Fusion-Woche vom 30. August 2021 vorgenommen wurden.

Eine Liste aller letzten Änderungen finden Sie unter [Adobe Workfront Fusion-Release-Aktivität](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Eine Liste der aktuellen Fehlerbehebungen in Workfront Fusion finden Sie auf der Seite [Workfront Maintenance Updates](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) und suchen Sie nach Aktualisierungen, die als Workfront Fusion Maintenance Update bezeichnet werden.

## Filtern von Ereignissen, die das Modul &quot;Workfront > Ereignisse überwachen&quot;Trigger haben

1. Richten Sie einen benutzerdefinierten Filter für Ereignisse ein, die auf das Modul Workfront > Ereignisse überwachen Trigger werden.

   Um die Anzahl unnötiger Szenario-Ausführungen zu reduzieren, haben wir das Modul Workfront > Datensätze überwachen aktualisiert, um die Ereignisfilterung zu aktivieren. Jetzt können Sie einen Filter festlegen, wenn Sie einen Webhook erstellen. Dadurch kann das Szenario nur Trigger werden, wenn das Ereignis bestimmte Kriterien erfüllt.

   Der Ereignisfilter bietet derzeit die folgenden Vorgänge:

   * Gleich: Trigger eines Szenarios nur, wenn ein Ereignis den Filterbedingungen entspricht. Sie können beispielsweise einen Filter einrichten, der ein Szenario nur dann Trigger, wenn das Ereignis in einem bestimmten Projekt auftritt.
   * Nicht gleich: Trigger eines Szenarios nur dann, wenn ein Ereignis nicht mit den Filterbedingungen übereinstimmt. Sie können beispielsweise einen Filter erstellen, der ein Szenario nur dann Trigger, wenn das Problem, bei dem ein Ereignis auftritt, in nicht den Status Geschlossen aufweist.

   Zuvor hat das Modul Datensätze überwachen alle Datensätze abgerufen. Benutzer konnten nur filtern, indem sie später im Szenario Filter eingerichtet haben.

   Um die Ereignisfilterung zu nutzen, erstellen Sie einen neuen Webhook in Ihrem Modul &quot;Watch-Ereignisse&quot;. Es ist derzeit nicht möglich, vorhandene Webhooks zu bearbeiten, um diese Funktion aufzunehmen. Es wird dringend empfohlen, neue Webhooks zu erstellen, die Ereignisfilter für Ihre vorhandenen Szenarien verwenden.

1. Filtern Sie Ereignisse, die von der aktuellen Verbindung ausgelöst werden.

   Um die Einrichtung Ihrer Webhooks für das Modul Workfront > Ereignisse überwachen zu vereinfachen, haben wir den häufigsten Ereignisfilter eingefügt. Jetzt kann der Webhook alle Änderungen herausfiltern, die von Modulen mithilfe der für das Modul &quot;Ereignisse überwachen&quot;angegebenen Verbindung vorgenommen wurden. Mit anderen Worten: Wenn dieser Filter aktiviert ist, können alle Änderungen, die vom mit dieser Verbindung verknüpften Workfront-Benutzer vorgenommen wurden, das Szenario nicht Trigger werden.

   Zuvor war dieser Filter nicht verfügbar. Daher war es einfacher, in Workfront-Modulen vorgenommene Änderungen an Trigger-Szenarien vorzunehmen, die diese Module enthalten, wodurch Szenarien möglicherweise selbst in einer Endlosschleife Trigger werden.

Weitere Informationen zu Ereignisfiltern im Modul Workfront > Ereignisse überwachen finden Sie unter [Adobe Workfront-Module](../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).

