---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Bearbeiten von Storeninformationen
description: Beim Anzeigen einer Story-Kachel auf der Kanban-Pinnwand stehen bestimmte Informationen zur Inline-Bearbeitung zur Verfügung, direkt über die Story-Kachel.
author: Lisa
feature: Agile
exl-id: a22a7b61-b331-4c98-9421-e7fccedcd096
source-git-commit: 9da0c8234f563a0202cd15017b37a341476f7406
workflow-type: tm+mt
source-wordcount: '433'
ht-degree: 0%

---

# Bearbeiten von Storeninformationen

## Informationen darüber, welche Informationen angezeigt und bearbeitet werden können {#understand-what-information-can-be-viewed-and-edited}

Beim Anzeigen einer Story-Kachel auf der [!UICONTROL Kanban] -Pinnwand, sind die Informationen in der folgenden Tabelle verfügbar. Sie können die meisten Informationen inline bearbeiten, direkt über die Kachel &quot;Geschichte&quot;.

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
   <td> <p>Der Projektname mit einem Link direkt zum Projekt</p> </td> 
   <td>✓ </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Die Anzahl der vollständigen Punkte oder Stunden der Meldung und die Anzahl der der Meldung zugewiesenen Punkte oder Stunden<br>Diese Zahlen werden verwendet, um den "Percent Complete"für jede Meldung zu berechnen und anzuzeigen.</p> </td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Prozentualer Abschluss] für jede Geschichte und jedes Thema.<br>[!UICONTROL Der prozentuale Abschluss] für die Iteration wird auf der Grundlage des [!UICONTROL Prozentsatzes abgeschlossen] für jede Geschichte berechnet.<br></p> <p>Bei der Aktualisierung von [!UICONTROL Prozent Vollständigkeit] für eine Meldung oder ein Problem können Sie eine beliebige Zahl zwischen 0 und 100 wählen.</p> </td> 
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
   <td> <p>Alle zusätzlichen Felder (einschließlich benutzerdefinierter Felder), die möglicherweise zur agilen Ansicht hinzugefügt wurden, indem die agile Ansicht geändert wurde, wie unter "Erstellen und Anpassen einer Agile-Ansicht"in <a href="../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Ansichten - Übersicht in [!DNL Adobe Workfront]</a></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
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
   <td> <p>[!UICONTROL Worker] oder höher</p> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administratoren können die Zugriffsebene ändern, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Anzeigen und Bearbeiten von Informationen zu einem Story-Baustein

1. Klicken Sie auf *[!UICONTROL *Hauptmenü]** Symbol ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Teams]**.

1. (Optional) Klicken Sie auf die **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder ein neues Kanban-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Navigieren Sie zu [!UICONTROL Kanban] Pinnwand.
1. Erweitern Sie die Kachel &quot;Geschichte&quot;, um alle Felder anzuzeigen, die mit der Geschichte verbunden sind.

   ![](assets/story-expanded-on-kanban-board-2021-350x405.png)

1. (Optional) Um ein Feld zu bearbeiten, klicken Sie auf das Feld und nehmen Sie dann alle Änderungen vor.\
   Sie müssen [!UICONTROL Bearbeiten] Berechtigungen für die Aufgabe oder das Problem, um die Story-Kachel zu bearbeiten.\
   Weitere Informationen zu den einzelnen Feldern und darüber, ob sie bearbeitet werden können, finden Sie unter [Informationen darüber, welche Informationen angezeigt und bearbeitet werden können](#understand-what-information-can-be-viewed-and-edited).

>[!NOTE]
>
>So ändern Sie die [!UICONTROL Prozent abgeschlossen], müssen Sie eine Zahl zwischen 0 und 100 eingeben. Das Feld ist kein Schieberegler, den Sie verschieben können.
