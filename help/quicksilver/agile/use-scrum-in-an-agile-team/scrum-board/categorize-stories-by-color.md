---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Kategorisieren von Meldungen nach Farbe auf der Scrum-Pinnwand
description: Die standardmäßige Farbzuordnung von Scrum-Board-Meldungen hängt davon ab, ob sich das Story-Forum auf einer Iteration oder einem Projekt befindet.
author: Lisa
feature: Agile
exl-id: 8e351505-73d1-4c8f-b369-53c965b88c95
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Kategorisieren von Meldungen nach Farbe auf der [!UICONTROL Scrum] Pinnwand

## Ändern der standardmäßigen Farbzuordnung von Geschichten

Die standardmäßige Farbzuordnung von Geschichten hängt davon ab, ob sich das Storyboard in einer Iteration oder in einem Projekt befindet:

* **[!UICONTROL Iteration]**: Bei einer Iteration sind die Story-Pinnwände entsprechend dem Projekt, mit dem die Geschichte verknüpft ist, farbcodiert. (Jedem Projekt wird willkürlich eine Farbe auf dem Storyboard zugewiesen.) Sie können dieses Standardverhalten für jedes agile Team ändern. Farben für agile Geschichten bei einer Iteration können an das Projekt (Standard), die Priorität der Geschichte, den Eigentümer oder die freie Form gebunden werden. Weitere Informationen finden Sie unter [Konfigurieren der Verwendung von Farbindikatoren für Meldungen auf der Landingpage](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur4) im Artikel [Konfigurieren von Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* **[!UICONTROL Projekt]**: Bei einem Projekt stimmen alle Unteraufgaben mit der Farbe der übergeordneten Aufgabe überein, sodass die Farben aller Geschichten in jeder Swimlane identisch sind. Farben werden Aufgaben zufällig zugewiesen, wenn sie erstellt werden, wenn die Aufgabe keine Unteraufgaben hat oder keine übergeordnete Aufgabe hat. Sie können dieses Standardverhalten ändern, indem Sie die agile Ansicht ändern. Farben für agile Geschichten in einem Projekt können an die übergeordnete Geschichte (Standard), die Priorität einer Geschichte, den Eigentümer oder die freie Form gebunden werden. Weitere Informationen finden Sie unter [Erstellen oder Anpassen von [!UICONTROL Agile] Ansicht](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [Ansichten - Übersicht in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

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
   <td> <p>[!UICONTROL Worker] oder höher</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administratoren können die Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Ändern der Farbe von Geschichten bei Verwendung von Freiform

Wenn die agile Team-Einstellungen so konfiguriert wurden, dass die [!UICONTROL Kartenfarbe zuordnen zu] ist auf [!UICONTROL Kostenlose Form], können Benutzer die Farbe einzelner Story-Kacheln manuell ändern. Dies kann nützlich sein, um andere für das Team oder die Organisation wichtige Arten von Informationen zu kommunizieren:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe] Workfront, und klicken Sie dann auf **[!UICONTROL Teams]**.

1. (Optional) Klicken Sie auf die **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie im linken Bereich die Option **[!UICONTROL Iterationen]** , um eine bestimmte Iteration auszuwählen, oder wählen Sie **[!UICONTROL Aktuelle Iteration]**.
1. Bewegen Sie den Mauszeiger über das farbige Banner am oberen Rand der Kachel &quot;Geschichte&quot;.

   ![](assets/agile-story-color1-nwe-350x140.png)

1. Klicken **[!UICONTROL Farbe ändern]** und wählen Sie dann die gewünschte Farbe aus.

   ![](assets/agile-story-color2-nwe-350x138.png)
