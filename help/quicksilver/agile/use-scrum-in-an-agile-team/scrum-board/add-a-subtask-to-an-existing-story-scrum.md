---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Hinzufügen einer Unteraufgabe zu einer vorhandenen Story auf dem Scrum-Board
description: Beachten Sie beim Erstellen von Unteraufgaben für vorhandene Storys die Einstellung Fertigstellungsmodus für das Projekt, da dies beeinflusst, wie Storys aktualisiert werden.
author: Lisa
feature: Agile
exl-id: 264e66e9-94c7-4904-baad-f733d39b4791
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# Hinzufügen einer Unteraufgabe zu einer vorhandenen Story auf dem [!UICONTROL Scrum]-Board

Beachten Sie beim Erstellen von Unteraufgaben für vorhandene Storys Folgendes:

**Wenn die Einstellung [!UICONTROL Fertigstellungsmodus] für das Projekt auf &quot;[!UICONTROL Manuell]:**

* Wenn Sie eine übergeordnete Story mit Teilaufgaben nach [!UICONTROL Abgeschlossen] verschieben, wird die übergeordnete Story auf 100 % und der [!UICONTROL Status] auf [!UICONTROL Abgeschlossen] aktualisiert. Teilaufgaben werden nicht aktualisiert.
* Um den [!UICONTROL Prozent abgeschlossen] für die Story zu aktualisieren, müssen Sie ihn über die Registerkarte [!UICONTROL Storys] oder über die Seite [!UICONTROL Details] des Objekts aktualisieren.

**Wenn die Einstellung [!UICONTROL Fertigstellungsmodus] für das Projekt auf &quot;[!UICONTROL &quot;]**:

* Wenn Sie eine übergeordnete Story mit Teilaufgaben nach [!UICONTROL Abgeschlossen] verschieben, wird die übergeordnete Story auf 100 % und der [!UICONTROL Status] auf [!UICONTROL Abgeschlossen] aktualisiert. Teilaufgaben werden ebenfalls auf 100 % aktualisiert und der [!UICONTROL Status] wird auf [!UICONTROL Abgeschlossen] aktualisiert.
* Um den [!UICONTROL Prozent abgeschlossen] für die Story zu aktualisieren, müssen Sie den [!UICONTROL Prozent abgeschlossen] für alle Teilaufgaben aktualisieren. Der [!UICONTROL Prozent abgeschlossen] für die Story wird anhand des [!UICONTROL Prozent abgeschlossen] aller Teilaufgaben berechnet.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p> 
   oder
   <p>Aktuell: [!UICONTROL Work] oder höher</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Zugriff von [!UICONTROL Contribute] oder [!UICONTROL Manage] auf die Aufgabe, für die die Unteraufgabe ausgeführt wird </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hinzufügen einer Unteraufgabe zu einer vorhandenen Story auf dem Scrum-Board

{{step1-to-team}}

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Symbol Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Scrum-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Gehen Sie zur agilen Iteration oder zum Projekt, das die Story enthält, der/dem Sie eine Unteraufgabe hinzufügen möchten. Weitere Informationen zum Navigieren zu einer Iteration finden Sie unter [Anzeigen einer Iteration](../../../agile/use-scrum-in-an-agile-team/iterations/view-iteration.md).
1. Wechseln Sie zur Story-Kachel auf dem Story Board, dem Sie eine Unteraufgabe hinzufügen möchten.
1. Klicken Sie **[!UICONTROL Unteraufgabe hinzufügen]** auf der Karte für die Hauptgeschichte an, um eine Unteraufgabe für die Geschichte zu erstellen.

   ![Teilaufgabe hinzufügen](assets/agile-story-addsubtask-NWE.png)

   Oder

   Klicken Sie **[!UICONTROL Unteraufgabe hinzufügen]** auf einer Unteraufgabenkachel, um eine Unteraufgabe zur Unteraufgabe zu erstellen.

   [!DNL Workfront] unterstützt unendliche Ebenen von Unteraufgaben, aber nur zwei Ebenen (Unteraufgaben von Unteraufgaben) werden im Agile-Story-Board angezeigt.

   ![Teilaufgabe hinzufügen](assets/agile-story-addsubtask2-NWE.png)

   Beim Hinzufügen einer Unteraufgabe zu einer Story, die derzeit keine Anzeigespur hat, wird die übergeordnete Aufgabe in die Spalte [!UICONTROL Übergeordnete Story“ ] und die Unteraufgabe wird in die Anzeigespur verschoben.

1. Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Name Teilaufgabe]</strong></td>
      <td> Geben Sie einen Namen für die Teilaufgabe an.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Beschreibung]</strong></td>
      <td>Geben Sie eine Beschreibung für die Teilaufgabe an.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Schätzung]</strong></td>
      <td>Geben Sie den Voranschlag für die Teilaufgabe an.<br><p>Beachten Sie beim Erstellen von Schätzungen Folgendes:</p>
       <ul>
        <li>Wenn Ihr agiles Team so konfiguriert ist, dass Geschichten in Punkten geschätzt werden, entspricht standardmäßig 1 Punkt 8 Stunden. Die Schätzungen werden als [!UICONTROL Geplante Stunden] zur Story hinzugefügt.</li>
        <li>Die kombinierten Schätzungen für alle Teilaufgaben bestimmen die Schätzung der übergeordneten Story. Weitere Informationen finden Sie unter <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/update-status-of-stories-and-subtasks.md" class="MCXref xref">Aktualisieren des Status von Storys und Teilaufgaben auf dem Scrum-Board</a>.</li>
        <li>Wenn Sie eine neue Teilaufgabe erstellen, ist das Feld [!UICONTROL Schätzung] bereits festgelegt. Wenn Sie die Schätzung für die Teilaufgabe zurücksetzen, wird die Schätzung für die übergeordnete Story zurückgesetzt (da die übergeordnete Story die Summe aller ihrer Teilaufgaben ist).</li>
       </ul><br></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Geplante Stunden]</strong></td>
      <td> (Nur in Projekten verfügbar) Geben Sie die Anzahl der geplanten Stunden für die Aufgabe an.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL-Zuweisung]</strong></td>
      <td>Geben Sie den Namen des Teams ein, dem Sie die Unteraufgabe zuweisen möchten, und klicken Sie dann auf den Namen, wenn er in der Dropdown-Liste angezeigt wird.</td>
     </tr>
    </tbody>
   </table>

1. Klicken Sie auf **[!UICONTROL Erstellen]**.
