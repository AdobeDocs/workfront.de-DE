---
product-area: reporting
navigation-topic: reporting-elements
title: Erstellen oder Bearbeiten von Ansichten in Adobe Workfront
description: Sie können die Art der Informationen, die Sie auf dem Bildschirm anzeigen, mithilfe von Ansichten anpassen. Sie können in Adobe Workfront verschiedene Ansichtstypen verwenden.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '893'
ht-degree: 4%

---

# Erstellen oder Bearbeiten von Ansichten in Adobe Workfront

<!-- Audited: 11/2024 -->

Sie können die Art der Informationen, die Sie auf dem Bildschirm anzeigen, mithilfe von Ansichten anpassen. Sie können in Adobe Workfront verschiedene Ansichtstypen verwenden.

In diesem Artikel wird beschrieben, wie Sie Standardansichten für Listen und Berichte erstellen und bearbeiten.

Weitere Informationen finden Sie unter [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</strong></td> 
   <td> 
    <p>Mitwirkender oder höher</p>
    <p>Anfrage oder höher</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um eine Ansicht in einem Bericht zu erstellen</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten der Berechtigungen für einen Bericht zum Erstellen oder Bearbeiten einer Ansicht in einem Bericht</p> <p>Verwalten von Berechtigungen für eine Ansicht, um sie zu bearbeiten</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Erstellen oder Anpassen einer Ansicht

Der Prozess zum Erstellen oder Anpassen einer Ansicht unterscheidet sich, je nachdem, ob Sie eine Standardansicht oder eine Pinnwand-Ansicht erstellen oder anpassen.

### Erstellen oder Anpassen einer Standardansicht {#create-or-customize-a-standard-view}

Sie können eine neue Standardansicht erstellen oder eine vorhandene Standardansicht, die Sie zuvor erstellt haben, anpassen.

1. Klicken Sie auf **Dropdown** Menü „Ansicht“ in einer Liste, in der Sie eine Ansicht erstellen oder anpassen möchten.

1. Klicken Sie auf die Schaltfläche **+ Neue Ansicht**, um eine neue Ansicht zu erstellen.
oder
Klicken Sie auf **Bearbeiten**-Symbol ![Bearbeiten](assets/edit-icon.png), das beim Bewegen der Maus über rechts neben einer vorhandenen Ansicht angezeigt wird, die Sie bearbeiten möchten.
Das **Ansicht anpassen** wird angezeigt.

1. Führen Sie **Abschnitt** Spaltenvorschau“ einen der folgenden Schritte aus:

   * Ändern Sie den Wert einer beliebigen Spalte, indem Sie auf den Spaltentitel klicken und dann ein neues Feld auswählen.
   * Fügen Sie eine Spalte hinzu, indem Sie auf **Spalte hinzufügen** klicken, den Namen der Spalte eingeben, die Sie hinzufügen möchten, und dann auf sie klicken, wenn sie in der Dropdown-Liste angezeigt wird.
   * Passen Sie die Reihenfolge der Spalten an, indem Sie den Spaltentitel an eine neue Position ziehen.

   * Klicken Sie im Bereich **Spalteneinstellungen** auf **Diese Spalte zusammenfassen nach** und wählen Sie aus, wie die Daten in der Spalte angezeigt werden sollen. Diese Option ist für die folgenden Spaltentypen verfügbar:
     <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Datumsfelder</strong></td> 
           <td><ul>
           <li>Maximum</li>
         <li>Minimum</li>
           </ul></td> 
          </tr> 
          <tr>
           <td role="rowheader"><strong>Währungsfelder</strong></td> 
           <td><ul>
           <li>Count</li>
         <li>Sum</li>
           <li>Durchschnitt</li>
         <li>Maximum</li>
           <li>Minimum</li>
         </ul></td> 
          </tr> 
         <tr>
           <td role="rowheader"><strong>Zeichenfolgen- und boolesche Felder</strong></td> 
           <td><ul><li>Count</li></ul>
           <p>Hinweis: Workfront empfiehlt im Allgemeinen nicht, ein boolesches Feld nach Anzahl zusammenzufassen, da der Wert immer „true“/„false“ sein wird.</p></td> 
          </tr> 
         </tbody> 
        </table>

     >[!NOTE]
     >
     >Die folgenden Ausnahmen gelten für übergeordnete Objekte (z. B. übergeordnete Aufgaben), wenn Sie Werte für die folgenden Felder in Gruppierungen zusammenfassen:
     >   
     > * Alle Felder für Zahl und Währung außer Iststunden (z. B. geplante/Ist-Lohnkosten, geplante/Ist-Ausgaben-Kosten, geplante/Ist-Kosten, geplante Stunden) fassen die Werte nur für untergeordnete Aufgaben und eigenständige Aufgaben zusammen. Sie fassen die Werte für die übergeordneten Aufgaben oder die übergeordneten Aufgaben nicht zusammen.
     > * Tatsächliche Stunden fassen die Werte für die übergeordnete Hauptaufgabe und die eigenständigen Aufgaben zusammen. Sie fassen nicht die Zahlen für die übergeordneten Aufgaben oder die untergeordneten Aufgaben zusammen.
     > * Benutzerdefinierte Datenfelder für Zahlen- und Währungswerte fassen alle Aufgaben zusammen: Eltern, Kinder, Eltern von Eltern und eigenständige Aufgaben.
     >
     >Weitere Informationen zur Verwendung von Gruppierungen in einem Bericht finden Sie im Artikel [Gruppierungen - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * (Optional) Klicken Sie auf **Erweiterte Optionen**, um die folgenden Informationen für die Spalte anzugeben:

        <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Benutzerdefiniertes Spalten-Label</strong></td> 
           <td><p>Geben Sie eine benutzerdefinierte Beschriftung für die Spalte an. Diese Beschriftung ersetzt die Standardbeschriftung. Es wird empfohlen, nur UTF-8-Zeichen zu verwenden, um Kompatibilitätsprobleme zu vermeiden.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Feldformat</strong></td> 
           <td>Wählen Sie das Format aus, in dem die Werte für Felder in der Spalte angezeigt werden sollen.</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Diese Spalte im Dashboard anzeigen</strong></td> 
           <td><p>Wählen Sie diese Option aus, um diese Spalte auf einem Dashboard anzuzeigen, wenn der Bericht Seite an Seite mit einem anderen Bericht angezeigt wird. Wenn diese Option deaktiviert ist, wird diese Spalte nicht angezeigt, wenn der Bericht in einem Dashboard angezeigt wird, in dem Berichte nebeneinander angezeigt werden.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Spaltenregeln</strong></td> 
           <td><p>Klicken Sie auf <strong>+ Regel für diese Spalte hinzufügen</strong> um eine Regel für die Spalte zu definieren. Nachdem Sie eine Regel hinzugefügt haben, können Sie Feld- und Textstile dafür definieren, wie Felder, die dieser Regel entsprechen, angezeigt werden. Klicken Sie <strong>Regel hinzufügen</strong> nachdem Sie die Definition der Regel abgeschlossen haben.</p></td> 
          </tr> 
         </tbody> 
        </table>

        Weitere Informationen zur bedingten Formatierung von Ansichten in Berichten finden Sie im Artikel [Verwenden der bedingten Formatierung im Textmodus](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

1. (Bedingt) Wenn Sie auf **Erweiterte Optionen** geklickt haben, klicken Sie auf **Fertig**.

1. Klicken Sie **Ansicht speichern**, um eine neue Ansicht zu erstellen oder die aktuelle Ansicht durch Ihre Änderungen zu ersetzen.\
   ODER\
   Klicken Sie **Als neue Ansicht speichern**, um Ihre Änderungen als neue Ansicht zu speichern.

   >[!TIP]
   >
   >Die **Als neue Ansicht speichern** ist die einzige Option, die beim Anpassen einer integrierten Workfront-Ansicht verfügbar ist.

   Ihr Zugriff bestimmt, wie die Ansicht gespeichert wird. Wenn Sie die Ansicht ursprünglich erstellt haben, können Sie die Änderungen speichern. Andernfalls werden Sie aufgefordert, eine Version zu speichern. Beachten Sie, dass sich Änderungen an der Ansicht auf Benutzende auswirken, für die die Ansicht freigegeben wurde.

### Erstellen oder Anpassen einer Board-Ansicht {#create-or-customize-an-agile-view}

Sie können Projekte mit einer Agile-Methode mithilfe einer Board-Ansicht verwalten.

Pinnwand-Ansichten sind nur für Listen von Aufgaben und Problemen in einem Projekt verfügbar.

Sie sind vorkonfiguriert, Sie können jedoch bestimmte Einstellungen für sie ändern.

Weitere Informationen zu Agile- oder Board-Ansichten finden Sie im Artikel [Verwalten eines Agile-Projekts in der Board-Ansicht](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

<!-- Legacy Agile views were deprecated with 25.3. This is old: 

>[!NOTE]
>
>This procedure only applies to the legacy Agile view, not to the board view of a project.

To create or customize an Agile view:

1. Go to the list of tasks on a project.
1. Click the **Board** icon ![Board icon](assets/board-icon-for-agile-view.png), and then click **Use legacy agile** on the board view.

1. (Conditional) To customize an existing Agile view:

   1. Click the **View** drop-down menu, then select the Agile view you want to customize.  
      You cannot customize the default Agile view.
   
   1. Click the **View** drop-down menu again, then click **Customize View**.  
      ![Customize view](assets/view-agile-customize.png)

1. (Conditional) To create a new Agile view, click **New View**.  
   The **Customize Agile View** dialog box displays.  

1. In the **Customize Agile View** dialog box, specify a name for the Agile view.  
   We recommend that you include the word "Agile" in your view name, so users know this is an Agile view.  
   This name is displayed in the **View** drop-down menu when selecting a view.

1. Define the status columns to display on the story board in the Agile view. These are the task statuses that are defined by the Workfront administrator, as described in [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Only system statuses are available to use on the Agile story board. If a status is available only for an individual group you are a member of, the status is not available on the Agile story board. Furthermore, tasks that are in a status that is available only to a custom group are not visible when viewing the project in an Agile view.

   Users can move stories among these status columns on the Agile story board.  
   When defining status columns, you can do the following:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Reorder status columns:</strong> </td> 
      <td> Drag a status column to the order where you want it to appear.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Remove status columns:</strong> </td> 
      <td>Click the (x) icon on the column that you want to remove.<br>You cannot remove the "New" status unless a custom status has been added to the view and that custom status equates with "New."<br>For information about creating a custom status, see <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Add status columns:</strong> </td> 
      <td> <p>Click the <strong>Plus</strong> icon, then select the status you want to add.<br>All default system statuses are displayed, as well as any custom statuses that have been shared with you.<br>You can configure up to 10 statuses to display.</p></td> 
     </tr> 
    </tbody> 
   </table>

   *********   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       *************

1. In the **Associate Card Color to** area, select from the following options:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Story:</strong> </td> 
      <td>Any subtasks match the color of the parent task, so that the colors of all stories in any given swimlane are the same.<br>Colors are randomly assigned to tasks when they are created if the task does not have any subtasks or does not have a parent task.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Free Form:</strong> </td> 
      <td> All cards are displayed as blue by default until a user changes the color manually, as described in the article <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Categorize stories by color on the Scrum board</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Priority:</strong> </td> 
      <td> <p> Colors are associated with the story priority, as follows:</p> 
       <ul> 
        <li>High = Red</li> 
        <li>Medium = Yellow</li> 
        <li>Low = Green<br>If your Workfront administrator has configured custom priorities for your Workfront system, the highest priority is red, the second-highest is yellow, and the remaining are green.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Task Owner:</strong> </td> 
      <td> All stories with the same primary assignee are the same color.<br>The primary assignee is the user who was first assigned to the task. </td> 
     </tr> 
    </tbody> 
   </table>

1. In the **Additional Fields** area, click **Add Field**, then select the field you want to add to story cards. (These are the same fields you can add when creating customizing a view or creating columns for a report.)  
   Repeat this process to add up to three additional fields to the story cards.  
   When you add fields to story cards, fields are view-only and display only when the field is populated.

   By default, the following types of data is displayed on the story card:

   * Story name with a link directly to the task
   * The project name with a link directly to the project  
     This link is displayed only when using the Agile view on an iteration; it is not displayed when using an Agile view on a project.
   * The task description
   * Current commitment
   * View and edit the percent complete either by adjusting the percent complete itself or by adjusting the number of points or hours that are complete
   * Assigned Users

   You can display additional data (including custom data) on story cards. You might want to display additional fields on story cards for any number of reasons. For example, you might want to display the Customer ID if you are working on stories for multiple customers within the project, or you might want to display the Task Start Date.

1. Click **Save**.  
   Your access dictates how the view is saved. If you created the view originally, you can save the changes; otherwise, you are prompted to save a version. Keep in mind that changes you make to the view impact users with whom the view has been shared.

1. (Optional) Click the **List** icon to return to the list of tasks.

-->
