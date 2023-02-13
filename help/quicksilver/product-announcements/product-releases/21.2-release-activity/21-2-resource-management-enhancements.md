---
content-type: release-notes
keywords: notes,vierteljährlich,update,release
navigation-topic: 2021-2-release-activity
title: 21.2 Verbesserungen bei der Ressourcenverwaltung
description: Auf dieser Seite werden alle Verbesserungen an der Ressourcenverwaltung beschrieben, die mit Version 21.2 der Vorschaufunktion vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung ab der Woche vom 10. Mai 2021 verfügbar sein. Eine Liste aller in Version 21.2 verfügbaren Änderungen finden Sie in der Versionshinweise 21.2 .
author: Luke
feature: Product Announcements
exl-id: 00133efe-f779-4217-87af-a223dcf043ee
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# 21.2 Verbesserungen bei der Ressourcenverwaltung

Auf dieser Seite werden alle Verbesserungen an der Ressourcenverwaltung beschrieben, die mit Version 21.2 der Vorschaufunktion vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung ab der Woche vom 10. Mai 2021 verfügbar sein. Eine Liste aller in Version 21.2 verfügbaren Änderungen finden Sie unter [21.2 Versionsübersicht](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Ansicht auf Monatsebene im Arbeitslastausgleich

Um Ihnen bei der Verwaltung der Ressourcenzuweisung für längere Zeiträume zu helfen, haben wir jetzt eine Ansicht auf Monatsebene für den Arbeitslastausgleich implementiert. Sie können bis zu drei Monate gleichzeitig anzeigen und die monatlichen Ressourcenzuweisungen aktualisieren. Vor dieser Änderung konnten Sie den Lastenausgleich nur nach Tag oder Woche anzeigen.

Weitere Informationen finden Sie unter [Navigieren Sie zum Lastenausgleich .](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Verbindung zwischen dem Szenario-Planer, dem Arbeitslastausgleich und der Aufgabenliste

>[!NOTE]
>
>Nur im neuen Adobe Workfront-Erlebnis verfügbar.

Um Sie bei der strategischen Planung Ihrer Projekte zu unterstützen und sicherzustellen, dass sie mit den größeren Initiativen des Szenario-Planers in Einklang stehen, haben wir einen neuen Bereich für das Projekt erstellt, in dem die Anforderungen an die Rolle von Arbeitsplätzen aus den Initiativen sowie die geplanten Arbeitszeiten für die Arbeitselemente des Projekts dargestellt werden. Dieser Bereich ist für den Arbeitslastausgleich auf Projektebene sowie für die Aufgabenliste im neuen Workfront-Erlebnis verfügbar. Im klassischen Erlebnis ist dies nur für den Projekt Workload Balancer verfügbar.

Weitere Informationen finden Sie in den folgenden Artikeln:

* [Übersicht über die Abstimmung der Ressourcenzuweisungen zwischen Projekten und Initiativen](../../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).
* [Navigieren Sie zum Lastenausgleich .](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)

>[!IMPORTANT]
>
>Diese neue Funktion ist für alle Benutzer sichtbar, sowohl im neuen als auch im klassischen Workfront-Erlebnis. Dies ist auch für Kunden sichtbar, die keine Workfront Scenario Planer-Lizenz erworben haben.

## Verwenden Sie geplante Stunden bei der Berechnung der Nettowerte im Ressourcenplaner.

Eine neue Einstellung im Resource Planer ermöglicht die Verwendung von &quot;Geplante Stunden&quot;bei der Berechnung von Netzwerten.

Vor dieser Verbesserung berechnete Workfront die Nettowerte nur unter Verwendung von Budgetzeit. Der Nettowert zeigt die Differenz zwischen verfügbaren und geplanten oder geplanten Stunden, FTE oder Kosten an. Budgetierte Stunden sind bei der Berechnung der Nettowerte weiterhin die Standardeinstellung.

Weitere Informationen finden Sie unter [Übersicht über Stunden, FTE und Kosteninformationen in den Projekt- und Rollenansichten des Ressourcenplaners](../../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md).

## 12-wöchige Ansicht im Arbeitslastausgleich

Sie können jetzt bis zu 12 Wochen Informationen im Arbeitslastausgleich anzeigen. Vor dieser Verbesserung konnten Sie Informationen zu 2, 4 und 6 Wochen anzeigen.

Informationen zum Anzeigen des Lastenausgleichs finden Sie unter [Navigieren Sie zum Lastenausgleich .](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)Navigieren Sie zum Lastenausgleich.

## Änderung der Funktionsweise des Filters &quot;Auftragsrolle&quot;im Bereich &quot;Nicht zugewiesen&quot;des Workload-Balancers

Um die Funktionsweise des Filters &quot;Auftragsrolle&quot;im Arbeitslastausgleich zu verbessern und die Erwartungen der Benutzer zu erfüllen, haben wir die Funktionalität des Filters im Bereich Nicht zugewiesen geändert. Sie können jetzt nur die Stunden anzeigen, die den im Filter angegebenen Auftragsrollen zugeordnet sind.

Vor dieser Verbesserung wurden beim Anwenden des Filters Auftragsrolle auf den nicht zugewiesenen Bereich im Arbeitslastausgleich alle Stunden angezeigt, die mit den den Auftragsrollen zugewiesenen Arbeitselementen verknüpft sind.

Informationen zum Filtern von Informationen im Arbeitslastausgleich finden Sie unter [Verwalten von Filtern im Lastenausgleich](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).
