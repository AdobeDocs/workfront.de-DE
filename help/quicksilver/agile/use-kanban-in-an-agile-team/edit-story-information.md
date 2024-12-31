---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Story-Informationen bearbeiten
description: Beim Anzeigen einer Story-Kachel auf dem Kanban-Board stehen bestimmte Informationen zur Inline-Bearbeitung direkt über die Story-Kachel zur Verfügung.
author: Lisa
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Story-Informationen bearbeiten

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
   <td> <p>Die [!UICONTROL Prozent abgeschlossen] für jede Story und jedes Problem.<br>[!UICONTROL Percent Complete] für die Iteration wird basierend auf [!UICONTROL Percent Complete] für jede Story berechnet.<br></p> <p>Beim Aktualisieren von [!UICONTROL Prozent abgeschlossen] für eine Story oder ein Problem können Sie eine beliebige Zahl zwischen 0 und 100 auswählen.</p> </td> 
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
   <td> <p>Alle zusätzlichen Felder (einschließlich benutzerdefinierter Felder), die der agilen Ansicht hinzugefügt wurden, indem die agile Ansicht geändert wurde, wie in „Erstellen und Anpassen einer agilen Ansicht“ in "<a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref"> in [!DNL Adobe Workfront]</a>" beschrieben</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

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
   <td> <p>Neu: [!UICONTROL Standard]</p> 
   oder
   <p>Aktuell: [!UICONTROL Work] oder höher</p> </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anzeigen und Bearbeiten von Informationen auf einer Story-Kachel

{{step1-to-team}}

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Symbol Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Kanban-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Zum Kanban[!UICONTROL Board ].
1. Erweitern Sie die Kachel Story , um alle mit der Story verbundenen Felder anzuzeigen.

   ![](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. (Optional) Um ein Feld zu bearbeiten, klicken Sie auf das Feld und nehmen Sie dann Änderungen vor.
Sie müssen über [!UICONTROL Bearbeiten]-Rechte für die Aufgabe oder das Problem verfügen, um die Story-Kachel bearbeiten zu können.
Weitere Informationen zu den einzelnen Feldern und dazu, ob sie bearbeitet werden können, finden Sie unter [Informationen, die angezeigt und bearbeitet werden können](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>Um den [!UICONTROL Prozent abgeschlossen] zu ändern, müssen Sie eine Zahl zwischen 0 und 100 eingeben. Das Feld ist kein Schieberegler, den Sie verschieben können.
