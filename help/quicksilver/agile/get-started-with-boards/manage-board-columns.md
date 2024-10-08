---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Pinnwandspalten verwalten
description: Eine neue Pinnwand enthält standardmäßig drei Spalten. Sie können zusätzliche Spalten hinzufügen, die Reihenfolge der Spalten ändern, Spalten umbenennen und nicht benötigte Spalten löschen. Sie können auch Spaltenrichtlinien definieren.
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '1160'
ht-degree: 0%

---

# Verwalten von Pinnwandspalten

<!-- Audited: 05/2024 -->

Eine neue Pinnwand enthält standardmäßig drei Spalten. Sie können zusätzliche Spalten hinzufügen, die Reihenfolge der Spalten ändern, Spalten umbenennen und nicht benötigte Spalten löschen.

Die Spalteneinstellungen enthalten Richtlinien, mit denen Sie Optionen definieren können, was mit einer Karte passiert, wenn sie in diese Spalte verschoben wird.

Informationen zum Sortieren der Karten in Spalten finden Sie unter [Filtern und Suchen in einer Pinnwand](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

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
   <td> <p>Neu: Mitarbeiter oder höher </p>
        <p>oder</p> 
        <p>Aktuell: [!UICONTROL Anforderung] oder höher </p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hinzufügen einer Spalte zu einer Pinnwand

{{step1-to-boards}}

1. Öffnen Sie eine Pinnwand. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten einer Pinnwand](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicken Sie rechts neben den vorhandenen Spalten auf **[!UICONTROL Spalte hinzufügen]** .
1. Geben Sie in die neue Spalte einen Namen ein und klicken Sie auf **[!UICONTROL Spalte hinzufügen]**.

   ![Neue Spalte hinzufügen](assets/boards-add-column.png)

>[!TIP]
>
>Informationen zum Hinzufügen einer Ansaugsäule finden Sie unter [Hinzufügen einer Ansaugsäule zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Neuanordnen von Spalten auf einer Pinnwand

1. Rufen Sie die Pinnwand auf.
1. Ziehen Sie die Spalten in die richtige Reihenfolge. Wählen Sie unbedingt den oberen Rand der Spalte aus, bevor Sie sie an eine andere Position ziehen.

   ![Spalte per Drag-and-Drop verschieben](assets/boards-dragdropcolumn.png)

## Umbenennen einer Pinnwandspalte

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf den Spaltennamen, geben Sie den neuen Namen ein und drücken Sie die Eingabetaste.

   Oder

   Klicken Sie auf das Menü **[!UICONTROL Mehr]** ![Mehr Menü](assets/more-icon-spectrum.png) in der Spalte und wählen Sie **[!UICONTROL Bearbeiten]** aus. Geben Sie im Bereich &quot;Einstellungen&quot;den neuen Namen in das Feld **[!UICONTROL Spaltenname]** ein und klicken Sie auf **[!UICONTROL Schließen]**.

## Pinnwandspalte löschen

Wenn Sie eine Spalte aus einer Pinnwand löschen, kann sie nicht wiederhergestellt werden.

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** ![Mehr Menü](assets/more-icon-spectrum.png) in der Spalte und wählen Sie **[!UICONTROL Löschen]**.

   >[!NOTE]
   >
   >Spalten mit Karten, einschließlich archivierter Karten, können nicht gelöscht werden. Wenn Sie versuchen, eine Spalte zu löschen, die Karten enthält, müssen Sie eine andere Spalte für diese Karten auswählen.

## Anzahl der Karten anzeigen

Sie können eine Konfigurationseinstellung verwenden, um die Anzahl der Karten in jeder Spalte anzuzeigen.

Wenn Sie die WIP-Beschränkung für eine Spalte verwenden, wird kein separater Zähler für die Karte hinzugefügt. Weitere Informationen zu WIP-Beschränkungen finden Sie unter [Verwalten der Beschränkung [!UICONTROL Laufende Arbeit] (WIP) auf einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie rechts auf der Pinnwand auf **[!UICONTROL Konfigurieren]** , um den Bereich &quot;Konfigurieren&quot;zu öffnen.
1. Erweitern Sie **[!UICONTROL Spalte]**.
1. Aktivieren Sie **[!UICONTROL Spaltenkartenanzahl anzeigen]**.

   ![Schalten Sie den Kartenzähler ein](assets/display-card-count.png)

   Der Kartenzähler wird oben in jeder Spalte angezeigt.

1. Klicken Sie auf **[!UICONTROL Konfigurieren ausblenden]** , um den Bereich [!UICONTROL Konfigurieren] zu schließen.

## Spalteneinstellungen und Richtlinien definieren

Zu den Spaltenrichtlinien gehören die automatische Aktualisierung von Feldwerten und das Festlegen einer Grenze für laufende Arbeit.

Die Richtlinie zum Aktualisieren des Status funktioniert sowohl für die Karte als auch für die Spalte automatisch:

* Wenn eine Karte in eine Spalte mit einer Richtlinie verschoben wird, wird der Kartenstatus auf den in der Richtlinie definierten Status aktualisiert. Dies gilt sowohl für Ad-hoc-Karten als auch für verbundene Karten.
* Wenn der Status einer Ad-hoc-Karte oder einer verbundenen Karte auf der Karte aktualisiert wird, um dem Spaltenstatus in der Richtlinie zu entsprechen, oder ein Status einer verbundenen Karte an anderer Stelle in Workfront aktualisiert wird, wird die Karte automatisch in diese Spalte verschoben. Wenn ein benutzerdefinierter Status auf einer Karte mit dem Systemstatus übereinstimmt, der der Spalte zugewiesen ist, wird die Karte in diese Spalte verschoben.

Eine Karte verbleibt in einer Spalte, in der sie platziert wird, wenn der Kartenstatus mit keinem in bestehenden Spaltenrichtlinien festgelegten Status übereinstimmt.

>[!NOTE]
>
>Dynamische Pinnwände platzieren immer Karten in der Spalte, die ihrem Status entspricht, unabhängig davon, ob Spaltenrichtlinien aktiviert oder deaktiviert sind. Die Karten kehren bei der Aktualisierung der Pinnwand zu den zugewiesenen Spalten zurück.
> 
>Wenn Sie eine Karte für alle Pinnwandtypen von einer Spalte in eine andere mit demselben Status verschieben, kehrt die Karte bei der Aktualisierung der Pinnwand zur ursprünglichen Spalte zurück.

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf das Menü **[!UICONTROL Mehr]** ![Mehr Menü](assets/more-icon-spectrum.png) in der Spalte und wählen Sie **[!UICONTROL Bearbeiten]** aus.

   Der Bereich [!UICONTROL Einstellungen] wird angezeigt. Der **[!UICONTROL Spaltenname]** gibt an, für welche Spalte Sie Einstellungen definieren.

1. Aktivieren Sie die Richtlinie **[!UICONTROL Feldwerte automatisch aktualisieren]** , um bestimmte Feldwerte automatisch zu ändern, wenn eine Karte in diese Spalte verschoben wird.

   ![Spalteneinstellungen und Richtlinien](assets/boards-column-policies-enabled.png)

1. (Optional) Legen Sie einen Wert für den Kartenstatus fest:

   1. Aktivieren Sie das Kontrollkästchen **[!UICONTROL Status]** .

   1. Wählen Sie den Status aus, der auf eine Karte angewendet werden soll, wenn sie in diese Spalte verschoben wird.

      ![Status für Spalten](assets/boards-column-status.png)

      Die Statusübersetzungsoptionen für verbundene Karten werden ebenfalls angezeigt. (Die Statusübersetzung gilt nicht für Ad-hoc-Karten.) Diese Optionen bestimmen den benutzerdefinierten Status, der auf die Aufgabe oder das Problem in [!DNL Workfront] angewendet wird, wenn eine verbundene Karte in diese Spalte verschoben wird.

   1. Wählen Sie den Status [!UICONTROL **Benutzerdefiniert**] aus, um ihn auf die Karte für Aufgaben und Probleme anzuwenden.

      Wenn eine Karte in diese Spalte verschoben wird, versucht [!DNL Workfront] zunächst, den benutzerdefinierten Status anzuwenden (z. B. &quot;Gelöst&quot;). Wenn der ausgewählte benutzerdefinierte Status für diese Karte nicht verfügbar ist, werden Sie aufgefordert, einen anderen Status auszuwählen, der dem Systemstatus entspricht (aus Schritt b oben). Weitere Informationen zu Status finden Sie unter [Statusübersicht](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

      Wenn der Status der verbundenen Aufgabe oder des Problems in den in der Spaltenrichtlinie festgelegten benutzerdefinierten Status oder Systemstatus geändert wird, wird die Karte automatisch in die Spalte verschoben.

1. (Optional) Legen Sie einen Wert für die Kartenverantwortlichen fest:

   1. Aktivieren Sie das Kontrollkästchen **[!UICONTROL Zuweisungen]** .
   1. Wählen Sie eine Aktion aus.

      * **[!UICONTROL Auf Bevollmächtigten hinzufügen]:** Die von Ihnen ausgewählten Bevollmächtigten werden der bestehenden Liste der Bevollmächtigten auf einer Karte hinzugefügt, wenn sie in diese Spalte verschoben werden.
      * **[!UICONTROL Zuweisung überschreiben]:** Die von Ihnen ausgewählten Bevollmächtigten überschreiben alle anderen Bevollmächtigten und werden zum einzigen Bevollmächtigten auf einer Karte, wenn sie in diese Spalte verschoben werden.

   1. Klicken Sie auf [!UICONTROL **Zuweisung hinzufügen**] und suchen Sie nach einem Benutzer. Wählen Sie die Bevollmächtigten aus den Suchergebnissen aus. Alle Workfront-Benutzer und -Teams können aus dieser Gruppe auswählen.

      ![Zuweisung für Spalte](assets/boards-column-assignees.png)

1. (Optional) Legen Sie einen Wert für die Karten-Tags fest:

   1. Aktivieren Sie das Kontrollkästchen **[!UICONTROL Karten]** .
   1. Wählen Sie eine Aktion aus.

      * **[!UICONTROL Auf Tags hinzufügen]:** Die von Ihnen ausgewählten Tags werden der vorhandenen Liste der Tags auf einer Karte hinzugefügt, wenn sie in diese Spalte verschoben wird.
      * **[!UICONTROL Tags überschreiben]:** Die Tags, die Sie auswählen, überschreiben alle anderen Tags und werden die einzigen Tags auf einer Karte, wenn sie in diese Spalte verschoben werden.

   1. Wählen Sie die Tags aus der Dropdownliste aus. Es können nur Tags ausgewählt werden, die bereits im [!UICONTROL Tag-Manager] erstellt wurden. Informationen zum Hinzufügen neuer Tags finden Sie unter [Tags hinzufügen](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![Tags für Spalte](assets/boards-column-tags.png)

1. Aktivieren Sie die Richtlinie **[!UICONTROL Laufende Grenze bearbeiten]** , um die Anzahl der Karten zu begrenzen, die der Spalte hinzugefügt werden können. Geben Sie dann die Begrenzungsnummer in das Feld **[!UICONTROL Begrenzung festlegen]** ein.

   ![WIP-Limit für Spalte](assets/boards-wip-limit-in-column.png)

   Weitere Informationen finden Sie unter [Grenzwert für laufende Arbeit (WIP) auf einer Pinnwand verwalten](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Klicken Sie auf **[!UICONTROL Schließen]** , um den Einstellungsbereich zu verlassen und die Spalte und deren Karten anzuzeigen.
