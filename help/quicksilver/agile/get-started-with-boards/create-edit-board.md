---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Pinnwand erstellen oder bearbeiten
description: Aus dem [!UICONTROL Pinnwände] Dashboard können Sie eine neue Pinnwand erstellen oder eine vorhandene Pinnwand bearbeiten.
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: 5e73603b695ff7456216ca7a4e15ce527b01559d
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 3%

---

# Pinnwand erstellen oder bearbeiten

Aus dem [!UICONTROL Pinnwände] Dashboard können Sie eine neue Pinnwand erstellen oder eine vorhandene Pinnwand bearbeiten.

Informationen zum Hinzufügen einer Pinnwand zu einem Workstream finden Sie unter [Workflows verwalten](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

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
   <td> <p>[!UICONTROL Anforderung] oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Neue Pinnwand erstellen

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Pinnwände]**.
1. Um eine eigenständige Pinnwand zu erstellen, klicken Sie auf **[!UICONTROL Pinnwand hinzufügen]** im [!UICONTROL Pinnwände] Bereich. Informationen zum Hinzufügen einer Pinnwand zu einem Workstream finden Sie unter [Workflows verwalten](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

1. Wählen Sie eine Vorlage für die Pinnwand aus.

   | Vorlage | Beschreibung |
   |---------|----------|
   | Einfache Pinnwand | Auf der Pinnwand werden drei Standardspalten bereitgestellt. Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen. <p>Auf der Pinnwand werden drei Standardspalten bereitgestellt. Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen. |
   | Kanban-Board | Die folgenden Spalten werden auf der Pinnwand bereitgestellt: Rückstau, Neu, In Bearbeitung, Abgeschlossen und Auf Warten. Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen.<p>Um den Rückstand zu verwenden, müssen Sie Filter für die Ansauspalte einrichten. Weitere Informationen finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Um die Standardrichtlinien für jede Spalte zu überprüfen, klicken Sie auf die [!UICONTROL **Mehr** Menü] in einer Spalte und wählen Sie [!UICONTROL **Bearbeiten**]. Sie können diese voreingestellten Richtlinien ändern. Weitere Informationen finden Sie unter [Pinnwandspalten verwalten](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | Rückblickende Pinnwand | Die folgenden Spalten werden auf der Pinnwand bereitgestellt: Was ist gut gelaufen? Was könnte verbessert werden? Wer soll gefeiert werden? Wie können wir unsere Verfahren beschleunigen? Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen. <p>Es werden keine Spaltenrichtlinien angewendet. |
   | Dynamische Pinnwand | Die folgenden Spalten werden auf der Pinnwand bereitgestellt: Nicht ausgewählt, Neu, In Bearbeitung, Auf Halten und Abschließen. Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen. (Die Spalte Nicht ausgewählt kann umbenannt, aber nicht gelöscht werden. Diese Spalte enthält alle Karten mit einem Status, der keinem der anderen Spaltenstatus entspricht.) <p>Die standardmäßigen Spaltenrichtlinien weisen Spalten basierend auf ihrem Status Karten zu. Weitere Informationen finden Sie unter [Pinnwandspalten verwalten](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). <p>**HINWEIS:** Die dynamische Pinnwand ist nur über die frühe Funktion des Opt-ins für Workfront-Pinnwände verfügbar. |

1. Führen Sie die Schritte des Einrichtungsassistenten nur für eine dynamische Pinnwand aus:

   1. Suchen und Auswählen [!DNL Workfront] [!UICONTROL **Projekte**] , um Aufgaben und Probleme in den Vorstand zu bringen.
   1. Suchen und Auswählen [!UICONTROL **Zuweisungen**] , um Aufgaben und Probleme in den Vorstand zu bringen.

      Alle Objekte werden auf der Pinnwand als verbundene Karten angezeigt.

      Die [!UICONTROL **Hinzufügen von Karten**] Zähler zeigt an, wie viele Karten auf der Pinnwand vorhanden sein werden. Wenn Sie beispielsweise ein Projekt mit 100 Aufgaben und Problemen auswählen, zeigt der Zähler 100 an. Wenn Sie eine Benutzerzuweisung hinzufügen und diese Person fünf Aufgaben im Projekt zugewiesen ist, zeigt der Zähler 5 an.

   1. (Optional) Wählen Sie [!UICONTROL **Fertiggestellte Arbeit einschließen**] , um abgeschlossene Karten in die Pinnwand aufzunehmen.

      >[!NOTE]
      >
      >Wenn diese Option nicht ausgewählt ist und Karten in anderen Status als vollständig markiert sind, werden sie auf der Pinnwand &quot;abfallen&quot;und nicht mehr angezeigt.

   1. (Optional) Klicken Sie auf [!UICONTROL **Erweiterte Filter verwenden**] , um weitere Filteroptionen anzuzeigen.

      Dies entspricht dem Erstellen eines Filters für eine Annahmespalte. Weitere Informationen finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

   1. Klicken Sie nach dem Hinzufügen der Filter auf [!UICONTROL **Pinnwand erstellen**].

1. Geben Sie einen Namen für die Pinnwand im **[!UICONTROL Board]** und drücken Sie die Eingabetaste.
1. Konfigurieren Sie die Pinnwand nach Bedarf.

   Weitere Informationen finden Sie unter [Hinzufügen oder Entfernen von Mitgliedern aus einer Pinnwand](../../agile/get-started-with-boards/add-members-to-board.md), [Pinnwandspalten verwalten](../../agile/get-started-with-boards/manage-board-columns.md), [Hinzufügen einer Ad-hoc-Karte zu einer Pinnwand](../../agile/get-started-with-boards/add-card-to-board.md)und [Angeschlossene Karten auf Pinnwänden verwenden](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. Klicken **[!UICONTROL Alle Pinnwände]** , um zum Dashboard der Pinnwände zurückzukehren.

   Sie können auch das mit dem Namen der aktuellen Pinnwand beschriftete Dropdown-Menü suchen und darauf klicken, um zu einer anderen Pinnwand zu wechseln.

   ![Liste der Foren](assets/boards-button-list-of-boards-350x188.png)

## Vorhandene Pinnwand bearbeiten

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Pinnwände]**.
1. Wählen Sie im Dashboard die zu öffnende Pinnwand aus.
1. Bearbeiten Sie die Pinnwand nach Bedarf. Sie können auf den Pinnwandnamen klicken, um ihn umzubenennen.

   Weitere Informationen finden Sie unter [Hinzufügen oder Entfernen von Mitgliedern aus einer Pinnwand](../../agile/get-started-with-boards/add-members-to-board.md), [Pinnwandspalten verwalten](../../agile/get-started-with-boards/manage-board-columns.md)und [Hinzufügen einer Karte zu einer Pinnwand](../../agile/get-started-with-boards/add-card-to-board.md).

1. Klicken **[!UICONTROL Alle Pinnwände]** , um zum Dashboard der Pinnwände zurückzukehren.

   Sie können auch das mit dem Namen der aktuellen Pinnwand beschriftete Dropdown-Menü suchen und darauf klicken, um zu einer anderen Pinnwand zu wechseln.
