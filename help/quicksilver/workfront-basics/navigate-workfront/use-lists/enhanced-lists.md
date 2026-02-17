---
navigation-topic: get-started-with-workfront
title: Erweiterte Listen verwenden
description: Erweiterte Listen verwenden ein Tabellenformat für die Anzeige der Listenelemente und haben ein anderes Erscheinungsbild als die Standardlisten
author: Lisa
feature: Get Started with Workfront
exl-id: 4c25ed54-b147-4fd3-8d00-6f1ba61bbd38
source-git-commit: ee5bb3cbf6a69b85c3d6b87500164f85a1ba114a
workflow-type: tm+mt
source-wordcount: '1617'
ht-degree: 2%

---

# Erweiterte Listen verwenden

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
   <p>Mitwirkender oder höher</p>
   <p>Anfrage oder höher</p></td>
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
|--- |--- |
| Prioritäten | <ul><li>Startseite > Wählen Sie im linken Menü das Symbol Prioritäten aus.</li><li>Hauptmenü > Prioritäten</li></ul> |
| Liste der Anfragen | <ul><li>Anfragen (nur für neue Erlebnisse)</li><li>Widget „Meine Anfragen“ auf der Startseite</li></ul> |
| Listen mit Status, Prioritäten, Schweregraden und Wechselkursen im Setup | <ul><li>Setup > Projektvoreinstellungen > Status</li><li>Setup > Projektvoreinstellungen > Prioritäten</li><li>Setup > Projektvoreinstellungen > Schweregrade</li><li>Einrichten > Projektvoreinstellungen > Wechselkurse</li></ul> |

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

## Hinzufügen und Entfernen von Spalten mit dem Spalten-Manager

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

## Anzeigen von Daten mit Ansichten in einer erweiterten Liste

Eine Ansicht ist ein personalisierter Satz von Spaltenanordnungen und Filtern, die Sie auf eine Liste anwenden können. Sie können neue Ansichten erstellen und vorhandene Ansichten bearbeiten.

### Anwenden und Erstellen von Ansichten

Um eine Ansicht anzuwenden, klicken Sie auf **Dropdown** und wählen Sie die Ansicht aus, die Sie auf die Liste anwenden möchten.

Erstellen einer neuen Ansicht:

1. Klicken Sie auf **Ansichten** und wählen Sie **Neue Ansicht** aus.
1. Geben Sie einen Namen für die Ansicht ein und klicken Sie auf **Erstellen**.
1. (Optional) Ausblenden, Anzeigen oder Neuanordnen der Spalten. Weitere Informationen finden Sie unter [Anpassen von Spalten in einer erweiterten Liste](#customize-columns-in-an-enhanced-list).
1. (Optional) Filtern und Gruppieren der Listenelemente. Weitere Informationen finden Sie unter [Elemente in einer erweiterten Liste filtern und gruppieren](#filter-and-group-items-in-an-enhanced-list).

   Änderungen an Ansichten werden automatisch gespeichert und die Änderungen sind für alle sichtbar, die die Ansicht verwenden.

   Wenn Sie diese Ansicht das nächste Mal anwenden, bleiben die Spalten- und Filtereinstellungen so, wie Sie sie festlegen.

### Ansicht freigeben

In der **Ansichten** Dropdown-Liste werden möglicherweise drei Kategorien von Ansichten angezeigt:

* **Systemansichten**: Ansichten, die Ihnen vom Systemadministrator zugewiesen wurden.
* **Freigegebene**: Ansichten, die von anderen Benutzern für Sie freigegeben wurden.
* **Meine Ansichten**: Ansichten, die Sie erstellt haben und für andere freigeben können. Sie können Ansichten für andere Benutzer, Teams oder Gruppen freigeben.

So geben Sie eine Ansicht frei:

1. Bewegen Sie in **Dropdown** Ansicht“ den Mauszeiger über die Ansicht in **Meine Ansichten**, die Sie freigeben möchten, und klicken Sie dann auf das Dreipunkt-Menü, wenn es angezeigt wird.
1. Wählen Sie **Freigeben** aus.
1. Geben Sie im Dialogfeld Freigeben die Namen der Benutzer, Teams oder Gruppen ein, für die Sie die Ansicht freigeben möchten, und wählen Sie sie dann aus der Liste aus, wenn sie angezeigt werden.

   Sie können den Empfängerinnen und Empfängern die folgenden Berechtigungen erteilen:

   * **Ansicht**: Benutzer können die Ansicht auf die Liste anwenden, sie jedoch nicht freigeben.
   * **Verwalten**: Benutzer können die Ansicht umbenennen, sie für andere freigeben und löschen.

1. Klicken Sie auf **Speichern**.

## Elemente filtern und gruppieren

Filter helfen Ihnen, die Menge an Informationen zu reduzieren, die Sie in der Liste anzeigen. Durch Gruppierungen werden Objekte auf der Liste in Bereichen nach bestimmten Kriterien getrennt.

### Verwenden von Filtern

1. Klicken Sie **Filter** über der Liste auf.
1. Klicken Sie im Feld Filter auf **Bedingung hinzufügen**.
1. Wählen Sie ein Feld aus, nach dem gefiltert werden soll.
1. Wählen Sie einen Filtermodifikator aus, z. B. „Hat eines von“, „Hat keines von“, „ist vor“ oder „ist nach“. Die Modifikatoroptionen unterscheiden sich je nach dem Typ des Felds, nach dem Sie filtern.
1. Wählen Sie die Feldwerte aus. Je nach Feldtyp, nach dem Sie filtern, werden Sie möglicherweise aufgefordert, das Element aus einer Liste auszuwählen, danach zu suchen oder einen Kalender zu verwenden, um einen Datumsbereich auszuwählen.

   ![Filter in erweiterten Listen](assets/glist-filter-with-options.png)

   Der Filter wird automatisch auf die Liste angewendet.

   >[!TIP]
   >
   >Um einen Platzhalter für einen aktuellen Benutzer anzuwenden, wählen Sie **Ich (angemeldeter Benutzer)** als Feldwert aus. Der Filter gilt dann für den Benutzer, der die Liste anzeigt. Dieser Platzhalter ist in Feldern verfügbar, in denen der Wert ein Benutzer ist.

1. Klicken Sie **Bedingung hinzufügen**, um dem Filter eine weitere Bedingung als OR-Anweisung hinzuzufügen.
1. Wenn der Filter angewendet wird, können Sie die Optionen **Filter** erneut öffnen, um die Filteroptionen zu ändern oder alle Filter zu löschen.

   Wenn ein Filter auf die Liste angewendet wird **wird auf der** „Filter“ ein Indikator angezeigt.

   ![Angewendeter Filter-Indikator](assets/glist-filter-applied-indicator.png)

### Gruppierungen verwenden

1. Klicken Sie **Gruppe** über der Liste auf.
1. Gruppierung auswählen, um die Liste zu organisieren.

   ![Gruppierung auswählen](assets/glist-grouping-choose-a-group-by.png)

1. Wenn die Gruppierung angewendet wird, können Sie die Gruppenoptionen erneut öffnen, um alle Gruppierungen gleichzeitig ein- oder auszublenden, die Gruppierung in ein anderes Feld zu ändern oder alle Gruppierungen zu löschen.

   ![Gruppieren in erweiterten Listen](assets/glist-group-by-due-date-priorities.png)

   Auf der Schaltfläche **Gruppe** wird ein Indikator angezeigt, wenn eine Gruppierung auf die Liste angewendet wird.

   ![Gruppierung angewendet Indikator](assets/glist-grouping-applied-indicator.png)

## Sortieren und Suchen in einer erweiterten Liste

So sortieren Sie einzelne Spalten:

1. Wechseln Sie zur Spalte und klicken Sie auf den Abwärtspfeil.

   Ein Symbol neben einem Spaltennamen gibt an, dass die Liste nach den Werten in dieser Spalte und der Sortierrichtung sortiert wird.

   >[!NOTE]
   >
   >Einige Spalten sind je nach Liste möglicherweise nicht sortierbar.

   ![Nach Spalte sortieren](assets/glist-sort-by-column.png)

So sortieren Sie Ihre Arbeit innerhalb einer Gruppierung:

1. Klicken Sie **Gruppe** und wählen Sie aus, ob Sie in auf- oder absteigender Reihenfolge sortieren möchten.

   ![Sortieren in einer Gruppierung](assets/sort-in-groups.png)

Zum Suchen:

1. Geben Sie den Suchbegriff in das Suchfeld oberhalb der Liste ein. Die Ergebnisse werden bei der Eingabe in der Liste hervorgehoben.

   ![Suchbegriff hervorgehoben](assets/glist-search-highlighted.png)
