---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Erstellen eines agilen Teams
description: Adobe Workfront ermöglicht es agile Teams, ihre Arbeit inkrementell und organisiert abzuschließen.
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '1012'
ht-degree: 1%

---

# Erstellen eines agilen Teams

<!--Audited: 01/2024-->

Mit [!DNL Adobe Workfront] können agile Teams die Arbeit inkrementell und organisiert abschließen.

Jeder Benutzer in der Organisation kann das agile Team sehen und alle agilen Komponenten für das Team anzeigen, einschließlich Rückstand, Iterationen, Storyboard und individuellen Meldungen. Allerdings können nur Mitglieder des Teams, die Zugriff auf [!UICONTROL Bearbeiten] haben, Änderungen an der dem Team zugewiesenen Arbeit vornehmen.

[!DNL Workfront] unterstützt die folgenden agilen Methoden:

* **[!UICONTROL Scrum]**: Teams verfügen über einen Arbeitsrückstand, der durchgeführt werden muss. Wenn das Team bereit ist, an einem bestimmten Arbeitsbereich zu arbeiten, wird die Arbeit vom Rückstadium in eine Iteration verschoben. Weitere Informationen zum Verwalten eines Scrum-Teams finden Sie unter [Scrum in einem agilen Team](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban]:** Teams bewegen ihre Arbeit in der Kanban-Ansicht über vorbestimmte Status. Die Standardstatus sind: &quot;backlog&quot;, &quot;In-process&quot;und &quot;done&quot;. Weitere Informationen zur Verwaltung eines Kanban-Teams finden Sie unter [Kanban in einem agilen Team](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

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

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan oder welchen Lizenztyp Sie haben.

+++

## Entscheidung über eine agile Methode

Sie können für Ihr agiles Team entweder eine Scrum- oder Kanban-agile-Methode verwenden. Jede Methode bietet verschiedene Vorteile. Die Funktionsweise Ihres agilen Teams bestimmt die agile Methodik, die Sie verwenden.

Sowohl die agile Scrum- als auch die Kanban-Methodik in [!DNL Workfront] ermöglichen es Ihnen, Geschichten über ein Storyboard zu verschieben, um eine Statusänderung und den Fortschritt der Geschichte anzuzeigen.

Die agilen Scrum- und Kanban-Methoden in [!DNL Workfront] unterscheiden sich auf folgende Weise:

### Vorteile der Verwendung von Kanban in [!DNL Workfront]

Die [!DNL Kanban] agile Methodik in [!DNL Workfront] ermöglicht es Ihnen, Geschichten einfacher über eine agile Storyboard zu verschieben und gleichzeitig den Umfang der laufenden Arbeit zu begrenzen. Bei Verwendung der agile Methode [!DNL Kanban] gibt es keine Start- und Enddaten.

Die folgende Funktion unterstützt diese Methode:

* Rufen Sie den Rückstand auf der Karte [!DNL Kanban] für eine agile Meldung auf.\
   Weitere Informationen finden Sie unter [Hinzufügen des Rückstands zur [!UICONTROL Kanban]-Pinnwand](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* Konfigurieren Sie Elemente im Rückstand so, dass sie automatisch zum agilen Storyboard [!UICONTROL Kanban] hinzugefügt werden, wenn andere Elemente in einen Status verschoben werden, der dem Status Complete entspricht.\
   Weitere Informationen finden Sie im Abschnitt [Meldungen konfigurieren, die automatisch aus dem Rückstau hinzugefügt werden](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) im Artikel [Kanban konfigurieren](../../agile/get-started-with-agile-in-workfront/configure-kanban.md) .

* Konfigurieren Sie eine Beschränkung für laufende Arbeiten (WIP), die auf dem agilen Storyboard [!UICONTROL Kanban] angezeigt werden soll.\
   Weitere Informationen finden Sie unter [Limit für laufende Arbeiten (WIP) auf der Kanban-Pinnwand verwalten](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Vorteile der Verwendung von Scrum in [!DNL Workfront]

Die agile Methode Scrum in [!DNL Workfront] ermöglicht es Ihnen, eine Reihe von Geschichten zu einer agilen Iteration hinzuzufügen und eine Story-Pinnwand für diese Iteration zu erstellen. Die Iteration basiert auf den von Ihnen definierten Start- und Enddaten.

Die folgende Funktion unterstützt diese Methode:

* Einbeziehen von Problemen auf der [!UICONTROL Scrum]-Storyplatine
* Probleme im Rückstand eines agilen Teams einschließen
* Unteraufgaben können auf der Storyboard [!UICONTROL Scrum] angezeigt werden
* In einer Aufschlüsselungsgrafik können Sie den Fortschritt bei der Iteration anhand von Meldungen anzeigen.\
   Weitere Informationen finden Sie unter [Übersicht über die Agile-Burndown-Grafik](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Erstellen eines agilen Teams

{{step1-to-team}}

1. Klicken Sie auf das Symbol **[!UICONTROL Teams wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und dann auf **[!UICONTROL Neues Team erstellen]**.

   ![Wählen Sie Neues Team erstellen.](assets/create-new-team-350x198.png)

   Das Feld Neues Team wird angezeigt.

1. Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Name]</strong> </td> 
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
      <td> <p>Beginnen Sie mit der Eingabe des Namens einer Gruppe, die dem Team hinzugefügt werden soll, und wählen Sie dann den Namen aus, wenn er in der Dropdown-Liste angezeigt wird.</p> <p><b>NOTIZ</b></p> <p> Wenn ein Team einer Gruppe oder Untergruppe zugewiesen wird, können Gruppenadministratoren dieser Gruppe oder Untergruppe das Team verwalten, ohne Mitglied des Teams zu sein. Gruppenadministratoren können im [!UICONTROL Hauptmenü] den Bereich [!UICONTROL Teams] aufrufen und auf den Pfeil <img src="assets/switch-team-icon.png" alt="Symbol &quot;Team wechseln&quot;"> [!UICONTROL Switch Teams] klicken, um alle Teams aufzulisten, die den von ihnen verwalteten Gruppen zugewiesen sind.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Teammitglieder]</strong> </td> 
      <td>Beginnen Sie mit der Eingabe des Namens eines Benutzers für das Team und wählen Sie dann den Namen aus, wenn er in der Dropdown-Liste angezeigt wird.<br>Wiederholen Sie diesen Vorgang, um mehrere Benutzer zum Team hinzuzufügen.<br>Da Benutzer mehreren Teams angehören können, können sie sich sowohl in agilen als auch in nicht agilen Teams befinden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Beschreibung]</strong> </td> 
      <td><p>Geben Sie eine Beschreibung für das Team ein.</p> <p>Die Beschreibung wird bei der Auswahl des Teams oben rechts im Bereich [!UICONTROL Teams] angezeigt.</p>
      <p>Wenn die Beschreibung lang ist, können Sie darauf klicken, um die vollständige Beschreibung in einem Popup-Fenster anzuzeigen. Wenn Sie Zugriff auf die [!UICONTROL Team-Einstellungen] haben, können Sie die Beschreibung auch direkt im Popup-Fenster bearbeiten.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Erstellen]**.

   Informationen zum Konfigurieren eines Agile-Teams finden Sie in den folgenden Artikeln:

   * [Konfigurieren von [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Konfigurieren von [!UICONTROL scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Ein vorhandenes Team in ein agiles Team konvertieren

Sie können ein vorhandenes Team in ein agiles Team konvertieren:

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Teams]**.![](assets/main-menu-icon.png)
1. Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder aus dem Dropdown-Menü ein neues Team aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie das Team aus, das Sie in ein agiles Team konvertieren möchten.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** und wählen Sie dann **[!UICONTROL Bearbeiten]** aus.\
   Nur Teammitglieder mit einer [!UICONTROL Plan] - oder [!UICONTROL Work] -Lizenz sehen diese Option.\
   ![](assets/edit-team-settings-350x205.png)

1. Wählen Sie im Abschnitt **[!UICONTROL Agile]** die Option **[!UICONTROL Dies ist ein Agile-Team]**.

1. Wählen Sie im Abschnitt **[!UICONTROL Methodologie]** aus, ob das Team eine agile Methode des Typs **[!UICONTROL Scrum]** oder **[!UICONTROL Kanban]** verwendet.

1. Klicken Sie auf **Änderungen speichern.**

   Das Team wird als Agile-Team gespeichert. Sie können das neue Team als Scrum- oder Kanban-Team konfigurieren, wenn Sie das Team bearbeiten.

   Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Konfigurieren von [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Konfigurieren von [!UICONTROL scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
