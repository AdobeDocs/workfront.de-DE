---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Karte aus einer Pinnwand löschen oder archivieren
description: Wenn Sie eine Karte aus einer Pinnwand löschen, wird sie dauerhaft gelöscht und kann nicht wiederhergestellt werden. Durch die Archivierung einer Karte wird diese an das Archiv gesendet und Sie können sie später wieder auf der Pinnwand speichern.
author: Lisa
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: 46099e6ceba4310453743c023823e8952f5ce553
workflow-type: tm+mt
source-wordcount: '505'
ht-degree: 0%

---

# Karte aus einer Pinnwand löschen oder archivieren

Wenn Sie eine Ad-hoc-Karte aus einer Pinnwand löschen, wird sie dauerhaft gelöscht und kann nicht wiederhergestellt werden. Verbundene Karten können nach dem Löschen manuell zu einer Pinnwand hinzugefügt werden.

Wenn Sie eine verbundene Karte aus einer dynamischen Pinnwand löschen, wird sie bei der Aktualisierung der Pinnwand wieder angezeigt, da dieser Pinnwandtyp alle Aufgaben und Probleme aus einem bestimmten Projekt einbezieht. Um die Karte zu löschen, müssen Sie die verbundene Aufgabe oder das Problem aus dem Workfront-Projekt löschen.

Wenn Sie eine verbundene Karte aus einem anderen Pinnwandtyp löschen, der über eine Ansauspalte verfügt, wird die Karte bei der Aktualisierung der Pinnwand wieder in der Ansauspalte angezeigt, wenn die verbundene Aufgabe oder das Problem noch nicht als abgeschlossen markiert wurde. Weitere Informationen zu Aufnahmespalten finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

Durch die Archivierung einer Karte wird diese an das Archiv gesendet und Sie können sie später wieder auf der Pinnwand speichern.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Anforderung] oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Löschen einer Karte aus einer Pinnwand

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Pinnwände]**.
1. Öffnen Sie eine Pinnwand. Weitere Informationen finden Sie unter [Pinnwand erstellen oder bearbeiten](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü ![Mehr Menü](assets/more-icon-spectrum.png) auf der Karte und wählen Sie **[!UICONTROL Löschen]**.
1. Klicks **[!UICONTROL Löschen]** in der Bestätigungsnachricht angezeigt.

## Karte aus einer Pinnwand archivieren

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü ![Mehr Menü](assets/more-icon-spectrum.png) auf der Karte und wählen Sie **[!UICONTROL Archivieren]**.

   Archivierte Karten werden auf der Pinnwand ausgeblendet, es sei denn, Sie wenden einen Filter an, um sie anzuzeigen. Weitere Informationen finden Sie unter [Filtern einer Pinnwand, um archivierte Karten anzuzeigen](#filter-a-board-to-show-archived-cards) in diesem Artikel.

   Ein [!UICONTROL Archivieren] icon ![Archivieren](assets/archive-icon-spectrum-25x20.png) wird auf archivierten Karten angezeigt. Sie können eine archivierte Karte nicht bearbeiten, sie jedoch löschen oder in eine andere Spalte verschieben.

1. Um eine archivierte Karte wiederherzustellen, klicken Sie auf die Schaltfläche **[!UICONTROL Mehr]** Menü ![Mehr Menü](assets/more-icon-spectrum.png) auf der Karte und wählen Sie **[!UICONTROL Wiederherstellen]**.

## Filtern einer Pinnwand, um archivierte Karten anzuzeigen {#filter-a-board-to-show-archived-cards}

Standardmäßig werden nur aktive Karten auf einer Pinnwand angezeigt. Sie können die Pinnwand filtern, um auch alle archivierten Karten anzuzeigen.

1. Rufen Sie die Pinnwand auf.
1. Klicks [!UICONTROL **Konfigurieren**] auf der rechten Seite der Pinnwand, um den Bereich Konfigurieren zu öffnen.
1. Erweitern [!UICONTROL **Karten**].
1. Aktivieren [!UICONTROL **Archivierte Karten auf der Pinnwand anzeigen**].
1. Klicks [!UICONTROL **Filter**], erweitern Sie die [!UICONTROL Archivierte Karten] und wählen Sie **[!UICONTROL Archivierte Karten]** , um alle archivierten Karten anzuzeigen.

   Der Filter zeigt die Anzahl der archivierten Karten an.

   ![Archivierte Karten filtern](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >Die [!UICONTROL Archivierte Karten] ist im Filter nicht verfügbar, wenn Sie die Konfigurationseinstellung zur Anzeige archivierter Karten nicht aktiviert haben. Weitere Informationen finden Sie unter [Anpassen der angezeigten Felder auf einer Karte](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Auswählen **[!UICONTROL Archivierte Karten]** erneut, um die Option zu löschen und nur aktive Karten anzuzeigen.
