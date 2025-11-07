---
navigation-topic: get-started-with-workfront
title: Erweiterte Listen verwenden
description: Erweiterte Listen verwenden ein Tabellenformat für die Anzeige der Listenelemente und haben ein anderes Erscheinungsbild als die Standardlisten
author: Lisa
feature: Get Started with Workfront
exl-id: 4c25ed54-b147-4fd3-8d00-6f1ba61bbd38
source-git-commit: ddae871559a756f00ef96e70254e1019964ce882
workflow-type: tm+mt
source-wordcount: '1288'
ht-degree: 1%

---

# Erweiterte Listen verwenden

Erweiterte Listen sind in einigen Bereichen von Adobe Workfront verfügbar. Diese Listen verwenden ein Tabellenformat für die Anzeige der Listenelemente und haben ein anderes Erscheinungsbild als die Standardlisten. Die Verwaltung von Ansichten wurde ebenfalls verbessert, einschließlich Filtern, Gruppieren, Verwalten von Spalten und Suchen.

Informationen zu den Standardlisten finden Sie unter [Erste Schritte mit Listen in Adobe Workfront](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

>[!NOTE]
>
>Jede erweiterte Liste kann anders konfiguriert werden, damit Sie die benötigten Daten anzeigen können. Nicht alle in diesem Artikel beschriebenen Funktionen werden in jeder Liste verwendet, und einige Listen können spezielle Funktionen enthalten, die nur für diese Liste gelten.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
>Diese Liste ist nicht vollständig. Jede dieser Objektlisten kann auch in einem Bericht oder Dashboard angezeigt werden. Beispielsweise zeigt ein Projektbericht oder ein Dashboard, der bzw. das einen Projektbericht enthält, auch eine Liste der Projekte an.

| Workfront-Liste | Speicherort der Objektliste |
|--- |--- |
| Prioritäten | <ul><li>Startseite > Wählen Sie im linken Menü das Symbol Prioritäten aus.</li><li>Hauptmenü > Prioritäten</li></ul> |
| Liste der Anfragen | <ul><li>Anfragen (nur für neue Erlebnisse)</li><li>Widget „Meine Anfragen“ auf der Startseite</li></ul> |
| Listen mit Status, Prioritäten, Schweregraden und Wechselkursen im Setup | <ul><li>Setup > Projektvoreinstellungen > Status</li><li>Setup > Projektvoreinstellungen > Prioritäten</li><li>Setup > Projektvoreinstellungen > Schweregrade</li><li>Einrichten > Projektvoreinstellungen > Wechselkurse</li></ul> |

## Hinzufügen und Bearbeiten von Elementen in einer erweiterten Liste

Je nach Konfiguration der erweiterten Liste gibt es möglicherweise zwei Möglichkeiten, ein Element zur Liste hinzuzufügen:

* Klicken Sie auf eine Schaltfläche oberhalb der Liste. Diese Option öffnet ein Dialogfeld, in dem Sie Informationen eingeben und speichern können.
* Klicken Sie **Neue**) unten in der Liste auf. Mit dieser Option fügen Sie der Tabelle eine neue Zeile hinzu und geben Informationen in jede Zelle ein.

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

  Wenn Sie eine Zelle bearbeiten, hat jeder Feldtyp seine eigenen Bearbeitungsoptionen.

Um ein Element in der Liste zu bearbeiten, doppelklicken Sie in die Zelle, die Sie bearbeiten möchten, und geben Sie die Informationen ein. Einige Zellen sind möglicherweise schreibgeschützt.

![Beispiel für eine erweiterte Liste](assets/glist-exchange-rates.png)

## Verwenden der Aktionsleiste und des Menüs Mehr in einer erweiterten Liste

Wenn Sie das Kontrollkästchen neben einem Element in der erweiterten Liste aktivieren, wird die Aktionsleiste am unteren Bildschirmrand angezeigt und zeigt Aktionen an, die Sie für das Element ausführen können. Einige Aktionen sind möglicherweise spezifisch für diese Liste und werden in keiner anderen Liste angezeigt.

>[!NOTE]
>
>Verschiedene erweiterte Listen ermöglichen möglicherweise die Auswahl eines einzelnen Elements, die Massenbearbeitung (die Auswahl mehrerer Elemente) oder die Auswahl keiner Elemente.

Klicken Sie in der Aktionsleiste auf eine Schaltfläche, um diese Aktion auszuführen, z. B. das Anzeigen des Listenelements, das Löschen des Elements oder das Bearbeiten des Elements.

Wenn für das ausgewählte Element keine Aktionen verfügbar sind, wird in der Aktionsleiste „Keine verfügbaren Aktionen“ angezeigt.

![Beispiel für Aktionsleiste](assets/glist-action-bar-statuses.png)

Das **Mehr**-Menü ist das Dreipunkt-Menü, das neben einem Primärfeld in einem Listenelement angezeigt wird, wenn Sie den Mauszeiger darüber bewegen. (Das primäre Feld ist die Spalte in der Tabelle, die sich ganz links befindet.)

Klicken Sie auf das Menü, um zusätzliche Aktionen für das Element anzuzeigen. Einige Aktionen sind möglicherweise spezifisch für diese Liste und werden in keiner anderen Liste angezeigt.

![Weitere Menübeispiele](assets/glist-more-menu-priorities.png)

## Anpassen von Spalten in einer erweiterten Liste

Einige erweiterte Listen ermöglichen es Ihnen, Spalten auszublenden und anzuzeigen sowie die Spalten neu anzuordnen.

1. Klicken Sie **Spalten** über der Liste auf.

   ![Beispiel für Spalten anzeigen](assets/glist-display-move-columns.png)

1. Verwenden Sie die Umschalter zum Anzeigen oder Ausblenden von Spalten in der Liste.
1. Um die Spalten neu anzuordnen, klicken Sie auf das **Ziehen**-Symbol und verschieben Sie eine Spalte an die gewünschte Position. Durch das Verschieben von Spalten wird die Liste automatisch geändert.

   >[!NOTE]
   >
   >Das primäre Feld ist die Spalte in der Tabelle, die sich ganz links befindet. Sie ist an der ersten Position fixiert und kann nicht geändert werden. Wenn die Anzahl der Spalten groß ist, wird das primäre Feld nach links eingefroren, und wenn Sie horizontal scrollen, wird es immer angezeigt.
   >
   >Das Symbol neben einem Feldnamen zeigt den Feldtyp an, z. B. Text oder Datumsfeld.

   Ein Indikator wird auf der Schaltfläche **Spalten** angezeigt, wenn Spalten ausgeblendet sind. Der Indikator wird bei der Neuanordnung der Spalten nicht angezeigt.

   ![Indikator für ausgeblendete Spalten](assets/glist-columns-hidden-indicator.png)

## Anwenden einer Ansicht auf eine erweiterte Liste

Eine Ansicht ist ein personalisierter Satz von Spaltenanordnungen und Filtern, die Sie auf eine Liste anwenden können. Sie können neue Ansichten erstellen und vorhandene Ansichten bearbeiten.

Um eine Ansicht anzuwenden, klicken Sie auf **Dropdown** und wählen Sie die Ansicht aus, die Sie auf die Liste anwenden möchten.

Erstellen einer neuen Ansicht:

1. Klicken Sie auf **Ansichten** und wählen Sie **Neue Ansicht** aus.
1. Geben Sie einen Namen für die Ansicht ein und klicken Sie auf **Erstellen**.
1. (Optional) Ausblenden, Anzeigen oder Neuanordnen der Spalten. Weitere Informationen finden Sie unter [Anpassen von Spalten in einer erweiterten Liste](#customize-columns-in-an-enhanced-list).
1. (Optional) Filtern und Gruppieren der Listenelemente. Weitere Informationen finden Sie unter [Elemente in einer erweiterten Liste filtern und gruppieren](#filter-and-group-items-in-an-enhanced-list).

   Änderungen an Ansichten werden automatisch gespeichert und die Änderungen sind für alle sichtbar, die die Ansicht verwenden.

   Wenn Sie diese Ansicht das nächste Mal anwenden, bleiben die Spalten- und Filtereinstellungen so, wie Sie sie festlegen.

## Elemente in einer erweiterten Liste filtern und gruppieren

Filter helfen Ihnen, die Menge an Informationen zu reduzieren, die Sie in der Liste anzeigen. Durch Gruppierungen werden Objekte auf der Liste in Bereichen nach bestimmten Kriterien getrennt.

### Verwenden von Filtern

1. Klicken Sie **Filter** über der Liste auf.
1. Klicken Sie im Feld Filter auf **Bedingung hinzufügen**.
1. Wählen Sie ein Feld aus, nach dem gefiltert werden soll.
1. Wählen Sie einen Filtermodifikator aus, z. B. „Hat eines von“, „Hat keines von“, „ist vor“ oder „ist nach“. Die Modifikatoroptionen unterscheiden sich je nach dem Typ des Felds, nach dem Sie filtern.
1. Wählen Sie die Feldwerte aus. Je nach Feldtyp, nach dem Sie filtern, werden Sie möglicherweise aufgefordert, das Element aus einer Liste auszuwählen, danach zu suchen oder einen Kalender zu verwenden, um einen Datumsbereich auszuwählen.

   ![Filter in erweiterten Listen](assets/glist-filter-with-options.png)

   Der Filter wird automatisch auf die Liste angewendet.

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

Um einzelne Spalten zu sortieren, gehen Sie zur Spalte und klicken Sie auf den Abwärtspfeil. Ein Symbol neben einem Spaltennamen gibt an, dass die Liste nach den Werten in dieser Spalte und der Sortierrichtung sortiert wird.

>[!NOTE]
>
>Einige Spalten sind möglicherweise nicht sortierbar.

![Nach Spalte sortieren](assets/glist-sort-by-column.png)

Um Ihre Arbeit innerhalb einer Gruppierung zu sortieren, öffnen Sie **Gruppe** und wählen Sie aus, ob Sie in auf- oder absteigender Reihenfolge sortieren möchten.

![Sortieren in einer Gruppierung](assets/sort-in-groups.png)

Geben Sie zum Suchen Ihren Suchbegriff in das Suchfeld über der Liste ein. Die Ergebnisse werden bei der Eingabe in der Liste hervorgehoben.

![Suchbegriff hervorgehoben](assets/glist-search-highlighted.png)
