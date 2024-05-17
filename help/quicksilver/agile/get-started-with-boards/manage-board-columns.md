---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Verwalten von Pinnwandspalten
description: Eine neue Pinnwand enthält standardmäßig drei Spalten. Sie können zusätzliche Spalten hinzufügen, die Reihenfolge der Spalten ändern, Spalten umbenennen und nicht benötigte Spalten löschen. Sie können auch Spaltenrichtlinien definieren.
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 040dd446ff2b347dabf8a139feb17fd1a7d50e4e
workflow-type: tm+mt
source-wordcount: '1149'
ht-degree: 0%

---

# Verwalten von Pinnwandspalten

<!-- Audited: 05/2024 -->

Eine neue Pinnwand enthält standardmäßig drei Spalten. Sie können zusätzliche Spalten hinzufügen, die Reihenfolge der Spalten ändern, Spalten umbenennen und nicht benötigte Spalten löschen.

Die Spalteneinstellungen enthalten Richtlinien, mit denen Sie Optionen definieren können, was mit einer Karte passiert, wenn sie in diese Spalte verschoben wird.

Informationen zum Sortieren der Karten in Spalten finden Sie unter [Filtern und Suchen in einer Pinnwand](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

## Zugriffsanforderungen

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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Hinzufügen einer Spalte zu einer Pinnwand

{{step1-to-boards}}

1. Öffnen Sie eine Pinnwand. Weitere Informationen finden Sie unter [Pinnwand erstellen oder bearbeiten](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicks **[!UICONTROL Spalte hinzufügen]** rechts von den vorhandenen Spalten.
1. Geben Sie in die neue Spalte einen Namen ein und klicken Sie auf **[!UICONTROL Spalte hinzufügen]**.

   ![Neue Spalte hinzufügen](assets/boards-add-column.png)

>[!TIP]
>
>Informationen zum Hinzufügen einer Aufnahmespalte finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Neuanordnen von Spalten auf einer Pinnwand

1. Rufen Sie die Pinnwand auf.
1. Ziehen Sie die Spalten in die richtige Reihenfolge. Wählen Sie unbedingt den oberen Rand der Spalte aus, bevor Sie sie an eine andere Position ziehen.

   ![Spalte per Drag &amp; Drop verschieben](assets/boards-dragdropcolumn.png)

## Umbenennen einer Pinnwandspalte

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf den Spaltennamen, geben Sie den neuen Namen ein und drücken Sie die Eingabetaste.

   Oder

   Klicken Sie auf **[!UICONTROL Mehr]** Menü ![Mehr Menü](assets/more-icon-spectrum.png) in der Spalte und wählen Sie **[!UICONTROL Bearbeiten]**. Geben Sie im Bereich &quot;Einstellungen&quot;den neuen Namen in die **[!UICONTROL Spaltenname]** und klicken Sie auf **[!UICONTROL Schließen]**.

## Pinnwandspalte löschen

Wenn Sie eine Spalte aus einer Pinnwand löschen, kann sie nicht wiederhergestellt werden.

1. Rufen Sie die Pinnwand auf.
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü ![Mehr Menü](assets/more-icon-spectrum.png) in der Spalte und wählen Sie **[!UICONTROL Löschen]**.

   >[!NOTE]
   >
   >Spalten mit Karten, einschließlich archivierter Karten, können nicht gelöscht werden. Wenn Sie versuchen, eine Spalte zu löschen, die Karten enthält, müssen Sie eine andere Spalte für diese Karten auswählen.

## Anzahl der Karten anzeigen

Sie können eine Konfigurationseinstellung verwenden, um die Anzahl der Karten in jeder Spalte anzuzeigen.

Wenn Sie die WIP-Beschränkung für eine Spalte verwenden, wird kein separater Zähler für die Karte hinzugefügt. Weitere Informationen zu WIP-Beschränkungen finden Sie unter [Verwalten Sie die [!UICONTROL Laufende Arbeiten] (WIP)-Beschränkung auf einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Rufen Sie die Pinnwand auf.
1. Klicks **[!UICONTROL Konfigurieren]** auf der rechten Seite der Pinnwand, um den Bereich Konfigurieren zu öffnen.
1. Erweitern **[!UICONTROL Spalte]**.
1. Aktivieren **[!UICONTROL Spaltenkartenanzahl anzeigen]**.

   ![Kartenzähler einschalten](assets/display-card-count.png)

   Der Kartenzähler wird oben in jeder Spalte angezeigt.

1. Klicks **[!UICONTROL Konfigurieren ausblenden]** zum Schließen der [!UICONTROL Konfigurieren] Bedienfeld.

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
1. Klicken Sie auf **[!UICONTROL Mehr]** Menü ![Mehr Menü](assets/more-icon-spectrum.png) in der Spalte und wählen Sie **[!UICONTROL Bearbeiten]**.

   Die [!UICONTROL Einstellungen] angezeigt. Die **[!UICONTROL Spaltenname]** informiert Sie darüber, für welche Spalte Sie Einstellungen definieren.

1. Aktivieren Sie die **[!UICONTROL Automatische Aktualisierung von Feldwerten]** Richtlinie, um bestimmte Feldwerte automatisch zu ändern, wenn eine Karte in diese Spalte verschoben wird.

   ![Spalteneinstellungen und Richtlinien](assets/boards-column-policies-enabled.png)

1. (Optional) Legen Sie einen Wert für den Kartenstatus fest:

   1. Wählen Sie die **[!UICONTROL Status]** aktivieren.

   1. Wählen Sie den Status aus, der auf eine Karte angewendet werden soll, wenn sie in diese Spalte verschoben wird.

      ![Status der Spalten](assets/boards-column-status.png)

      Die Statusübersetzungsoptionen für verbundene Karten werden ebenfalls angezeigt. (Die Statusübersetzung gilt nicht für Ad-hoc-Karten.) Diese Optionen bestimmen den benutzerdefinierten Status, der auf die Aufgabe oder das Problem in [!DNL Workfront] wenn eine verbundene Karte in diese Spalte verschoben wird.

   1. Wählen Sie eine [!UICONTROL **Benutzerdefiniert**] Status, der auf die Karte für Aufgaben und Probleme angewendet wird.

      Wenn eine Karte in diese Spalte verschoben wird, [!DNL Workfront] Versuchen Sie zunächst, den benutzerdefinierten Status anzuwenden (z. B. &quot;Gelöst&quot;). Wenn der ausgewählte benutzerdefinierte Status für diese Karte nicht verfügbar ist, werden Sie aufgefordert, einen anderen Status auszuwählen, der dem Systemstatus entspricht (aus Schritt b oben). Weitere Informationen zu Status finden Sie unter [Statusübersicht](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

      Wenn der Status der verbundenen Aufgabe oder des Problems in den in der Spaltenrichtlinie festgelegten benutzerdefinierten Status oder Systemstatus geändert wird, wird die Karte automatisch in die Spalte verschoben.

1. (Optional) Legen Sie einen Wert für die Kartenverantwortlichen fest:

   1. Wählen Sie die **[!UICONTROL Zuweisung]** aktivieren.
   1. Wählen Sie eine Aktion aus.

      * **[!UICONTROL Hinzufügen zu Bevollmächtigten]:** Die von Ihnen ausgewählten Bevollmächtigten werden zur bestehenden Liste der Bevollmächtigten auf einer Karte hinzugefügt, wenn sie in diese Spalte verschoben werden.
      * **[!UICONTROL Zuweisung überschreiben]:** Die von Ihnen ausgewählten Bevollmächtigten überschreiben alle anderen Bevollmächtigten und werden zum einzigen Bevollmächtigten auf einer Karte, wenn sie in diese Spalte verschoben werden.

   1. Klicks [!UICONTROL **Zuweisung hinzufügen**] und nach einem Benutzer suchen. Wählen Sie die Bevollmächtigten aus den Suchergebnissen aus. Alle Workfront-Benutzer und -Teams können aus dieser Gruppe auswählen.

      ![Zuweisung für Spalte](assets/boards-column-assignees.png)

1. (Optional) Legen Sie einen Wert für die Karten-Tags fest:

   1. Wählen Sie die **[!UICONTROL Karten]** aktivieren.
   1. Wählen Sie eine Aktion aus.

      * **[!UICONTROL Tags hinzufügen]:** Die von Ihnen ausgewählten Tags werden der vorhandenen Liste der Tags auf einer Karte hinzugefügt, wenn sie in diese Spalte verschoben wird.
      * **[!UICONTROL Tags überschreiben]:** Die Tags, die Sie auswählen, überschreiben alle anderen Tags und werden zum einzigen Tags auf einer Karte, wenn sie in diese Spalte verschoben werden.

   1. Wählen Sie die Tags aus der Dropdownliste aus. Nur Tags, die bereits in der [!UICONTROL Tag-Manager] zur Auswahl stehen. Informationen zum Hinzufügen neuer Tags finden Sie unter [Tags hinzufügen](/help/quicksilver/agile/get-started-with-boards/add-tags.md).

      ![Tags für Spalte](assets/boards-column-tags.png)

1. Aktivieren Sie die **[!UICONTROL Laufende Arbeit]** -Richtlinie, um die Anzahl der Karten zu begrenzen, die der Spalte hinzugefügt werden können. Geben Sie dann die Begrenzungsnummer in das Feld **[!UICONTROL Begrenzung festlegen]** -Feld.

   ![WIP-Beschränkung für Spalte](assets/boards-wip-limit-in-column.png)

   Weitere Informationen finden Sie unter [Grenze für laufende Arbeit (WIP) auf einer Pinnwand verwalten](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md).

1. Klicks **[!UICONTROL Schließen]** , um den Einstellungsbereich zu verlassen und die Spalte und deren Karten anzuzeigen.
