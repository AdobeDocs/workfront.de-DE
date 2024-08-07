---
content-type: release-notes
navigation-topic: product-releases-archive
title: Beta-Version 2018.1 - Aktivität "Abschließende Version"
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschauumgebung mit der endgültigen Beta-Version 2018.1 verfügbar waren. Die Funktion wurde am 31. Januar 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird im März 2018 in der Produktionsumgebung zur Verfügung gestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 35bd3604-5452-4b46-afb1-78bc2fbb48ec
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# Beta-Version 2018.1 - Aktivität &quot;Abschließende Version&quot;

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschauumgebung mit der endgültigen Beta-Version 2018.1 verfügbar waren. Die Funktion wurde am 31. Januar 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird im März 2018 in der Produktionsumgebung zur Verfügung gestellt.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen, die 2018.1 vorgenommen wurden, finden Sie unter  [Übersicht über die Veröffentlichungsaktivität 2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

Die endgültige Version 2018.1 von Beta enthält Verbesserungen für Workfront-Administratoren und andere Benutzer:

**Für Administratoren**

* [Konfigurieren der Ressourcenverfügbarkeit und der Benutzerzuordnungen zur Berechnung auf der Grundlage des Benutzerzeitplans](#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule)

**Für alle Benutzer**

* [Mobile Verbesserungen](#mobile-enhancements)
* [Jira-Integration](#jira-integration)
* [Aktualisierung zum Testen von Viewer-Namen](#update-to-proofing-viewer-names)
* [Wechsel zur Synchronisierungskadenz bei der Synchronisierung von der Testproduktionsumgebung zur Vorschau ](#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview)
* [Warnmeldung wird angezeigt, wenn die 2.000 Elementgrenze im Ressourcenplaner erreicht ist](#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner)

## Mobile Verbesserungen {#mobile-enhancements}

Die folgenden Funktionen werden Anfang März 2018 in den Appstores verfügbar sein:

* Neue Navigation: Die Startseite unserer mobilen Apps wurde neu gestaltet.
* Startseite auf Mobile: Unsere neue Startseite wurde jetzt auch in unseren mobilen Apps aktualisiert.

Die neue Funktion wird sowohl für die iOS- als auch für die Android-Plattformen unterstützt.

## Jira-Integration {#jira-integration}

Sie können jetzt Jira-Probleme mit Workfront-Aufgaben oder -Problemen verknüpfen, indem Sie das Workfront-Add-on für Jira installieren und konfigurieren. Mit dieser Integration können Ihre Projektmanager weiterhin in Workfront arbeiten, während Ihre Entwicklungstechniker weiterhin in Jira arbeiten können, während ihre einzelnen Elemente durch die Integration von Workfront mit Jira verknüpft werden.

Sie können Folgendes über diese Integration konfigurieren:

* Legen Sie Trigger für Workfront-Zuweisungen fest, um automatisch Jira-Probleme zu erstellen, wenn sie auftreten.
* Verknüpfen Sie Jira-Probleme manuell mit Workfront-Aufgaben oder -Problemen, die bereits erstellt wurden.
* Geben Sie Felder an, die mit den verknüpften Elementen synchronisiert werden sollen, sobald eines der Elemente in einer der Anwendungen aktualisiert wurde.

Das Workfront-Add-on ist für die On-Premise- und On-Demand-Versionen von Jira verfügbar. Das Add-on ist kostenlos und steht ab März 2018 im Atlassian Marketplace zum Download bereit.

Weitere Informationen zum Workfront-Add-on für Jira, einschließlich eines Links zum Herunterladen, finden Sie unter [Verwenden von Workfront mit Jira](https://support.workfront.com/hc/en-us/sections/115001130053).

## Aktualisierung von Viewer-Namen für die Überprüfung {#update-to-proofing-viewer-names}

Die Namen des HTML5-basierten Testversand-Viewers und der Flash-basierten Testversand-Viewer wurden im gesamten Workfront-System neu benannt. Die vorherigen und aktualisierten Namen lauten wie folgt: 

| **Vorheriger Name** | **Aktualisierter Name** |
|---|---|
| HTML5-Testversand-Viewer | Neuer Testversand-Viewer |
| Flash Proofing-Viewer | Alter Testversand-Viewer |

{style="table-layout:auto"}

 Weitere Informationen zur Verwendung des neuen Testversand-Viewers finden Sie unter [Überprüfen von Testsendungen im Testversand-Viewer.](https://support.workfront.com/hc/en-us/sections/115000275214)

## Konfigurieren der Ressourcenverfügbarkeit und der Benutzerzuordnungen zur Berechnung auf der Grundlage des Benutzerzeitplans {#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule}

>[!NOTE]
>
>Die Tools für die Ressourcenplanung wurden mit Version 23.1 eingestellt und aus Workfront entfernt. Weitere Informationen zum Planen von Ressourcen mit dem Lastenausgleich finden Sie unter [Übersicht über den Lastenausgleich](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Der Workfront-Administrator kann jetzt bestimmen, wie Workfront die Ressourcenverfügbarkeit und die Benutzerzuweisung auf Systemebene berechnet (unter Berücksichtigung von Stunden und FTE-Verfügbarkeit). Der Workfront-Administrator kann die Ressourcenverfügbarkeit und die Benutzerzuordnung so konfigurieren, dass sie entweder anhand des Standardzeitplans oder des Benutzerzeitplans berechnet werden.

Diese Einstellung wirkt sich bei der Planung von Ressourcen auf die Benutzerverfügbarkeit in den folgenden Situationen aus:

* Wenn es Workfront ermöglicht, Ressourcen automatisch zuzuweisen, wie unter &quot;Nicht zugewiesene Aufgaben und Probleme manuell in den Planungsbereichen zuweisen&quot;beschrieben.

* Beim Anzeigen von Zuordnungsindikatoren, wie unter &quot;Verwalten von Benutzerzuweisungen in den Planungsbereichen&quot;beschrieben.

Weitere Informationen finden Sie unter &quot;Konfigurieren, wie Workfront Ressourcenstunden und die FTE-Verfügbarkeit für den Planungsbereich berechnet&quot;.

>[!NOTE]
>
>Die Tools für die Ressourcenplanung wurden mit Version 23.1 eingestellt und aus Workfront entfernt. Weitere Informationen zum Planen von Ressourcen mit dem Lastenausgleich finden Sie unter [Übersicht über den Lastenausgleich](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).


## Änderung an der Synchronisierungskadenz bei der Synchronisierung von der Testproduktionsumgebung in die Vorschau {#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview}

>[!NOTE]
>
>Diese Änderung tritt am 11. Februar 2018 in Kraft.

Daten aus der Workfront Proof-Produktionsumgebung werden nun wöchentlich mit der Workfront Proof-Vorschau-Umgebung synchronisiert.

Vor dieser Änderung wurden die Daten monatlich aus der Workfront Proof-Produktionsumgebung in die Vorschau-Umgebung synchronisiert, während die Daten aus der Workfront-Produktionsumgebung wöchentlich mit der Workfront-Vorschau-Umgebung synchronisiert wurden. Diese Diskrepanz verursachte einige Synchronisierungsfehler bei der Verwendung der Proofing-Funktion in der Workfront-Vorschau-Umgebung. 

Weitere Informationen finden Sie unter [Vorschau der Sandbox-Testumgebung - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md). 

## Warnmeldung wird angezeigt, wenn die 2.000 Elementgrenze im Ressourcenplaner erreicht ist {#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner}

Da wir derzeit an einer dauerhafteren Lösung arbeiten, um die Leistung im Ressourcen-Planer zu verbessern, haben wir für jede Ansicht, die Sie auf den Ressourcen-Planer anwenden können, eine Beschränkung von 2.000 Elementen eingeführt:

* In der Benutzeransicht werden nur 2.000 Zuweisungen angezeigt
* In der Projektansicht werden nur 2.000 Projekte angezeigt
* In der Rollenansicht werden nur 2.000 Rollen angezeigt

Wenn der Ressourcen-Planer versucht, mehr als 2.000 Elemente zu laden, wird eine Benachrichtigung angezeigt, die Sie darauf hinweist, dass nur 2.000 Elemente angezeigt werden können.

Weitere Informationen zu diesen Beschränkungen und deren Auswirkungen auf den Ressourcen-Planer finden Sie unter [Anzeigebeschränkungen für Ressourcen-Planer](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our beta program for the Resource Planner performance, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a>.</p>
-->
