---
product-area: agile-and-teams
navigation-topic: work-in-an-agile-environment
title: Verwalten des agilen Rückprotokolls
description: Aufgaben und Probleme können einem agilen Team zugewiesen und dem Backlog dieses Teams je nach der vom Team verwendeten agilen Methode als Meldungen hinzugefügt werden.
author: Lisa
feature: Agile
exl-id: 59660840-7ab8-482e-8b43-96b4a1ecc538
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '1371'
ht-degree: 0%

---

# Verwalten des agilen Rückprotokolls

Die folgenden Arbeitselemente können einem agilen Team zugewiesen und diesem Team je nach der vom Team verwendeten agilen Methode als Meldungen hinzugefügt werden:

* **[!UICONTROL Trommelteams ]:** Aufgaben und Probleme können dem agilen Team zugewiesen und dem Rückstand hinzugefügt werden.
* **[!UICONTROL Kanban agile teams]:** Aufgaben können dem agilen Team zugewiesen und dem Rückstand hinzugefügt werden. Benutzer können den Rückstand direkt aus dem agilen Storyboard anzeigen, wie unter [[!UICONTROL Den Rückstand hinzufügen] zum Kanban-Forum hinzufügen](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md) beschrieben. Das Team verwendet diesen Rückstand, um seine Arbeitswarteschlange zu priorisieren und zu verwalten.

Aufgaben oder Probleme können dem Team zugewiesen (und anschließend dem Team-Backlog hinzugefügt) werden, und zwar von überall aus mit [!DNL Adobe Workfront]. Beispielsweise kann einem einzelnen Team Arbeitszuweisungen aus mehreren Projekten zugewiesen werden.

>[!NOTE]
>
>Wenn Sie einem Rückholelement mehrere Teams hinzufügen, wird die Aufgabe bzw. das Problem nur im Rückstand des Hauptteams angezeigt. Das Hauptteam ist das zuerst zugewiesene Team.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Lizenz</strong></td> 
   <td> <p>Neu: [!UICONTROL Standard]</p><p>Oder</p><p>Aktuell: [!UICONTROL Arbeit] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene</strong></td> 
   <td> <p>Neu: [!UICONTROL Standard]</p><p>Oder</p><p>Aktuell: [!UICONTROL Worker] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Verwalten] Zugriff auf das Projekt, auf dem sich die Story befindet</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen und Verwalten von Storys im Backlog

* [Erstellungsgeschichten](#reorder-stories)
* [[!UICONTROL  Aufschlüsseln von ] Meldungen](#break-down-stories)
* [Bearbeitungsgeschichten](#edit-stories)

### Erstellungsgeschichten {#reorder-stories}

Mit der Drag &amp; Drop-Methode können Sie die Reihenfolge der Meldungen in der Liste ändern.

1. Gehen Sie in den agilen Backlog, in dem Sie Meldungen neu anordnen möchten.
1. Wählen Sie im Dropdown-Menü **[!UICONTROL Ansicht]** die Ansicht **[!UICONTROL Rückprotokoll]** oder eine benutzerdefinierte Ansicht, die die Spalte **[!UICONTROL Bestellung]** enthält.

   >[!NOTE]
   >
   >Wenn einer Aufgabe oder einem Problem ein agiles Team zugewiesen wurde und das Projekt keinen Status aufweist, der mit Aktuell übereinstimmt, werden sie nicht im Rückstand angezeigt. Sie wirken sich jedoch weiterhin auf die Rückstandsanzahl in der Spalte Bestellung aus.

1. Wählen Sie einen oder mehrere Storys aus und ziehen Sie dann die Meldungen in die Reihenfolge, in der sie im Rückstand angezeigt werden sollen.\
   ![Ziehen Sie die Elemente im Rückstadium per Drag-and-Drop](assets/agile-backlog-drag-and-drop.png)

### Meldungen aufschlüsseln {#break-down-stories}

Da Geschichten in einem Rückstau unterschiedlich groß sind, können Benutzer sie für eine Iteration in funktionierende Größen unterteilen. Wenn Sie eine Meldung aufschlüsseln, werden Unteraufgaben für die Aufgabe erstellt, die die Meldung darstellt, und die ursprüngliche Aufgabe im Rückstand ersetzt. Sie können eine übergeordnete Aufgabe oder deren Unteraufgaben einem agilen Team zuweisen, aber Sie können nicht beide gleichzeitig einem Team zugewiesen haben.

>[!NOTE]
>
>Beachten Sie beim Aufschlüsseln von Meldungen die folgenden Einschränkungen:
>
>* Es können nur Meldungen aufgeschlüsselt werden, die Aufgaben darstellen. Sie können keine Meldungen aufschlüsseln, die Probleme darstellen.
>* Geschichten können nur aufgeschlüsselt werden, wenn sie mit einem Projekt verknüpft sind.


So unterteilen Sie eine Geschichte:

1. Gehen Sie in den Rückstand, der die Meldung enthält, die Sie aufschlüsseln möchten.
1. Wählen Sie die Geschichte aus, die Sie unterteilen möchten, und klicken Sie dann auf **[!UICONTROL Aufschlüsselungsmeldung]**.\
   Das Dialogfeld [!UICONTROL Aufschlüsselungsmeldung] wird angezeigt.\
   ![Dialogfeld &quot;Aufschlüsselungsmeldung&quot;](assets/backlog-breakdown-dialog.png)

1. Geben Sie einen Namen und eine Schätzung für die Geschichte ein und wählen Sie aus, ob die Geschichte fertig ist.
1. Klicken Sie auf **[!UICONTROL Geschichte hinzufügen]** , um eine weitere Geschichte aus der Originalgeschichte zu erstellen.
1. Klicken Sie auf **[!UICONTROL Speichern]**.

### Bearbeitungsgeschichten {#edit-stories}

Sie können Geschichten direkt über die Registerkarten [!UICONTROL Meldungen] oder [!UICONTROL Probleme] im Backlog bearbeiten, da Sie alle Aufgaben oder Probleme innerhalb eines Projekts stapelweise bearbeiten würden, wie unter [Aufgaben stapelweise bearbeiten](../../manage-work/tasks/manage-tasks/edit-tasks.md#edit-tasks-in-bulk) in [Aufgaben bearbeiten](../../manage-work/tasks/manage-tasks/edit-tasks.md) und [Probleme bearbeiten](../../manage-work/issues/manage-issues/edit-issues.md) beschrieben.

## Erstellen neuer Meldungen im Backlog {#create-new-stories-on-the-backlog}

Sie können neue Meldungen im Rückstand erstellen, indem Sie die Meldung direkt aus dem Rückstand erstellen oder einem agilen Team eine vorhandene Aufgabe oder ein Problem zuweisen.

* [Erstellen Sie eine Geschichte aus dem Rückstand.](#create-a-story-from-the-backlog)
* [Aufgabe oder Problem einem agilen Team zuweisen](#assign-a-task-or-issue-to-an-agile-team)

### Erstellen Sie eine Geschichte aus dem Rückstand. {#create-a-story-from-the-backlog}

Wenn Sie eine Geschichte aus dem Rückstand erstellen, wird die Geschichte als Aufgabe oder Problem innerhalb eines Projekts erstellt. Es ist nicht möglich, eine Meldung aus dem Rückstand als Problem zu erstellen.

So erstellen Sie eine Geschichte aus dem Rückstand:

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]**, das Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf **[!UICONTROL Teams]**.

1. (Optional) Klicken Sie auf das Symbol &quot;**[!UICONTROL Team wechseln]**&quot;![Team-Symbol wechseln](assets/switch-team-icon.png)&quot;. Wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team und wählen Sie es aus, wenn es angezeigt wird.

1. Wählen Sie im linken Bereich **[!UICONTROL Rückprotokoll]** aus.
1. Führen Sie je nachdem, ob Sie eine Aufgabe oder ein Problem erstellen möchten, einen der folgenden Schritte aus:

   * **So erstellen Sie eine Aufgabe:** Klicken Sie auf **[!UICONTROL Meldungen]**.

   * **Um ein Problem zu erstellen:** Klicken Sie auf **[!UICONTROL Probleme]**.

1. Klicken Sie auf **[!UICONTROL Neue Meldung]** oder **[!UICONTROL Neues Problem]**.

1. Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story Name]</strong></td>
      <td> Geben Sie einen Namen für die Geschichte ein.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Beschreibung]</strong></td>
      <td>(Optional) Geben Sie eine Beschreibung für den Artikel ein.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Bereit]</strong></td>
      <td> Wählen Sie aus, ob die Geschichte bereit ist, einer Iteration hinzugefügt zu werden. Diese Einstellung ist nur informativ. Meldungen können einer Iteration unabhängig vom Status dieser Einstellung hinzugefügt werden.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Schätzung]</strong></td>
      <td>Geben Sie einen Punkt oder eine stündliche Schätzung für die Geschichte an. Schätzwerte wirken sich auf das Diagramm aus. Die Abbruchgrafik für eine Iteration ist nur dann korrekt, wenn jede Geschichte eine genaue Schätzung enthält. (Wenn Sie eine Punktschätzung angeben, müssen Sie bereits in den Teameinstellungen festgelegt haben, wie viele Stunden jeder Punkt darstellt.)</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Übergeordnetes Projekt]</strong></td>
      <td>Beginnen Sie mit der Eingabe des Namens des Projekts, in dem diese Geschichte erstellt werden soll, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.<br>Der Status des Projekts muss auf [!UICONTROL Aktuell] festgelegt sein. Wenn der Projektstatus etwas Anderes als [!UICONTROL Aktuell] ist, wird er nicht im Dropdown-Menü angezeigt.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Übergeordnete Aufgabe von [!UICONTROL]</strong></td>
      <td>(Optional) Beginnen Sie mit der Eingabe des Namens der übergeordneten Aufgabe, der diese Meldung untergeordnet ist, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td> (Optional) Wählen Sie benutzerdefinierte Formulare aus, die Sie diesem Artikel hinzufügen möchten.</td>
     </tr>
    </tbody>
   </table>

1. Klicken Sie auf **[!UICONTROL Geschichte speichern]**.

### Aufgabe oder Problem einem agilen Team zuweisen {#assign-a-task-or-issue-to-an-agile-team}

Sie können eine Aufgabe oder ein Problem einem agilen Team zuweisen. Nachdem sie zugewiesen wurde, erscheint die Aufgabe oder das Problem als neue Meldung im Team-Backlog.

So weisen Sie einem agilen Team eine Aufgabe oder ein Problem zu:

1. Rufen Sie das Projekt auf, das die Aufgabe enthält, die Sie zuweisen möchten.
1. Wählen Sie die Aufgabe oder das Problem in der Liste aus.
1. Klicken Sie auf **[!UICONTROL Bearbeiten]**.
1. Klicken Sie auf **[!UICONTROL Zuweisungen]**.
1. (Optional) Löschen Sie alle vorhandenen Bevollmächtigten.
1. Klicken Sie auf **[!UICONTROL Zuweisung hinzufügen]**.
1. Beginnen Sie mit der Eingabe des Namens des agilen Teams, das Sie der Aufgabe oder dem Problem zuweisen möchten, und klicken Sie dann auf den Teamnamen, wenn er in der Dropdown-Liste angezeigt wird.
1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.\
   Die Aufgabe oder das Problem ist jetzt im Team-Backlog verfügbar.

## Verschieben von Meldungen in den oder aus dem Rückstand

{#move-stories-from-the-backlog-to-an-iteration-or-kanban-board}

* [Verschieben von Meldungen aus dem Rückstadium in eine Iteration oder + Pinnwand](#move-stories-from-the-backlog-to-an-iteration-or--board)
* [Verschieben vorhandener Meldungen in den Backlog](#move-existing-stories-to-the-backlog)
* [Exportieren von Meldungen aus dem Rückstand](#export-stories-from-the-backlog)

### Verschieben von Meldungen aus dem Rückstadium in eine Iteration oder + Pinnwand

1. Gehen Sie zum Rückstand des agile Teams.
1. Wählen Sie die Geschichten aus, die Sie in eine Iteration oder Kanban-Pinnwand verschieben möchten, und klicken Sie dann auf **[!UICONTROL Mehr]** > **[!UICONTROL Verschieben nach]**.\
   Wenn Sie die Geschichte auf eine [!UICONTROL Kanban]-Pinnwand verschieben, wird die Pinnwand [!UICONTROL Geschichte in die Kanban]-Pinnwand verschoben.\
   Wenn Sie die Geschichte in eine Iteration verschieben, wird das Dialogfeld [!UICONTROL Geschichte in eine Iteration verschieben] angezeigt.\
   ![Dialogfeld &quot;Geschichte verschieben&quot;](assets/agile-backlog-addtoiteration.png)

1. Führen Sie einen der folgenden Schritte aus:

   * **Für Scrum-Teams:** Wählen Sie im Feld **[!UICONTROL Iteration auswählen]** die Iteration aus, in die Sie die Geschichten verschieben möchten.

   * **Für Kanban-Teams:** Wählen Sie im Feld **[!UICONTROL Kanban-Mainboard auswählen]** Ihr Team [!UICONTROL Kanban]-Pinnwand aus. (Kanban-Teams können nur ein [!UICONTROL Kanban]-Board haben.)

1. Klicken Sie auf **[!UICONTROL Geschichte verschieben]**.

### Verschieben vorhandener Meldungen in den Backlog {#move-existing-stories-to-the-backlog}

Wenn Sie sich entscheiden, dass Ihr Team noch nicht bereit ist, an einer Geschichte zu arbeiten, können Sie die Geschichte in den Rückstand versetzen.

Weitere Informationen finden Sie unter [Verschieben einer agilen Meldung](../../agile/work-in-an-agile-environment/move-an-agile-story.md).

### Exportieren von Meldungen aus dem Rückstand {#export-stories-from-the-backlog}

Sie können einen oder mehrere Meldungen (einschließlich Aufgaben und Probleme) direkt aus dem Rückstand exportieren.

Sie exportieren Meldungen aus dem Rückstand auf dieselbe Weise wie andere Daten in [!DNL Workfront], wie in [Daten exportieren](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md) beschrieben.
