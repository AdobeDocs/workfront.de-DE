---
product-area: reporting
navigation-topic: reporting-elements
title: Spaltenbreite und -reihenfolge ändern
description: Lesen Sie diesen Artikel, um mehr über die Richtlinien zur Spaltenbreite und darüber zu erfahren, wie die Spaltenbreite und -reihenfolge in Workfront geändert werden.
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
* Workfront passt die Spaltenbreite automatisch an die `valueformat`Informationen in allen Listen und Berichten an, sofern im Textmodus der Spalte nichts anderes angegeben ist.

  >[!NOTE]
  >
  >Workfront passt die Spaltenbreite nicht an die `valueformat` -Informationen in den Listen an, die in den Bereichen Einrichtung und Berichte verfügbar sind.

  Der Wert `valueformat` definiert, welche Art von Informationen in der Spalte angezeigt werden. Beispielsweise sind Spalten, die eine Zahl anzeigen, enger als Spalten, in denen das Feld Beschreibung angezeigt wird.

* Sie können die Spaltenbreite in Ihren Workfront-Listen und -Berichten an Ihre Anforderungen anpassen, je nachdem, welche Art von Informationen in Spalten angezeigt werden soll.

  Sie können die Breite der Spalten vorübergehend ändern, während Sie eine Liste, einen Bericht oder einen Bericht anzeigen, oder dauerhaft, indem Sie die Breite der Spalte im Ansichtsaufbau anpassen. Informationen zum temporären Ändern der Breite von Spalten finden Sie im Abschnitt [Überlegungen beim temporären Ändern der Breite und Reihenfolge von Spalten](#considerations-when-temporarily-modifying-the-width-and-order-of-columns) in diesem Artikel.

* Spalten, die in integrierten Ansichten angezeigt werden, haben Breiten, die zuvor von Workfront definiert wurden und hartcodiert sind. Um diese Breiten zu ändern, müssen Sie die Breite dieser Spalten mithilfe des Textmodus im Ansichts-Builder manuell aktualisieren.

  Informationen zum Ändern der Spalte im Textmodus finden Sie unter [Ansicht: Breite einer Spalte dauerhaft bearbeiten](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-Lizenz*</strong></td> 
   <td> 
      <p>Neu:</p>
         <ul>
         <li><p>Mitwirkende oder höher</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Anforderung oder höher</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um die Ansicht in einem Bericht zu bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Berechtigungen für einen Bericht zum Bearbeiten einer Ansicht in einem Bericht verwalten</p> <p>Berechtigungen für eine Ansicht verwalten</p></td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Spaltenbreite und -reihenfolge ändern

Sie können die Breite und Reihenfolge der Spalten in Ihren Berichten wie folgt ändern:

* [Breite und Reihenfolge der Spalten vorübergehend ändern](#modify-width-and-order-of-columns-temporarily)
* [Breite und Reihenfolge der Spalten dauerhaft ändern](#modify-width-and-order-of-columns-permanently)

### Länge und Reihenfolge der Spalten vorübergehend ändern {#modify-width-and-order-of-columns-temporarily}

Sie können Spaltenränder ziehen, um die Spaltengröße zu ändern, und Spalten per Drag-and-Drop verschieben, um sie vorübergehend in den meisten Listen auf der Workfront-Site neu anzuordnen. Dazu gehören Berichte, Ansichten, Berichte in Dashboards und die Gantt-Ansicht.

Weitere Informationen zu Workfront-Listen finden Sie im Artikel [Erste Schritte mit Listen in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* [Überlegungen beim zeitweiligen Ändern der Breite und Reihenfolge der Spalten](#considerations-when-temporarily-modifying-the-width-and-order-of-columns)
* [Spaltengröße vorübergehend ändern](#resize-columns-temporarily)
* [Spalten vorübergehend neu ordnen](#reorder-columns-temporarily)

#### Überlegungen beim zeitweiligen Ändern der Breite und Reihenfolge der Spalten {#considerations-when-temporarily-modifying-the-width-and-order-of-columns}

Sie können die Breite und Reihenfolge der Spalten in einer Liste vorübergehend ändern, ohne die Ansicht zu bearbeiten.

Beachten Sie Folgendes bei der zeitweiligen Größenanpassung und Sortierung von Spalten:

* Bei der Größenanpassung von Spalten werden die neuen Spaltengrößen im lokalen Speicher Ihres Browsers gespeichert und standardmäßig gespeichert. Wenn Sie einen anderen Browser verwenden, den Cache leeren oder Daten durchsuchen, wird die Spaltengröße auf den Standardwert zurückgesetzt. Durch die Aktualisierung Ihrer Seite werden die Änderungen an der Spaltenbreite beibehalten.

>[!NOTE]
> 
>Die Spaltenbreiten sind durch die Größe des Browser-Fensters begrenzt. Wenn die Seite aktualisiert wird, werden die Spalten so lange breiter, bis alle Spalten ohne horizontalen Bildlauf in das Fenster passen. Um zu erzwingen, dass eine Spalte breiter bleibt, als der Browser ausreicht, müssen Sie die Breite der Spalte im Textmodus festlegen, wie unter [Breite und Reihenfolge der Spalten dauerhaft ändern](#modify-width-and-order-of-columns-permanently) beschrieben. Außerdem müssen Sie vermeiden, Spaltenbreiten manuell durch Ziehen ihrer Rahmen anzupassen.
>

* Bei der Neuanordnung von Spalten wird die von Ihnen gewählte Reihenfolge nur beibehalten, bis Sie von der Liste weg navigieren oder die Browser-Seite aktualisieren. Nachdem Sie von der Liste weg navigiert oder die Browser-Seite aktualisiert haben, kehren die Spalten zur Standardreihenfolge zurück.
* Um eine optimale Leistung zu erzielen, sollten die neu anzuordnenden Spalten nicht mehr als 100 Elemente in der Liste enthalten.
* Wenn Sie die Größe von Spalten ändern, gelten Ihre Änderungen nur für die derzeit verwendete Ansicht und sind nur für Sie sichtbar. Wenn Sie eine Ansicht für einen anderen Benutzer freigeben, werden die von Ihnen definierten Spaltengrößen nicht gemeinsam verwendet.
* Wenn Sie die Größe einer Spalte durch Ziehen des Rahmens nach rechts ändern, bleibt die Breite der benachbarten Spalte erhalten, mit Ausnahme der folgenden:

   * Der Einrichtungsbereich
   * Der Bereich Berichte
   * Dokumentlisten und Berichte

  >[!NOTE]
  >
  >Der linke Rand einer Spalte kann in keiner Liste über den linken Rand der benachbarten Spalte verschoben werden.

* Wenn Sie eine Liste in eine Datei exportieren, wird die temporäre Reihenfolge der Spalten nicht in die exportierte Datei übertragen. Die exportierte Datei zeigt die Reihenfolge der Spalten in der ursprünglichen Liste an, bevor die Spalten neu angeordnet wurden.

Weitere Informationen zum Exportieren von Daten aus Listen und Berichten finden Sie im Artikel [Daten exportieren](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

#### Spaltengröße vorübergehend ändern {#resize-columns-temporarily}

1. Markieren Sie die Liste, die Sie ändern möchten.
1. Ziehen Sie den Rand einer Spaltenüberschrift, bis die Spalte die gewünschte Größe erreicht.\
   ![](assets/column-resize-350x124.png)

#### Spalten vorübergehend neu ordnen {#reorder-columns-temporarily}

1. Markieren Sie die Liste, die Sie ändern möchten.
1. Klicken Sie auf die Spaltenüberschrift, die Sie an die gewünschte Position verschieben möchten, und ziehen Sie sie.

>[!TIP]
>
>Dies ist besonders nützlich, wenn das Gantt-Diagramm und die Listenansicht gleichzeitig angezeigt werden. Beim Anzeigen des Gantt-Diagramms können Spalten ausgeblendet werden. Um eine Spalte anzuzeigen, während das Gantt-Diagramm angezeigt wird, ziehen Sie einfach die Spalte, die Sie anzeigen möchten, so, dass sie auf der linken Seite der Seite angezeigt wird.

### Breite und Reihenfolge der Spalten dauerhaft ändern {#modify-width-and-order-of-columns-permanently}

Informationen zum dauerhaften Neuanordnen von Spalten finden Sie im Abschnitt [Erstellen oder Anpassen einer Standardansicht](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view) im Artikel [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md) .

Sie können die Breite einer Spalte nur im Textmodus dauerhaft ändern.

Weitere Informationen zum Verwenden des Textmodus und zum dauerhaften Ändern der Breite einer Spalte finden Sie im Artikel [Überblick über die häufigsten Verwendungen für den Textmodus](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
