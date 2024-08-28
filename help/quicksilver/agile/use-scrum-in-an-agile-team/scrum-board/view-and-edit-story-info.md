---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Anzeigen und Bearbeiten von Meldungsinformationen auf der Randplatine
description: Beim Anzeigen einer Story-Kachel auf der Kanban-Pinnwand stehen bestimmte Informationen zur Inline-Bearbeitung zur Verfügung, direkt über die Story-Kachel.
author: Lisa
feature: Agile
exl-id: 88d156ea-0913-425e-b3eb-6ae81d2d2336
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '464'
ht-degree: 0%

---

# Anzeigen und Bearbeiten von Story-Informationen auf der [!UICONTROL Scrum]-Pinnwand

## Informationen darüber, welche Informationen angezeigt und bearbeitet werden können

Bei der Anzeige einer Storykachel auf der Storyboard-Pinnwand sind die Informationen in der folgenden Tabelle verfügbar. Sie können die meisten Informationen inline bearbeiten, direkt über den Bereich &quot;Geschichte&quot;.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Information</strong> </th> 
   <th><strong>Sichtbar</strong> </th> 
   <th><strong>Bearbeitbare Inline-Anzeige</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Der Name des Verlaufs mit einem Link direkt zur Aufgabe oder zum Problem</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Der Projektname mit einem Link direkt zum Projekt<br>Dieser Link wird nur bei Geschichten (übergeordnete Aufgaben, keine Unteraufgaben) angezeigt, wenn die agile Ansicht bei einer Iteration verwendet wird. Er wird nicht angezeigt, wenn eine agile Ansicht für ein Projekt verwendet wird.</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Die Anzahl der Punkte oder Stunden, die für die Meldung vollständig sind, und die Anzahl der Punkte oder Stunden, die der Meldung zugewiesen sind<br>Diese Zahlen werden verwendet, um die [!UICONTROL Prozentzahl abgeschlossen] für jede Meldung zu berechnen und anzuzeigen.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Prozentualer Abschluss] für jede Geschichte und jedes Thema.<br>Der [!UICONTROL Prozentwert pro Abschluss] für die Iteration wird anhand des [!UICONTROL Prozentsatzes pro Abschluss] für jede Geschichte berechnet.</p> <p>Bei der Aktualisierung von [!UICONTROL Prozent Vollständigkeit] für eine Meldung oder ein Problem können Sie eine beliebige Zahl zwischen 0 und 100 wählen.</p> </td> 
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
   <td> <p>Alle zusätzlichen Felder (einschließlich benutzerdefinierter Felder), die möglicherweise zur agilen Ansicht hinzugefügt wurden, indem die agile Ansicht geändert wurde, wie unter Erstellen und Anpassen einer [!UICONTROL Agile]-Ansicht in der <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Übersicht über Ansichten in [!UICONTROL Adobe Workfront]</a> beschrieben.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p> 
   oder
   <p>Aktuell: [!UICONTROL Arbeit] oder höher</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>[!UICONTROL Contribute] oder [!UICONTROL] Zugriff auf die Aufgabe oder das Problem verwalten</td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anzeigen und Bearbeiten von Informationen zu einem Story-Baustein

{{step1-to-team}}

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie im linken Bereich **[!UICONTROL Iterationen]** aus, um eine bestimmte Iteration auszuwählen, oder wählen Sie **[!UICONTROL Aktuelle Iteration]**.

1. Gehen Sie zur agilen Storyboard [!UICONTROL Scrum].
1. Erweitern Sie die Kachel [!UICONTROL story] , um alle Felder anzuzeigen, die mit der Geschichte verbunden sind.

   ![](assets/agile-storycard-scrum-2021-350x333.png)

1. (Optional) Um ein Feld zu bearbeiten, klicken Sie auf das Feld und nehmen Sie dann alle Änderungen vor.

   Sie müssen über die Berechtigung [!UICONTROL Bearbeiten] für die Aufgabe oder das Problem verfügen, um die Story-Kachel zu bearbeiten.

>[!NOTE]
>
>Um den [!UICONTROL Prozentsatz abgeschlossen] zu ändern, müssen Sie eine Zahl zwischen 0 und 100 eingeben. Das Feld ist kein Schieberegler, den Sie verschieben können.
