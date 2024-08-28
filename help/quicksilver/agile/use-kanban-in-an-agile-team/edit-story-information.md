---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Bearbeiten von Story-Informationen
description: Beim Anzeigen einer Story-Kachel auf der Kanban-Pinnwand stehen bestimmte Informationen zur Inline-Bearbeitung zur Verfügung, direkt über die Story-Kachel.
author: Lisa
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: 452f8ddc5268a0d67e32090d166199f2fad7dbc7
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 0%

---

# Bearbeiten von Storeninformationen

## Informationen darüber, welche Informationen angezeigt und bearbeitet werden können {#understand-what-information-can-be-viewed-and-edited}

Bei der Anzeige eines Story-Bausteins auf der [!UICONTROL Kanban]-Pinnwand sind die Informationen in der folgenden Tabelle verfügbar. Sie können die meisten Informationen inline bearbeiten, direkt über den Bereich &quot;Geschichte&quot;.

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
   <td> <p>Der Projektname mit einem Link direkt zum Projekt</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Die Anzahl der Punkte oder Stunden, die für die Meldung vollständig sind, und die Anzahl der Punkte oder Stunden, die der Meldung zugeordnet sind<br>Diese Zahlen werden verwendet, um die Prozentzahl der Vollständigkeit für jede Meldung zu berechnen und anzuzeigen.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Prozentualer Abschluss] für jede Geschichte und jedes Thema.<br>[!UICONTROL Der prozentuale Abschluss] für die Iteration wird basierend auf dem [!UICONTROL Prozentwert für jeden Artikel berechnet.<br></p> <p>Bei der Aktualisierung von [!UICONTROL Prozent Vollständigkeit] für eine Meldung oder ein Problem können Sie eine beliebige Zahl zwischen 0 und 100 wählen.</p> </td> 
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
   <td> <p>Alle zusätzlichen Felder (einschließlich benutzerdefinierter Felder), die möglicherweise zur agilen Ansicht hinzugefügt wurden, indem die agile Ansicht geändert wurde, wie unter "Erstellen und Anpassen einer Agile-Ansicht"in <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Übersicht über Ansichten in [!DNL Adobe Workfront]</a> beschrieben.</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

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
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p> 
   oder
   <p>Aktuell: [!UICONTROL Arbeit] oder höher</p> </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anzeigen und Bearbeiten von Informationen zu einem Story-Baustein

{{step1-to-team}}

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Kanban-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Gehen Sie zur [!UICONTROL Kanban]-Pinnwand.
1. Erweitern Sie die Kachel &quot;Geschichte&quot;, um alle Felder anzuzeigen, die mit der Geschichte verbunden sind.

   ![](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. (Optional) Um ein Feld zu bearbeiten, klicken Sie auf das Feld und nehmen Sie dann alle Änderungen vor.
Sie müssen über die Berechtigung [!UICONTROL Bearbeiten] für die Aufgabe oder das Problem verfügen, um die Kachel &quot;Geschichte&quot;bearbeiten zu können.
Weitere Informationen zu den einzelnen Feldern und dazu, ob sie bearbeitet werden können, finden Sie unter [Informationen darüber, welche Informationen angezeigt und bearbeitet werden können](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>Um den [!UICONTROL Prozentsatz abgeschlossen] zu ändern, müssen Sie eine Zahl zwischen 0 und 100 eingeben. Das Feld ist kein Schieberegler, den Sie verschieben können.
