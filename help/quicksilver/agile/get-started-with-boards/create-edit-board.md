---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Pinnwand erstellen oder bearbeiten
description: Im Dashboard [!UICONTROL Pinnwände] können Sie eine neue Pinnwand erstellen oder eine vorhandene Pinnwand bearbeiten.
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: 0c0c1f538cfd12e18c504fcb42ee424789d1cde8
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 1%

---

# Pinnwand erstellen oder bearbeiten

<!-- Audited: 12/2023 -->

Im Dashboard [!UICONTROL Pinnwände] können Sie eine neue Pinnwand erstellen oder eine vorhandene Pinnwand bearbeiten.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: Mitarbeiter oder höher </p>
 <p>oder</p> 
<p>Aktuell: [!UICONTROL Anforderung] oder höher </p> 
</td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Neue Pinnwand erstellen

{{step1-to-boards}}

1. Klicken Sie auf **[!UICONTROL Pinnwand hinzufügen]**.

1. Wählen Sie eine Vorlage für die Pinnwand aus.

   | Vorlage | Beschreibung |
   |---------|----------|
   | Einfache Pinnwand | Auf der Pinnwand werden drei Standardspalten bereitgestellt. Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen. <p>Auf der Pinnwand werden drei Standardspalten bereitgestellt. Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen. |
   | Kanban-Board | Die folgenden Spalten werden auf der Pinnwand bereitgestellt: &quot;Backlog&quot;, &quot;Neu&quot;, &quot;In Bearbeitung&quot;, &quot;Abgeschlossen&quot;und &quot;Auf Warten&quot;. Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen.<p>Um den Rückstand zu verwenden, müssen Sie Filter für die Ansauspalte einrichten. Weitere Informationen finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Um die Standardrichtlinien für jede Spalte zu überprüfen, klicken Sie auf das Menü [!UICONTROL **Mehr**] in einer Spalte und wählen Sie [!UICONTROL **Bearbeiten**] aus. Sie können diese voreingestellten Richtlinien ändern. Weitere Informationen finden Sie unter [Pinnwandspalten verwalten](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | Retrospektiv-Board | Die folgenden Spalten werden auf der Pinnwand bereitgestellt: Was ist gut gelaufen? Was könnte verbessert werden? Wen sollten wir feiern? Was können wir tun, um schneller zu handeln? Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen. <p>Es werden keine Spaltenrichtlinien angewendet. |
   | Dynamische Pinnwand | Die folgenden Spalten werden auf der Pinnwand bereitgestellt: &quot;Nicht ausgewählt&quot;, &quot;Neu&quot;, &quot;In Bearbeitung&quot;, &quot;Nicht gedrückt&quot;und &quot;Fertig gestellt&quot;. Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen. (Die Spalte Nicht ausgewählt kann umbenannt, aber nicht gelöscht werden. Diese Spalte enthält alle Karten mit einem Status, der keinem der anderen Spaltenstatus entspricht.) <p>Die standardmäßigen Spaltenrichtlinien weisen Spalten basierend auf ihrem Status Karten zu. Weitere Informationen finden Sie unter [Pinnwandspalten verwalten](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

1. Führen Sie die Schritte des Einrichtungsassistenten nur für eine dynamische Pinnwand aus:

   1. Geben Sie einen Namen für die Pinnwand ein und klicken Sie auf [!UICONTROL **Weiter**].
   1. Suchen Sie nach und wählen Sie [!DNL Workfront] [!UICONTROL **Projekte**] aus, um Aufgaben und Probleme auf die Pinnwand zu übertragen.
   1. Suchen Sie nach und wählen Sie [!UICONTROL **Zuweisungen**] aus, um Aufgaben und Probleme auf die Pinnwand zu übertragen.

      Alle Objekte werden auf der Pinnwand als verbundene Karten angezeigt.

      Der Zähler [!UICONTROL **Karten, die hinzugefügt werden**] gibt an, wie viele Karten auf der Pinnwand vorhanden sein werden. Wenn Sie beispielsweise ein Projekt mit 100 Aufgaben und Problemen auswählen, zeigt der Zähler 100 an. Wenn Sie eine Benutzerzuweisung hinzufügen und diese Person fünf Aufgaben im Projekt zugewiesen ist, zeigt der Zähler 5 an.

      >[!NOTE]
      >
      >Die maximale Kartenanzahl für dynamische Pinnwände beträgt 700 Aufgaben und 700 Probleme, für insgesamt 1.400 Karten. Eine hohe Anzahl von Karten auf der Pinnwand kann die Leistung der Pinnwand beeinflussen. Alle archivierten Karten, sowohl ausgeblendet als auch sichtbar, zählen zu dieser Grenze.

   1. (Optional) Wählen Sie [!UICONTROL **Nicht abgeschlossene Karten archivieren**] aus, um abgeschlossene Aufgaben und Probleme als sichtbare Karten in der Spalte &quot;Abgeschlossen&quot;auf die Pinnwand zu bringen. Wenn diese Option nicht ausgewählt ist, werden abgeschlossene Karten zum Zeitpunkt der Pinnwanderstellung als archivierte Karten auf die Pinnwand gebracht.

      >[!NOTE]
      >
      >Standardmäßig werden archivierte Karten nicht auf der Pinnwand angezeigt. Um archivierte Karten anzuzeigen, müssen Sie eine Konfigurationseinstellung aktivieren und dann die Pinnwand filtern, um archivierte Karten anzuzeigen. Weitere Informationen finden Sie unter [Anpassen, welche Felder auf einer Karte angezeigt werden](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md) und [Filtern und Suchen in einer Pinnwand](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

   1. (Optional) Klicken Sie auf [!UICONTROL **Erweiterte Filter verwenden**] , um weitere Filteroptionen anzuzeigen.

      Dies entspricht dem Erstellen eines Filters für eine Annahmespalte. Weitere Informationen finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

      Wenn Sie die Filter auf einer dynamischen Pinnwand aktualisieren, nachdem sie erstellt wurde, werden Karteneinstellungen zurückgesetzt, die nicht Teil der Workfront-Aufgabe oder des Problems sind (z. B. Tags).

   1. Klicken Sie nach dem Hinzufügen der Filter auf [!UICONTROL **Pinnwand erstellen**].

1. Geben Sie im Feld **[!UICONTROL Pinnwand]** einen Namen für die Pinnwand ein und drücken Sie die Eingabetaste.
1. Konfigurieren Sie die Pinnwand nach Bedarf.

   Weitere Informationen finden Sie unter [Hinzufügen oder Entfernen von Mitgliedern aus einer Pinnwand](../../agile/get-started-with-boards/add-members-to-board.md), [Verwalten von Pinnwandspalten](../../agile/get-started-with-boards/manage-board-columns.md), [Hinzufügen einer Ad-hoc-Karte zu einer Pinnwand](../../agile/get-started-with-boards/add-card-to-board.md) und [Verwenden Sie verbundene Karten auf Pinnwänden](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. Klicken Sie auf **[!UICONTROL Alle Pinnwände]** , um zum Dashboard der Pinnwände zurückzukehren.

   Sie können auch das mit dem Namen der aktuellen Pinnwand beschriftete Dropdown-Menü suchen und darauf klicken, um zu einer anderen Pinnwand zu wechseln.

   ![Liste der Pinnwände](assets/boards-button-list-of-boards-350x188.png)

## Vorhandene Pinnwand bearbeiten

{{step1-to-boards}}

1. Wählen Sie im Dashboard die zu öffnende Pinnwand aus.
1. Bearbeiten Sie die Pinnwand nach Bedarf. Sie können auf den Pinnwandnamen klicken, um ihn umzubenennen.

   Um verbundene Karten mit Workfront zu synchronisieren und neue Aufgaben und Probleme auf die Pinnwand oder die Ansauspalte zu übertragen, klicken Sie auf das Menü **[!UICONTROL Mehr]** Menü ![[!UICONTROL Mehr Menü]](assets/more-icon-spectrum.png) neben dem Pinnwandnamen und wählen Sie **[!UICONTROL Verknüpfte Elemente synchronisieren]**.

   Weitere Informationen finden Sie unter [Hinzufügen oder Entfernen von Mitgliedern aus einer Pinnwand](../../agile/get-started-with-boards/add-members-to-board.md), [Verwalten von Pinnwandspalten](../../agile/get-started-with-boards/manage-board-columns.md) und [Hinzufügen einer Karte zu einer Pinnwand](../../agile/get-started-with-boards/add-card-to-board.md).

1. Klicken Sie auf **[!UICONTROL Alle Pinnwände]** , um zum Dashboard der Pinnwände zurückzukehren.

   Sie können auch das mit dem Namen der aktuellen Pinnwand beschriftete Dropdown-Menü suchen und darauf klicken, um zu einer anderen Pinnwand zu wechseln.

