---
title: Konfigurieren einer Tabellenspalte auf der Reporting-Arbeitsfläche
description: Konfigurieren einer Tabellenspalte auf der Reporting-Arbeitsfläche
hidefromtoc: true
hide: true
exl-id: ce33888f-344d-4f69-b527-9679340d134b
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 2%

---

# Konfigurieren einer Tabellenspalte auf der Reporting-Arbeitsfläche

Die Spalten in einer Tabelle können zur Anzeige konfiguriert werden. Sie können die folgenden Aspekte einer Spalte ändern:

* Name
* Sortierung
* Berechtigung bearbeiten
* Hover-Text
* Aggregation
* Bedingte Formatierung

## Voraussetzungen

Bevor Sie beginnen, müssen Sie sich für die Betaversion der Reporting-Arbeitsfläche registrieren. Weitere Informationen finden Sie unter [Reporting-Arbeitsfläche - Betaversion: Übersicht](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## Ändern von Spalten in einer Tabelle

1. Um zu einem vorhandenen Bericht zu wechseln, klicken Sie auf das Symbol **Mehr Menü** Symbol ![Mehr](assets/more-icon.png) in der Berichtskopfzeile und wählen Sie dann **Bearbeiten**.
1. Klicken Sie in der Tabellenkopfzeile im Bericht auf das Symbol **Bearbeiten** ![Symbol Bearbeiten](assets/edit-icon.png).

   ![Bearbeitungssymbol in der Tabellenkopfzeile](assets/edit-icon-table-header-350x71.png)

   >[!NOTE]
   >
   >Wenn Sie die Tabelle gerade erstellt und noch keine Felder hinzugefügt haben, klicken Sie stattdessen auf die Schaltfläche Bearbeiten in der Mitte der Tabelle.

1. (Optional) Hinzufügen, Neupositionieren oder Löschen von Spalten in der Tabelle. Weitere Informationen zum Bearbeiten der Felder in einer Tabelle finden Sie unter [Hinzufügen oder Bearbeiten eines Tabellenblocks auf der Reporting-Arbeitsfläche](../../../reports-and-dashboards/reporting-canvas/table-blocks/add-or-edit-report-table.md)

   | Neue Spalte hinzufügen | Um eine Spalte zu einer Tabelle hinzuzufügen, klicken Sie entweder auf ein Feld im Bedienfeld **Felder** auf der rechten Seite der Seite und ziehen es in die Tabelle, in der Sie es platzieren möchten, oder doppelklicken Sie auf ein Feld, um es als ganz rechts liegende Spalte hinzuzufügen. |
   |---|---|
   | Spalte verschieben | Um die Spaltenreihenfolge in einer Tabelle zu ändern, klicken Sie auf einen Spaltennamen und ziehen Sie ihn an eine neue Position. |
   | Spalte löschen | Um eine Spalte aus einer Tabelle zu löschen, klicken Sie auf die Spalte, die Sie löschen möchten, und klicken Sie dann rechts neben dem Spaltennamen auf das x. |

   {style="table-layout:auto"}

1. Um eine Spalte zu konfigurieren, klicken Sie auf den Namen der Spalte, die Sie ändern möchten, in der Kopfzeile der Tabelle und dann auf eine der folgenden Registerkarten im rechten Bedienfeld:

   <table style="table-layout:auto"> 
    <col> class=„TableStyle-TableStyle-List-options-in-step-Column-Column1“ /&gt;
    <tbody>
     <tr data-mc-conditions="">
      <th role="rowheader" colspan="2">Registerkarte „Daten“</th>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Durchschnitt basierend auf</td>
      <td><p> Um die Informationen in einer Spalte zu aggregieren (in der Kopfzeile zusammenzufassen), wählen Sie im Dropdown-Menü <strong>Aggregat basierend</strong> den gewünschten Aggregationstyp aus. Die verfügbaren Optionen hängen vom Typ der in der Spalte enthaltenen Daten ab.</p><p>Wenn Sie in der Tabelle Gruppen verwenden, wird der aggregierte Wert in der Gruppenzeile über dem Spaltennamen und nicht neben dem Spaltennamen angezeigt.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Feldformat</td>
      <td><p>(Nur verfügbar, wenn die Spalte Datums-, Prozent-, Währungs- oder Zeitdaten enthält, keinen Text.) Wählen Sie in der Dropdown-Liste <b>Feldformat“ das </b> für die Daten aus. Sie können beispielsweise Prozentzeichen nach den Zahlen in einer Spalte anzeigen oder die Anzeige von Datumsangaben ändern.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">Feld ist bearbeitbar</td>
      <td><span>Aktivieren Sie <strong>Feld kann bearbeitet werden</strong> wenn Sie Benutzern, die die Tabelle anzeigen, erlauben möchten, den Namen der Spalte zu bearbeiten.</span></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Sortieren</strong></td>
      <td><p>Standardmäßig wird die Tabelle anhand der Daten in der Spalte ganz links in aufsteigender Reihenfolge sortiert. Um stattdessen nach der ausgewählten Spalte zu sortieren, klicken Sie auf den Abwärtspfeil neben <strong>Sortieren</strong> und aktivieren Sie dann das Kontrollkästchen <b>Sortieren nach dieser Spalte</b>. Sie können dann eine <strong>Sortierrichtung</strong> (aufsteigende oder absteigende Werte) und eine <strong>Sortierreihenfolge</strong> (die relative Sortierpriorität dieser Spalte im Vergleich zu anderen Sortierspalten in der Tabelle) auswählen.</p><p>Sie können diesen Vorgang wiederholen, um die Tabelle nach bis zu fünf verschiedenen Spalten zu sortieren. Stellen Sie sicher, dass jede Spalte die richtige <strong>Sortierreihenfolge</strong> relativ zu allen neuen Spalten aufweist, die Sie für die Sortierung auswählen.</p><p>Hinweis: Wenn Sie eine Spalte löschen, die zum Sortieren einer Tabelle ausgewählt ist, und eine andere Spalte ebenfalls zum Sortieren ausgewählt ist, wird diese Spalte verwendet, um die Tabelle statt in absteigender Reihenfolge zu sortieren. Wenn keine anderen Spalten für die Sortierung ausgewählt sind, kehrt die Tabelle zum Standardwert zurück: Sortierung nach der ersten Spalte.</p><p>Wenn Sie eine Spalte zum Sortieren der Tabelle angeben, wird neben dem Spaltennamen ein kleines Feld mit einer Zahl angezeigt, die die relative Priorität der Spalte beim Sortieren der Tabelle angibt (die Tabelle wird zuerst nach 1, dann nach 2 usw. sortiert), und einem Pfeil, um anzugeben, ob die Sortierrichtung auf- oder absteigend ist. </p><p><img src="assets/sorting-indicator-350x170.png" style="width: 350;height: 170;"></p></td>
     </tr>
    </tbody>
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <th role="rowheader" colspan="2">Registerkarte „Stil“</th> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Benutzerdefinierte Spaltenbeschriftung</strong> </td> 
      <td>Geben Sie einen neuen Anzeigenamen für die Spalte ein (maximal 100 Zeichen).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hover-Text anzeigen</td> 
      <td> <p>Legen Sie fest, ob erklärender Text angezeigt werden soll, wenn jemand den Mauszeiger über einen Spaltennamen bewegt.</p> <p>Diese Option ist standardmäßig deaktiviert.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hover-Text</td> 
      <td>(Nur verfügbar, wenn <strong>Hover-Text anzeigen</strong> aktiviert ist.) Passen Sie den erklärenden Text an, der angezeigt wird, wenn jemand den Mauszeiger über einen Spaltennamen bewegt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Bedingte Formatierung</strong> </td> 
      <td> 
       <ol data-mc-continue="false"> 
        <li value="1"> <p>Fügen Sie <img src="assets/add-rule.png"> hinzu, bearbeiten Sie <img src="assets/edit-icon.png"> oder löschen Sie <img src="assets/delete.png"> einer Regel, die Zellen in der Spalte formatiert, wenn ihre Werte die von Ihnen angegebenen Kriterien erfüllen.</p> <p>Sie können beispielsweise eine Regel erstellen, die die Schriftart im Feld „Projektstatus“ in Fett-Lila ändert, wenn der Wert dieses Felds „Gebäude“ lautet.</p> <p>Sie können auch <b>Symbol anzeigen</b> verwenden, um jedem Element in der Spalte mit dem Status „Aktuell“ ein grünes Markierungssymbol hinzuzufügen.</p> <p> <img src="assets/conditional-formatting-options.png"> </p> <p>Hinweis: Wenn Sie <strong>Symbol anzeigen</strong> verwenden, sind die anderen Formatierungsoptionen nicht verfügbar.</p> <p>Sie können <strong>Auf die gesamte Zeile anwenden</strong> auswählen, wenn sich die Formatierung auf die gesamte Zeile einer Zelle auswirken soll, die die Bedingung Ihrer Regel erfüllt. Sie können beispielsweise Projekte hervorheben, die nach einem bestimmten Datum fällig sind, indem Sie eine gelbe Hintergrundfarbe nicht nur auf die Datumszellen in der Spalte „Fällig am“ anwenden, sondern auf die gesamte Zeile, in der diese Daten auftreten.</p> <p>Tipp: Wenn Sie einer Regel Formatierungsoptionen hinzufügen, wird das daraus resultierende Zellenformat unter <strong>Vorschau</strong> am unteren Rand des Bedienfelds angezeigt.</p> </li> 
        <li value="2">Wenn Sie mit dem Hinzufügen einer Regel fertig sind, klicken Sie auf <strong>Speichern</strong>.</li> 
        <li value="3"> <p>(Optional) Klicken Sie auf <b>+ Regel hinzufügen</b>, um derselben Spalte zusätzliche Regeln hinzuzufügen.</p> <p>Mehrere bedingte Formatierungsregeln in einer Tabelle werden in der folgenden Reihenfolge angewendet:</p> 
         <ul> 
          <li> <p>Regeln, die für ganze Zeilen gelten, werden zuerst von links nach rechts für jede Spalte und dann von oben nach unten innerhalb einer Spalte ausgewertet.</p> <p>Hinweis: Die Zeilenformatierung überschreibt andere bedingte Formatierungen für Zellen in dieser Zeile, auch wenn diese ansonsten die Bedingung der Regel einer anderen Spalte erfüllen würden.</p> </li> 
          <li> <p>Als Nächstes werden andere Regeln von oben nach unten ausgewertet, da sie im rechten Bedienfeld für eine Spalte aufgeführt werden. Sie können <img src="assets/drag-object-icon.png"> gespeicherten Regeln in dieses Bedienfeld ziehen, um ihre Reihenfolge zu ändern.</p> <p>Hinweis: Zellen werden basierend auf der ersten Bedingung, die sie erfüllen, formatiert. Sie werden auch dann nicht weiter formatiert, wenn sie andere Bedingungen erfüllen.</p> </li> 
         </ul> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Pfeil „Zurück** in der oberen linken Ecke des Bildschirms, um zu Ihrem Bericht zurückzukehren.
