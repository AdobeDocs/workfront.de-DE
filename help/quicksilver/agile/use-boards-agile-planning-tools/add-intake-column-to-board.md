---
content-type: overview
product-area: agile-and-teams
navigation-topic: agile-navigation-topic
title: Hinzufügen einer Aufnahmespalte zu einer Pinnwand
description: Sie können optional eine Aufnahmespalte zu Ihrer Pinnwand hinzufügen, die Aufgaben und Probleme automatisch als verbundene Karten einfügt, wenn sie in Workfront hinzugefügt werden. Dies erfolgt auf der Grundlage der von Ihnen definierten Filter.
author: Lisa
feature: Agile
exl-id: 4991f4f7-6f3d-4e15-ae8d-96433ed46557
source-git-commit: 070bc906d7ca0729697cf9def08416b00e691fc8
workflow-type: tm+mt
source-wordcount: '984'
ht-degree: 0%

---

# Hinzufügen einer Aufnahmespalte zu einer Pinnwand

Sie können optional eine Aufnahmespalte zu Ihrer Pinnwand hinzufügen, die Aufgaben und Probleme automatisch als verbundene Karten einzieht, wenn sie in [!DNL Workfront], basierend auf von Ihnen definierten Filtern. Die Ansauspalte kann als Rückstau für ein Kanban-Team dienen, als Aufnahmeort für ein Support-Team, um Probleme zu sehen, wenn sie einer Anfragewarteschlange hinzugefügt werden, oder zu einem anderen Zweck, den Sie benötigen.

Auf einer Pinnwand ist nur eine Aufnahmespalte erlaubt, und sie erscheint immer als ganz links liegende Spalte.

Die Ansaugspalte ist auf einer dynamischen Pinnwand nicht verfügbar.

Die Aufnahmespalte ist nicht auf Pinnwänden verfügbar, die Teil eines Workflows sind. Stattdessen können Sie eine Rückstandsspalte einrichten, um Karten aus der Kartenliste abzurufen. Weitere Informationen zum Hinzufügen einer Spalte mit dem Rückstand zu einer Pinnwand in einem Workstream finden Sie unter [Konfigurieren des Rückstands auf einer Arbeitsfläche](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-backlog-workstream-board.md).

Die Ansauspalte ist auf 300 Aufgaben und 300 Probleme beschränkt. Die Standardreihenfolge der Elemente in der Ansaugluft-Spalte lautet wie folgt:

Aufgaben:

* Primäre Reihenfolge: Projektname
* Sekundäre Reihenfolge: Struktur der Arbeitsaufschlüsselung

Probleme:

* Primäre Reihenfolge: Projektname
* Sekundäre Reihenfolge: Referenznummer

Weitere Informationen zu Spalten finden Sie unter [Pinnwandspalten verwalten](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). Informationen zu verbundenen Karten finden Sie unter [Angeschlossene Karten auf Pinnwänden verwenden](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

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
   <td> <p>[!DNL Request] oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Ansauspalte mit einfachen Filtern erstellen

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **[!UICONTROL Pinnwände]**.
1. Öffnen Sie eine Pinnwand. Weitere Informationen finden Sie unter [Pinnwand erstellen oder bearbeiten](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicks **[!UICONTROL Konfigurieren]** auf der rechten Seite der Pinnwand, um den Bereich Konfigurieren zu öffnen.
1. Erweitern **[!UICONTROL Board]**.
1. Aktivieren **[!UICONTROL Dynamische Aufnahme von Elementen an Bord]**.

   ![Einzugsspalten - einfache Filteroptionen](assets/intake-column-simple-filters.png)

   Die Ansaugspalte wird auf der linken Seite der Pinnwand hinzugefügt. Sie bleibt leer, bis Sie Filter darauf anwenden.

1. (Optional) Suchen Sie nach und wählen Sie [!DNL Workfront] [!UICONTROL **Projekte**].
1. (Optional) Suchen Sie nach Benutzern oder Teams und wählen Sie sie aus. [!UICONTROL **Zuweisungen**].
1. Auswählen [!UICONTROL **Fertiggestellte Arbeit einschließen**] , um Aufgaben und Probleme mit dem Status Fertig stellen in der Spalte Aufnahme anzuzeigen.

   >[!NOTE]
   >
   >Wenn diese Option nicht ausgewählt ist und Karten in anderen Status als vollständig markiert sind, werden sie auf der Pinnwand &quot;abfallen&quot;und nicht mehr angezeigt.

1. Klicks [!UICONTROL **Anwenden**].

   Alle Objekte werden in der Spalte für die Aufnahme der Pinnwand als verbundene Karten angezeigt.

   ![Aufnahmespalte](assets/intake-column-added3.png)

## Erstellen einer Annahmespalte mit erweiterten Filtern

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **[!UICONTROL Pinnwände]**.
1. Öffnen Sie eine Pinnwand. Weitere Informationen finden Sie unter [Pinnwand erstellen oder bearbeiten](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicks **[!UICONTROL Konfigurieren]** auf der rechten Seite der Pinnwand, um den Bereich Konfigurieren zu öffnen.
1. Erweitern **[!UICONTROL Board]**.
1. Aktivieren **[!UICONTROL Dynamische Aufnahme von Elementen an Bord]**.

   Die Ansaugspalte wird auf der linken Seite der Pinnwand hinzugefügt. Sie bleibt leer, bis Sie Filter darauf anwenden.

1. Klicks [!UICONTROL **Erweiterte Filter verwenden**].
1. Klicks **[!UICONTROL Hinzufügen von Filterquellen]** und wählen **[!UICONTROL Aufgaben]** oder **[!UICONTROL Probleme]**.

   ![Erweiterte Filteroptionen für Spalten aufnehmen](assets/intake-column-advanced-filters1.png)

   >[!NOTE]
   >
   >Sie können die Aufnahmespalte filtern, um sowohl Aufgaben als auch Probleme einzuschließen. Sie müssen die Filter jedoch für jeden Objekttyp separat einrichten.
   >
   >Außerdem können Sie gespeicherte Filter und Systemstandardfilter auswählen.

1. Klicken Sie im Filterbereich auf **[!UICONTROL Neuer Filter]** um zu beginnen.

   ![Klicken Sie auf Neuen Filter](assets/intake-filter-dialog5.png)

1. Erstellen Sie Ihren Filter und klicken Sie auf **[!UICONTROL Als neu speichern]**.

   ![Filter Builder](assets/intake-filter-dialog6.png)

   Dieses Beispiel zeigt einen Filter für Aufgaben aus einem bestimmten Projekt, die sich im Status von [!UICONTROL Neu] oder [!UICONTROL In Bearbeitung]und werden mir zugewiesen.

   Weitere Informationen zum Erstellen eines Filters finden Sie im Artikel unter &quot;Erstellen oder Bearbeiten eines Filters im Standard-Builder&quot;im Abschnitt [Erstellen und Bearbeiten von Filtern in [!DNL Adobe Workfront]](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

1. Benennen Sie den Filter und klicken Sie auf **[!UICONTROL Speichern]**.

   ![Geben Sie einen Namen für den Filter ein](assets/intake-filter-dialog7.png)

   Wenn Sie dem Filter einen eindeutigen Namen geben, können Sie später danach suchen.

1. Der Filter wird in der Liste der gespeicherten Filter angezeigt und automatisch auf die Ansauspalte angewendet. Klicken Sie auf das X oben im Filterbereich, um es zu schließen.

   ![Gespeicherter Filter](assets/intake-filter-dialog8.png)

1. (Optional) Um den Filter für andere freizugeben, halten Sie den Mauszeiger über den gespeicherten Filter und klicken Sie auf **[!UICONTROL Mehr]** Menü ![Weitere Menüsymbole](assets/more-icon-spectrum.png)und wählen Sie **[!UICONTROL Freigeben]**. Wählen Sie im Feld Freigabe filtern die Benutzer oder Teams aus, für die Sie eine Freigabe vornehmen möchten. Weitere Informationen finden Sie unter [Filter, Ansichten oder Gruppierungen freigeben](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).
1. (Optional) Um sowohl Aufgaben als auch Probleme in die Ansauspalte aufzunehmen, klicken Sie auf **[!UICONTROL Quellen filtern]** und wählen Sie das andere Objekt aus, um einen weiteren Filter zu erstellen.
1. Wenn Sie mit dem Hinzufügen von Filtern fertig sind, überprüfen Sie in der Spalte Aufnahme , ob die richtigen Aufgaben und Probleme angezeigt werden.

   ![Aufnahmespalte](assets/intake-column-added3.png)

   >[!NOTE]
   >
   >Sie können die Filter jederzeit aktualisieren, indem Sie das Fenster &quot;Konfigurieren&quot;öffnen und auf **[!UICONTROL Quellen filtern]** und wählen Sie **[!UICONTROL Aufgaben]** oder **[!UICONTROL Probleme]**.

## Annahmespalte verwenden

Die Karten in der Annahmespalte können erst bearbeitet werden, wenn Sie sie in andere Pinnwandspalten verschieben. Sie können auf die Karte klicken, um sie in einer schreibgeschützten Ansicht zu öffnen, oder auf ![Aufgabe oder Problem öffnen](assets/boards-launch-icon.png) , um die Aufgabe oder das Problem in einer neuen Browser-Registerkarte zu öffnen.


Sie können die Elemente in der Annahmespalte manuell neu anordnen.

Die Symbole oben rechts in der Aufnahmespalte zeigen an, wie viele Karten sich derzeit in der Spalte befinden und wie viele Filter angewendet werden.

1. (Optional) Klicken Sie auf , um in der Ansaugluft nach einem Element zu suchen. ![Suchsymbol](assets/search-icon.png) in der Spalte ein.
1. (Optional) Um eine Karte aus der Ansauspalte in eine andere Spalte zu verschieben, ziehen Sie die Karte an die gewünschte Position.

   Oder

   Klicken Sie auf **[!UICONTROL Mehr]** Menü ![Weitere Menüsymbole](assets/more-icon-spectrum.png) auf der Karte und wählen Sie **[!UICONTROL Verschieben]**. Klicken Sie anschließend auf die **[!UICONTROL Element verschieben]** auswählen, eine andere Spalte auswählen und **[!UICONTROL Verschieben]**.

1. (Optional) Klicken Sie zum Löschen der Annahmespalte auf die **[!UICONTROL Mehr]** Menü ![Weitere Menüsymbole](assets/more-icon-spectrum.png) und wählen **[!UICONTROL Löschen]**.
