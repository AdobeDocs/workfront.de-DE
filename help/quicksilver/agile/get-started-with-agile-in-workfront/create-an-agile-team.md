---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Erstellen eines agilen Teams
description: Adobe Workfront ermöglicht es agile Teams, ihre Arbeit inkrementell und organisiert abzuschließen.
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: cf044c8cff6b1172ec460ae232cd07c9b7c808b7
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 0%

---

# Erstellen eines agilen Teams

<!--Audited: 01/2024-->

[!DNL Adobe Workfront] ermöglicht es agile Teams, die Arbeit inkrementell und organisiert abzuschließen.

Jeder Benutzer in der Organisation kann das agile Team sehen und alle agilen Komponenten für das Team anzeigen, einschließlich Rückstand, Iterationen, Storyboard und individuellen Meldungen. Es sind jedoch nur Mitglieder des Teams mit [!UICONTROL Bearbeiten] Der Zugriff auf die Arbeit kann Änderungen an der dem Team zugewiesenen Arbeit vornehmen.

[!DNL Workfront] unterstützt die folgenden agilen Methoden:

* **[!UICONTROL Scrum]**: Teams verfügen über einen Rückstand bei der Arbeit, der noch erledigt werden muss. Wenn das Team bereit ist, an einem bestimmten Arbeitsbereich zu arbeiten, wird die Arbeit vom Rückstadium in eine Iteration verschoben. Weitere Informationen zur Verwaltung eines Scrum-Teams finden Sie unter [In einem agilen Team scrum](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban]:** Teams bewegen ihre Arbeit in der Kanban-Ansicht über vordefinierte Status. Die Standardstatus sind: &quot;backlog&quot;, &quot;In-process&quot;und &quot;done&quot;. Weitere Informationen zur Verwaltung eines Kanban-Teams finden Sie unter [Kanban in einem agilen Team](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

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
   <td> <p>Neu: Standard</p>
   Aktuell: 
   <ul><li><p>[!UICONTROL Plan] zur Einrichtung eines neuen agilen Teams</p></li> 
   <li><p>[!UICONTROL Arbeit oder höher zur Konvertierung eines Teams in ein agiles Team</p></li></ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Entscheidung über eine agile Methode

Sie können für Ihr agiles Team entweder eine Scrum- oder Kanban-agile-Methode verwenden. Jede Methode bietet verschiedene Vorteile. Die Funktionsweise Ihres agilen Teams bestimmt die agile Methodik, die Sie verwenden.

Sowohl Scrum- als auch Kanban-agile-Methoden in [!DNL Workfront] ermöglichen es Ihnen, Geschichten über eine Story-Pinnwand zu verschieben, um eine Statusänderung und den Fortschritt der Geschichte anzuzeigen.

agile Scrum- und Kanban-Methoden in [!DNL Workfront] unterscheiden sich wie folgt:

### Vorteile der Verwendung von Kanban in [!DNL Workfront]

Die [!DNL Kanban] agile Methode in [!DNL Workfront] ermöglicht es Ihnen, Geschichten einfacher über ein agiles Storyboard zu verschieben und gleichzeitig den Umfang der laufenden Arbeit zu begrenzen. Bei Verwendung der Variablen [!DNL Kanban] agile Methode.

Die folgende Funktion unterstützt diese Methode:

* Anzeigen des Rückstands im [!DNL Kanban] agile Story Board.\
   Weitere Informationen finden Sie unter [Fügen Sie dem [!UICONTROL Kanban] Pinnwand](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* Konfigurieren Sie Elemente im Rückstand, die automatisch zum [!UICONTROL Kanban] agile Story-Pinnwand, wenn andere Elemente in einen Status verschoben werden, der dem Status Complete entspricht.\
   Weitere Informationen finden Sie im Abschnitt . [Konfigurieren von Storys, die automatisch aus dem Backlog hinzugefügt werden sollen](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) im Artikel [Kanban konfigurieren](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Konfigurieren einer Beschränkung für laufende Arbeit (WIP), die auf der Seite [!UICONTROL Kanban] agile Story Board.\
   Weitere Informationen finden Sie unter [Verwalten der Grenze für laufende Arbeiten (WIP) auf dem Kanban-Board](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Vorteile der Verwendung von Scrum in [!DNL Workfront]

Die agile Scrum-Methode in [!DNL Workfront] ermöglicht es Ihnen, einer agilen Iteration eine Reihe von Geschichten hinzuzufügen und eine Story-Pinnwand für diese Iteration zu erstellen. Die Iteration basiert auf den von Ihnen definierten Start- und Enddaten.

Die folgende Funktion unterstützt diese Methode:

* Einbeziehen von Problemen in die [!UICONTROL Scrum] Storyboard
* Probleme im Rückstand eines agilen Teams einschließen
* Unteraufgaben können auf der Seite [!UICONTROL Scrum] Storyboard
* In einer Aufschlüsselungsgrafik können Sie den Fortschritt bei der Iteration anhand von Meldungen anzeigen.\
   Weitere Informationen finden Sie unter [Übersicht über die Agile-Burndown-Liste](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Erstellen eines agilen Teams

{{step1-to-team}}

1. Klicken Sie auf **[!UICONTROL Switch-Teams]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png)Klicken Sie auf **[!UICONTROL Neues Team erstellen]**.

   ![Wählen Sie Neues Team erstellen aus.](assets/create-new-team-350x198.png)

   Das Feld Neues Team wird angezeigt.

1. Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Teamname]</strong> </td> 
      <td>Geben Sie einen Namen für das neue agile Team ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Dies ist ein Agile-Team]</strong> </td> 
      <td>Wählen Sie diese Option aus, um dieses neue Team als agiles Team zu konfigurieren.</td> 
     </tr>

   <tr> 
      <td role="rowheader"><strong>[!UICONTROL ist aktiv]</strong> </td> 
      <td>Wählen Sie diese Option aus, um dieses Team zu aktivieren. Inaktive Teams sind nicht für andere Benutzer sichtbar, die sie für die Arbeit zuweisen können. </td> 
     </tr>


   <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Group]</strong> </td> 
      <td> <p>Beginnen Sie mit der Eingabe des Namens einer Gruppe, die dem Team hinzugefügt werden soll, und wählen Sie dann den Namen aus, wenn er in der Dropdown-Liste angezeigt wird.</p> <p><b>NOTIZ</b></p> <p> Wenn ein Team einer Gruppe oder Untergruppe zugewiesen wird, können Gruppenadministratoren dieser Gruppe oder Untergruppe das Team verwalten, ohne Mitglied des Teams zu sein. Gruppenadministratoren können im [!UICONTROL Hauptmenü] den Bereich [!UICONTROL Teams] aufrufen und auf den Pfeil [!UICONTROL Switch Teams] klicken. <img src="assets/switch-team-icon.png" alt="Symbol &quot;Team wechseln&quot;"> , um alle Teams aufzulisten, die den von ihnen verwalteten Gruppen zugewiesen sind.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Teammitglieder]</strong> </td> 
      <td>Beginnen Sie mit der Eingabe des Namens eines Benutzers für das Team und wählen Sie dann den Namen aus, wenn er in der Dropdown-Liste angezeigt wird.<br>Wiederholen Sie diesen Vorgang, um mehrere Benutzer zum Team hinzuzufügen.<br>Da Benutzer mehreren Teams angehören können, können sie sich sowohl in mobilen als auch in nicht agilen Teams befinden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Beschreibung]</strong> </td> 
      <td><p>Geben Sie eine Beschreibung für das Team ein.</p> <p>Die Beschreibung wird bei der Auswahl des Teams oben rechts im Bereich [!UICONTROL Teams] angezeigt.</p>
      <p>Wenn die Beschreibung lang ist, können Sie darauf klicken, um die vollständige Beschreibung in einem Popup-Fenster anzuzeigen. Wenn Sie Zugriff auf die [!UICONTROL Team-Einstellungen] haben, können Sie die Beschreibung auch direkt im Popup-Fenster bearbeiten.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Klicks **[!UICONTROL Erstellen]**.

   Informationen zum Konfigurieren eines Agile-Teams finden Sie in den folgenden Artikeln:

   * [Konfigurieren [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Konfigurieren [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Ein vorhandenes Team in ein agiles Team konvertieren

Sie können ein vorhandenes Team in ein agiles Team konvertieren:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Teams]**.
1. Klicken Sie auf **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das Team aus, das Sie in ein agiles Team konvertieren möchten.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü und wählen Sie **[!UICONTROL Bearbeiten]**.\
   Nur Teammitglieder mit einer [!UICONTROL Plan] oder [!UICONTROL Arbeit] -Lizenz sehen Sie diese Option.\
   ![](assets/edit-team-settings-350x205.png)

1. Im **[!UICONTROL Agile]** Bereich, wählen Sie **[!UICONTROL Dies ist ein Agile-Team]**.

1. Im **[!UICONTROL Methode]** auswählen, ob das Team eine **[!UICONTROL Scrum]** oder **[!UICONTROL Kanban]** agile Methode.

1. Klicks **Speichern Sie die Änderungen.**

   Das Team wird als Agile-Team gespeichert. Sie können das neue Team als Scrum- oder Kanban-Team konfigurieren, wenn Sie das Team bearbeiten.

   Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Konfigurieren [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Konfigurieren [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
