---
product-area: agile-and-teams;setup
navigation-topic: get-started-with-agile-in-workfront
title: Kanban konfigurieren
description: Sie können die folgenden Optionen für agile Kanban-Teams während oder nach der Erstellung des Teams konfigurieren.
author: Lisa
feature: Agile
exl-id: b4c417a6-64c8-43e0-bace-b73572247b3e
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '1484'
ht-degree: 1%

---

# Konfigurieren von [!UICONTROL Kanban]

<!--Audited: 12/2023-->

Sie können ein agiles Team in [!DNL Adobe Workfront] erstellen, wie beschrieben in [Erstellen eines agilen Teams](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md). Beim Erstellen eines agilen Teams können Sie die Methode auswählen, die das Team verwendet, um seine Arbeit abzuschließen. Sie können aus den folgenden Optionen wählen:

* Scrum
* Kanban

In diesem Artikel wird beschrieben, wie Sie die Einstellungen für ein Kanban-Team konfigurieren. Nachdem Sie ein agiles Team erstellt und die Kanban-Methode ausgewählt haben, können Sie diesen Artikel lesen, um die folgenden Einstellungen zu aktualisieren:

* Ob Geschichten in Punkten oder Stunden geschätzt werden
* Die Statusspalten im Agile-Story-Board
* Zusätzliche Felder zur Anzeige auf Story-Karten im Agile-Story-Board
* Das Limit für laufende Arbeiten (Work In Progress, WIP)
* Automatisches Hinzufügen von Storys aus dem Rückstand
* Wie lange Karten auf dem Kanban-Board bleiben

Informationen zum Konfigurieren eines Scrum-Teams finden Sie unter [Konfigurieren von Scrum](../get-started-with-agile-in-workfront/configure-scrum.md).

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
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Teams bearbeiten</p>  </td> 
  </tr>

</tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurieren, ob Storys in Punkten oder Stunden geschätzt werden

Sie können Storys so konfigurieren, dass sie entweder anhand von Punkten oder Stunden geschätzt werden.

So konfigurieren Sie, wie Storys für Ihr agiles Team geschätzt werden:

{{step1-to-team}}

1. Klicken Sie auf **[!UICONTROL Symbol]** Teams wechseln![](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie im Suchfeld nach einem Team.
1. Wählen Sie das Agile-Team aus, das Sie verwalten möchten.
1. Klicken Sie auf das **[!UICONTROL Mehr]**-![](assets/more-menu.png) und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.

   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Wählen Sie im Abschnitt **[!UICONTROL Agile]** im Bereich **[!UICONTROL Geschichten schätzen in]** aus, ob Sie Punkte oder Stunden für die Schätzung der Größe (Arbeitslast) von Geschichten verwenden möchten. Wenn Sie Punkte wählen, geben Sie an, wie viele Stunden 1 Punkt entsprechen. (Der Standardwert ist 1 Punkt = 8 Stunden.) Dies ist die Anzahl der geplanten Stunden, die der Story hinzugefügt werden.

   **Beispiel** Wenn Sie ausgewählt haben, dass Geschichten in Punkten geschätzt werden sollen, und 1 Punkt 8 Stunden entspricht und ein Geschoss auf 3 Punkte geschätzt wird, werden dem Geschoss 24 geplante Stunden hinzugefügt.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.

## Konfigurieren von Statusspalten im Agile-Story-Board

Sie können die Status definieren, die im Story Board für das Agile-Team vorhanden sind. Dies sind die einzigen Status, die auf dem Storyboard angezeigt werden.

So definieren Sie die Status, die für das mit dem Agile-Team verknüpfte Story Board verfügbar sind:

{{step1-to-team}}

1. Klicken Sie auf **[!UICONTROL Team wechseln]**-Symbol ![Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das Agile-Team aus, das Sie verwalten möchten.
1. Klicken Sie auf das **[!UICONTROL Mehr]**-Menü und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.

   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Suchen Sie im Abschnitt **[!UICONTROL Agile]** den Bereich **[!UICONTROL Story Board]** .

1. (Optional) Klicken Sie auf **[!UICONTROL Spalte hinzufügen]**, um dem Storyboard eine zusätzliche Statusspalte hinzuzufügen.
1. (Optional) Ziehen Sie eine beliebige Statusspalte mit der Drag-and-Drop-Anzeige, um die Statusspalten auf dem Storyboard neu anzuordnen. Die erste Spalte kann nicht verschoben werden und Sie können keine weitere Spalte vor die erste Spalte ziehen.

   ![Drag-and-Drop](assets/agile-story-card-drag-and-drop.png)

1. Aufgabenstatus auswählen.

   >[!IMPORTANT]
   >
   >Es stehen nur gesperrte systemweite Status zur Auswahl. Gruppenspezifische Status können nicht ausgewählt werden. Der Status der ersten Spalte entspricht immer **[!UICONTROL Neu]**.

   Sie können benutzerdefinierte Status hinzufügen, wenn sie von Ihrem [!DNL Workfront] konfiguriert wurden. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten eines Status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.

## Konfigurieren Sie zusätzliche Felder, die auf Story-Karten im Agile-Story-Board angezeigt werden sollen

Wenn Sie Felder zu Story-Karten hinzufügen, sind die Felder schreibgeschützt und werden nur angezeigt, wenn das Feld ausgefüllt ist.

Standardmäßig werden die folgenden Datentypen auf der Story-Karte für Aufgaben und Probleme angezeigt:

* Name der Story mit direktem Link zur Aufgabe oder zum Problem
* Der Projektname mit einem Link direkt zum Projekt
* Dieser Link wird nur für Storys angezeigt, nicht für Teilaufgaben
* Die Aufgaben- oder Problembeschreibung
* Laufende Mittelbindung
* Sie können den abgeschlossenen Prozentsatz anzeigen und bearbeiten, indem Sie entweder den abgeschlossenen Prozentsatz selbst oder die Anzahl der abgeschlossenen Punkte oder Stunden anpassen
* Zugewiesene Benutzer

Sie können zusätzliche Daten (einschließlich benutzerdefinierter Daten) auf Story-Karten anzeigen. Möglicherweise möchten Sie aus verschiedenen Gründen zusätzliche Felder auf Story-Karten anzeigen. Beispielsweise können Sie die Kunden-ID anzeigen, wenn Sie an Storys für mehrere Kunden innerhalb der Iteration arbeiten, oder Sie möchten das Projektstartdatum oder das Projektabschlussdatum anzeigen.

>[!NOTE]
>
>Wenn Sie ein benutzerdefiniertes Feld auf einer Story-Karte verwenden, darf es keinen Punkt (oder Punkt) im Namen enthalten.

So konfigurieren Sie Story-Karten, die dem agilen Team zugewiesen sind, um zusätzliche Felder anzuzeigen:

{{step1-to-team}}

1. Klicken Sie auf **[!UICONTROL Team wechseln]**-Symbol ![Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das Agile-Team aus, das Sie verwalten möchten.
1. Klicken Sie auf das **[!UICONTROL Mehr]**-Menü und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.

   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Geben Sie im Abschnitt **[!UICONTROL Agile]** einen Feldnamen ein, um es zu finden.

   ![Zusätzliche Felder](assets/agile-additional-fields-kanban.png)

1. Wählen Sie den Namen des Felds aus, das Sie hinzufügen möchten.
1. Geben Sie den **[!UICONTROL Anzeigenamen]** für das Feld ein, das auf der Story- oder Problemkarte angezeigt werden soll.
1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.

## Konfigurieren Sie das Work In Progress (WIP)-Limit.

Wenn Sie die Fertigungsgrenze eines Kanban-Teams definieren, können Sie die Anzahl der Elemente steuern, an denen das Team derzeit arbeitet, indem Sie die Anzahl der Aufgaben begrenzen, die in der Spalte [!UICONTROL Neu] oder [!UICONTROL In Bearbeitung] auf der [!UICONTROL Kanban]-Pinnwand angezeigt werden können.

Nachdem Sie die WIP-Beschränkung für ein Kanban-Team konfiguriert haben, können Sie die WIP-Beschränkung anzeigen und im Agile-Story-Board von [!UICONTROL Kanban] aktualisieren, wie in [Verwalten der Work In Progress (WIP)-Beschränkung auf der [!UICONTROL Kanban]-Pinnwand](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md) beschrieben.

So beschränken Sie den laufenden Arbeitsaufwand für Ihr Kanban-Team:

{{step1-to-team}}

1. Klicken Sie auf **[!UICONTROL Team wechseln]**-Symbol ![Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das Kanban-Team aus, das Sie verwalten möchten.
1. Klicken Sie auf die **&#x200B;**&#x200B;Mehr![](assets/more-menu.png) und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.

   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Stellen Sie **[!UICONTROL Abschnitt]** Agile“ im Abschnitt **[!UICONTROL Methodik]** sicher, dass Kanban ausgewählt ist.

1. Geben Sie im Abschnitt **[!UICONTROL Storyboard]** im Feld **[!UICONTROL WIP-Limit]** die maximale Anzahl von Elementen an, die in jeder Spalte des agilen Storyboards [!UICONTROL Kanban] zulässig ist. Sie können für jede Spalte ein anderes Limit festlegen. Die maximale Begrenzung, die Sie für jede Spalte festlegen können, beträgt 100.
Wenn dieser Wert festgelegt ist, wird beim Überschreiten des Grenzwerts für jede Spalte [!UICONTROL &#x200B; Storyboard eine Warnmeldung &#x200B;] dem agilen Storyboard (Kanban) angezeigt. Diese Warnmeldung wird nur angezeigt, wenn das WIP-Limit zum ersten Mal überschritten wird. Diese Warnmeldung wird nicht in Spalten angezeigt, deren Status mit &quot;[!UICONTROL &quot; &#x200B;].
Die WIP-Beschränkung ist lediglich eine visuelle Warnung und hindert Ihr Team nicht daran, mehr Elemente in einer Spalte als die von Ihnen festgelegte Beschränkung zu haben.

   ![WIP-Limit](assets/wip-limit-350x193.png)

1. Klicken Sie auf **Änderungen speichern**.

## Automatisches Hinzufügen von Storys aus dem Rückstand konfigurieren

<!-- this functionality needs to be verified-->

Sie können Storys aus dem Rückstand so konfigurieren, dass sie automatisch der ersten Spalte auf der [!UICONTROL Kanban]-Pinnwand hinzugefügt werden, sobald ein Element aus dieser Spalte verschoben wird.

{{step1-to-team}}

1. Klicken Sie auf **[!UICONTROL Team wechseln]**-Symbol ![Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das Kanban-Team aus, das Sie verwalten möchten.
1. Klicken Sie auf die **&#x200B;**&#x200B;Mehr![](assets/more-menu.png) und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.

   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Wählen Sie **[!UICONTROL Nächste Story automatisch aus dem Rückstand hinzufügen]**, um zu konfigurieren, dass das nächste Element aus dem Rückstand automatisch zur Spalte **[!UICONTROL Neu]** hinzugefügt wird, wenn ein Element aus der Spalte **[!UICONTROL In Bearbeitung]** verschoben wird.

   Benutzer müssen die Einstellung **Rückstand anzeigen** auf der [!UICONTROL Kanban]-Pinnwand aktivieren, damit diese Funktion wirksam wird. Wenn Benutzende die Einstellung [!UICONTROL Rückstand anzeigen] auf dem [!UICONTROL Kanban-Board] aktivieren, erfolgt die folgende Funktion:

   Jedes Mal, wenn eine Story von der Spalte [!UICONTROL In Bearbeitung] in eine Spalte auf dem Storyboard verschoben wird, die einen [!UICONTROL Abgeschlossen]-Status (oder einen Status, der [!UICONTROL Abgeschlossen] entspricht) darstellt, wird eine Story aus der Rückstandsspalte automatisch in die Spalte [!UICONTROL Neu] des [!UICONTROL Kanban-Boards].
Wenn die Story mit der höchsten Priorität aus dem Rückstand hinzugefügt wird, wird sie dem Story Board hinzugefügt.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.

## Konfigurieren Sie, wie lange Karten auf der Kanban[!UICONTROL Pinnwand &#x200B;] bleiben

Sie können auswählen, wie lange ausgefüllte Karten auf der [!UICONTROL Kanban]-Pinnwand bleiben. Aufgaben, die vom Kanban[!UICONTROL Board &#x200B;], können weiterhin im ursprünglichen Projekt aufgerufen werden.

{{step1-to-team}}

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Teams wechseln]** ![Symbol Teams wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Kanban-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.
1. Wählen Sie das Kanban-Team aus.
1. Klicken Sie auf das **[!UICONTROL Mehr]**-![](assets/more-menu.png) und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.

   ![Team bearbeiten](assets/edit-team-settings-350x205.png)

1. Wählen Sie im Dropdown-Menü **[!UICONTROL Anzahl der Tage, die die abgeschlossenen Karten auf dem Kanban]** Board bleiben, einen Wert aus.

   Sie können eine Zahl zwischen 1 und 30 Tagen auswählen.
1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.
