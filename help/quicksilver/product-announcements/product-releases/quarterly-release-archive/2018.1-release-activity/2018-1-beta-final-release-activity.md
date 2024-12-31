---
content-type: release-notes
navigation-topic: product-releases-archive
title: Beta-Aktivität zur endgültigen Version 2018.1
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit der Beta-Endversion 2018.1 verfügbar waren. Die Funktion wurde am 31. Januar 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird ab März 2018 in der Produktionsumgebung verfügbar sein.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 35bd3604-5452-4b46-afb1-78bc2fbb48ec
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 0%

---

# Beta-Aktivität zur endgültigen Version 2018.1

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit der Beta-Endversion 2018.1 verfügbar waren. Die Funktion wurde am 31. Januar 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird ab März 2018 in der Produktionsumgebung verfügbar sein.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktion kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen in Version 2018.1 finden Sie unter  Übersicht über die Versionsaktivität [2018.1](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md).

Die Beta-Endversion 2018.1 enthält Verbesserungen für Workfront-Admins und andere Benutzende:

**Für Administratoren**

* [Konfigurieren Sie die Ressourcenverfügbarkeit und die Benutzerzuteilungen, die basierend auf dem Benutzerzeitplan berechnet werden sollen](#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule)

**Für alle Benutzer**

* [Verbesserungen für Mobilgeräte](#mobile-enhancements)
* [Jira-Integration](#jira-integration)
* [Aktualisieren der Proofing-Viewer-Namen](#update-to-proofing-viewer-names)
* [Änderung der Synchronisierungskadenz bei der Synchronisierung von der Proofing-Produktionsumgebung zur Vorschau](#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview)
* [Es wird eine Warnmeldung angezeigt, wenn das Limit von 2.000 Elementen im Ressourcenplaner erreicht wird](#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner)

## Verbesserungen für Mobilgeräte {#mobile-enhancements}

Anfang März 2018 kommen folgende Funktionen in die Mobile App Stores:

* Neue Navigation: Die Startseite unserer Mobile Apps wurde neu gestaltet.
* Home on Mobile: Unsere neue Home-Funktion wurde jetzt auch in unseren Mobile Apps aktualisiert.

Die neue Funktion wird sowohl für die iOS- als auch für die Android-Plattform unterstützt.

## Jira-Integration {#jira-integration}

Sie können jetzt Jira-Probleme mit Workfront-Aufgaben oder -Problemen verknüpfen, indem Sie das Workfront-Add-on für Jira installieren und konfigurieren. Mit dieser Integration können Ihre Projektmanager weiterhin in Workfront arbeiten, während Ihre Entwicklungsingenieure weiterhin in Jira arbeiten können, während ihre einzelnen Elemente durch die Integration von Workfront mit Jira verknüpft werden.

Durch diese Integration können Sie Folgendes konfigurieren:

* Erstellen Sie Trigger für Workfront-Arbeitsaufträge, um Jira-Probleme automatisch zu erstellen, wenn sie auftreten.
* Jira-Probleme manuell mit Workfront-Aufgaben oder zuvor erstellten Problemen verknüpfen.
* Geben Sie Felder an, die in den verknüpften Elementen synchronisiert werden sollen, sobald eines der Elemente in einem der Programme aktualisiert wird.

Das Workfront-Add-on wird sowohl für On-Premise- als auch für On-Demand-Versionen von Jira verfügbar sein. Das Add-on ist kostenlos und wird Anfang März 2018 im Atlassian Marketplace zum Download zur Verfügung stehen.

Weitere Informationen zum Workfront-Add-on für Jira, einschließlich eines Links zum Herunterladen, finden Sie unter [Verwenden von Workfront mit Jira.](https://support.workfront.com/hc/en-us/sections/115001130053)

## Aktualisieren der Proofing-Viewer-Namen {#update-to-proofing-viewer-names}

Die Namen des HTML5-basierten Proofing Viewers und der Flash-basierten Proofing Viewer wurden im gesamten Workfront-System umbenannt. Die bisherigen und aktualisierten Namen lauten wie folgt: 

| **vorheriger Name** | **Name aktualisiert** |
|---|---|
| HTML5 Proofing Viewer | Neuer Proofing Viewer |
| Flash Proofing Viewer | Legacy Proofing Viewer |

{style="table-layout:auto"}

 Weitere Informationen zur Verwendung des neuen Proofing Viewers finden Sie unter [Testsendungen im Proofing Viewer überprüfen“](https://support.workfront.com/hc/en-us/sections/115000275214)

## Konfigurieren Sie die Ressourcenverfügbarkeit und die Benutzerzuteilungen, die basierend auf dem Benutzerzeitplan berechnet werden sollen {#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule}

>[!NOTE]
>
>Die Tools zur Ressourcenplanung werden nicht mehr unterstützt und mit Version 23.1 aus Workfront entfernt. Informationen zur Planung von Ressourcen mit dem Workload Balancer finden Sie unter [Übersicht über den Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Der Workfront-Administrator kann jetzt festlegen, wie Workfront die Ressourcenverfügbarkeit und die Benutzerzuordnung auf Systemebene berechnet (unter Berücksichtigung der Stunden sowie der FTE-Verfügbarkeit). Der Workfront-Administrator kann die Ressourcenverfügbarkeit und Benutzerzuordnung konfigurieren, die entweder anhand des Standardzeitplans oder des Benutzerzeitplans berechnet werden.

Diese Einstellung wirkt sich in den folgenden Fällen beim Planen von Ressourcen auf die Benutzerverfügbarkeit aus:

* Wenn Workfront die automatische Zuweisung von Ressourcen erlaubt, wie in „Manuelles Zuweisen nicht zugewiesener Aufgaben und Probleme in den Zeitplanbereichen“ beschrieben.

* Bei der Anzeige von Zuordnungsindikatoren, wie unter Verwalten von Benutzerzuweisungen in den Zeitplanbereichen beschrieben.

Weitere Informationen finden Sie unter „Konfigurieren der von Workfront berechneten Ressourcenverfügbarkeit für den Planungsbereich“.

>[!NOTE]
>
>Die Tools zur Ressourcenplanung werden nicht mehr unterstützt und mit Version 23.1 aus Workfront entfernt. Informationen zur Planung von Ressourcen mit dem Workload Balancer finden Sie unter [Übersicht über den Workload Balancer](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).


## Ändern der Synchronisierungskadenz bei der Synchronisierung von der Proofing-Produktionsumgebung zur Vorschau {#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview}

>[!NOTE]
>
>Diese Änderung tritt am 11. Februar 2018 in Kraft.

Daten aus der Workfront Proof-Produktionsumgebung werden jetzt wöchentlich mit der Workfront Proof-Vorschau-Umgebung synchronisiert.

Vor dieser Änderung wurden Daten monatlich von der Workfront Proof-Produktionsumgebung mit der Vorschau-Umgebung synchronisiert, während die Daten aus der Workfront-Produktionsumgebung wöchentlich mit der Workfront-Vorschau-Umgebung synchronisiert wurden. Diese Diskrepanz führte zu einigen Synchronisierungsfehlern bei der Verwendung der Proofing-Funktion in der Workfront-Vorschau-Umgebung. 

Weitere Informationen finden Sie unter [Vorschau der Sandbox-Testumgebung - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md). 

## Es wird eine Warnmeldung angezeigt, wenn das Limit von 2.000 Elementen im Ressourcenplaner erreicht wird {#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner}

Da wir derzeit an einer dauerhafteren Lösung arbeiten, um die Leistung im Ressourcenplaner zu verbessern, haben wir ein Limit von 2.000 Elementen für jede Ansicht eingeführt, die Sie auf den Ressourcenplaner anwenden können:

* In der Benutzeransicht werden nur 2.000 Zuweisungen angezeigt
* In der Projektansicht werden nur 2.000 Projekte angezeigt
* Die Rollenansicht zeigt nur 2.000 Rollen an

Wenn der Ressourcenplaner versucht, mehr als 2.000 Elemente zu laden, werden Sie durch eine Benachrichtigung darauf hingewiesen, dass nur 2.000 Elemente angezeigt werden können.

Weitere Informationen zu diesen Einschränkungen und deren Auswirkungen auf den Ressourcenplaner finden Sie unter [Anzeigebeschränkungen für den Ressourcenplaner](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our beta program for the Resource Planner performance, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a>.</p>
-->
