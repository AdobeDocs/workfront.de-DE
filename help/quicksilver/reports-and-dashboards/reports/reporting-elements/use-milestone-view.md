---
product-area: reporting
navigation-topic: reporting-elements
title: Verwenden der Milestone-Ansicht
description: Sie können die Meilensteinansicht auf eine Projektliste oder einen Bericht anwenden.
author: Alina
feature: Reports and Dashboards
exl-id: c55e53b5-5559-4b6a-a8d7-5028be6af30f
source-git-commit: dcdcf21903d0fceb3c05039689bb87ae4c834d07
workflow-type: tm+mt
source-wordcount: '1397'
ht-degree: 1%

---

# Verwenden der Milestone-Ansicht

Sie können die Meilensteinansicht auf eine Projektliste oder einen Bericht anwenden.

Bevor Sie die Meilensteinansicht verwenden können, müssen Meilensteine konfiguriert werden, Meilensteinpfade müssen zu Projekten hinzugefügt werden und Meilensteine müssen mit Aufgaben verknüpft werden, wie in den Artikeln beschrieben. [Meilensteinpfad erstellen](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md) und [Verknüpfen von Meilensteinen mit Aufgaben](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

Die Meilensteinansicht ist verfügbar, wenn Sie eine Projektliste oder einen Projektbericht anzeigen. In den folgenden Abschnitten wird beschrieben, wie Sie die Meilensteinansicht anzeigen und verwenden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> <p>Arbeit oder höher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender oder höher anzeigen</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Anzeigen von Berechtigungen für einen Projektbericht zum Anwenden der Meilensteinansicht auf einen Bericht</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Wechseln zur Meilensteinansicht {#switch-to-the-milestone-view}

1. Gehen Sie zur Projektliste oder zum Projektbericht, der die Meilensteine enthält, die Sie anzeigen möchten.
1. Klicken Sie auf **Ansicht** Dropdown-Menü, und klicken Sie auf **Milestone**.

   Die Liste oder der Bericht wird in einer Meilensteinansicht angezeigt.

   Informationen zur Meilensteinansicht finden Sie im Abschnitt . [Übersicht zur Meilensteinansicht](#milestone-view-overview) in diesem Artikel.

## Übersicht zur Meilensteinansicht {#milestone-view-overview}

Die Meilensteinansicht ist in Projektlisten und Projektberichten verfügbar. Diese Ansicht ermöglicht es Ihnen, alle Meilensteine, die mit Aufgaben in den angezeigten Projekten verknüpft sind, schnell anzuzeigen.


>[!NOTE]
>
>Die Meilensteinansicht ist in den folgenden Bereichen nicht verfügbar:
>* Timesheets beim Hinzufügen eines Projekts in der Projektliste.



Informationen zum Wechseln zur Meilensteinansicht finden Sie im Abschnitt . [Wechseln zur Meilensteinansicht](#switch-to-the-milestone-view) in diesem Artikel.

![Projekt mit Meilensteinansicht](assets/project-with-milestone-view-with-complete.png)

### Milestone-Ansichtsabschnitte

Wenn Sie die Meilensteinansicht auf eine Liste von Projekten anwenden, werden die Projekte in den folgenden Abschnitten angezeigt:

* Die Projekte, die mit einem Meilensteinpfad verknüpft sind, werden zuerst angezeigt, und zwar unter dem Namen der jeweiligen Meilensteinpfade.

   Workfront sortiert die Projekte im ersten Abschnitt nach folgenden Kriterien in dieser Reihenfolge:

   1. Meilensteinpfad-ID. Sie können die Meilensteinpfad-ID in einem Meilensteinpfad -Bericht anzeigen.

   2. Das Feld, das in der zuvor auf die Projektliste angewendeten Ansicht als erstes Sortierfeld für die Projektliste ausgewählt wurde, bevor Sie die Meilensteinansicht ausgewählt haben.

* Die Projekte, die keinem Milestobe-Pfad zugeordnet sind, werden als Nächstes im Abschnitt Nicht zugewiesen angezeigt. Workfront sortiert die Projekte im Abschnitt Nicht zugewiesen nach dem Feld, das als erstes Sortierfeld für die Projektliste ausgewählt wurde, in der zuvor auf die Projektliste angewendeten Ansicht, bevor Sie die Meilensteinansicht ausgewählt haben.

### Projektinformationen in der Milestone-Ansicht

Beim Anzeigen einer Projektliste oder eines Projektberichts in der Meilensteinansicht sind die folgenden Informationen verfügbar:

* **Geplante Datumswerte oder geplante Daten:** Geben Sie an, ob in der Meilensteinansicht geplante Datumswerte oder geplante Daten angezeigt werden sollen.\
   Die Daten werden für den Start und den Abschluss sowie für jeden Meilenstein im Meilensteinpfad angezeigt.\
   Wenn Sie geplante Daten anzeigen und auch Zugriff auf das Projekt verwalten haben, können Sie die folgenden Daten direkt in der Meilensteinansicht bearbeiten: (Bei der Anzeige der geplanten Datumswerte können die Daten nicht bearbeitet werden, da die geplanten Datumswerte berechnet werden und nicht manuell geändert werden können.)

   * **Projektstartdaten:** Wenn ein Projekt ab dem Startdatum geplant ist, können Sie das Anfangsdatum des Projekts manuell ändern und anschließend das Abschlussdatum berechnen.
   * **Projektabschlussdaten:** Wenn ein Projekt ab dem Abschlussdatum geplant ist, können Sie das Abschlussdatum des Projekts manuell ändern und anschließend das Startdatum berechnen.
   * **Aufgabenkomplementdaten:** Sie können den Abschluss für Aufgaben manuell direkt über die Meilensteinansicht aktualisieren.

* **Prozent abgeschlossen:** Zeigt den Fertigstellungsprozentsatz jeder Aufgabe und jedes Projekts an.\
   Sie können die Anzeige des Fertigungsprozentsatzes deaktivieren, wie im Abschnitt beschrieben [Konfigurieren der in der Meilensteinansicht angezeigten Informationen](#configure-what-information-displays-in-the-milestone-view) in diesem Artikel.\
   Sie können den Fertigungsprozentsatz direkt über die Meilensteinansicht anpassen, wie im Abschnitt beschrieben [Anpassen des Prozentsatzes Abgeschlossen für Aufgaben in der Meilensteinansicht](#adjust-percent-complete-for-tasks-in-the-milestone-view) in diesem Artikel.

* **Symbole für Aufgabenstatus:** Neben jedem Projekt und jeder Aufgabe wird in der Meilensteinansicht ein Statussymbol angezeigt.

   * Im Zeitplan\
      ![](assets/gantt-ontime.png)

   * In Verzug\
      ![](assets/gantt-behind.png)

   * Gefährdet\
      ![](assets/gantt-atrisk.png)

   * In Verzug\
      ![](assets/gantt-late.png)
   Sie können die Anzeige dieser Statussymbole deaktivieren, wie im Abschnitt beschrieben [Konfigurieren der in der Meilensteinansicht angezeigten Informationen](#configure-what-information-displays-in-the-milestone-view) in diesem Artikel.\
   Weitere Informationen zu den einzelnen Statustypen finden Sie im Artikel [Übersicht über den Task Progress Status](../../../manage-work/tasks/task-information/task-progress-status.md).

* **Aufgabenstatusschattierung für abgeschlossene Aufgaben**: Nachdem eine Aufgabe als abgeschlossen markiert wurde, wird der Hintergrund der Aufgabe in der Meilensteinansicht schattiert, um anzugeben, ob die Aufgabe rechtzeitig oder zu spät abgeschlossen wurde:

   * **Rote Schattierung für Aufgabenspalte**: Der Hintergrund einer Aufgabe ist rot, wenn der Fortschrittsstatus **Verspätet**.

   * **Grüne Schattierung für Aufgabenspalte**: Der Hintergrund einer Aufgabe ist grün, wenn der Fortschrittsstatus **Einschaltzeit**.

* **Projektstatusschattierung für die Spalten Projektstart und -abschluss**:

   * **Projektstartspalte**: Der Hintergrund der Spalte Projektstart ist nur rot oder grün, wenn das tatsächliche Startdatum ausgefüllt ist:

      * **Rote Schattierung für die Spalte &quot;Projektstart&quot;**: Der Hintergrund der Spalte Projektstart ist rot, wenn der Fortschrittsstatus des Projekts **Verspätet**.

      * **Grüne Schattierung für die Spalte &quot;Projektstart&quot;**: Der Hintergrund der Spalte Projektstart ist grün, wenn der Fortschrittsstatus des Projekts **Einschaltzeit**.
   * **Spalte &quot;Projektabschluss&quot;**: Der Hintergrund der Spalte Projektabschluss ist nur rot oder grün, wenn das tatsächliche Abschlussdatum angegeben ist:

      * **Rote Schattierung für Spalte &quot;Projektabschluss&quot;**: Der Hintergrund der Spalte Projektabschluss ist rot, wenn der Fortschrittsstatus des Projekts **Verspätet**.

      * **Grüne Schattierung für die Spalte Projektabschluss**: Der Hintergrund der Spalte &quot;Projektabschluss&quot;ist grün, wenn der Fortschrittsstatus des Projekts **Einschaltzeit**.
   * Den Spalten &quot;Start&quot;und &quot;Abschluss&quot;wird keine Farbschattierung zugewiesen, wenn die Aufgaben den Fortschrittsstatus &quot;Risiko&quot;oder &quot;Hinter&quot;aufweisen.

   ![Meilensteinansicht mit Schattierung](assets/milestone-view-with-shading.png)

* **Projektname**: Der Projektname wird mit einem Link zum Projekt angezeigt.
* **Symbol &quot;Projektbedingung&quot;**: Neben dem Projektnamen wird ein Symbol angezeigt, das die Bedingung des Projekts angibt.

## Konfigurieren der in der Meilensteinansicht angezeigten Informationen {#configure-what-information-displays-in-the-milestone-view}

Sie können konfigurieren, ob die folgenden Elemente in der Meilensteinansicht angezeigt werden:

* Symbole für Fortschrittsstatus
* Prozentualer Abschluss der Projekte und Aufgaben

Standardmäßig werden die Symbole für den Projektstatus und der prozentuale Abschluss der Projekte angezeigt.

Alle Änderungen, die Sie an diesen Optionen vornehmen, gelten nur für Sie. andere Benutzer nicht betroffen sind. Die Änderungen, die Sie vornehmen, werden beim nächsten Anmelden bei Adobe Workfront beibehalten.

So konfigurieren Sie, ob die Symbole für den Projektstatus und der Prozentsatz der Projektabschlüsse angezeigt werden:

1. Gehen Sie zur Projektliste oder zum Projektbericht, der die Meilensteine enthält, die Sie anzeigen möchten.
1. Klicken Sie auf **Ansicht** Dropdown-Menü, und klicken Sie auf **Milestone**.\
   Wenn Sie eine Projektliste innerhalb eines Portfolios oder Programms anzeigen, wählen Sie die **Milestone** unterregistrieren.

1. Klicken **Optionen** in der oberen rechten Ecke der Milestone-Ansicht.\
   ![milestone_view_options.png](assets/milestone-view-options-350x141.png)

1. Wählen Sie aus den folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Fortschritt</td> 
      <td> <p>Wählen Sie diese Option aus, um neben jedem Projekt und jeder Aufgabe Symbole für den Fortschrittsstatus anzuzeigen.</p> <p>Diese Option ist standardmäßig aktiviert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prozent abgeschlossen</td> 
      <td> <p>Wählen Sie diese Option aus, um den Fertigstellungsprozentsatz neben jedem Projekt und jeder Aufgabe anzuzeigen.</p> <p>Diese Option ist standardmäßig aktiviert.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Anpassen des Prozentsatzes Abgeschlossen für Aufgaben in der Meilensteinansicht {#adjust-percent-complete-for-tasks-in-the-milestone-view}

Sie können den Prozentsatz der Abgeschlossen für Aufgaben in der Meilensteinansicht anpassen. Sie können den &quot;Percent Complete&quot;für eine übergeordnete Aufgabe (eine Aufgabe, die Unteraufgaben enthält) nicht anpassen.

So passen Sie den Prozentsatz an, der für eine Aufgabe in der Meilensteinansicht abgeschlossen ist:

1. Gehen Sie zur Projektliste oder zum Projektbericht, der die Meilensteine enthält, die Sie anzeigen möchten.
1. Klicken Sie auf **Ansicht** Dropdown-Menü, und klicken Sie auf **Milestone**.

1. (Bedingt) Wenn die Fertigstellungsprozentsätze in der Meilensteinansicht nicht aktuell angezeigt werden, klicken Sie auf **Optionen** in der oberen rechten Ecke der Milestone-Ansicht, stellen Sie sicher, dass **Prozent abgeschlossen** aktiviert ist.

1. Klicken Sie auf den Fertigstellungsprozentsatz unterhalb einer Aufgabe, geben Sie einen neuen Prozentsatz an und drücken Sie die Eingabetaste.
