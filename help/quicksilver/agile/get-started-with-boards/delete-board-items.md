---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Löschen oder Archivieren einer Karte von einer Pinnwand
description: Wenn Sie eine Karte von einer Pinnwand löschen, wird sie dauerhaft gelöscht und kann nicht wiederhergestellt werden. Wenn Sie eine Karte archivieren, wird sie an das Archiv gesendet und Sie können sie später auf der Pinnwand wiederherstellen.
author: Lisa
feature: Agile
exl-id: 68b7d2e5-92f0-462d-8122-eaecb1e6b87c
source-git-commit: 81e87793905fd925db00c7a0ac107150263a1365
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 0%

---

# Löschen oder Archivieren einer Karte von einer Pinnwand

Wenn Sie eine Ad-hoc-Karte von einer Pinnwand löschen, wird sie dauerhaft gelöscht und kann nicht wiederhergestellt werden. Verbundene Karten können nach dem Löschen manuell wieder zu einer Pinnwand hinzugefügt werden.

Wenn Sie eine verbundene Karte von einer dynamischen Pinnwand löschen, wird sie beim Aktualisieren der Pinnwand erneut angezeigt, da dieser Pinnwand-Typ alle Aufgaben und Probleme aus einem bestimmten Projekt abruft. Um die Karte zu löschen, müssen Sie die damit verbundene Aufgabe oder Anfrage aus dem Workfront-Projekt löschen.

Wenn Sie eine verbundene Karte aus einem anderen Pinnwand-Typ löschen, der über eine Aufnahmespalte verfügt, wird die Karte erneut in der Aufnahmespalte angezeigt, wenn Sie die Pinnwand aktualisieren, falls die verbundene Aufgabe oder das verbundene Problem noch nicht als „abgeschlossen“ markiert ist. Weitere Informationen zu Aufnahmespalten finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

Wenn Sie eine Karte archivieren, wird sie an das Archiv gesendet und Sie können sie später auf der Pinnwand wiederherstellen.

Archivierte Karten werden nicht mit Workfront-Aufgaben und -Problemen synchronisiert. Wenn Sie eine Karte wiederherstellen, wird sie erneut synchronisiert.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> 
   <p>Neu: [!UICONTROL Contributor] oder höher</p> 
   <p>oder</p>
   <p>Aktuell: [!UICONTROL-Anfrage] oder höher</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Löschen einer Karte von einer Pinnwand

{{step1-to-boards}}

1. Zugriff auf eine Pinnwand. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten einer Pinnwand](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicken Sie auf das **[!UICONTROL Mehr]**-Menü ![Mehr](assets/more-icon-spectrum.png) auf der Karte und wählen Sie **[!UICONTROL Löschen]**.
1. Klicken **[!UICONTROL auf]** Bestätigungsmeldung.

## Archivieren einer Karte von einer Pinnwand

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf das **[!UICONTROL Mehr]**-Menü ![Mehr](assets/more-icon-spectrum.png) auf der Karte und wählen Sie **[!UICONTROL Archivieren]**.

   Archivierte Karten werden auf der Pinnwand ausgeblendet, es sei denn, Sie wenden einen Filter an, um sie anzuzeigen. Weitere Informationen finden Sie unter [Pinnwand filtern, um archivierte Karten anzuzeigen](#filter-a-board-to-show-archived-cards) in diesem Artikel.

   Ein [!UICONTROL Archiv]-Symbol ![Archiv](assets/archive-icon-spectrum-25x20.png) wird auf archivierten Karten angezeigt. Eine archivierte Karte kann nicht bearbeitet, aber gelöscht oder in eine andere Spalte verschoben werden.

1. Um eine archivierte Karte wiederherzustellen, klicken Sie auf das **[!UICONTROL Mehr]** Menü ![Mehr](assets/more-icon-spectrum.png) auf der Karte und wählen Sie **[!UICONTROL Wiederherstellen]**.

## Pinnwand filtern, um archivierte Karten anzuzeigen

Standardmäßig werden nur aktive Karten auf einer Pinnwand angezeigt. Sie können die Pinnwand so filtern, dass auch archivierte Karten angezeigt werden.

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie [!UICONTROL **rechts auf**] Pinnwand auf „Konfigurieren“, um das Bedienfeld „Konfigurieren“ zu öffnen.
1. Erweitern Sie [!UICONTROL **Karten**].
1. Schalten Sie [!UICONTROL **Anzeige archivierter Karten auf der Pinnwand**] ein.
1. Klicken Sie [!UICONTROL **Filtern**] erweitern Sie den Abschnitt [!UICONTROL Archivierte Karten] und wählen Sie **[!UICONTROL Archivierte Karten]** aus, um alle archivierten Karten anzuzeigen.

   Der Filter zeigt die Anzahl der archivierten Karten an.

   ![Archivierte Karten filtern](assets/filter-by-archived-cards.png)

   >[!NOTE]
   >
   >Der Abschnitt [!UICONTROL Archivierte Karten] ist im Filter nicht verfügbar, wenn Sie die Konfigurationseinstellung zur Anzeige archivierter Karten nicht aktiviert haben. Weitere Informationen finden Sie unter [Anpassen der auf einer Karte angezeigten Felder](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Wählen Sie **[!UICONTROL Archivierte Karten]** erneut aus, um die Option zu deaktivieren und nur aktive Karten anzuzeigen.
