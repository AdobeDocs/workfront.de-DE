---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Hinzufügen einer Unteraufgabe zu einem vorhandenen Artikel auf der Scrum-Pinnwand
description: Beachten Sie beim Erstellen von Unteraufgaben für vorhandene Meldungen die Einstellung "Abschlussmodus"für das Projekt, da sich dies auf die Aktualisierung von Meldungen auswirkt.
author: Lisa
feature: Agile
exl-id: 264e66e9-94c7-4904-baad-f733d39b4791
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '656'
ht-degree: 0%

---

# Hinzufügen einer Unteraufgabe zu einem vorhandenen Artikel auf der [!UICONTROL Scrum] Pinnwand

Beachten Sie beim Erstellen von Unteraufgaben für bestehende Meldungen Folgendes:

**Wenn die [!UICONTROL Abschlussmodus] -Einstellung für das Projekt auf [!UICONTROL Manuell]:**

* Verschieben einer übergeordneten Geschichte mit Unteraufgaben in [!UICONTROL Fertig] aktualisiert die übergeordnete Meldung auf 100 % und die [!UICONTROL Status] nach [!UICONTROL Fertig]. Unteraufgaben werden nicht aktualisiert.
* So aktualisieren Sie die [!UICONTROL Prozent abgeschlossen] für die Geschichte müssen Sie sie über die [!UICONTROL Meldungen] oder aus dem [!UICONTROL Details] -Seite des -Objekts.

**Wenn die [!UICONTROL Abschlussmodus] -Einstellung für das Projekt auf [!UICONTROL Automatisch]**:

* Verschieben einer übergeordneten Geschichte mit Unteraufgaben in [!UICONTROL Fertig] aktualisiert die übergeordnete Meldung auf 100 % und die [!UICONTROL Status] nach [!UICONTROL Fertig]. Unteraufgaben werden auch auf 100 % aktualisiert und die [!UICONTROL Status] aktualisiert auf [!UICONTROL Fertig].
* So aktualisieren Sie die [!UICONTROL Prozent abgeschlossen] für die Geschichte müssen Sie die [!UICONTROL Prozent abgeschlossen] für alle Unteraufgaben. Die [!UICONTROL Prozent abgeschlossen] für die Erzählung anhand der [!UICONTROL Prozent abgeschlossen] aller Unteraufgaben.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Arbeit] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL Worker] oder höher</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Contribute] oder [!UICONTROL Verwalten] Zugriff auf die Aufgabe, in der sich die Unteraufgabe befindet</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Hinzufügen einer Unteraufgabe zu einem vorhandenen Artikel auf der Scrum-Pinnwand

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Teams]**.

1. (Optional) Klicken Sie auf die **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wechseln Sie zur agilen Iteration oder zum Projekt, die bzw. das die Geschichte enthält, der Sie eine Unteraufgabe hinzufügen möchten. Informationen zum Navigieren zu einer Iteration finden Sie unter [Iteration anzeigen](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md).
1. Gehen Sie in den Bereich &quot;Geschichte&quot;des Forums, in dem Sie eine Unteraufgabe hinzufügen möchten.
1. Klicken **[!UICONTROL Unteraufgabe hinzufügen]** auf der Hauptstory-Karte, um eine Unteraufgabe für die Geschichte zu erstellen.

   ![Unteraufgabe hinzufügen](assets/agile-story-addsubtask-NWE.png)

   Oder

   Klicken **[!UICONTROL Unteraufgabe hinzufügen]** in einer Unteraufgaben-Kachel, um eine Unteraufgabe für die Unteraufgabe zu erstellen.

   [!DNL Workfront] unterstützt unendliche Ebenen von Unteraufgaben, aber nur zwei Ebenen (Unteraufgaben von Unteraufgaben) werden auf dem agilen Storyboard angezeigt.

   ![Unteraufgabe hinzufügen](assets/agile-story-addsubtask2-NWE.png)

   Beim Hinzufügen einer Unteraufgabe zu einer Geschichte, die derzeit keine Swimlane hat, wird die übergeordnete Aufgabe in die [!UICONTROL Übergeordnete Meldung] und die Unteraufgabe sich in der Swimlane bewegt.

1. Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Subtask Name]</strong></td>
      <td> Geben Sie einen Namen für die Unteraufgabe an.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Beschreibung]</strong></td>
      <td>Geben Sie eine Beschreibung für die Unteraufgabe an.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Schätzung]</strong></td>
      <td>Geben Sie die Schätzung für die Unteraufgabe an.<br><p>Beachten Sie bei der Erstellung von Schätzungen Folgendes:</p>
       <ul>
        <li>Wenn Ihr agile Team so konfiguriert ist, dass Geschichten in Punkten geschätzt werden, entspricht standardmäßig 1 Punkt 8 Stunden. Schätzungen werden in der Story als [!UICONTROL Planed Hours] hinzugefügt.</li>
        <li>Die kombinierten Schätzungen für alle Unteraufgaben bestimmen die Schätzung der übergeordneten Meldung. Weitere Informationen finden Sie unter <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref">Status von Meldungen und Unteraufgaben auf der Scrum-Pinnwand aktualisieren</a>.</li>
        <li>Wenn Sie eine neue Unteraufgabe erstellen, ist das Feld [!UICONTROL Schätzung] bereits festgelegt. Wenn Sie die Schätzung für die Unteraufgabe zurücksetzen, setzen Sie die Schätzung für die übergeordnete Meldung zurück (da die übergeordnete Meldung die Summe aller Unteraufgaben ist).</li>
       </ul><br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Geplante Stunden]</strong></td>
      <td> (Nur in Projekten verfügbar) Geben Sie die Anzahl der geplanten Stunden für die Aufgabe an.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Zuweisung]</strong></td>
      <td>Geben Sie den Namen des Teams ein, dem Sie die Unteraufgabe zuweisen möchten, und klicken Sie dann auf die Unteraufgabe, wenn sie in der Dropdown-Liste angezeigt wird.</td>
     </tr>
    </tbody>
   </table>

1. Klicken Sie auf **[!UICONTROL Erstellen]**.
