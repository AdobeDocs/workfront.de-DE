---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: Verwalten des Agile-Rückstands
description: Aufgaben und Probleme können einem agilen Team zugewiesen und dem Rückstand dieses Teams als Geschichten hinzugefügt werden, je nach der agilen Methodik, die das Team verwendet.
author: Jenny
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1334'
ht-degree: 0%

---

# Verwalten des agilen Rückstands

Die folgenden Arbeitselemente können einem agilen Team zugewiesen und dem Rückstand dieses Teams als Geschichten hinzugefügt werden, je nach der agilen Methodik, die das Team verwendet:

* **[!UICONTROL Scrum-Agile-]:** Aufgaben und Probleme können dem Agile-Team zugewiesen und dem Rückstand hinzugefügt werden.
* **[!UICONTROL Kanban-Agile]Teams:** Aufgaben können dem Agile-Team zugewiesen und dem Rückstand hinzugefügt werden. Benutzer können den Rückstand direkt vom Agile-Story-Board anzeigen, wie beschrieben in [[!UICONTROL Hinzufügen des Rückstands] zum Kanban-Board](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md). Das Team verwendet diesen Rückstand, um seine Arbeitswarteschlange zu priorisieren und zu verwalten.

Aufgaben oder Probleme können dem Team von überall in [!DNL Adobe Workfront] zugewiesen (und dann zum Team-Rückstand hinzugefügt) werden. Beispielsweise kann einem einzelnen Team Arbeitsaufträge aus mehreren Projekten zugewiesen werden.

>[!NOTE]
>
>Wenn Sie einem Rückstandselement mehrere Teams hinzufügen, wird die Aufgabe oder das Problem nur im Rückstand des primären Teams angezeigt. Das primäre Team ist das Team, das zuerst zugewiesen wurde.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p> 
   <p>Arbeit oder höher</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Zugriff auf das Projekt verwalten, an dem sich die Story befindet </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Storys im Rückstand erstellen und verwalten

* [Storys neu anordnen](#reorder-stories)
* [[!UICONTROL Geschichten &#x200B;].](#break-down-stories)
* [Storys bearbeiten](#edit-stories)

### Storys neu anordnen {#reorder-stories}

Mithilfe der Drag-and-Drop-Methode können Sie Storys in der Rückstandsliste neu anordnen.

1. Navigieren Sie zum agilen Auftragsbestand, in dem Sie Storys neu anordnen möchten.
1. Wählen Sie **[!UICONTROL Dropdown]** Menü „Ansicht“ die Ansicht **[!UICONTROL Rückstand]** oder eine benutzerdefinierte Ansicht aus, die die Spalte **[!UICONTROL Reihenfolge]** enthält.

   >[!NOTE]
   >
   >Wenn einer Aufgabe oder einem Problem ein agiles Team zugewiesen ist und das Projekt nicht den Status „Aktuell“ aufweist, werden sie bzw. es nicht im Rückstand angezeigt. Sie wirken sich jedoch weiterhin auf die Anzahl der Rückstände in der Spalte Bestellung aus.

1. Wählen Sie eine oder mehrere Storys aus und ziehen Sie die Storys in die Reihenfolge, in der sie im Auftragsbestand angezeigt werden sollen.
   ![Elemente im Auftragsbestand per Drag-and-Drop verschieben](assets/agile-backlog-drag-and-drop.png)

### Geschichten aufschlüsseln {#break-down-stories}

Da Storys in einem Rückstand unterschiedlich groß sind, können Benutzer sie für eine Iteration in praktikable Größen aufschlüsseln. Wenn Sie eine Story aufschlüsseln, werden Teilaufgaben für die Aufgabe erstellt, die die Story darstellt, und die ursprüngliche Aufgabe im Auftragsbestand wird ersetzt. Sie können eine übergeordnete Aufgabe oder deren Unteraufgaben einem agilen Team zuweisen lassen, aber Sie können nicht beide gleichzeitig einem Team zuweisen.

>[!NOTE]
>
>Beachten Sie beim Aufschlüsseln von Storys die folgenden Einschränkungen:
>
>* Nur Storys, die Aufgaben darstellen, können aufgeschlüsselt werden. Sie können keine Geschichten aufschlüsseln, die Probleme darstellen.
>* Storys können nur aufgeschlüsselt werden, wenn sie mit einem Projekt verknüpft sind.


So schlüsseln Sie eine Story auf:

1. Navigieren Sie zum Auftragsbestand, der die Story enthält, die Sie aufschlüsseln möchten.
1. Wählen Sie die Story aus, die Sie aufschlüsseln möchten, und klicken Sie dann auf **[!UICONTROL Story aufschlüsseln]**.
Das [!UICONTROL Story aufschlüsseln] wird angezeigt.
   ![Dialogfeld Story aufschlüsseln](assets/backlog-breakdown-dialog.png)

1. Geben Sie einen Namen und eine Schätzung für die Story an und wählen Sie aus, ob die Story bereit ist.
1. Klicken Sie **[!UICONTROL Story hinzufügen]**, um eine weitere Story aus der ursprünglichen Story zu erstellen.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

### Storys bearbeiten {#edit-stories}

Sie können Storys direkt über die Registerkarten [!UICONTROL Storys] oder [!UICONTROL Probleme] im Rückstand bearbeiten, wie Sie alle Aufgaben oder Probleme innerhalb eines Projekts stapelweise bearbeiten würden, wie [Aufgaben stapelweise bearbeiten](../../manage-work/tasks/manage-tasks/edit-tasks.md#edit-tasks-in-bulk) in [Aufgaben bearbeiten](../../manage-work/tasks/manage-tasks/edit-tasks.md) und [Probleme bearbeiten](../../manage-work/issues/manage-issues/edit-issues.md) beschrieben.

## Neue Storys im Auftragsbestand erstellen {#create-new-stories-on-the-backlog}

Sie können neue Storys im Rückstand erstellen, indem Sie die Story direkt aus dem Rückstand erstellen oder indem Sie eine vorhandene Aufgabe oder ein vorhandenes Problem einem agilen Team zuweisen.

* [Story aus dem Auftragsbestand erstellen](#create-a-story-from-the-backlog)
* [Aufgabe oder Problem einem agilen Team zuweisen](#assign-a-task-or-issue-to-an-agile-team)

### Story aus dem Auftragsbestand erstellen {#create-a-story-from-the-backlog}

Wenn Sie eine Story aus dem Rückstand erstellen, wird die Story als Aufgabe oder Problem in einem Projekt erstellt.

So erstellen Sie eine Story aus dem Auftragsbestand:

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **[!UICONTROL Teams]**.

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Symbol Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Scrum-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team und wählen Sie es aus, wenn es angezeigt wird.

1. Wählen **[!UICONTROL Auftragsbestand]** im linken Bedienfeld aus.
1. Führen Sie einen der folgenden Schritte aus, je nachdem, ob Sie eine Aufgabe oder ein Problem erstellen möchten:

   * **So erstellen Sie eine Aufgabe** Klicken Sie auf **[!UICONTROL Storys]**.

   * **So erstellen Sie ein Problem:** Klicken Sie auf **[!UICONTROL Probleme]**.

1. Klicken Sie auf **[!UICONTROL Neue Story]** oder **[!UICONTROL Neues Problem]**.

1. Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story-Name]</strong></td>
      <td> Geben Sie einen Namen für die Story ein.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Beschreibung]</strong></td>
      <td>(Optional) Geben Sie eine Beschreibung für die Story ein.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL bereit]</strong></td>
      <td> Wählen Sie aus, ob die Story bereit zum Hinzufügen zu einer Iteration ist. Diese Einstellung dient nur zu Informationszwecken. Storys können einer Iteration unabhängig vom Status dieser Einstellung hinzugefügt werden.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Schätzung]</strong></td>
      <td>Geben Sie einen Punkt oder eine stündliche Schätzung für die Story an. Schätzungen wirken sich auf das Burndown-Diagramm aus. Das Burndown-Diagramm für eine Iteration ist nur dann korrekt, wenn jede Story eine genaue Schätzung enthält. (Wenn Sie eine Punktschätzung angeben, müssen Sie bereits in den Team-Einstellungen festgelegt haben, wie viele Stunden jeder Punkt repräsentiert.)</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Übergeordnetes Projekt]</strong></td>
      <td>Geben Sie den Namen des Projekts ein, in dem die Story erstellt werden soll, und klicken Sie auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.<br>Der Status des Projekts muss auf [!UICONTROL Current] gesetzt werden. Wenn der Status des Projekts alles andere als [!UICONTROL Current] ist, wird er nicht im Dropdown-Menü angezeigt.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Übergeordnete Aufgabe]</strong></td>
      <td>(Optional) Geben Sie den Namen der übergeordneten Aufgabe ein, der diese Story untergeordnet ist, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td> (Optional) Wählen Sie alle benutzerdefinierten Formulare aus, die Sie dieser Story hinzufügen möchten.</td>
     </tr>
    </tbody>
   </table>

1. Klicken Sie **[!UICONTROL Story speichern]**.

### Aufgabe oder Problem einem agilen Team zuweisen {#assign-a-task-or-issue-to-an-agile-team}

Sie können einem agilen Team eine Aufgabe oder ein Problem zuweisen. Nachdem sie zugewiesen wurde, wird die Aufgabe oder das Problem als neue Story im Team-Rückstand angezeigt.

So weisen Sie einem agilen Team eine Aufgabe oder ein Problem zu:

1. Wechseln Sie zu dem Projekt, das die Aufgabe enthält, die Sie zuweisen möchten.
1. Aufgabe oder Problem in der Liste auswählen.
1. Klicken Sie auf **[!UICONTROL Bearbeiten]**.
1. Klicken Sie **[!UICONTROL Arbeitsaufträge]**.
1. (Optional) Löschen Sie alle vorhandenen Zugewiesenen.
1. Klicken Sie **[!UICONTROL Verantwortlichen hinzufügen]**.
1. Geben Sie den Namen des agilen Teams ein, das der Aufgabe oder dem Problem zugewiesen werden soll, und klicken Sie dann auf den Team-Namen, wenn er in der Dropdown-Liste angezeigt wird.
1. Klicken Sie **[!UICONTROL Änderungen speichern]**.
Die Aufgabe oder das Problem ist jetzt im Team-Rückstand verfügbar.

## Storys in den oder aus dem Auftragsbestand verschieben

* [Storys aus dem Rückstand in eine Iteration oder Pinnwand verschieben](#move-stories-from-the-backlog-to-an-iteration-or--board)
* [Vorhandene Storys in den Auftragsbestand verschieben](#move-existing-stories-to-the-backlog)
* [Stories aus dem Auftragsbestand exportieren](#export-stories-from-the-backlog)

### Storys aus dem Rückstand in eine Iteration oder Pinnwand verschieben

1. Rufen Sie den Rückstand des agilen Teams auf.
1. Wählen Sie die Storys aus, die Sie in eine Iteration oder ein Kanban-Board verschieben möchten, und klicken Sie dann auf **[!UICONTROL Mehr]** > **[!UICONTROL Verschieben nach]**.
Wenn Sie die Story auf ein Kanban[!UICONTROL Board verschieben] wird das [!UICONTROL Story in das Kanban]Board verschieben angezeigt.
Wenn Sie die Story in eine Iteration verschieben[!UICONTROL &#x200B; wird das Dialogfeld „Story in eine Iteration &#x200B;]&quot; angezeigt.
   ![Dialogfeld „Story verschieben“](assets/agile-backlog-addtoiteration.png)

1. Führen Sie einen der folgenden Schritte aus:

   * **Für Scrum-Teams:** Wählen Sie im Feld **[!UICONTROL Wiederholung auswählen]** die Iteration aus, in die Sie die Storys verschieben möchten.

   * **Für Kanban-Teams:** Wählen Sie im Feld **[!UICONTROL Kanban-]** auswählen Ihr Team [!UICONTROL Kanban]Board aus. (Kanban-Teams können nur ein [!UICONTROL Kanban]-Board haben.)

1. Klicken Sie **[!UICONTROL Story verschieben]**.

### Vorhandene Storys in den Auftragsbestand verschieben {#move-existing-stories-to-the-backlog}

Wenn Sie entscheiden, dass Ihr Team noch nicht bereit ist, an einer Story zu arbeiten, können Sie die Story in den Rückstand verschieben.

Weitere Informationen finden Sie unter [Verschieben einer agilen Story](../../agile/work-in-an-agile-environment/move-an-agile-story.md).

### Stories aus dem Auftragsbestand exportieren {#export-stories-from-the-backlog}

Sie können eine oder mehrere Storys (einschließlich Aufgaben und Problemen) direkt aus dem Rückstand exportieren.

Der Export von Storys aus dem Auftragsbestand erfolgt auf die gleiche Weise wie der Export anderer Daten in [!DNL Workfront], wie unter [Exportieren von Daten](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md) beschrieben.
