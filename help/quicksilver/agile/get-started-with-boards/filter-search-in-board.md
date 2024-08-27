---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Filtern und Suchen in einer Pinnwand
description: Sie können eine Pinnwand so filtern, dass nur bestimmte Karten angezeigt werden.
author: Lisa
feature: Agile
exl-id: 26abce82-dcd9-4865-96f4-c710f7f0a0d8
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 0%

---

# Filtern und Suchen in einer Pinnwand

Sie können eine Pinnwand filtern, um Folgendes anzuzeigen:

* Karten, die bestimmten Personen zugewiesen wurden
* Karten mit bestimmten Tags
* Karten mit einem bestimmten Status
* Karten, die in einem bestimmten Zeitrahmen fällig sind
* Archivierte Karten
* Karten, die mit einem bestimmten Projekt verbunden sind

Durch Sortieren der Pinnwand werden alle Karten in den Spalten sortiert. Eine einzelne Spalte kann nicht sortiert werden und der Rückstand oder die Annahmespalte sind nicht sortiert.

Die Suche hilft Ihnen auch, eine bestimmte Karte auf der Pinnwand zu finden.

Wenn Filter angewendet werden, wird auf der Pinnwand ![Auf Pinnwand angewendeter Filter](assets/boards-filterapplied-30x30.png) ein Indikator angezeigt. Klicken Sie auf **[!UICONTROL Alle löschen]** , um alle Filter aus der Pinnwand zu entfernen, und klicken Sie auf das Symbol &quot;Reduzieren&quot;, um den Filterbereich zu schließen.

![Filterbereich](assets/boards-all-filters-collapsed-0823.png)

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

## Pinnwand nach Bevollmächtigten filtern

{{step1-to-boards}}

1. Öffnen Sie eine Pinnwand. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten einer Pinnwand](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicken Sie auf [!UICONTROL **Filter**], erweitern Sie den Abschnitt [!UICONTROL Mitglieder] und wählen Sie die Person(en) aus, deren Karten Sie sehen möchten. Sie können auch nicht zugewiesene Karten anzeigen.

   ![Filtern nach Mitglied](assets/boards-filter-by-assignees-0822.png)

## Pinnwand nach Tags filtern

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf [!UICONTROL **Filter**], erweitern Sie den Abschnitt [!UICONTROL Tags] und wählen Sie die Tags aus, die angezeigt werden sollen.

   ![Filtern nach Tag](assets/boards-filter-by-tags-0822.png)

## Pinnwand nach Status filtern

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf [!UICONTROL **Filter**], erweitern Sie den Abschnitt [!UICONTROL Status] und wählen Sie die Statustypen aus, die angezeigt werden sollen.

   Sie können auch abgeschlossene Karten ausblenden.

   ![Filtern nach Status](assets/boards-filter-by-status-0822.png)

## Pinnwand nach Fälligkeitsdatum filtern

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf [!UICONTROL **Filter**], erweitern Sie den Abschnitt [!UICONTROL Fälligkeitsdatum] und wählen Sie die Datumsoptionen aus, die angezeigt werden sollen.

   Es werden nur Karten aus den ausgewählten Datumsbereichen angezeigt.

   ![Nach Fälligkeitsdatum filtern](assets/boards-filter-by-due-date-0822.png)

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

## Pinnwand nach Verbindung filtern

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf [!UICONTROL **Filter**], erweitern Sie den Abschnitt [!UICONTROL Verbindung] und wählen Sie die [!DNL Workfront] Projekte für die verbundenen Karten aus, die Sie sehen möchten.

   Sie können auch Karten anzeigen, die nicht mit einem Projekt verbunden sind.

   ![Nach Verbindung filtern](assets/boards-filter-by-connection.png)

## Auf Pinnwand sortieren

Wenn Sie eine Sortieroption auswählen, werden alle Spalten sortiert. Eine einzelne Spalte kann nicht sortiert werden und der Rückstand oder die Annahmespalte sind nicht sortiert.

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf &quot;[!UICONTROL **Sortieren nach**]&quot;und wählen Sie &quot;[!UICONTROL **Name**]&quot;, &quot;[!UICONTROL **Fälligkeitsdatum**]&quot;, &quot;[!UICONTROL **Schätzung**]&quot;, &quot;[!UICONTROL **Status**]&quot;oder &quot;[!UICONTROL **Verbindung**]&quot;.

   Die Verbindung (Projektname) gilt nur für verbundene Karten. Die anderen Optionen sortieren sowohl verbundene als auch Ad-hoc-Karten in den Spalten.

   Die Option &quot;Benutzerreihenfolge&quot;gibt die Karten in der Reihenfolge zurück, in der sie manuell festgelegt wurden, bevor andere Sortieroptionen angewendet wurden. Dies ist die Standardsortierung für die Spalten.

1. Wählen Sie [!UICONTROL **Reihenfolge umkehren**] aus, um die Spalten in umgekehrter Reihenfolge der Sortieroption zu sortieren.

   Der Pfeil auf dem Sortiersymbol gibt an, ob die Spalten in auf- oder absteigender Reihenfolge sortiert werden.

   Wenn eine andere Sortierung als die Standardsortierung angewendet wird, wird auf dem Sortiersymbol ![Angewandte Sortierung](assets/sort-applied-boards.png) ein Indikator angezeigt.

   ![Sortieren nach Spalten auf einer Pinnwand](assets/sort-by-columns-in-board.png)

## Durchsuchen einer Pinnwand

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf [!UICONTROL **Suchen**] und geben Sie einen Suchbegriff ein. Drücken Sie dann die Eingabetaste.

   Alle Karten, die den Suchbegriff enthalten, werden angezeigt.

   Klicken Sie auf das X, um die Suche zu löschen.

   ![Suche nach Karten in einer Pinnwand](assets/boards-searchbox.png)
