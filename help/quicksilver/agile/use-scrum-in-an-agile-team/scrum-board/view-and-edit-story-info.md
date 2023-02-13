---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Anzeigen und Bearbeiten von Story-Informationen auf der Scrum-Pinnwand
description: Beim Anzeigen einer Story-Kachel auf der Kanban-Pinnwand stehen bestimmte Informationen zur Inline-Bearbeitung zur Verfügung, direkt über die Story-Kachel.
author: Lisa
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Anzeigen und Bearbeiten von Story-Informationen auf [!UICONTROL Scrum] Pinnwand

## Informationen darüber, welche Informationen angezeigt und bearbeitet werden können

Bei der Anzeige einer Storykachel auf der Storyboard-Pinnwand sind die Informationen in der folgenden Tabelle verfügbar. Sie können die meisten Informationen inline bearbeiten, direkt über die Kachel &quot;Geschichte&quot;.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Informationen</strong> </th> 
   <th><strong>Sichtbar</strong> </th> 
   <th><strong>Bearbeitbare Inline-Zeilen</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Der Name des Verlaufs mit einem Link direkt zur Aufgabe oder zum Problem</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Der Projektname mit einem Link direkt zum Projekt<br>Dieser Link wird nur bei Geschichten (übergeordnete Aufgaben, keine Unteraufgaben) angezeigt, wenn die agile Ansicht bei einer Iteration verwendet wird. sie wird bei Verwendung einer agilen Ansicht in einem Projekt nicht angezeigt.</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Die Anzahl der vollständigen Punkte oder Stunden der Meldung und die Anzahl der der Meldung zugewiesenen Punkte oder Stunden<br>Diese Zahlen werden verwendet, um den [!UICONTROL Prozentwert pro Vollständigkeit] für jede Geschichte zu berechnen und anzuzeigen.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Prozentualer Abschluss] für jede Geschichte und jedes Thema.<br>Der [!UICONTROL Prozentwert pro Abschluss] für die Iteration wird auf der Grundlage des [!UICONTROL Prozentsatzes abgeschlossen] für jede Geschichte berechnet.</p> <p>Bei der Aktualisierung von [!UICONTROL Prozent Vollständigkeit] für eine Meldung oder ein Problem können Sie eine beliebige Zahl zwischen 0 und 100 wählen.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Wem die Geschichte zugeordnet ist</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Die Farbe oder Kategorie der Kachel</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Alle zusätzlichen Felder (einschließlich benutzerdefinierter Felder), die möglicherweise zur agilen Ansicht hinzugefügt wurden, indem die agile Ansicht geändert wurde, wie unter "Erstellen und Anpassen einer [!UICONTROL Agile]-Ansicht"in <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Übersicht über Ansichten in [!UICONTROL Adobe Workfront]</a>.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

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
   <td> <p>Zugriff auf die Aufgabe oder das Problem bearbeiten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Anzeigen und Bearbeiten von Informationen zu einem Story-Baustein

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Teams]**.

1. (Optional) Klicken Sie auf die **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie im linken Bereich die Option **[!UICONTROL Iterationen]** , um eine bestimmte Iteration auszuwählen, oder wählen Sie **[!UICONTROL Aktuelle Iteration]**.

1. Navigieren Sie zu [!UICONTROL Scrum] agile Story Board.
1. Erweitern Sie die [!UICONTROL Geschichte] -Kachel, um alle Felder anzuzeigen, die mit der Geschichte verknüpft sind.

   ![](assets/agile-storycard-scrum-2021-350x333.png)

1. (Optional) Um ein Feld zu bearbeiten, klicken Sie auf das Feld und nehmen Sie dann alle Änderungen vor.

   Sie müssen [!UICONTROL Bearbeiten] Berechtigungen für die Aufgabe oder das Problem, um die Story-Kachel zu bearbeiten.

>[!NOTE]
>
>So ändern Sie die [!UICONTROL Prozent abgeschlossen], müssen Sie eine Zahl zwischen 0 und 100 eingeben. Das Feld ist kein Schieberegler, den Sie verschieben können.
