---
navigation-topic: get-started-with-workfront
title: Erweiterte Listen verwenden
description: Erweiterte Listen verwenden ein Tabellenformat für die Anzeige der Listenelemente und haben ein anderes Erscheinungsbild als die Standardlisten
author: Lisa
feature: Get Started with Workfront
exl-id: 4c25ed54-b147-4fd3-8d00-6f1ba61bbd38
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 0c4904a380dd62b9ea01dd1030ee02d82a869541
workflow-type: tm+mt
source-wordcount: '2931'
ht-degree: 2%

---

# Verwenden von erweiterten Listen

Erweiterte Listen sind in einigen Bereichen von Adobe Workfront verfügbar. Diese Listen verwenden ein Tabellenformat für die Anzeige der Listenelemente und haben ein anderes Erscheinungsbild als die Standardlisten. Die Verwaltung von Ansichten wurde ebenfalls verbessert, einschließlich Filtern, Gruppieren, Verwalten von Spalten und Suchen.

Informationen zu den Standardlisten finden Sie unter [Erste Schritte mit Listen in Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

>[!NOTE]
>
>Jede erweiterte Liste kann anders konfiguriert werden, damit Sie die benötigten Daten anzeigen können. Nicht alle in diesem Artikel beschriebenen Funktionen werden in jeder Liste verwendet, und einige Listen können spezielle Funktionen enthalten, die nur für diese Liste gelten.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>
   <p>Mitwirkende oder höher</p>
   <p>Anfragende oder höher</p></td>
  </tr>
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Objekte, die erweiterte Listen verwenden

Im Folgenden finden Sie einige Typen von Workfront-Objektlisten, die das erweiterte Listenformat verwenden, sowie einige der Bereiche, in denen sie standardmäßig angezeigt werden, wenn Sie über die Berechtigung zum Anzeigen des Objekts verfügen.

>[!NOTE]
>
>Diese Liste ist nicht vollständig. Jede dieser Objektlisten kann auch in einem Bericht oder Dashboard angezeigt werden. Beispielsweise zeigt ein Anfragebericht oder ein Dashboard, das einen Anfragebericht enthält, auch eine Liste von Anfragen an.

| Workfront-Liste | Speicherort der Objektliste |
| --- | --- |
| Prioritäten | <ul><li>Startseite > Wählen Sie im linken Menü das Symbol Prioritäten aus.</li><li>Hauptmenü > Prioritäten</li></ul> |
| Liste der Anfragen | <ul><li>Anfragen (nur für neue Erlebnisse)</li><li>Widget „Meine Anfragen“ auf der Startseite</li></ul> |
| Listen mit Status, Prioritäten, Schweregraden und Wechselkursen im Setup | <ul><li>Setup > Projektvoreinstellungen > Status</li><li>Setup > Projektvoreinstellungen > Prioritäten</li><li>Setup > Projektvoreinstellungen > Schweregrade</li><li>Einrichten > Projektvoreinstellungen > Wechselkurse</li></ul> |
| Liste von Berichten | Berichte (**Freigebbare Ordner verwenden** müssen aktiviert sein) |
| Liste der Aufgabengebiete und Tarife auf einer Tarifkarte | Einrichten > Tarifkarten > Tarifkarte auswählen > Aufgabengebiete und Tarife |
| Liste der Übersetzungen | Setup > Lokalisierung |
| Liste der Momentaufnahmen | Projekt > Momentaufnahmen |
| Liste der Ressourcen für die Abrechnung | Projekt > Ressource für Abrechnung |
| Neue erweiterte Zuweisungen für eine Aufgabe | Aufgabe > Arbeitsaufträge > Erweitert |
| Dokumente zu Adobe Enterprise Storage | Projekt, Aufgabe, Problem, Portfolio, Programmvorlage > Dokumente |

## Hinzufügen von Elementen zu einer erweiterten Liste

Führen Sie je nach angezeigter erweiterter Liste eine der folgenden Aktionen aus:

1. Klicken Sie oben rechts in der Liste auf die blaue Schaltfläche. Diese Option öffnet ein Dialogfeld, in dem Sie Informationen eingeben können. Die Daten werden als neue Zeile in der Tabelle gespeichert.

   ODER

1. Klicken Sie **Neue**) unten in der Liste auf. Mit dieser Option wird der Tabelle eine neue Zeile hinzugefügt. Doppelklicken Sie in eine Zelle, um darin Informationen einzugeben. Jede Zelle stellt ein Feld für das Listenelement dar. Felder müssen vorhanden sein, bevor sie in der Liste angezeigt werden.

   Erweiterte Listen unterstützen diese Feldtypen:

   * Text
   * Zahl
   * Währung
   * Datum
   * Datum und Uhrzeit
   * Dropdown-Listen für Einzel-/Mehrfachauswahl
   * Typeahead
   * Absatz
   * Zugewiesener (ein oder mehrere)
   * Farbwähler

   >[!NOTE]
   >
   >Jeder Feldtyp verfügt über seine eigenen Bearbeitungsoptionen. Einige Felder sind möglicherweise schreibgeschützt.

![Beispiel für eine erweiterte Liste](assets/glist-exchange-rates.png)

## Elemente über die Aktionsleiste bearbeiten

Sie können die Aktionsleiste in einer erweiterten Liste verwenden, um Elemente in der Liste zu bearbeiten. Nicht alle Aktionsleisten enthalten dieselben Optionen. Außerdem können Sie in einigen Listen möglicherweise keine Elemente auswählen, und die Aktionsleiste ist nicht verfügbar.

1. Aktivieren Sie das Kontrollkästchen neben einem Element in einer erweiterten Liste.

   Die Aktionsleiste wird am unteren Bildschirmrand angezeigt.

   >[!NOTE]
   >
   >Je nachdem, welche Liste Sie bearbeiten, können Sie ein oder mehrere Elemente auswählen, um die Aktionsleiste zu verwenden.

1. Klicken Sie auf eine Aktion in der Leiste, um Elemente zu bearbeiten. Beispiele für Aktionen, die Sie auswählen können:

   * Ansicht
   * Bearbeiten
   * Löschen
   * Kopieren
   * In Ordner verschieben
   * Freigeben

   Wenn für das ausgewählte Element keine Aktionen verfügbar sind, wird in der Aktionsleiste „Keine verfügbaren Aktionen“ angezeigt.

   ![Beispiel für Aktionsleiste](assets/glist-action-bar-statuses.png)

1. Bewegen Sie den Mauszeiger über das Primärfeld eines Listenelements und klicken Sie dann auf das **Mehr** Menü ![Mehr Menüsymbol](assets/more-icon.png), um zusätzliche Aktionen anzuzeigen. Einige Aktionen sind möglicherweise spezifisch für diese Liste.

   >[!TIP]
   >
   >Das primäre Feld wird in der ersten Spalte der Liste angezeigt.

   ![Weitere Menübeispiele](assets/glist-more-menu-priorities.png)

## Spalten anpassen

Je nachdem, welche Objekte Sie in einer erweiterten Liste anzeigen, können Sie Spalten in der Liste ausblenden, anzeigen oder neu anordnen.

1. Klicken Sie **Spalten** über der Liste auf.

   ![Beispiel für Spalten anzeigen](assets/glist-display-move-columns.png)

1. Verwenden Sie die Umschalter zum Anzeigen oder Ausblenden von Spalten in der Liste.
1. Um die Spalten neu anzuordnen, klicken Sie auf das Symbol **Ziehen** (![-Symbol](assets/drag-icon.png) und verschieben Sie eine Spalte an die gewünschte Position. Durch das Verschieben von Spalten wird die Liste automatisch geändert.

   >[!NOTE]
   >
   >Das primäre Feld ist die erste Spalte in der Liste. Sie ist an der ersten Position fixiert und kann nicht geändert werden. Wenn die Anzahl der Spalten groß ist, wird das primäre Feld nach links eingefroren, und wenn Sie horizontal scrollen, wird es immer angezeigt.
   >
   >Das Symbol neben einem Feldnamen zeigt den Feldtyp an, z. B. Text oder Datumsfeld.

   Ein Indikator wird auf der Schaltfläche **Spalten** angezeigt, wenn Spalten ausgeblendet sind. Der Indikator wird bei der Neuanordnung der Spalten nicht angezeigt.

   ![Indikator für ausgeblendete Spalten](assets/glist-columns-hidden-indicator.png)

### Spalten umbenennen

Einige Spalten ermöglichen es Ihnen, einen benutzerdefinierten Namen für den Spaltentitel zu speichern.

1. Bewegen Sie den Mauszeiger über die Spalte, klicken Sie dann auf den Abwärtspfeil und wählen Sie **Umbenennen** aus.

   ![Wählen Sie Umbenennen in Spalte aus](assets/glist-rename-or-sort-column.png)

1. Geben Sie im Dialogfeld **Umbenennen** den Namen für die Spalte in das Feld **Benutzerdefinierte**) ein und klicken Sie auf **Speichern**.

   Der neue Spaltenname wird in der Liste angezeigt.

### Hinzufügen und Entfernen von Spalten mit dem Spalten-Manager

Sie können den **Spalten-Manager** in einigen erweiterten Listen verwenden, um Spalten einfach zur Liste hinzuzufügen und daraus zu entfernen. Sie können sowohl System- als auch benutzerdefinierte Felder, die bereits in Workfront als Spalten vorhanden sind, zu einer erweiterten Liste hinzufügen oder entfernen.

So fügen Sie Spalten hinzu und entfernen sie:

1. Klicken Sie oben rechts in der Tabelle auf das Symbol &quot;+&quot;, um das Feld **Spalten-Manager“** öffnen.
1. Suchen Sie in der Spalte **Verfügbar** nach einem vorhandenen Objektfeld und klicken Sie dann rechts neben dem Feldnamen auf + , um es der Spalte **Ausgewählt** hinzuzufügen.
1. Klicken Sie rechts neben einem Feld in der Spalte **Ausgewählt**, um es aus der Liste zu entfernen.

   >[!NOTE]
   >
   >Einige Felder sind möglicherweise unveränderlich und können nicht entfernt werden.

   <!-- Add info about Properties and KPIs when something gets released with those options -->

1. Klicken Sie auf **Speichern**.

   ![Spalten-Manager](assets/glist-column-manager.png)

   Die Liste aktualisiert die Spalten entsprechend den von Ihnen getroffenen Entscheidungen.

### Ändern der Zeilenhöhe in einer Ansicht

>[!NOTE]
>
>Nicht alle erweiterten Listen enthalten alle in diesem Abschnitt beschriebenen Elemente.

1. Klicken Sie auf **Symbol „Zeilenhöhe** ![ (Symbol „Zeilenhöhe](assets/row-height-icon.png) in einer erweiterten Liste.

   Dadurch wird die vertikale Länge einer Zeile aktualisiert. Wählen Sie aus den folgenden Optionen:
   * Kurz
   * Standard. Dies ist die Standardauswahl.
   * Mittel
   * Groß

## Aktualisieren von erweiterten Listenelementen

Die folgenden Elemente sind Komponenten einer erweiterten Liste:

* **Ansicht**: Definiert die Spalten, Filter und Gruppierungen in der Liste mit den Voreinstellungen.
* **Filter**: Begrenzt die Anzahl der in der Liste angezeigten Informationen
* **Gruppierungen**: Organisieren der Listenelemente nach allgemeinen Feldern
* **Sortieren**: Ordnet die Elemente in einer Liste entsprechend der Reihenfolge an, die Sie für ein bestimmtes Feld identifizieren
* **Suche**: Sucht mithilfe eines Suchbegriffs schnell nach einem Element

### Anwenden und Erstellen von Ansichten

>[!NOTE]
>
>Nicht alle erweiterten Listen enthalten alle in diesem Abschnitt beschriebenen Elemente.

So wenden Sie eine Ansicht an bzw. erstellen eine Ansicht:

1. Klicken Sie auf **Ansichten** und wählen Sie eine vorhandene Ansicht aus, um sie auf die Liste anzuwenden

   ODER

   Klicken Sie auf **Neue Ansicht**, um eine Ansicht zu erstellen.

1. (Bedingt) Geben Sie zum Hinzufügen einer neuen Ansicht einen Namen für die Ansicht ein und klicken Sie dann auf **Erstellen**.
1. (Optional) Ausblenden, Anzeigen oder Neuanordnen der Spalten. Weitere Informationen finden Sie unter [Anpassen von Spalten in einer erweiterten Liste](#customize-columns-in-an-enhanced-list).
1. (Optional) Filtern Sie die Liste. Weitere Informationen finden Sie unter [Elemente in einer erweiterten Liste filtern](#filter-items-in-an-enhanced-list).
1. (Optional) Gruppieren Sie die Elemente in der Liste. Weitere Informationen finden Sie unter [Gruppieren von Elementen in einer erweiterten Liste](#group-items-in-an-enhanced-list).

   Änderungen an Ansichten werden automatisch gespeichert. The next time you apply this view, the column and filter settings remain the way you set them.

### Ansicht freigeben

>[!NOTE]
>
>Nicht alle erweiterten Listen enthalten alle in diesem Abschnitt beschriebenen Elemente.

In the **Views** dropdown, you may see three categories of views:

* **System Views**: Views that the system administrator assigned to you. You cannot share System views.
* **Shared Views**: Views that have been shared with you by other users.
* **My Views**: Views that you created and can share with others. You can share views with other users, teams, or groups.

When you share a view, all of the view elements (columns, filters, and groupings) are included.

To share a view:

1. In the **Views** dropdown, hover over the view in **My Views** that you want to share, click the **More** menu ![More menu](assets/more-icon.png), and click **Share**.
1. In the Share dialog, enter the names of the users, teams, groups, companies, or job roles that you want to share the view with, then select them from the list when they appear.

   You can give the following permissions to the recipients:

   * **View**: Users can apply the view to the list but not share it.

     When View access users update the view, those changes are saved to the user&#39;s personal preferences. A blue dot on the view name (in the user&#39;s **Shared Views**) shows that personal updates are applied to the view.

   * **Manage**: Users can rename, share, or delete the view, and edit the view&#39;s elements.

     When Manage access users make changes to the view, all users who have the view shared with them will see those updates when the view is applied to the list.

1. Klicken Sie auf **Speichern**.

   If you share a view with a user and then remove that access, the view is removed from the user&#39;s **Shared Views**. If the user had the shared view applied to the list when their access is removed, then the system default view is applied.

### Copy a view

>[!NOTE]
>
>Nicht alle erweiterten Listen enthalten alle in diesem Abschnitt beschriebenen Elemente.

When a view is shared with you to which you do not have permission to edit, you can copy the view and save it with a new name. You must first make changes to the view before you can copy it.

1. In the Views dropdown, hover over the view in **Shared Views** that you modified the settings of and which want to copy, click the **More** menu ![More menu](assets/more-icon.png), and click **Copy with preferences**.

   A new view is created automatically. The name of the copied view follows the following pattern: `Original view name (copy)`and it displays in the **My Views** section of views.

   You are the owner of this view, and you can rename, edit, share, or delete it. If the owner of the original view removes your shared access to that view, you still have access to the view that you created by copying the shared original.

   >[!NOTE]
   >
   >The **Copy with preferences** option is only available when you have made changes to a view that was shared with you.

### Reset a view

>[!NOTE]
>
>Nicht alle erweiterten Listen enthalten alle in diesem Abschnitt beschriebenen Elemente.

When a view is shared with you that you do not have permission to edit, and you update that view, you can reset it back to the original view.

1. In the **Views** dropdown, hover over the view in **Shared Views** that you want to reset, click the **More** menu ![More menu](assets/more-icon.png), and click **Reset to default**.

   The view elements (columns, filters, and groupings) are reset to their original settings that were shared with you.

   >[!NOTE]
   >
   >The **Reset to default** option is only available when you have made changes to a view that was shared with you.

   ![Copy and reset a view options](assets/glist-copy-view-shared-with-you.png)

### Apply conditional formatting in a view

>[!NOTE]
>
>Nicht alle erweiterten Listen enthalten alle in diesem Abschnitt beschriebenen Elemente.

Conditional formatting helps you highlight important information in the view based on common criteria.

1. Click the **Format cells** icon ![Format cells icon](assets/format-cells-icon.png). The **Format** box opens.

1. Click **Add condition**.
1. In the **If** line, select  a field and choose a field value and add a modifier. Modifiers change, depending on the field type you choose.

   >[!TIP]
   >
   >Only fields visible in the enhanced list are available for conditional formatting.

1. (Optional) Instead of adding a field value, click the **Compare to another field** icon ![Compare to another field](assets/compare-to-another-field-icon.png) and choose a field whose value you want to compare to the value of your selected field. For example, you can compare the Subject and Description fields on request items.

   >[!TIP]
   >
   >Only fields visible in the list view are available for conditional formatting. The fields you compare must be of the same type.

1. (Optional) Click **Add condition** in the **If** line to add more conditions to the same rule.

   >[!TIP]
   >
   >You can add up to 10 conditions in a conditioning rule and you can have up to 20 rules for a field.

1. Click the **Or** connector between conditions to change to **And** and to indicate that multiple conditions must be met at the same time. **Or** is the default connector.
1. In the **Format** line, select a field to indicate which column will be formatted.
1. (Optional) Click the **color circle** icon ![Color format icon](assets/color-format-icon.png) next to the field selected, to expand it and choose another color in the **Cell fill** area to change the color of the background in a cell or pick a color from the **Text color** area to change the color of text in a cell.
1. Click the **Text format** icon ![Text format icon](assets/text-format-icon.png) and select from the following options to format the text in a cell:
   * Fett
   * Kursiv

1. Turn on the **Apply to row** setting to apply the formatting to the entire row of the field that meets the conditions.

1. (Optional) Click **Add condition** in the **Format** box to add another rule for another field and the repeat the steps above.
1. (Optional) Click **Clear all** to remove all formatting.
1. Click outside the **Format** box to close it.

   This returns you to the list view.
The formatting is applied immediately to the list view.
There is a blue dot next to the **Format cells** icon to indicate that the view has special formatting applied.

### Filter items in an enhanced list

>[!NOTE]
>
>Nicht alle erweiterten Listen enthalten alle in diesem Abschnitt beschriebenen Elemente.

Filters help you reduce the amount of information you display in the list.

1. Click **Filter** above the list.
1. In the Filter box, click **Add condition**.
1. Select a field to filter by.
1. Select a filter modifier, such as &quot;Has any of,&quot; &quot;Has none of,&quot; &quot;Is before,&quot; or &quot;Is after.&quot; The modifier options are different depending on the type of field you are filtering by.
1. Select the field value or values. Depending on the field type you are filtering by, you might be prompted to select the item from a list, search for it, or use a calendar to select a date range.

   ![Filter in erweiterten Listen](assets/glist-filter-with-options.png)

   Der Filter wird automatisch auf die Liste angewendet.

   >[!TIP]
   >
   >Um einen personalisierten Filter anzuwenden, wählen Sie eine der folgenden Optionen für einen Feldwert aus:
   >
   >* **Ich (angemeldeter Benutzer)** um in Feldern, die auf Benutzer verweisen, auf den angemeldeten Benutzer zu verweisen.
   >
   >* **Meine Teams** oder **Mein Home-Team**, um auf Ihre Teams in Feldern zu verweisen, die auf Teams verweisen.
   >
   >* **Meine Gruppen** oder **Meine Hauptgruppe**, um auf Ihre Gruppen in Feldern zu verweisen, die auf Gruppen verweisen.
   >
   >* **Meine Firma**, um auf Ihre Firma in Feldern zu verweisen, die auf Firmen verweisen.
   > 
   >* **Meine Rollen** oder **Meine primäre Rolle**, um auf Ihre Aufgabengebiete in Feldern zu verweisen, die auf Rollen verweisen.

1. Klicken Sie **Bedingung hinzufügen**, um dem Filter eine weitere Bedingung hinzuzufügen.

   Sie können mehrere Filter über einen AND- oder EINEN OR-Connector verbinden.

1. Wenn der Filter angewendet wird, können Sie die Optionen **Filter** erneut öffnen, um die Filteroptionen zu ändern oder alle Filter zu löschen.

   Wenn ein Filter auf die Liste angewendet wird **wird auf der** „Filter“ ein Indikator angezeigt.

   ![Angewendeter Filter-Indikator](assets/glist-filter-applied-indicator.png)

### Elemente in einer erweiterten Liste gruppieren

>[!NOTE]
>
>Nicht alle erweiterten Listen enthalten alle in diesem Abschnitt beschriebenen Elemente.

Durch Gruppierungen werden die Objekte auf der Liste anhand bestimmter Kriterien in Bereiche unterteilt.

Workfront bietet eine begrenzte Anzahl vordefinierter Gruppierungen, die Sie nicht ändern können.

1. Klicken Sie **Gruppierung** über der Liste auf.
1. Gruppierung auswählen, um die Liste zu organisieren.

   ![Gruppierung auswählen](assets/glist-grouping-choose-a-group-by.png)

1. Klicken Sie **Alle reduzieren**, um die Liste mit allen reduzierten Gruppierungen anzuzeigen. Die Standardoption besteht darin, die Liste mit allen Gruppierungen anzuzeigen.
1. Wenn die Gruppierung angewendet wird, können Sie die Gruppenoptionen erneut öffnen, um alle Gruppierungen gleichzeitig ein- oder auszublenden, die Gruppierung in ein anderes Feld zu ändern oder alle Gruppierungen zu löschen.

   ![Gruppieren in erweiterten Listen](assets/glist-group-by-due-date-priorities.png)

   Auf der Schaltfläche **Gruppierung** wird ein Indikator angezeigt, wenn eine Gruppierung auf die Liste angewendet wird.

   ![Gruppierung angewendet Indikator](assets/glist-grouping-applied-indicator.png)

### Sortieren in eine erweiterte Liste

>[!NOTE]
>
>Nicht alle erweiterten Listen enthalten alle in diesem Abschnitt beschriebenen Elemente.

So sortieren Sie einzelne Spalten:

1. Bewegen Sie den Mauszeiger über die Spalte, klicken Sie dann auf den Abwärtspfeil und wählen Sie **Sortieren** aus.

   Ein Symbol neben einem Spaltennamen gibt an, dass die Liste nach den Werten in dieser Spalte und der Sortierrichtung sortiert wird.

   >[!NOTE]
   >
   >Einige Spalten sind je nach Liste möglicherweise nicht sortierbar.

   ![Nach Spalte sortieren](assets/glist-sort-by-column.png)

1. (Optional) Um Ihre Arbeit innerhalb einer Gruppierung zu sortieren, klicken Sie auf **Gruppierung**, gehen Sie zur Zeile der angewendeten Gruppierung, klicken Sie auf das Sortier-Dropdown-Menü und wählen Sie eine aufsteigende oder absteigende Reihenfolge.

   ![Sortieren in einer Gruppierung](assets/sort-in-groups.png)

   >[!TIP]
   >
   >Die Sortierreihenfolge unterscheidet sich je nach Feldtyp, nach dem Sie sortieren.

### Suche in einer erweiterten Liste

>[!NOTE]
>
>Nicht alle erweiterten Listen enthalten alle in diesem Abschnitt beschriebenen Elemente.

1. Geben Sie einen Suchbegriff ein, nach dem Sie suchen möchten, in das Suchfeld in der oberen rechten Ecke der Liste. Die Ergebnisse werden bei der Eingabe in der Liste hervorgehoben.

   ![Suchbegriff hervorgehoben](assets/glist-search-highlighted.png)

   >[!NOTE]
   >
   >Die Suche untersucht alle Spalten in allen Listenelementen. Wenn die Liste lang ist, enthält die Suche Elemente, die Sie möglicherweise scrollen müssen, um sie zu sehen. Wenn die Liste gefiltert wird, bezieht sich die Suche nur auf das, was gerade angezeigt wird.


