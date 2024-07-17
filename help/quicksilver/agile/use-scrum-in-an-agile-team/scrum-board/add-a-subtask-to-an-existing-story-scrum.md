---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Hinzufügen einer Unteraufgabe zu einem vorhandenen Artikel auf der Trommelplatine
description: Beachten Sie beim Erstellen von Unteraufgaben für vorhandene Meldungen die Einstellung "Abschlussmodus"für das Projekt, da sich dies auf die Aktualisierung von Meldungen auswirkt.
author: Lisa
feature: Agile
exl-id: 264e66e9-94c7-4904-baad-f733d39b4791
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 0%

---

# Hinzufügen einer Unteraufgabe zu einem vorhandenen Artikel auf der Pinnwand [!UICONTROL Scrum]

Beachten Sie beim Erstellen von Unteraufgaben für bestehende Meldungen Folgendes:

**Wenn die Einstellung [!UICONTROL Abschlussmodus] für das Projekt auf [!UICONTROL Manuell] festgelegt ist:**

* Wenn Sie eine übergeordnete Meldung mit Unteraufgaben auf [!UICONTROL Fertig stellen] verschieben, wird die übergeordnete Meldung auf 100 % und der [!UICONTROL Status] auf [!UICONTROL Fertig stellen] aktualisiert. Unteraufgaben werden nicht aktualisiert.
* Um den [!UICONTROL Percent Complete] für die Meldung zu aktualisieren, müssen Sie ihn auf der Registerkarte [!UICONTROL Meldungen] oder auf der Seite [!UICONTROL Details] des Objekts aktualisieren.

**Wenn die Einstellung [!UICONTROL Abschlussmodus] für das Projekt auf [!UICONTROL Automatisch]** festgelegt ist:

* Wenn Sie eine übergeordnete Meldung mit Unteraufgaben auf [!UICONTROL Fertig stellen] verschieben, wird die übergeordnete Meldung auf 100 % und der [!UICONTROL Status] auf [!UICONTROL Fertig stellen] aktualisiert. Unteraufgaben werden auch auf 100 % aktualisiert und der [!UICONTROL Status] wird auf [!UICONTROL Abgeschlossen] aktualisiert.
* Um den [!UICONTROL Percent Complete] für die Meldung zu aktualisieren, müssen Sie den [!UICONTROL Percent Complete] für alle Unteraufgaben aktualisieren. Die [!UICONTROL Prozent abgeschlossen] für die Meldung wird basierend auf der [!UICONTROL Prozent abgeschlossen] aller Unteraufgaben berechnet.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Arbeit] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL Worker] oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Contribute] oder [!UICONTROL] Zugriff auf die Aufgabe verwalten, in der sich die Unteraufgabe befindet</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Hinzufügen einer Unteraufgabe zu einem vorhandenen Artikel auf der Trommelplatine

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Teams]**.![](assets/main-menu-icon.png)

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wechseln Sie zur agilen Iteration oder zum Projekt, die bzw. das die Geschichte enthält, der Sie eine Unteraufgabe hinzufügen möchten. Informationen zum Navigieren zu einer Iteration finden Sie unter [Iteration anzeigen](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md).
1. Gehen Sie in den Bereich &quot;Geschichte&quot;des Forums, in dem Sie eine Unteraufgabe hinzufügen möchten.
1. Klicken Sie auf der Hauptstory-Karte auf **[!UICONTROL Unteraufgabe hinzufügen]** , um eine Unteraufgabe für die Meldung zu erstellen.

   ![Unteraufgabe hinzufügen](assets/agile-story-addsubtask-NWE.png)

   Oder

   Klicken Sie in einer Unteraufgabenkachel auf **[!UICONTROL Unteraufgabe hinzufügen]** , um eine Unteraufgabe für die Unteraufgabe zu erstellen.

   [!DNL Workfront] unterstützt unendliche Ebenen von Unteraufgaben, aber nur zwei Ebenen (Unteraufgaben von Unteraufgaben) werden auf der agilen Story-Pinnwand angezeigt.

   ![Unteraufgabe hinzufügen](assets/agile-story-addsubtask2-NWE.png)

   Beim Hinzufügen einer Unteraufgabe zu einer Geschichte, die derzeit keine Swimlane hat, wird die übergeordnete Aufgabe in die Spalte [!UICONTROL Übergeordnete Meldung] umgewandelt und die Unteraufgabe wird in die Swimlane verschoben.

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
        <li>Die kombinierten Schätzungen für alle Unteraufgaben bestimmen die Schätzung der übergeordneten Meldung. Weitere Informationen finden Sie unter <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref">Status von Meldungen und Unteraufgaben auf der Trommelplatine aktualisieren</a>.</li>
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
