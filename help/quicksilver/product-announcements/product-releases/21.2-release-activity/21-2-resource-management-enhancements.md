---
content-type: release-notes
keywords: Hinweise,vierteljährlich,Aktualisierung,Freigabe
navigation-topic: 2021-2-release-activity
title: 21.2 Verbesserungen beim Ressourcenmanagement
description: Auf dieser Seite werden alle Verbesserungen des Ressourcen-Managements beschrieben, die mit der Version 21.2 an der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Woche vom 10. Mai 2021 in der Produktionsumgebung verfügbar gemacht. Eine Liste aller mit Version 21.2 verfügbaren Änderungen finden Sie in der Übersicht über die Version 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# 21.2 Verbesserungen beim Ressourcenmanagement

Auf dieser Seite werden alle Verbesserungen des Ressourcen-Managements beschrieben, die mit der Version 21.2 an der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Woche vom 10. Mai 2021 in der Produktionsumgebung verfügbar gemacht. Eine Liste aller mit Version 21.2 verfügbaren Änderungen finden Sie unter Übersicht über Version [21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Ansicht auf Monatsebene im Workload Balancer

Um Ihnen bei der Verwaltung der Ressourcenzuweisung für längere Zeiträume zu helfen, haben wir jetzt eine Monatsansicht für den Workload Balancer implementiert. Sie können bis zu drei Monate auf einmal anzeigen und die monatlichen Ressourcenzuteilungen aktualisieren. Vor dieser Änderung konnten Sie den Workload Balancer nur nach Tag oder Woche anzeigen.

Weitere Informationen finden Sie unter [Navigieren im Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Verbindung zwischen dem Szenario-Planer, dem Workload-Balancer und der Aufgabenliste

>[!NOTE]
>
>Nur in der neuen Adobe Workfront-Version verfügbar.

Um Ihnen bei der strategischen Planung Ihrer Projekte zu helfen und sicherzustellen, dass sie mit den übergeordneten Initiativen des Szenarienplaners übereinstimmen, haben wir einen neuen Bereich im Projekt erstellt, der die Aufgabengebiet-Anforderungen der Initiativen sowie die geplanten Stunden, die für die Arbeitselemente des Projekts geschätzt wurden, anzeigt. Dieser Bereich ist für den Workload Balancer auf Projektebene sowie für die Aufgabenliste in der neuen Workfront-Version verfügbar. In der klassischen Version ist dies nur für den Projekt-Workload-Balancer verfügbar.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Übersicht über die Abstimmung der Ressourcenzuweisungen zwischen Projekten und Initiativen](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).
* [Navigieren im Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>Diese neue Funktion ist für alle Benutzenden sichtbar, sowohl in der neuen als auch in der klassischen Workfront-Version. Dies ist auch für Kunden sichtbar, die keine Workfront Scenario Planner-Lizenz erworben haben.

## Geplante Stunden bei der Berechnung von Nettowerten im Ressourcenplaner verwenden

Eine neue Einstellung im Ressourcenplaner ermöglicht die Verwendung der geplanten Stunden bei der Berechnung der Nettowerte.

Vor dieser Verbesserung hat Workfront die Nettowerte nur anhand der budgetierten Stunden berechnet. Nettowerte zeigen die Differenz zwischen verfügbaren und budgetierten oder geplanten Stunden, FTE oder Kosten an. Budgetierte Stunden sind weiterhin die Standardeinstellung bei der Berechnung von Nettowerten.

Weitere Informationen finden Sie [Übersicht über Stunden, FTE und Kosten in den Projekt- und Rollenansichten des Ressourcenplaners](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## 12-Wochen-Ansicht im Workload Balancer

Im Workload-Balancer können jetzt Informationen von bis zu 12 Wochen angezeigt werden. Vor dieser Verbesserung konnten Sie Informationen über 2, 4 und 6 Wochen anzeigen.

Weitere Informationen zum Anzeigen des Workload-Balancer finden Sie unter [Navigieren im Workload-Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md) Navigieren im Workload-Balancer.

## Die Funktionsweise des Aufgabenrollenfilters im Bereich „Nicht zugewiesen“ des Workload-Balancer wird geändert

Um die Funktionsweise des Aufgabenrollenfilters im Workload Balancer zu verbessern und den Erwartungen der Benutzenden zu entsprechen, haben wir die Funktionalität des Filters im Bereich „Nicht zugewiesen“ geändert. Sie können jetzt nur die Stunden anzeigen, die den im Filter angegebenen Aufgabengebieten zugewiesen sind.

Vor dieser Verbesserung zeigte der Workload Balancer beim Anwenden des Aufgabenrollenfilters im Bereich Nicht zugewiesen alle Stunden an, die mit den Arbeitselementen verknüpft sind, die den Aufgabengebieten zugewiesen wurden.

Informationen zum Filtern von Informationen im Workload Balancer finden Sie unter [Verwalten von Filtern im Workload Balancer](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
