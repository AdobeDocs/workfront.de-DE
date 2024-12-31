---
product-area: reporting
navigation-topic: reporting-elements
title: Spaltenbreite und -reihenfolge ändern
description: In diesem Artikel erfahren Sie mehr über die Richtlinien für die Spaltenbreite und darüber, wie Sie die Spaltenbreite und -reihenfolge in Workfront ändern.
author: Nolan
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: 3cee374b68b26f2a423d41101300ec8b6685fadd
workflow-type: tm+mt
source-wordcount: '1010'
ht-degree: 0%

---

# Spaltenbreite und -reihenfolge ändern

<!-- Audited: 11/2024 -->

Im Folgenden finden Sie Richtlinien zur Funktionsweise von Spaltenbreiten in Adobe Workfront:

* Workfront definiert standardmäßig die Spaltenbreite in Listen und Berichten.
* Workfront passt die Spaltenbreite automatisch entsprechend den `valueformat`Informationen in allen Listen und Berichten an, sofern im Textmodus der Spalte nichts anderes angegeben ist.

  >[!NOTE]
  >
  >Workfront passt die Spaltenbreite nicht entsprechend den `valueformat` an, die in den Listen im Bereich Setup und Berichte verfügbar sind.

  Der `valueformat` definiert, welche Art von Informationen in der Spalte angezeigt wird. Beispielsweise sind Spalten, die eine Zahl anzeigen, schmaler als Spalten, die das Feld Beschreibung anzeigen.

* Sie können die Spaltenbreite in Ihren Workfront-Listen und -Berichten an Ihre Anforderungen anpassen, je nachdem, welche Art von Informationen Sie in Spalten anzeigen möchten.

  Sie können die Breite von Spalten vorübergehend ändern, während Sie eine Liste oder einen Bericht anzeigen, oder dauerhaft ändern, indem Sie die Breite der Spalte im View Builder anpassen. Informationen zum temporären Ändern der Spaltenbreite finden Sie im Abschnitt [Überlegungen beim temporären Ändern der Breite und Reihenfolge ](#considerations-when-temporarily-modifying-the-width-and-order-of-columns) Spalten“ in diesem Artikel.

* Spalten, die in integrierten Ansichten angezeigt werden, haben Breiten, die zuvor von Workfront definiert wurden und hartcodiert sind. Um diese Breiten zu ändern, müssen Sie die Breite dieser Spalten mithilfe des Textmodus im View Builder manuell aktualisieren.

  Informationen zum Ändern der Spalte im Textmodus finden Sie unter [Ansicht: Die Breite einer Spalte dauerhaft bearbeiten](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Mitwirkender oder höher</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Anfrage oder höher</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen der Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um die Ansicht in einem Bericht zu bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Verwalten der Berechtigungen für einen Bericht zum Bearbeiten einer Ansicht in einem Bericht</p> <p>Verwalten von Berechtigungen für eine Ansicht, um sie zu bearbeiten</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Spaltenbreite und -reihenfolge ändern

Sie können die Breite und Reihenfolge der Spalten in Ihren Berichten wie folgt ändern:

* [Ändern Sie die Breite und Reihenfolge der Spalten vorübergehend](#modify-width-and-order-of-columns-temporarily)
* [Breite und Reihenfolge der Spalten dauerhaft ändern](#modify-width-and-order-of-columns-permanently)

### Spaltenbreite und -reihenfolge vorübergehend ändern {#modify-width-and-order-of-columns-temporarily}

Sie können Spaltenrahmen ziehen, um die Spaltengröße zu ändern, und Spalten per Drag-and-Drop verschieben, um sie in den meisten Listen auf der gesamten Workfront-Site vorübergehend neu anzuordnen. Dazu gehören Berichte, Ansichten, Berichte zu Dashboards und die Gantt-Ansicht.

Weitere Informationen zu Workfront-Listen finden Sie im Artikel &quot;[ mit Listen in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* [Überlegungen beim vorübergehenden Ändern der Breite und Reihenfolge von Spalten](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [Spaltengröße vorübergehend ändern](#resize-columns-temporarily)
* [Spalten vorübergehend neu anordnen](#reorder-columns-temporarily)

#### Überlegungen beim vorübergehenden Ändern der Breite und Reihenfolge von Spalten {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

Sie können die Breite und Reihenfolge von Spalten in einer Liste vorübergehend ändern, ohne die Ansicht zu bearbeiten.

Beachten Sie Folgendes, wenn Sie die Größe von Spalten vorübergehend ändern und sie sortieren:

* Beim Ändern der Spaltengröße werden die neuen Spaltengrößen im lokalen Speicher Ihres Browsers gespeichert und standardmäßig gespeichert. Wenn Sie einen anderen Browser verwenden oder Ihren Cache löschen oder Daten durchsuchen, wird die Spaltengröße auf den Standardwert zurückgesetzt. Wenn Sie Ihre Seite aktualisieren, bleiben die Änderungen, die Sie an der Spaltenbreite vornehmen, erhalten.

>[!NOTE]
> 
>Spaltenbreiten werden durch die Größe des Browser-Fensters begrenzt. Wenn die Seite aktualisiert wird, wird die Breite der Spalten reduziert, bis alle Spalten ohne horizontalen Bildlauf in das Fenster passen. Um zu erzwingen, dass eine Spalte breiter bleibt, als der Browser passt, müssen Sie die Spaltenbreite im Textmodus festlegen, wie in [Ändern der Spaltenbreite und -reihenfolge](#modify-width-and-order-of-columns-permanently) beschrieben, und es vermeiden, Spaltenbreiten manuell anzupassen, indem Sie ihre Ränder ziehen.
>

* Bei der Neuanordnung von Spalten wird die ausgewählte Reihenfolge nur beibehalten, bis Sie die Liste verlassen oder die Browser-Seite aktualisieren. Nachdem Sie die Liste verlassen oder die Browser-Seite aktualisiert haben, kehren die Spalten in ihre Standardreihenfolge zurück.
* Um eine optimale Leistung zu erzielen, sollten die Spalten, die Sie neu anordnen, nicht mehr als 100 Elemente in der Liste enthalten.
* Wenn Sie die Größe von Spalten ändern, gelten Ihre Änderungen nur für die Ansicht, die Sie derzeit verwenden, und sind nur für Sie sichtbar. Bei der Freigabe einer Ansicht für einen anderen Benutzer werden die von Ihnen definierten Spaltengrößen nicht freigegeben.
* Nachdem Sie die Größe einer Spalte durch Ziehen des Rahmens nach rechts geändert haben, wird die Breite der benachbarten Spalte beibehalten, mit Ausnahme der folgenden:

   * Der Bereich Setup
   * Der Bereich Berichte
   * Dokumentlisten und Berichte

  >[!NOTE]
  >
  >Der linke Rand einer Spalte kann in keiner Liste über den linken Rand der benachbarten Spalte hinaus verschoben werden.

* Wenn Sie eine Liste in eine Datei exportieren, wird die temporäre Reihenfolge der Spalten nicht in die exportierte Datei übertragen. Die exportierte Datei zeigt die Reihenfolge der Spalten in der ursprünglichen Liste an, bevor die Spalten neu angeordnet wurden.

Weitere Informationen zum Exportieren von Daten aus Listen und Berichten finden Sie im Artikel [Exportieren von Daten](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

#### Spaltengröße vorübergehend ändern {#resize-columns-temporarily}

1. Navigieren Sie zur Liste, die Sie ändern möchten.
1. Ziehen Sie den Rahmen einer Spaltenüberschrift, bis die Spalte die gewünschte Größe erreicht.\
   ![](assets/column-resize-350x124.png)

#### Spalten vorübergehend neu anordnen {#reorder-columns-temporarily}

1. Navigieren Sie zur Liste, die Sie ändern möchten.
1. Klicken Sie auf die Spaltenüberschrift, und ziehen Sie sie an die gewünschte Position.

>[!TIP]
>
>Dies ist besonders nützlich, wenn das Gantt-Diagramm und die Listenansicht gleichzeitig angezeigt werden. Beim Anzeigen des Gantt-Diagramms können Spalten ausgeblendet werden. Um eine Spalte anzuzeigen, während das Gantt-Diagramm angezeigt wird, ziehen Sie einfach die Spalte, die Sie anzeigen möchten, sodass sie auf der linken Seite der Seite angezeigt wird.

### Breite und Reihenfolge der Spalten dauerhaft ändern {#modify-width-and-order-of-columns-permanently}

Informationen zur dauerhaften Neuanordnung von Spalten finden Sie im Abschnitt [Erstellen oder Anpassen einer Standardansicht](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view) im Artikel [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Sie können die Breite einer Spalte nur dauerhaft ändern, indem Sie den Textmodus verwenden.

Weitere Informationen zur Verwendung des Textmodus und zum dauerhaften Ändern der Breite einer Spalte finden Sie im Artikel [Übersicht über häufig verwendete Funktionen für den Textmodus](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
