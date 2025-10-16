---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Board-Spalten verwalten
description: Eine neue Pinnwand enthält standardmäßig drei Spalten. Sie können weitere Spalten hinzufügen, die Reihenfolge der Spalten ändern, Spalten umbenennen und alle nicht benötigten Spalten löschen. Sie können auch Spaltenrichtlinien definieren.
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '1081'
ht-degree: 0%

---

# Verwalten von Pinnwandspalten

<!-- Audited: 05/2024 -->

Eine neue Pinnwand enthält standardmäßig drei Spalten. Sie können weitere Spalten hinzufügen, die Reihenfolge der Spalten ändern, Spalten umbenennen und alle nicht benötigten Spalten löschen.

Spalteneinstellungen enthalten Richtlinien, mit denen Sie festlegen können, was mit einer Karte passiert, wenn sie in diese Spalte verschoben wird.

Informationen zum Sortieren der Karten in Spalten finden Sie unter [Filtern und Suchen in einer Pinnwand](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Mitwirkender oder höher</p> 
   <p>Anfrage oder höher</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hinzufügen einer Spalte zu einer Pinnwand

{{step1-to-boards}}

1. Zugriff auf eine Pinnwand. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten einer Pinnwand](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicken Sie **[!UICONTROL Spalte hinzufügen]** rechts neben den vorhandenen Spalten.
1. Geben Sie in die neue Spalte einen Namen ein und klicken Sie auf **[!UICONTROL Spalte hinzufügen]**.

   ![Neue Spalte hinzufügen](assets/boards-add-column.png)

>[!TIP]
>
>Informationen zum Hinzufügen einer Aufnahmespalte finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Spalten auf einer Pinnwand neu anordnen

1. Rufen Sie die Pinnwand auf.
1. Ziehen Sie die Spalten in die richtige Reihenfolge. Wählen Sie den oberen Rand der Spalte aus, bevor Sie ihn an eine andere Position ziehen.

   ![Spalte per Drag-and-Drop verschieben](assets/boards-dragdropcolumn.png)

## Pinnwand-Spalte umbenennen

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf den Spaltennamen, geben Sie den neuen Namen ein und drücken Sie die Eingabetaste.

   Oder

   Klicken Sie auf das **[!UICONTROL Mehr]**-Menü ![Mehr](assets/more-icon-spectrum.png) in der Spalte und wählen Sie **[!UICONTROL Bearbeiten]**. Geben Sie im Bereich Einstellungen den neuen Namen in das Feld **[!UICONTROL Spaltenname]** ein und klicken Sie auf **[!UICONTROL Schließen]**.

## Pinnwand-Spalte löschen

Wenn Sie eine Spalte von einer Pinnwand löschen, kann sie nicht wiederhergestellt werden.

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf das **[!UICONTROL Mehr]**-Menü ![Mehr](assets/more-icon-spectrum.png) in der Spalte und wählen Sie **[!UICONTROL Löschen]**.

   >[!NOTE]
   >
   >Spalten, die Karten enthalten, einschließlich archivierter Karten, können nicht gelöscht werden. Wenn Sie versuchen, eine Spalte zu löschen, die Karten enthält, müssen Sie eine andere Spalte für diese Karten auswählen.

## Kartenanzahl anzeigen

In einer Konfigurationseinstellung können Sie die Anzahl der Karten in jeder Spalte anzeigen.

Wenn Sie die WIP-Beschränkung für eine Spalte verwenden, wird kein separater Kartenzähler hinzugefügt. Weitere Informationen zu Fertigungsbeschränkungen finden Sie unter [Verwalten der [!UICONTROL Work In Progress] (WIP) auf einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie **[!UICONTROL rechts auf]** Pinnwand auf „Konfigurieren“, um das Bedienfeld „Konfigurieren“ zu öffnen.
1. Erweitern Sie **[!UICONTROL Spalte]**.
1. Aktivieren Sie **[!UICONTROL Anzahl der Spaltenkarten anzeigen]**.

   ![Kartenzähler einschalten](assets/display-card-count.png)

   Der Kartenzähler wird oben in jeder Spalte angezeigt.

1. Klicken Sie auf **[!UICONTROL Konfigurieren ausblenden]**, um das Bedienfeld [!UICONTROL Konfigurieren] zu schließen.

## Definieren von Spalteneinstellungen und Richtlinien

Spaltenrichtlinien umfassen das automatische Aktualisieren von Feldwerten und das Festlegen eines Limits für laufende Arbeiten.

Die Richtlinie zum Aktualisieren des Status funktioniert automatisch sowohl für die Karte als auch für die Spalte:

* Wenn eine Karte in eine Spalte mit einer Richtlinie verschoben wird, wird der Kartenstatus auf den in der Richtlinie definierten Status aktualisiert. Dies gilt sowohl für Ad-hoc- als auch für verbundene Karten.
* Wenn der Status einer Ad-hoc-Karte oder einer verbundenen Karte auf der Karte aktualisiert wird, um ihn an den Spaltenstatus in der Richtlinie anzupassen, oder an einer anderen Stelle in Workfront der Status einer verbundenen Karte aktualisiert wird, wird die Karte automatisch in diese Spalte verschoben. Wenn außerdem ein benutzerdefinierter Status auf einer Karte mit dem Systemstatus übereinstimmt, der der Spalte zugewiesen wurde, wird die Karte in diese Spalte verschoben.

Eine Karte verbleibt in einer Spalte, in der sie platziert wird, wenn der Kartenstatus keinem in den Spaltenrichtlinien festgelegten Status entspricht.

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf das **[!UICONTROL Mehr]**-Menü ![Mehr](assets/more-icon-spectrum.png) in der Spalte und wählen Sie **[!UICONTROL Bearbeiten]**.

   Der Bereich [!UICONTROL Einstellungen] wird angezeigt. Der **[!UICONTROL Spaltenname]** gibt Aufschluss darüber, für welche Spalte Sie Einstellungen definieren.

1. Aktivieren Sie die Richtlinie **[!UICONTROL Feldwerte automatisch aktualisieren]**, um bestimmte Feldwerte automatisch zu ändern, wenn eine Karte in diese Spalte verschoben wird.

   ![Spalteneinstellungen und -richtlinien](assets/boards-column-policies-enabled.png)

1. (Optional) Legen Sie einen Wert für den Kartenstatus fest:

   1. Aktivieren Sie **[!UICONTROL Kontrollkästchen]** Status“.

   1. Wählen Sie den Status aus, der auf eine Karte angewendet werden soll, wenn sie in diese Spalte verschoben wird.

      ![Status für Spalten](assets/boards-column-status.png)

      Die Statusübersetzungsoptionen für verbundene Karten werden ebenfalls angezeigt. (Die Statusübersetzung gilt nicht für Ad-hoc-Karten.) Diese Optionen bestimmen den benutzerdefinierten Status, der auf die Aufgabe oder das Problem in [!DNL Workfront] angewendet wird, wenn eine verbundene Karte in diese Spalte verschoben wird.

   1. Wählen Sie [!UICONTROL **Status „Benutzerdefiniert**], um ihn auf die Karte für Aufgaben und Probleme anzuwenden.

      Wenn eine Karte in diese Spalte verschoben wird, versucht [!DNL Workfront] zunächst, den benutzerdefinierten Status anzuwenden (z. B. „Gelöst„). Wenn der ausgewählte benutzerdefinierte Status für diese Karte nicht verfügbar ist, werden Sie aufgefordert, einen anderen Status auszuwählen, der dem Systemstatus entspricht (aus Schritt b oben). Weitere Informationen zu Status finden Sie unter [Status - Übersicht](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

      Wenn der Status für die verbundene Aufgabe oder das verbundene Problem in den benutzerdefinierten oder Systemstatus geändert wird, der in der Spaltenrichtlinie festgelegt ist, wird die Karte automatisch in die Spalte verschoben.

1. (Optional) Legen Sie einen Wert für die Kartenbevollmächtigten fest:

   1. Aktivieren Sie **[!UICONTROL Kontrollkästchen]** Empfänger“.
   1. Aktion auswählen.

      * **[!UICONTROL Bei Verantwortlichen hinzufügen]:** Die von Ihnen ausgewählten Verantwortlichen werden der vorhandenen Liste der Verantwortlichen auf einer Karte hinzugefügt, wenn sie in diese Spalte verschoben wird.
      * **[!UICONTROL Empfänger überschreiben]:** Die Empfänger, die Sie auswählen, überschreiben alle anderen Empfänger und werden die einzigen Empfänger auf einer Karte, wenn sie in diese Spalte verschoben werden.

   1. Klicken Sie [!UICONTROL **Zuweisung hinzufügen**] und suchen Sie nach einem Benutzer. Wählen Sie die Verantwortlichen aus den Suchergebnissen aus. Alle Workfront-Benutzenden und -Teams können aus folgenden Optionen auswählen.

      ![Verantwortliche für Spalte](assets/boards-column-assignees.png)

1. (Optional) Legen Sie einen Wert für die Karten-Tags fest:

   1. Aktivieren Sie **[!UICONTROL Kontrollkästchen]** Karten“.
   1. Aktion auswählen.

      * **[!UICONTROL Bei Tags hinzufügen]:** Die ausgewählten Tags werden der vorhandenen Liste der Tags auf einer Karte hinzugefügt, wenn sie in diese Spalte verschoben werden.
      * **[!UICONTROL Tags überschreiben]:** Die Tags, die Sie auswählen, überschreiben alle anderen Tags und werden die einzigen Tags auf einer Karte, wenn sie in diese Spalte verschoben werden.

   1. Wählen Sie die Tags aus der Dropdown-Liste aus. Nur Tags, die bereits im [!UICONTROL Tag-Manager] erstellt wurden, stehen zur Auswahl. Informationen zum Hinzufügen neuer Tags finden Sie unter [Hinzufügen von Tags](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![Tags für Spalte](assets/boards-column-tags.png)

1. Aktivieren Sie **[!UICONTROL Richtlinie „Laufende Arbeit]**, um die Anzahl der Karten zu begrenzen, die der Spalte hinzugefügt werden können. Geben Sie dann die Zahl der Beschränkungen in das Feld **[!UICONTROL Limit festlegen]** ein.

   ![WIP-Beschränkung für Spalte](assets/boards-wip-limit-in-column.png)

   Weitere Informationen finden Sie unter [Verwalten des Grenzwerts für laufende Arbeiten (Work In Progress, WIP) auf einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Klicken Sie auf **[!UICONTROL Schließen]**, um den Bereich Einstellungen zu verlassen und die Spalte und ihre Karten anzuzeigen.
