---
title: Projekte löschen
product-area: projects
navigation-topic: manage-projects
description: Sie können ein Projekt löschen, wenn das Projekt und seine Daten nicht mehr benötigt werden. Als Alternative zum Löschen eines Projekts empfehlen wir, das Projekt zu bearbeiten und den Status in „Abgeschlossen“ oder „Inaktiv“ zu ändern. Dadurch werden alle aktuellen Aufgaben im Zusammenhang mit dem Projekt aus der Aufgabenliste eines Benutzers entfernt, alle mit dem Projekt verknüpften Daten werden jedoch gespeichert.
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
recommendations: noDisplay, noCatalog
source-git-commit: ba5089fd02ca099d25ce0d3c2c2c039c2c6e2fe2
workflow-type: tm+mt
source-wordcount: '1067'
ht-degree: 3%

---

# Projekte löschen

<!--Audited: 07/2024-->

Sie können ein Projekt löschen, wenn das Projekt und seine Daten nicht mehr benötigt werden.

Als Alternative zum Löschen eines Projekts empfehlen wir, das Projekt zu bearbeiten und den Status in „Abgeschlossen“ oder „Inaktiv“ zu ändern. Dadurch werden alle aktuellen Aufgaben im Zusammenhang mit dem Projekt aus der Aufgabenliste eines Benutzers entfernt, alle mit dem Projekt verknüpften Daten werden jedoch gespeichert.

Sie können ein Projekt in einer Projektliste oder auf Projektebene löschen.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront-Paket</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront-Lizenz</p> </td> 
   <td> <p>Standard</p>
   <p>Plan</p> 
   </td> 
  </tr> 
    <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte mit der Möglichkeit zum Erstellen und Löschen von Projekten bearbeiten</p> </td> 
  </tr> 
    <td> <p>Objektberechtigungen</p> </td> 
   <td> <p>Zugriff auf Projekte, Aufgaben und Probleme bearbeiten mit der Möglichkeit, Projekte, Aufgaben und Probleme zu löschen</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>New license: Standard </p>
   <p>Current license: Plan </p> 
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level configuration</td> 
   <td> <p>Edit access to Projects with ability to Create and Delete projects</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>Edit access to Projects, Tasks, Issues with ability to Delete projects, tasks, and issues</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Verstehen des Prozesses zum Löschen von Projekten

* [Einschränkungen für das Löschen von Projekten](#limitations-for-deleting-projects)
* [Auswirkungen des Löschens von Projekten](#the-impact-of-deleting-projects)

### Einschränkungen beim Löschen von Projekten  {#limitations-for-deleting-projects}

* Gelöschte Elemente werden 30 Tage lang in den Papierkorb verschoben und können nur vom Workfront-Administrator wiederhergestellt werden.

  Weitere Informationen zum Wiederherstellen von Objekten finden Sie im Artikel [Wiederherstellen gelöschter Elemente](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Wenn das Projekt Aufgaben oder Probleme mit protokollierten Stunden aufweist, muss der Workfront- oder Gruppenadministrator das Löschen dieser Aufgaben durch Konfigurieren der Voreinstellungen für Aufgaben und Probleme in Ihrer Workfront-Instanz zulassen, damit Sie das Projekt, das die Aufgaben enthält, löschen können.

  Weitere Informationen zum Aktivieren des Löschens von Aufgaben, Problemen oder Projekten, bei denen Stunden protokolliert werden, finden Sie im Abschnitt „Löschen“ in [Konfigurieren von systemweiten Aufgaben- und Problemeinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### Auswirkungen des Löschens von Projekten {#the-impact-of-deleting-projects}

* Wenn Sie ein Projekt löschen, wirkt sich dies auf andere mit dem Projekt verknüpfte Objekte aus.

  Die folgenden an ein Projekt angehängten Objekte werden ebenfalls gelöscht, wenn Sie ein Projekt löschen:

   * Dokumente

     Sie können ein Projekt, an das ein ausgechecktes Dokument angehängt ist, nicht löschen. Weitere Informationen zum Auschecken von Dokumenten finden Sie unter [Auschecken von Dokumenten](../../../documents/managing-documents/check-out-documents.md).

   * Aufgaben
   * Teilaufgaben
   * Probleme
   * Updates
   * Genehmigungen
   * Ausgaben
   * Risiken
   * Baselines
   * Business Case-Informationen
   * Warteschlangendetails-Informationen
   * Abrechnungssätze
   * Abrechnungseinträge

     Sie können kein Projekt löschen, das Rechnungsnachweise mit dem Status In Rechnung gestellt enthält. Weitere Informationen finden Sie unter [Rechnungsnachweise erstellen](../../projects/project-finances/create-billing-records.md).

* Je nachdem, wie Ihr Workfront-Administrator die Voreinstellungen für die Projekt-, Aufgaben- oder Problemlöschung in der Arbeitszeittabelle und den Stundeneinstellungen Ihrer Workfront-Instanz konfiguriert, werden die für die Aufgaben, Probleme oder das Projekt protokollierten Stunden beim Löschen des Projekts auf eine der folgenden Arten gehandhabt:

   * Die Stunden verbleiben auf der Arbeitszeittabelle als allgemeine Zeit.
   * Die Stunden werden gelöscht und werden wiederhergestellt, falls das Projekt jemals wiederhergestellt wird.

  Weitere Informationen zum Konfigurieren der Löschvoreinstellungen für Stunden, die bei Problemen protokolliert sind, finden Sie unter [Konfigurieren von Arbeitszeittabellen- und Stundenvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Wenn das zu löschende Projekt mit einer Initiative im Workfront-Szenarioplaner verknüpft ist:

   * Die Initiative bleibt im Plan, aber die Verknüpfung zum Projekt wird entfernt.
   * Wenn das zu löschende Projekt mit der einzigen veröffentlichten Initiative aus einem Plan verknüpft ist, wird auch der Hinweis entfernt, dass der Plan veröffentlicht wurde.
   * Wenn Sie ein gelöschtes Projekt wiederherstellen, wird das Projekt wiederhergestellt, aber sein Link zur Initiative wird nicht wiederhergestellt und der Bereich Szenario-Planer wird nicht mehr in den Projektdetails angezeigt.

     Für den Szenario-Planer ist eine zusätzliche Lizenz erforderlich. Weitere Informationen zum Workfront-Szenarioplaner finden Sie unter [Szenarioplaner - Übersicht](../../../scenario-planner/scenario-planner-overview.md).

     Informationen zu Projekten, die mit Initiativen im Szenario-Planer verknüpft sind, finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichung von Initiativen im Szenario-Planer](../../../scenario-planner/publish-scenarios-update-projects.md).

* Wenn das Projekt auch eine Aktivität für ein Ziel in Workfront Goals ist:

   * Das Projekt wird aus dem Ziel gelöscht. Der vom Projekt für das Ziel angegebene Fortschritt wird ebenfalls entfernt.

   * Wenn Sie das gelöschte Projekt wiederherstellen, wird das Projekt auch als Zielaktivität wiederhergestellt.

     Dies erfordert eine zusätzliche Lizenz. Informationen zu Workfront-Zielen finden Sie unter [Adobe Workfront-Ziele - Übersicht](../../../workfront-goals/goal-management/wf-goals-overview.md).

     Informationen zum Verknüpfen von Projekten mit Zielen finden Sie unter [Hinzufügen von Projekten zu Zielen in Adobe Workfront Goals](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## Löschen eines Projekts in einer Liste

Sie können Projekte aus einer Projektliste löschen.

1. Navigieren Sie zu einer Liste von Projekten oder einem Projektbericht.
1. Wählen Sie das bzw. die Projekte aus, die Sie löschen möchten, und klicken Sie dann oben in **Liste auf** Löschen![Symbol &quot;](assets/delete-icon.png)&quot;.

1. Klicken Sie auf **Ja, löschen**, um den Löschvorgang zu bestätigen.

   Die Projekte werden gelöscht und für 30 Tage im Papierkorb gespeichert. Ihr Workfront-Administrator kann gelöschte Projekte während dieses Zeitraums aus dem Papierkorb wiederherstellen.

## Löschen eines Projekts auf Projektebene

1. Wechseln Sie zu dem Projekt, das Sie löschen möchten.
1. Klicken Sie auf das **Mehr**-Symbol ![Mehr ](assets/qs-more-menu.png) rechts neben dem Projektnamen und klicken Sie dann auf **Projekt löschen**.

   ![Mehr Menü erweitert](assets/more-icon-expanded-delete-project-highlighted.png)

1. Klicken Sie **Ja, löschen**.

   Das Projekt wird gelöscht und für 30 Tage im Papierkorb gespeichert. Ihr Workfront-Administrator kann sie während dieses Zeitraums aus dem Papierkorb wiederherstellen.

## Löschen eines Projekts von der Seite „Verbundene Datensätze“ eines Workfront Planning-Datensatzes

>[!NOTE]
>
>Die Informationen in diesem Abschnitt beziehen sich auf Adobe Workfront Planning, eine zusätzliche Funktion von Adobe Workfront.
>
>Eine Liste der Anforderungen für den Zugriff auf Workfront Planning finden Sie unter [Zugriffsübersicht für Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).
> 
>Allgemeine Informationen zu Workfront Planning finden Sie unter [Erste Schritte mit Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Sie müssen über Folgendes verfügen, bevor Sie auf Projekte in einer Workfront Planning-Seite mit verbundenen Datensätzen zugreifen und sie löschen können:

* Planen von Datensatztypen im Zusammenhang mit Workfront-Projekten. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
* Planungsunterlagen. Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).
* Eine Seite mit verbundenen Datensätzen, auf der mit einem Planungsdatensatz verbundene Projekte angezeigt werden. Weitere Informationen finden Sie unter [Hinzufügen einer verbundenen Datensatzseite zu einem Datensatz](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

So löschen Sie einen Datensatz aus einer verbundenen Datensatzseite:

1. Bewegen Sie auf der Seite „Verbundene Datensätze“, auf der die mit einem Datensatz verbundenen Projekte angezeigt werden, den Mauszeiger über den Namen eines Projekts und klicken Sie auf das Symbol **Mehr** ![Mehr](assets/more-icon.png)

   ODER

   Ein oder mehrere Projekte in der Liste auswählen. Beachten Sie den blauen Balken am unteren Rand der Projektliste.

1. Klicken Sie **Löschen** und dann **Löschen** zur Bestätigung.

   Die Projekte werden gelöscht und in den Workfront-Papierkorb verschoben.

## Gelöschte Projekte wiederherstellen

Ein System- oder Gruppen-Administrator kann Projekte innerhalb von 30 Tagen nach dem Löschen wiederherstellen, wie im Artikel &quot;[ gelöschter Elemente wiederherstellen“ ](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
