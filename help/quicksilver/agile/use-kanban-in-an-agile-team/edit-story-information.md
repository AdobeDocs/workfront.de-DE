---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Story-Informationen bearbeiten
description: Beim Anzeigen einer Story-Kachel auf dem Kanban-Board stehen bestimmte Informationen zur Inline-Bearbeitung direkt über die Story-Kachel zur Verfügung.
author: Courtney
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YNFdopcCAju4MaN2oqssN0Q6H7k0Stg3udO0AipWIMs
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 340
ht-degree: 10%

---

# Bearbeiten von Story-Informationen

## Informationen, welche Informationen angezeigt und bearbeitet werden können {#understand-what-information-can-be-viewed-and-edited}

Wenn Sie eine Story-Kachel auf dem [!UICONTROL Kanban]-Board anzeigen, sind die Informationen in der folgenden Tabelle verfügbar. Die meisten Informationen können direkt über die Story-Kachel inline bearbeitet werden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Information</strong> </th> 
   <th><strong>sichtbar</strong> </th> 
   <th><strong>Bearbeitbar inline</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Der Name der Story mit einem Link direkt zur Aufgabe oder zum Problem</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Der Projektname mit einem Link direkt zum Projekt</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Die Anzahl der Punkte oder Stunden bis zum Abschluss eines Storys und die Anzahl der Punkte oder Stunden bis zum Abschluss eines <br>. Diese Zahlen werden zur Berechnung und Anzeige des Prozentsatzes bis zum Abschluss eines Storys verwendet.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Der [!UICONTROL Prozent abgeschlossen] für jede Story und jedes Problem.<br>[!UICONTROL Der Prozentsatz abgeschlossen] für die Iteration wird auf der Grundlage des [!UICONTROL Prozent abgeschlossen] für jede Story berechnet.<br></p> <p>Beim Aktualisieren von [!UICONTROL Prozent abgeschlossen] für eine Story oder ein Problem können Sie eine beliebige Zahl zwischen 0 und 100 auswählen.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Wem die Story zugewiesen ist</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Die Farbe oder Kategorie der Kachel</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Alle zusätzlichen Felder (einschließlich benutzerdefinierter Felder), die der Agile-Ansicht hinzugefügt wurden, indem die Agile-Ansicht geändert wurde, wie unter „Erstellen und Anpassen einer Agile-Ansicht“ in <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Überblick über Ansichten in [!DNL Adobe Workfront]</a> beschrieben</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
   <p>Work oder höher</p> </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Anzeigen und Bearbeiten von Informationen auf einer Story-Kachel

{{step1-to-team}}

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Symbol Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Kanban-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Zum Kanban[!UICONTROL Board &#x200B;].
1. Erweitern Sie die Kachel Story , um alle mit der Story verbundenen Felder anzuzeigen.

   ![Story-Karte](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. (Optional) Um ein Feld zu bearbeiten, klicken Sie auf das Feld und nehmen Sie dann Änderungen vor.
Sie müssen über [!UICONTROL Bearbeiten]-Rechte für die Aufgabe oder das Problem verfügen, um die Story-Kachel bearbeiten zu können.
Weitere Informationen zu den einzelnen Feldern und dazu, ob sie bearbeitet werden können, finden Sie unter [Informationen, die angezeigt und bearbeitet werden können](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>Um den [!UICONTROL Prozent abgeschlossen] zu ändern, müssen Sie eine Zahl zwischen 0 und 100 eingeben. Das Feld ist kein Schieberegler, den Sie verschieben können.
