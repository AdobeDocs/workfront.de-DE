---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Erstellen eines Agile-Teams
description: Adobe Workfront ermöglicht es agilen Teams, ihre Arbeit inkrementell und organisiert abzuschließen.
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: 79da9f7ed5149ca33f6eaeac347188149f410695
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 1%

---

# Erstellen eines agilen Teams

<!--Audited: 01/2024-->

[!DNL Adobe Workfront] ermöglicht es agilen Teams, ihre Arbeit inkrementell und organisiert abzuschließen.

Jeder Benutzer in der Organisation kann das Agile-Team sehen und alle agilen Komponenten für das Team anzeigen, einschließlich Rückstand, Iterationen, Story Board und einzelner Storys. Allerdings können nur Mitglieder des Teams mit [!UICONTROL Bearbeiten]-Zugriff Änderungen an der dem Team zugewiesenen Arbeit vornehmen.

[!DNL Workfront] unterstützt die folgenden agilen Methoden:

* **[!UICONTROL Scrum]**: Teams haben einen Rückstand an Arbeit, die erledigt werden muss. Wenn das Team bereit ist, an einem bestimmten Arbeitsblock zu arbeiten, wird die Arbeit aus dem Rückstand in eine Iteration verschoben. Weitere Informationen zum Verwalten eines Scrum-Teams finden Sie unter [Scrum in einem agilen Team](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban]:** Teams verschieben Arbeit in der Kanban-Ansicht über vorbestimmte Status hinweg. Standardstatus sind: „Rückstand“, „In Bearbeitung“ und „Fertig“. Weitere Informationen zum Verwalten eines Kanban-Teams finden Sie unter [Kanban in einem agilen Team](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: Standard</p>
   Aktuell: 
   <ul><li><p>[!UICONTROL Plan], um ein neues agiles Team zu erstellen</p></li> 
   <li><p>[!UICONTROL Work] oder höher, um ein Team in ein agiles Team zu konvertieren</p></li></ul> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Entscheidung über eine agile Methodik

Sie können für Ihr agiles Team entweder eine Scrum- oder Kanban-Agile-Methodik verwenden. Jede Methode bietet verschiedene Vorteile. Die Art und Weise, wie Ihr agiles Team arbeitet, bestimmt die Agile-Methodik, die Sie verwenden.

Sowohl Scrum- als auch Kanban-Agile-Methoden in [!DNL Workfront] ermöglichen es Ihnen, Storys über eine Story-Pinnwand zu verschieben, um eine Statusänderung und den Fortschritt der Story anzuzeigen.

Die agilen Methoden Scrum und Kanban in [!DNL Workfront] unterscheiden sich wie folgt:

### Vorteile der Verwendung von Kanban in [!DNL Workfront]

Die [!DNL Kanban] agile Methodik in [!DNL Workfront] ermöglicht es Ihnen, Storys einfacher über eine agile Story-Pinnwand zu verschieben und gleichzeitig den Umfang der laufenden Arbeit zu begrenzen. Bei Verwendung der [!DNL Kanban] agilen Methode gibt es keine Start- und Enddaten.

Die folgende Funktion unterstützt diese Methode:

* Zeigen Sie den Auftragsbestand auf dem [!DNL Kanban] Agile-Story-Board an.
Weitere Informationen finden Sie unter [Hinzufügen des Rückstands zum [!UICONTROL Kanban]-Board](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* Konfigurieren Sie Elemente im Rückstand, die automatisch zum agilen Story Board [!UICONTROL Kanban“ hinzugefügt werden] wenn andere Elemente in einen Status verschoben werden, der mit „Abgeschlossen“ übereinstimmt.
Weitere Informationen finden Sie im Abschnitt [Konfigurieren von Storys, die automatisch aus dem ](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) hinzugefügt werden“ im Artikel [Konfigurieren von Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Konfigurieren Sie ein Work In Progress (WIP)-Limit, das auf dem agilen Story Board [!UICONTROL Kanban] angezeigt werden soll.
Weitere Informationen finden Sie unter [Verwalten des Work In Progress (WIP)-Limits auf dem Kanban-Board](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Vorteile der Verwendung von Scrum in [!DNL Workfront]

Mit der agilen Scrum-Methodik in [!DNL Workfront] können Sie einer agilen Iteration eine Reihe von Storys hinzufügen und ein Story Board für diese Iteration erstellen. Die Iteration basiert auf dem von Ihnen definierten Start- und Enddatum.

Die folgende Funktion unterstützt diese Methode:

* Probleme im Story Board [!UICONTROL Scrum] einschließen
* Probleme im Rückstand eines agilen Teams einschließen
* Teilaufgaben können im Storyboard [!UICONTROL Scrum] angezeigt werden
* Burndown-Diagramm anzeigen, um den Fortschritt bei Storys während der Iteration anzuzeigen
Weitere Informationen finden Sie unter [Agile-Burndown-Diagramm - Übersicht](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Erstellen eines agilen Teams

{{step1-to-team}}

1. Klicken Sie auf das Symbol **[!UICONTROL Teams wechseln]** ![Symbol Team wechseln](assets/switch-team-icon.png) und klicken Sie dann auf **[!UICONTROL Neues Team erstellen]**.

   ![Wählen Sie Neues Team erstellen aus](assets/create-new-team.png)

   Das Feld Neues Team wird angezeigt.

1. Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Name]</strong> </td> 
      <td>Geben Sie einen Namen für das neue Agile-Team ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Dies ist ein agiles Team]</strong> </td> 
      <td>Wählen Sie diese Option, um dieses neue Team als agiles Team zu konfigurieren.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>[!UICONTROL ist aktiv]</strong> </td> 
      <td>Wählen Sie diese Option, um dieses Team zu aktivieren. Inaktive Teams sind für andere Benutzer, die sie der Arbeit zuweisen möchten, nicht sichtbar. </td> 
     </tr>


   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Group]</strong> </td> 
      <td> <p>Tippen Sie den Namen einer Gruppe, die dem Team hinzugefügt werden soll, und wählen Sie dann den Namen aus, wenn er in der Dropdown-Liste angezeigt wird.</p> <p><b>NOTIZ</b></p> <p> Wenn ein Team einer Gruppe oder Untergruppe zugewiesen wird, können alle Gruppenadministratoren dieser Gruppe oder Untergruppe das Team verwalten, ohne Mitglied des Teams zu sein. <img src="assets/switch-team-icon.png" alt="Team-Symbol wechseln"> Gruppenadministratoren können über das [!UICONTROL Hauptmenü] in den Bereich [!UICONTROL Teams] wechseln und auf den Pfeil [!UICONTROL Switch Teams] klicken, um alle Teams aufzulisten, die den von ihnen verwalteten Gruppen zugewiesen sind.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Members]</strong> </td> 
      <td>Geben Sie den Namen eines Benutzers ein, der dem Team angehören soll, und wählen Sie dann den Namen aus, wenn er in der Dropdown-Liste angezeigt wird.<br>Wiederholen Sie diesen Vorgang, um dem Team mehrere Benutzer hinzuzufügen.<br>Da Benutzer in mehr als einem Team arbeiten können, können sie sowohl in agilen als auch in nicht agilen Teams arbeiten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Beschreibung]</strong> </td> 
      <td><p>Beschreibung für das Team eingeben.</p> <p>Die Beschreibung wird oben rechts im Bereich [!UICONTROL Teams] angezeigt, wenn das Team ausgewählt wird.</p>
      <p>Wenn die Beschreibung lang ist, können Sie darauf klicken, um sie in einem Popup anzuzeigen. Wenn Sie Zugriff haben, um die [!UICONTROL Team-Einstellungen] zu bearbeiten, können Sie die Beschreibung auch direkt im Popup-Fenster bearbeiten.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

   Informationen zum Konfigurieren eines Agile-Teams finden Sie in den folgenden Artikeln:

   * [Konfigurieren von [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Konfigurieren von [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Konvertieren eines vorhandenen Teams in ein agiles Team

Sie können ein vorhandenes Team in ein agiles Team umwandeln:

{{step1-to-team}}

1. Klicken Sie auf **[!UICONTROL Team wechseln]**-Symbol ![Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das Team aus, das Sie in ein agiles Team konvertieren möchten.
1. Klicken Sie auf das **[!UICONTROL Mehr]**-Menü und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.

   Nur Team-Mitglieder mit einer [!UICONTROL Standard], [!UICONTROL Plan] oder [!UICONTROL Work]-Lizenz sehen diese Option.
   ![Bearbeiten auswählen](assets/edit-team-settings.png)

1. Wählen Sie im Abschnitt **[!UICONTROL Agile]** die Option **[!UICONTROL Dies ist ein Agile-Team]** aus.

1. Wählen Sie **[!UICONTROL Abschnitt]** Methodik“ aus, ob das Team eine **** Scrum- oder **[!UICONTROL Kanban]** Methode verwenden soll.

1. Klicken Sie auf **Änderungen speichern**.

   Das Team wird als Agile-Team gespeichert. Sie können das neue Team als Scrum- oder Kanban-Team konfigurieren, wenn Sie das Team bearbeiten.

   Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Konfigurieren von [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Konfigurieren von [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
