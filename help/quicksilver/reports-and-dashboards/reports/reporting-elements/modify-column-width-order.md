---
product-area: reporting
navigation-topic: reporting-elements
title: Spaltenbreite und -reihenfolge ändern
description: Lesen Sie diesen Artikel, um mehr über Richtlinien zur Spaltenbreite und darüber zu erfahren, wie die Spaltenbreite und -reihenfolge in Workfront geändert werden.
author: Nolan
feature: Reports and Dashboards
exl-id: ece3f908-a0da-45d4-9f4f-0b34c69ce8fa
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '990'
ht-degree: 0%

---

# Spaltenbreite und -reihenfolge ändern

Im Folgenden finden Sie Richtlinien zur Funktionsweise von Spaltenbreiten in Adobe Workfront:

* Workfront definiert standardmäßig die Spaltenbreite in Listen und Berichten.
* Workfront passt die Spaltenbreite automatisch an die `valueformat`Informationen in allen Listen und Berichten, sofern im Textmodus der Spalte nichts anderes angegeben ist.

   >[!NOTE]
   >
   >Workfront passt die Spaltenbreite nicht an die `valueformat` Informationen in den Listen, die in den Bereichen Einrichtung und Berichte verfügbar sind.

   Die `valueformat` -Wert definiert, welche Art von Informationen in der Spalte angezeigt werden. Beispielsweise sind Spalten, die eine Zahl anzeigen, enger als Spalten, in denen das Feld Beschreibung angezeigt wird.

* Sie können die Spaltenbreite in Ihren Workfront-Listen und -Berichten an Ihre Anforderungen anpassen, je nachdem, welche Art von Informationen in Spalten angezeigt werden soll.

   Sie können die Breite der Spalten vorübergehend ändern, während Sie eine Liste, einen Bericht oder einen Bericht anzeigen, oder dauerhaft, indem Sie die Breite der Spalte im Ansichtsaufbau anpassen. Informationen zum temporären Ändern der Spaltenbreite finden Sie unter [Überlegungen beim zeitweiligen Ändern der Breite und Reihenfolge der Spalten](#considerations-when-temporarily-modifying-the-width-and-order-of-columns) in diesem Artikel.

* Spalten, die in integrierten Ansichten angezeigt werden, haben Breiten, die zuvor von Workfront definiert wurden und hartcodiert sind. Um diese Breiten zu ändern, müssen Sie die Breite dieser Spalten mithilfe des Textmodus im Ansichts-Builder manuell aktualisieren.

   Informationen zum Ändern der Spalte im Textmodus finden Sie unter [Ansicht: Spaltenbreite dauerhaft bearbeiten](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-edit-column-width-permanently.md).

## Zugriffsanforderungen

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
   <td> <p>Anforderung oder höher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um die Ansicht in einem Bericht zu bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>Berechtigungen für einen Bericht zum Bearbeiten einer Ansicht in einem Bericht verwalten</p> <p>Berechtigungen für eine Ansicht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Spaltenbreite und -reihenfolge ändern

Sie können die Breite und Reihenfolge der Spalten in Ihren Berichten wie folgt ändern:

* [Länge und Reihenfolge der Spalten vorübergehend ändern](#modify-width-and-order-of-columns-temporarily)
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
* Bei der Neuanordnung von Spalten wird die von Ihnen gewählte Reihenfolge nur beibehalten, bis Sie von der Liste weg navigieren oder die Browser-Seite aktualisieren. Nachdem Sie von der Liste weg navigiert oder die Browser-Seite aktualisiert haben, kehren die Spalten zur Standardreihenfolge zurück.
* Um eine optimale Leistung zu erzielen, sollten die neu anzuordnenden Spalten nicht mehr als 100 Elemente in der Liste enthalten.
* Wenn Sie die Größe von Spalten ändern, gelten Ihre Änderungen nur für die derzeit verwendete Ansicht und sind nur für Sie sichtbar. Wenn Sie eine Ansicht für einen anderen Benutzer freigeben, werden die von Ihnen definierten Spaltengrößen nicht gemeinsam verwendet.
* Wenn Sie die Größe einer Spalte durch Ziehen des Rahmens nach rechts ändern, bleibt die Breite der benachbarten Spalte erhalten, mit Ausnahme der folgenden:

   * Der Einrichtungsbereich
   * Der Bereich &quot;Berichte&quot;
   * Dokumentlisten und Berichte

   >[!NOTE]
   >
   >Der linke Rand einer Spalte kann in keiner Liste über den linken Rand der benachbarten Spalte verschoben werden.

* Wenn Sie eine Liste in eine Datei exportieren, wird die temporäre Reihenfolge der Spalten nicht in die exportierte Datei übertragen. Die exportierte Datei zeigt die Reihenfolge der Spalten in der ursprünglichen Liste an, bevor die Spalten neu angeordnet wurden.

Weitere Informationen zum Exportieren von Daten aus Listen und Berichten finden Sie im Artikel [Daten exportieren](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

#### Spaltengröße vorübergehend ändern {#resize-columns-temporarily}

1. Markieren Sie die Liste, die Sie ändern möchten.
1. Ziehen Sie den Rand einer Spalte, bis die Spalte die gewünschte Größe erreicht.\
   ![](assets/column-resize-350x124.png)

#### Spalten vorübergehend neu ordnen {#reorder-columns-temporarily}

1. Markieren Sie die Liste, die Sie ändern möchten.
1. Klicken Sie auf eine Spalte, die Sie an eine andere Position verschieben möchten, um die Spalte auszuwählen.
1. Ziehen Sie die Spalte an die richtige Position.
1. Ziehen Sie die Spalte an die gewünschte Position, um sie zu verschieben.

   ![](assets/column-reorder-350x118.png)

>[!TIP]
>
>Dies ist besonders nützlich, wenn das Gantt-Diagramm und die Listenansicht gleichzeitig angezeigt werden. Beim Anzeigen des Gantt-Diagramms können Spalten ausgeblendet werden. Um eine Spalte anzuzeigen, während das Gantt-Diagramm angezeigt wird, ziehen Sie einfach die Spalte, die Sie anzeigen möchten, so, dass sie auf der linken Seite der Seite angezeigt wird.

### Breite und Reihenfolge der Spalten dauerhaft ändern {#modify-width-and-order-of-columns-permanently}

Informationen zum dauerhaften Neuanordnen von Spalten finden Sie im Abschnitt . [Standardansicht erstellen oder anpassen](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-a-standard-view) im Artikel [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Sie können die Breite einer Spalte nur im Textmodus dauerhaft ändern.

Weitere Informationen zum Verwenden des Textmodus und zum dauerhaften Ändern der Breite einer Spalte finden Sie im Artikel [Übersicht über die häufigsten Verwendungen für den Textmodus](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md).
