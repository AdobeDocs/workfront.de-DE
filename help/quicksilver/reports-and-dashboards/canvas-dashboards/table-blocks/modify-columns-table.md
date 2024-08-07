---
title: Konfigurieren einer Tabellenspalte auf der Berichtsarbeitsfläche
description: Konfigurieren einer Tabellenspalte auf der Berichtsarbeitsfläche
hidefromtoc: true
hide: true
exl-id: ce33888f-344d-4f69-b527-9679340d134b
source-git-commit: 535e9c8481ce0781ee0d35636bb6d56de4d1e102
workflow-type: tm+mt
source-wordcount: '1043'
ht-degree: 2%

---

# Konfigurieren einer Tabellenspalte auf der Berichtsarbeitsfläche

Die Spalten einer Tabelle können für die Anzeige konfiguriert werden. Sie können die folgenden Aspekte einer Spalte ändern:

* Name
* Sortierung
* Berechtigung bearbeiten
* Hover-Text
* Aggregation
* Bedingte Formatierung

## Voraussetzungen

Bevor Sie beginnen, müssen Sie sich in der Beta-Version der Reporting-Arbeitsfläche anmelden. Weitere Informationen finden Sie unter [Arbeitsfläche für die Berichterstellung Beta: Übersicht](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Spalten in einer Tabelle ändern

1. Wechseln Sie zu einem vorhandenen Bericht, klicken Sie auf das Symbol **Mehr Menü** ![](assets/more-icon.png) im Berichtkopf und wählen Sie dann **Bearbeiten** aus.
1. Klicken Sie in der Tabellenüberschrift im Bericht auf das Symbol **Bearbeiten** ![](assets/edit-icon.png).

   ![](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Wenn Sie die Tabelle gerade erstellt haben und noch keine Felder hinzugefügt haben, klicken Sie stattdessen in der Tabellenmitte auf die Schaltfläche Bearbeiten .

1. (Optional) Fügen Sie Spalten in der Tabelle hinzu, positionieren Sie sie oder löschen Sie sie. Weitere Informationen zum Bearbeiten der Felder in einer Tabelle finden Sie unter [Hinzufügen oder Bearbeiten eines Tabellenblocks in der Berichtsarbeitsfläche](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md)

   | Neue Spalte hinzufügen | Um einer Tabelle eine Spalte hinzuzufügen, klicken Sie auf ein Feld und ziehen Sie es aus dem Bedienfeld **Felder** rechts auf der Seite auf die Tabelle, in der es platziert werden soll, oder doppelklicken Sie auf ein Feld, um es als ganz rechts liegende Spalte hinzuzufügen. |
   |---|---|
   | Verschieben einer Spalte | Um die Reihenfolge der Spalten in einer Tabelle neu anzuordnen, klicken Sie auf einen Spaltennamen und ziehen Sie ihn an eine neue Position. |
   | Spalte löschen | Um eine Spalte aus einer Tabelle zu löschen, klicken Sie auf die Spalte, die Sie löschen möchten, und dann auf das x rechts neben dem Spaltennamen. |

   {style="table-layout:auto"}

1. Um eine Spalte zu konfigurieren, klicken Sie in der Kopfzeile der Tabelle auf den Namen der Spalte, die Sie ändern möchten, und dann auf eine der folgenden Registerkarten im rechten Bereich:

   <table style="table-layout:auto"> 
    <col> class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" /&gt;
    <tbody>
     <tr data-mc-conditions="">
      <th role="rowheader" colspan="2">Daten-Tab</th>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Durchschnitt basierend auf</td>
      <td><p> Um die Informationen in einer Spalte zu aggregieren (in der Kopfzeile zusammenfassen), wählen Sie den Aggregattyp aus dem Dropdownmenü <strong>Aggregat basierend auf </strong> aus. Die verfügbaren Optionen hängen vom Datentyp der Spalte ab.</p><p>Wenn Sie Gruppen in der Tabelle verwenden, wird der aggregierte Wert in der Gruppenzeile über dem Spaltennamen und nicht neben dem Spaltennamen angezeigt.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Feldformat</td>
      <td><p>(Nur verfügbar, wenn die Spalte Daten zu Datum, Prozent, Währung oder Uhrzeit enthält, nicht Text.) Wählen Sie in der Dropdown-Liste <b>Feldformat</b> das gewünschte Format für die Daten aus. Beispielsweise können Sie Prozentzeichen nach den Zahlen in einer Spalte anzeigen oder die Anzeige von Datumsangaben ändern.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Feld ist bearbeitbar</td>
      <td><span>Aktivieren Sie das Feld "<strong>Feld ist bearbeitbar</strong>", wenn Sie Benutzern, die die Tabelle anzeigen, erlauben möchten, den Namen der Spalte zu bearbeiten.</span></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Sortieren</strong></td>
      <td><p>Standardmäßig wird die Tabelle nach den Daten in der Spalte ganz links in aufsteigender Reihenfolge sortiert. Um stattdessen nach der ausgewählten Spalte zu sortieren, klicken Sie auf den Abwärtspfeil neben <strong>Sortieren</strong> und dann auf das Kontrollkästchen <b>Nach dieser Spalte sortieren</b>. Anschließend können Sie eine Richtung vom Typ <strong>Sortierung</strong> (aufsteigende oder absteigende Werte) und eine Sortierreihenfolge vom Typ <strong>Sortierreihenfolge</strong> auswählen (die relative Sortierpriorität dieser Spalte im Vergleich zu anderen Sortierungsspalten in der Tabelle).</p><p>Sie können diesen Vorgang wiederholen, um die Tabelle nach bis zu fünf verschiedenen Spalten zu sortieren. Stellen Sie sicher, dass jede Spalte die richtige <strong>Sortierreihenfolge</strong> im Verhältnis zu allen neuen Spalten aufweist, die Sie zum Sortieren auswählen.</p><p>Hinweis: Wenn Sie eine Spalte löschen, die zum Sortieren einer Tabelle ausgewählt wurde, und eine andere Spalte auch zum Sortieren ausgewählt ist, wird die Tabelle in dieser Spalte in absteigender Reihenfolge sortiert. Wenn keine anderen Spalten für die Sortierung ausgewählt sind, wird die Standardtabelle zurückgegeben: Sortieren nach der ersten Spalte.</p><p>Wenn Sie eine Spalte zum Sortieren der Tabelle bestimmen, wird neben dem Spaltennamen ein kleines Feld angezeigt, das die relative Priorität der Spalte bei der Sortierung der Tabelle angibt (die Tabelle wird zuerst nach 1, dann nach 2 usw. sortiert), sowie einen Pfeil, der angibt, ob die Sortierrichtung aufsteigend oder absteigend ist. </p><p><img src="assets/sorting-indicator-350x170.png" style="width: 350;height: 170;"></p></td>
     </tr>
    </tbody>
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <th role="rowheader" colspan="2">Registerkarte "Stil"</th> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Eigene Spaltenbezeichnung</strong> </td> 
      <td>Geben Sie einen neuen Anzeigenamen für die Spalte ein (maximal 100 Zeichen).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hover-Text anzeigen</td> 
      <td> <p>Bestimmen Sie, ob erläuternder Text angezeigt werden soll, wenn der Mauszeiger über einen Spaltennamen bewegt wird.</p> <p>Diese Option ist standardmäßig deaktiviert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hover-Text</td> 
      <td>(Nur verfügbar, wenn <strong>Hover-Text anzeigen</strong> aktiviert ist.) Passen Sie den erläuternden Text an, der angezeigt wird, wenn der Mauszeiger über einen Spaltennamen bewegt wird.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong> Bedingte Formatierung</strong> </td> 
      <td> 
       <ol data-mc-continue="false"> 
        <li value="1"> <p>Fügen Sie <img src="assets/add-rule.png"> hinzu, bearbeiten Sie <img src="assets/edit-icon.png"> oder löschen Sie <img src="assets/delete.png"> eine Regel, die Zellen in der Spalte formatiert, wenn ihre Werte die von Ihnen angegebenen Kriterien erfüllen.</p> <p>Sie können beispielsweise eine Regel erstellen, die die Schrift im Feld "Projektstatus"in "violett"ändert, wenn der Wert dieses Felds gleich "Gebäude"ist.</p> <p>Alternativ können Sie <b>Symbol anzeigen</b> verwenden, um jedem Element in der Spalte, das den Status "Aktuell"aufweist, ein grünes Flag-Symbol hinzuzufügen.</p> <p> <img src="assets/conditional-formatting-options.png"> </p> <p>Hinweis: Wenn Sie <strong>Symbol anzeigen</strong> verwenden, sind die anderen Formatierungsoptionen nicht verfügbar.</p> <p>Sie können <strong>Auf die gesamte Zeile anwenden</strong> auswählen, wenn sich die Formatierung auf die gesamte Zeile einer Zelle auswirken soll, die die Bedingung Ihrer Regel erfüllt. Sie können beispielsweise Projekte hervorheben, die nach einem bestimmten Datum anstehen, indem Sie eine gelbe Hintergrundfarbe nicht nur auf die Datumszellen in der Spalte "Fällig am"anwenden, sondern auf die gesamte Zeile, in der diese Datumsangaben vorkommen.</p> <p>Tipp: Wenn Sie einer Regel Formatierungsoptionen hinzufügen, wird das daraus resultierende Zellenformat unter <strong>Vorschau</strong> am unteren Rand des Bedienfelds angezeigt.</p> </li> 
        <li value="2">Wenn Sie mit dem Hinzufügen einer Regel fertig sind, klicken Sie auf <strong>Speichern</strong>.</li> 
        <li value="3"> <p>(Optional) Klicken Sie auf <b>+ Regel hinzufügen</b> , um derselben Spalte weitere Regeln hinzuzufügen.</p> <p>Mehrere bedingte Formatierungsregeln in einer Tabelle werden in der folgenden Reihenfolge angewendet:</p> 
         <ul> 
          <li> <p>Regeln, die für ganze Zeilen gelten, werden zuerst von links nach rechts für jede Spalte und dann von oben nach unten in einer Spalte ausgewertet.</p> <p>Hinweis: Die Zeilenformatierung setzt andere bedingte Formatierungen für Zellen in dieser Zeile außer Kraft, selbst wenn sie sonst die Bedingung einer anderen Spaltenregel erfüllen würden.</p> </li> 
          <li> <p>Andere Regeln werden als Nächstes von oben nach unten ausgewertet, da sie im rechten Bereich für eine Spalte aufgeführt sind. Sie können <img src="assets/drag-object-icon.png"> gespeicherte Regeln in dieses Bedienfeld ziehen, um deren Reihenfolge zu ändern.</p> <p>Hinweis: Zellen werden basierend auf der ersten Bedingung, die sie erfüllen, formatiert und auch dann nicht weiter formatiert, wenn sie andere Bedingungen erfüllen.</p> </li> 
         </ul> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie oben links im Bildschirm auf den Pfeil **Zurück** , um zu Ihrem Bericht zurückzukehren.
