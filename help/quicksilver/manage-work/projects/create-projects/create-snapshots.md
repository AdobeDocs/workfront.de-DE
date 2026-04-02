---
product-area: projects
navigation-topic: create-projects
title: Erstellen und Anzeigen von Projekt-Momentaufnahmen
description: Mit Momentaufnahmen in Adobe Workfront können Sie Unterschiede zwischen Momentaufnahmen (zu einem bestimmten Datum und zu einer bestimmten Uhrzeit) und den aktuellen Daten des Projekts anzeigen.
author: Lisa
feature: Work Management
hidefromtoc: true
hide: true
source-git-commit: 6ccb4669a973a8f855120e83de7c0d437c9495a4
workflow-type: tm+mt
source-wordcount: '1278'
ht-degree: 2%

---

# Erstellen und Anzeigen von Projekt-Momentaufnahmen

{{highlighted-preview-article-level}}

Projektleiter müssen oft die vergangenen Daten eines Projekts mit dem aktuellen Status vergleichen, um fundierte Entscheidungen zu treffen und zu sehen, wie sich ihre Projekte im Laufe der Zeit verändert haben.

Momentaufnahmen in Adobe Workfront bieten Ihnen die Möglichkeit, diese Unterschiede zwischen Momentaufnahmen (zu einem bestimmten Datum und zu einer bestimmten Uhrzeit) und den aktuellen Daten des Projekts schnell und präzise zu sehen, sodass Sie Projekte effektiver verwalten und bessere Entscheidungen treffen können. Momentaufnahmen-Vergleiche zeigen nebeneinander, wie sich das Projekt entwickelt hat.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td> <p>Workflow Ultimate</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
    <td>Standard</td> 
  </tr> 
  <tr> 
   <td>Konfiguration der Zugriffsebene</td> 
   <td>Zugriff auf Projekte bearbeiten</td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td>Beim Anzeigen eines Schnappschusses können Sie alle Felder anzeigen, für die Sie im ursprünglichen Projekt über die Berechtigung zum Anzeigen verfügen </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Snapshot erstellen

1. Gehe zu einem Projekt.
1. Klicken Sie im linken Bedienfeld auf **Momentaufnahmen**.

   ![Momentaufnahmen für ein Projekt](assets/snapshot-list.png)

1. Klicken Sie auf **Neuer Schnappschuss**.
1. Geben Sie einen Namen für den Schnappschuss im Dialogfeld **Neuer Schnappschuss** ein und klicken Sie auf **Speichern**.

   Der Snapshot-Name wird in der Liste angezeigt.

   >[!NOTE]
   >
   >Wenn Sie einen Schnappschuss erstellen, steht er nicht sofort zur Anzeige zur Verfügung. Basierend auf Daten, die im Hintergrund ausgeführt werden, kann es bis zu 4 Stunden dauern, bis sie bereit sind. Der Erstellungsstatus lautet **Ausstehend** wenn der Snapshot noch nicht verfügbar ist, und **Bereit** wenn Sie ihn anzeigen können.

## Einzelne Momentaufnahme anzeigen

1. Gehen Sie zu einem Projekt und klicken Sie **linken Bereich** Momentaufnahmen“.
1. Klicken Sie auf den Namen eines Schnappschusses in der Liste, um ihn zu öffnen. Der Status muss **Bereit** sein, bevor Sie ihn öffnen können.

   >[!TIP]
   >
   >Die Breadcrumbs oben im Bildschirm verlinken zurück zum Projekt und helfen Ihnen dabei zu ermitteln, ob Sie einen Schnappschuss anzeigen.

   Der Snapshot zeigt die folgenden Elemente so an, wie sie zum Zeitpunkt der Erstellung des Snapshots vorhanden waren:

   * Hierarchie der Aufgaben und Teilaufgaben im Projekt
   * Projektdetails und alle benutzerdefinierten Formulare, die an die Details angehängt sind
   * Zugeordnete Projekte und ihre Hierarchie
   * Probleme
   * Abrechnungssätze
   * Abrechnungseinträge
   * &#x200B;<!--* Bookings (on its own line of course when they get released)-->
   * Projektteam (Registerkarte „Personen„)

   Sie können alle Listen im Schnappschuss anpassen, indem Sie Spalten filtern, sortieren, hinzufügen und entfernen oder eine Ansicht anwenden. Es stehen zeitphasengesteuerte KPIs zur Verfügung, die der Schnappschussansicht hinzugefügt werden können. Weitere Informationen finden Sie unter [Anpassen von &#x200B;](#customize-snapshot-lists)) in diesem Artikel.

## Momentaufnahmen vergleichen

1. Gehen Sie zu einem Projekt und klicken Sie **linken Bereich** Momentaufnahmen“.
1. Option zum Vergleichen von Momentaufnahmen auswählen:

   * Um zwei oder mehr Momentaufnahmen miteinander zu vergleichen, aktivieren Sie die Kontrollkästchen neben den Momentaufnahmen in der Liste und klicken Sie **Vergleichen** in der Aktionsleiste am unteren Bildschirmrand.
   * Um Momentaufnahmen mit dem aktuellen Projekt zu vergleichen, aktivieren Sie die Kontrollkästchen neben den Momentaufnahmen in der Liste und klicken Sie **Mit aktuellem** vergleichen“ in der Aktionsleiste am unteren Bildschirmrand.

     >[!NOTE]
     >
     >Der Status jedes Snapshots, den Sie vergleichen möchten, muss **Bereit** sein.

1. Erweitern Sie auf dem Bildschirm Vergleich jede Momentaufnahme und das aktuelle Projekt, um die darunter liegende Hierarchie anzuzeigen.

   ![Snapshot-Vergleichsbildschirm](assets/snapshot-comparison.png)

1. Sie können den Vergleich anpassen, indem Sie sortieren, Spalten hinzufügen und entfernen oder eine Ansicht anwenden. Weitere Informationen finden Sie unter [Anpassen von &#x200B;](#customize-snapshot-lists)) in diesem Artikel.

## Schnappschüsse exportieren

Sie können die Liste aller Momentaufnahmen oder einen Schnappschussvergleich im .xlsx- oder .csv-Format exportieren. Alle angezeigten Spalten sind in der exportierten Datei enthalten.

1. Klicken Sie auf **Export**-Symbol ![Export-Symbol](assets/export-icon.png) in der Snapshot-Liste oder im Snapshot-Vergleich.
1. Wählen Sie das Format für die Exportdatei.

   Die Datei wird auf Ihrem Computer gespeichert. Sie werden möglicherweise aufgefordert, den Speicherort auszuwählen.

1. (Optional) Öffnen Sie die exportierte Liste mit dem entsprechenden Programm.

## Momentaufnahmenlisten anpassen

Sie können die Liste aller Momentaufnahmen sowie alle Listen innerhalb eines Schnappschusses oder Vergleichs anpassen, indem Sie Spalten filtern, sortieren, hinzufügen und entfernen oder eine Ansicht anwenden.

Weitere Informationen über die Anpassung von Listen finden Sie unter [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

### Elemente in einer Liste filtern

Filter helfen Ihnen, die Menge an Informationen zu reduzieren, die Sie in der Liste anzeigen.

1. Klicken Sie **Filter** über der Liste auf.
1. Klicken Sie im Feld Filter auf **Bedingung hinzufügen**.
1. Wählen Sie ein Feld aus, nach dem gefiltert werden soll.
1. Wählen Sie einen Filtermodifikator aus, z. B. „Hat eines von“, „Hat keines von“, „ist vor“ oder „ist nach“. Die Modifikatoroptionen unterscheiden sich je nach dem Typ des Felds, nach dem Sie filtern.
1. Wählen Sie die Feldwerte aus. Je nach Feldtyp, nach dem Sie filtern, werden Sie möglicherweise aufgefordert, das Element aus einer Liste auszuwählen, danach zu suchen oder einen Kalender zu verwenden, um einen Datumsbereich auszuwählen.

   ![Filtern Sie die Momentaufnahmenliste](assets/filter-snapshot-list.png)

   Der Filter wird automatisch auf die Liste angewendet.

1. Klicken Sie **Bedingung hinzufügen**, um dem Filter eine weitere Bedingung hinzuzufügen.

   Sie können mehrere Filter über einen AND- oder EINEN OR-Connector verbinden.

1. Wenn der Filter angewendet wird, können Sie die Optionen **Filter** erneut öffnen, um die Filteroptionen zu ändern oder alle Filter zu löschen.

   Wenn ein Filter auf die Liste angewendet wird **wird auf der** „Filter“ ein Indikator angezeigt.

   ![Angewendeter Filter-Indikator](assets/glist-filter-applied-indicator.png)

### In Liste sortieren

So sortieren Sie einzelne Spalten:

1. Bewegen Sie den Mauszeiger über die Spalte, klicken Sie dann auf den Abwärtspfeil und wählen Sie **Sortieren** aus.

   Ein Symbol neben einem Spaltennamen gibt an, dass die Liste nach den Werten in dieser Spalte und der Sortierrichtung sortiert wird.

   ![Sortieren Sie die Momentaufnahmenliste](assets/sort-snapshot-list.png)

### Spalten in einer Liste anpassen

Sie können Spalten in einer Liste ausblenden, anzeigen und neu anordnen.

1. Klicken Sie **Spalten** über der Liste auf.

   ![Spalten für Momentaufnahmenliste](assets/hide-display-columns-on-snapshot.png)

1. Verwenden Sie die Umschalter zum Anzeigen oder Ausblenden von Spalten in der Liste.
1. Um die Spalten neu anzuordnen, klicken Sie auf das Symbol **Ziehen** (![-Symbol](assets/drag-icon.png) und verschieben Sie eine Spalte an die gewünschte Position. Durch das Verschieben von Spalten wird die Liste automatisch geändert.

   >[!NOTE]
   >
   >Das primäre Feld ist die erste Spalte in der Liste. Sie ist an der ersten Position fixiert und kann nicht geändert werden. Wenn die Anzahl der Spalten groß ist, wird das primäre Feld nach links eingefroren, und wenn Sie horizontal scrollen, wird es immer angezeigt.
   >
   >Das Symbol neben einem Feldnamen zeigt den Feldtyp an, z. B. Text oder Datumsfeld.

   Ein Indikator wird auf der Schaltfläche **Spalten** angezeigt, wenn Spalten ausgeblendet sind. Der Indikator wird bei der Neuanordnung der Spalten nicht angezeigt.

   ![Indikator für ausgeblendete Spalten](assets/glist-columns-hidden-indicator.png)

### Hinzufügen und Entfernen von Spalten mit dem Spalten-Manager

Sie können den Spalten-Manager in einigen erweiterten Listen verwenden, um Spalten einfach zur Liste hinzuzufügen und daraus zu entfernen. Sie können sowohl System- als auch benutzerdefinierte Felder, die bereits in Workfront vorhanden sind, als Spalten hinzufügen oder entfernen.

1. Klicken Sie auf das Symbol **+** oben rechts in der Tabelle, um das Feld **Spalten-Manager** zu öffnen.

   ![Spalten-Manager für Momentaufnahmen](assets/column-manager-on-snapshot-no-kpi-tab.png)

1. Suchen Sie in der Spalte **Verfügbar** nach einem vorhandenen Objektfeld und klicken Sie dann auf **+** rechts neben dem Feldnamen, um es der Spalte **Ausgewählt** hinzuzufügen.
1. Klicken Sie auf **-** rechts neben einem Feld in der Spalte **Ausgewählt**, um es aus der Liste zu entfernen.
1. Klicken Sie auf **Speichern**.

   Die Liste aktualisiert die Spalten entsprechend den von Ihnen getroffenen Entscheidungen.

### Anwenden einer Ansicht auf eine Liste

So wenden Sie eine Ansicht an bzw. erstellen eine Ansicht:

1. Klicken Sie auf **Ansichten** und wählen Sie eine vorhandene Ansicht aus, um sie auf die Liste anzuwenden

   ODER

   Klicken Sie auf **Neue Ansicht**, um eine Ansicht zu erstellen.

   ![Menü „Ansichten“ auf einem Schnappschuss](assets/views-on-snapshot-list.png)

1. (Bedingt) Geben Sie zum Hinzufügen einer neuen Ansicht einen Namen für die Ansicht ein und klicken Sie dann auf **Erstellen**.
1. (Optional) Ausblenden, Anzeigen oder Neuanordnen der Spalten. Weitere Informationen finden Sie unter [Anpassen von Spalten in einer Liste](#customize-columns-in-a-list).
1. (Optional) Filtern Sie die Liste. Weitere Informationen finden Sie unter [Elemente in einer Liste filtern](#filter-items-in-a-list).

Änderungen an Ansichten werden automatisch gespeichert. Wenn Sie diese Ansicht das nächste Mal anwenden, bleiben die Spalten- und Filtereinstellungen so, wie Sie sie festlegen. Weitere Informationen zu Ansichten finden Sie unter [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

