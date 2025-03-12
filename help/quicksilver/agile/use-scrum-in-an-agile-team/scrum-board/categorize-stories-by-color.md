---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Storys auf dem Scrum-Board nach Farbe kategorisieren
description: Die Standardfarbzuordnung von Scrum-Board-Storys unterscheidet sich, je nachdem, ob sich das Storyboard in einer Iteration oder in einem Projekt befindet.
author: Lisa
feature: Agile
exl-id: 8e351505-73d1-4c8f-b369-53c965b88c95
source-git-commit: 91dc9946566e15bf32d0d89975e3e6b66b39e873
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# Kategorisieren von Storys nach Farbe auf dem [!UICONTROL Scrum]-Board

## Standardfarbzuordnung von Storys ändern

Die Standardfarbzuordnung von Storys unterscheidet sich, je nachdem, ob sich das Storyboard in einer Iteration oder in einem Projekt befindet:

* **[!UICONTROL Iteration]**: Bei einer Iteration werden Story-Board-Kacheln entsprechend dem Projekt, mit dem die Story verknüpft ist, farbcodiert. (Jedem Projekt wird willkürlich eine Farbe auf dem Storyboard zugewiesen.) Sie können dieses Standardverhalten für jedes agile Team ändern. Die Farben für agile Storys einer Iteration können an das Projekt (Standard), die Story-Priorität, den Eigentümer oder die Freiform gebunden werden. Weitere Informationen finden Sie unter [Konfigurieren der Verwendung von Farbindikatoren für Storys im Agile-Story](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur4) im Artikel [Konfigurieren von Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* **[!UICONTROL Projekt]**: In einem Projekt stimmen alle Teilaufgaben mit der Farbe der übergeordneten Aufgabe überein, sodass die Farben aller Storys in einem bestimmten Swimlane gleich sind. Farben werden Aufgaben nach dem Zufallsprinzip zugewiesen, wenn sie erstellt werden, wenn die Aufgabe keine Unteraufgaben hat oder keine übergeordnete Aufgabe hat. Sie können dieses Standardverhalten ändern, indem Sie die Agile-Ansicht ändern. Die Farben für agile Storys eines Projekts können an die übergeordnete Story (Standard), die Story-Priorität, den Eigentümer oder die Freiform gebunden werden. Weitere Informationen finden Sie unter [Erstellen oder Anpassen einer [!UICONTROL Agile]Ansicht](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [Ansichten - Übersicht in [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

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
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ändern der Farbe von Storys bei Verwendung von Freiformformularen

Wenn die Agile-Team-Einstellungen so konfiguriert wurden, dass die Option [!UICONTROL Kartenfarbe zuordnen zu] auf [!UICONTROL Freiform] festgelegt ist, können Benutzende die Farbe einzelner Story-Kacheln manuell ändern. Dies kann für die Kommunikation anderer Arten von Informationen nützlich sein, die für das Team oder die Organisation wichtig sind:

{{step1-to-team}}

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Symbol Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Scrum-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie im linken Bereich **[!UICONTROL Iterationen]**, um eine bestimmte Iteration auszuwählen, oder wählen Sie **[!UICONTROL Aktuelle Iteration]**.
1. Bewegen Sie den Mauszeiger über das farbige Banner oben auf der Story-Kachel.

   ![Story-Karte](assets/agile-story-color1-nwe-350x140.png)

1. Klicken Sie **[!UICONTROL Farbe ändern]** und wählen Sie dann die gewünschte Farbe aus.

   ![Farbe wählen](assets/agile-story-color2-nwe-350x138.png)
