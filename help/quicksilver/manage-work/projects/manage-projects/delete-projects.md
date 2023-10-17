---
title: Projekte löschen
product-area: projects
navigation-topic: manage-projects
description: Sie können ein Projekt löschen, wenn das Projekt und seine Daten nicht mehr benötigt werden.
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
source-git-commit: 5db9a4869e1321bd268e80f786d157fbb41c0656
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 1%

---

# Projekte löschen

Sie können ein Projekt löschen, wenn das Projekt und seine Daten nicht mehr benötigt werden.

Als Alternative zum Löschen eines Projekts wird empfohlen, das Projekt zu bearbeiten und den Status in &quot;Abgeschlossen&quot;oder &quot;Dead&quot;zu ändern. Dadurch werden alle aktuellen Aufgaben im Zusammenhang mit dem Projekt aus der Aufgabenliste eines Benutzers entfernt, jedoch alle mit dem Projekt verknüpften Daten gespeichert.

## Zugriffsanforderungen

<!-- drafted for P&P:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Projects with ability to Create <span>and Delete</span> projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>Edit access to Projects, Tasks, Issues with ability to Delete projects, tasks, and issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Bearbeiten des Zugriffs auf Projekte, Aufgaben, Probleme mit der Möglichkeit, Projekte, Aufgaben und Probleme zu löschen</p> <p><b>NOTIZ</b></p>

<p>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten Sie Berechtigungen für das Projekt, Aufgaben und Probleme im Projekt mit der Möglichkeit, das Projekt, die Aufgaben und Probleme zu löschen. </p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.
Sie können ein Projekt in einer Projektliste oder auf Projektebene löschen.

## Grundlegendes zum Löschen von Projekten

* [Einschränkungen beim Löschen von Projekten](#limitations-for-deleting-projects)
* [Auswirkungen des Löschens von Projekten](#the-impact-of-deleting-projects)

### Einschränkungen beim Löschen von Projekten  {#limitations-for-deleting-projects}

* Gelöschte Elemente werden 30 Tage lang in den Papierkorb verschoben und können nur vom Workfront-Administrator wiederhergestellt werden.

  Weitere Informationen zum Wiederherstellen von Objekten finden Sie im Artikel [Gelöschte Elemente wiederherstellen](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Wenn das Projekt Aufgaben oder Probleme mit angemeldeten Stunden hat, muss der Workfront- oder Gruppenadministrator das Löschen dieser Aufgaben zulassen, indem er die Voreinstellungen für Aufgaben und Probleme in Ihrer Workfront-Instanz konfiguriert, damit Sie das Projekt, das die Aufgaben enthält, löschen können.

  Weitere Informationen zum Aktivieren des Löschens von Aufgaben, Problemen oder Projekten, bei denen Stunden protokolliert werden, finden Sie im Abschnitt &quot;Löschen&quot;unter [Systemweite Aufgaben- und Problemeinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### Auswirkungen des Löschens von Projekten {#the-impact-of-deleting-projects}

* Wenn Sie ein Projekt löschen, wirkt sich dies auf andere Objekte aus, die mit dem Projekt verknüpft sind.

  Die folgenden Objekte, die an ein Projekt angehängt sind, werden auch beim Löschen eines Projekts gelöscht:

   * Dokumente

     Sie können ein Projekt mit einem angehängten Dokument, das ausgecheckt wurde, nicht löschen. Weitere Informationen zum Auschecken von Dokumenten finden Sie unter [Dokumente auschecken](../../../documents/managing-documents/check-out-documents.md).

   * Aufgaben
   * Teilaufgaben
   * Probleme
   * Updates
   * Genehmigungen
   * Ausgaben
   * Risiken
   * Baselines
   * Informationen zu Geschäftsfällen
   * Informationen zu Warteschlangendetails
   * Abrechnungssätze
   * Rechnungsnachweise

     Sie können ein Projekt mit dem Status Rechnungseinträge nicht löschen. Weitere Informationen finden Sie unter [Erstellen von Rechnungsdatensätzen](../../projects/project-finances/create-billing-records.md).

* Je nachdem, wie Ihr Workfront-Administrator die Voreinstellungen zum Projekt, zur Aufgabe oder zur Problemlöschung in den Voreinstellungen für das Arbeitsblatt und die Stunde Ihrer Workfront-Instanz konfiguriert, werden die für die Aufgaben, Probleme oder das Projekt protokollierten Stunden beim Löschen des Projekts auf eine der folgenden Arten verarbeitet:

   * Die Stunden bleiben auf dem Timesheet als allgemeine Zeit.
   * Die Stunden werden gelöscht und wiederhergestellt, wenn das Projekt jemals wiederhergestellt wird.

  Weitere Informationen zum Konfigurieren der Löscheinstellungen für Stunden, die bei Problemen protokolliert werden, finden Sie unter [Zeitblatt- und Stundenvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

* Wenn das Projekt, das Sie löschen, mit einer Initiative im Workfront-Szenario-Planer verknüpft ist:

   * Die Initiative bleibt im Plan, aber die Verknüpfung mit dem Projekt wird entfernt.
   * Wenn das Projekt, das Sie löschen, mit der einzigen veröffentlichten Initiative aus einem Plan verknüpft ist, wird auch der Hinweis, dass der Plan veröffentlicht wurde, entfernt.
   * Wenn Sie ein gelöschtes Projekt wiederherstellen, wird das Projekt zwar wiederhergestellt, die Verknüpfung zur Initiative jedoch nicht wiederhergestellt und der Bereich &quot;Szenario-Planer&quot;wird nicht mehr in den Projektdetails angezeigt.

     Der Szenario-Planer ist nur im neuen Adobe Workfront-Erlebnis verfügbar und erfordert eine zusätzliche Lizenz. Weitere Informationen zum Workfront-Szenario-Planer finden Sie unter [Übersicht über den Szenario-Planer](../../../scenario-planner/scenario-planner-overview.md).

     Informationen zu Projekten, die mit Initiativen im Szenario-Planer verknüpft sind, finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen im Szenario-Planer](../../../scenario-planner/publish-scenarios-update-projects.md).

* Wenn das Projekt auch eine Aktivität für ein Ziel in Workfront-Zielen ist:

   * Das Projekt wird aus dem Ziel gelöscht. Der durch das Projekt angegebene Fortschritt im Ziel wird ebenfalls entfernt.

   * Wenn Sie das gelöschte Projekt wiederherstellen, wird das Projekt auch als die Aktivität des Ziels wiederhergestellt.

     Dies erfordert eine zusätzliche Lizenz. Weitere Informationen zu Workfront-Zielen finden Sie unter [Übersicht über Adobe Workfront-Ziele](../../../workfront-goals/goal-management/wf-goals-overview.md).

     Weitere Informationen zum Verknüpfen von Projekten mit Zielen finden Sie unter [Hinzufügen von Projekten zu Zielen in Adobe Workfront-Zielen](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md).

## Projekt in einer Liste löschen

Sie können Projekte aus einer Liste von Projekten löschen.

1. Gehen Sie zu einer Liste von Projekten oder einem Projektbericht.
1. Wählen Sie das Projekt bzw. die Projekte aus, das/die Sie löschen möchten, und klicken Sie dann auf **Löschen** icon ![](assets/delete-icon.png) oben in der Liste.

1. Klicks **Ja, löschen** , um den Löschvorgang zu bestätigen.

   Die Projekte werden gelöscht und 30 Tage lang im Papierkorb gespeichert. Ihr Workfront-Administrator kann während dieser Zeit gelöschte Projekte aus dem Papierkorb wiederherstellen.

## Löschen eines Projekts auf Projektebene

1. Wechseln Sie zu dem Projekt, das Sie löschen möchten.
1. Klicken Sie auf **Mehr** icon ![](assets/qs-more-menu.png)Klicken Sie auf **Projekt löschen**.

   ![](assets/more-icon-expanded-delete-project-highlighted.png)

1. Klicks **Ja, löschen**.

   Das Projekt wird gelöscht und 30 Tage lang im Papierkorb gespeichert. Ihr Workfront-Administrator kann ihn während dieser Zeit aus dem Papierkorb wiederherstellen.

## Wiederherstellen gelöschter Projekte

Ein System- oder Gruppenadministrator kann Projekte innerhalb von 30 Tagen nach dem Löschen wiederherstellen, wie im Artikel beschrieben. [Gelöschte Elemente wiederherstellen](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).
