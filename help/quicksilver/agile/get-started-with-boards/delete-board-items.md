---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Löschen oder Archivieren einer Karte aus einer Pinnwand
description: Wenn Sie eine Karte aus einer Pinnwand löschen, wird sie dauerhaft gelöscht und kann nicht wiederhergestellt werden. Durch die Archivierung einer Karte wird diese an das Archiv gesendet und Sie können sie später wieder auf der Pinnwand speichern.
author: Lisa
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: 81e87793905fd925db00c7a0ac107150263a1365
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# Karte aus einer Pinnwand löschen oder archivieren

Wenn Sie eine Ad-hoc-Karte aus einer Pinnwand löschen, wird sie dauerhaft gelöscht und kann nicht wiederhergestellt werden. Verbundene Karten können nach dem Löschen manuell zu einer Pinnwand hinzugefügt werden.

Wenn Sie eine verbundene Karte aus einer dynamischen Pinnwand löschen, wird sie bei der Aktualisierung der Pinnwand wieder angezeigt, da dieser Pinnwandtyp alle Aufgaben und Probleme aus einem bestimmten Projekt einbezieht. Um die Karte zu löschen, müssen Sie die verbundene Aufgabe oder das Problem aus dem Workfront-Projekt löschen.

Wenn Sie eine verbundene Karte aus einem anderen Pinnwandtyp löschen, der über eine Ansauspalte verfügt, wird die Karte bei der Aktualisierung der Pinnwand wieder in der Ansauspalte angezeigt, wenn die verbundene Aufgabe oder das Problem noch nicht als abgeschlossen markiert wurde. Weitere Informationen zu Aufnahmespalten finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

Durch die Archivierung einer Karte wird diese an das Archiv gesendet und Sie können sie später wieder auf der Pinnwand speichern.

Archivierte Karten werden nicht mit Workfront-Aufgaben und -Problemen synchronisiert. Wenn Sie eine Karte wiederherstellen, wird sie erneut synchronisiert.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> 
   <p>Neu: [!UICONTROL Contributor] oder höher</p> 
   <p>oder</p>
   <p>Aktuell: [!UICONTROL Anforderung] oder höher</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Löschen einer Karte aus einer Pinnwand

{{step1-to-boards}}

1. Öffnen Sie eine Pinnwand. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten einer Pinnwand](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** ![Mehr Menü](assets/more-icon-spectrum.png) auf der Karte und wählen Sie **[!UICONTROL Löschen]**.
1. Klicken Sie in der Bestätigungsmeldung auf **[!UICONTROL Löschen]** .

## Karte aus einer Pinnwand archivieren

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** ![Mehr Menü](assets/more-icon-spectrum.png) auf der Karte und wählen Sie **[!UICONTROL Archivieren]**.

   Archivierte Karten werden auf der Pinnwand ausgeblendet, es sei denn, Sie wenden einen Filter an, um sie anzuzeigen. Weitere Informationen finden Sie unter [Filtern einer Pinnwand, um archivierte Karten anzuzeigen](#filter-a-board-to-show-archived-cards) in diesem Artikel.

   Ein [!UICONTROL Archiv] -Symbol ![Archiv](assets/archive-icon-spectrum-25x20.png) wird auf archivierten Karten angezeigt. Sie können eine archivierte Karte nicht bearbeiten, sie jedoch löschen oder in eine andere Spalte verschieben.

1. Um eine archivierte Karte wiederherzustellen, klicken Sie auf das Menü **[!UICONTROL Mehr]** Menü ![Mehr Menü](assets/more-icon-spectrum.png) auf der Karte und wählen Sie **[!UICONTROL Wiederherstellen]**.

## Filtern einer Pinnwand, um archivierte Karten anzuzeigen

Standardmäßig werden nur aktive Karten auf einer Pinnwand angezeigt. Sie können die Pinnwand filtern, um auch alle archivierten Karten anzuzeigen.

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie rechts auf der Pinnwand auf [!UICONTROL **Konfigurieren**] , um den Bereich &quot;Konfigurieren&quot;zu öffnen.
1. Erweitern Sie [!UICONTROL **Karten**].
1. Aktivieren Sie [!UICONTROL **Archivierte Karten auf der Pinnwand anzeigen**].
1. Klicken Sie auf [!UICONTROL **Filter**], erweitern Sie den Abschnitt [!UICONTROL Archivierte Karten] und wählen Sie **[!UICONTROL Archivierte Karten]** aus, um alle archivierten Karten anzuzeigen.

   Der Filter zeigt die Anzahl der archivierten Karten an.

   ![Archivierte Karten filtern](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >Der Abschnitt [!UICONTROL Archivierte Karten] ist im Filter nicht verfügbar, wenn Sie die Konfigurationseinstellung zur Anzeige archivierter Karten nicht aktiviert haben. Weitere Informationen finden Sie unter [Anpassen, welche Felder auf einer Karte angezeigt werden](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Wählen Sie erneut **[!UICONTROL Archivierte Karten]** aus, um die Option zu löschen und nur aktive Karten anzuzeigen.
