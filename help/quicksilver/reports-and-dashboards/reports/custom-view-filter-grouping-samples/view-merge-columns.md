---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Zusammenführungsinformationen aus mehreren Spalten in einer gemeinsamen Spalte"
description: Sie können die Informationen, die in mehreren separaten Spalten angezeigt werden, zusammenführen und in einer gemeinsamen Spalte anzeigen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d4f9db12-59ce-4cfc-90dd-e611b49fafdf
source-git-commit: 976e8c7fe0362392928ac9cd6be1a9ba7c653dda
workflow-type: tm+mt
source-wordcount: '1023'
ht-degree: 0%

---

# Ansicht: Zusammenführen von Informationen aus mehreren Spalten in einer gemeinsamen Spalte

Sie können die Informationen, die in mehreren separaten Spalten angezeigt werden, zusammenführen und in einer gemeinsamen Spalte anzeigen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung zum Ändern einer Ansicht </p>
   <p>Berichtänderung planen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Überlegungen beim Freigeben oder Zusammenführen von Spalten

* Sie können zwei nebeneinander liegende Spalten zusammenführen und die Informationen aus den einzelnen Spalten durch einen Zeilenumbruch trennen. Alternativ können Sie die Informationen in zwei benachbarten Spalten ohne Trennzeichen zwischen den Informationen aus den einzelnen Spalten zusammenführen.
* Sie können die Informationen aus mehr als zwei Spalten zusammenführen, indem Sie die in diesem Artikel beschriebene Syntax auf eine bereits gemeinsam genutzte Spalte und eine angrenzende Spalte anwenden.
* Die `valueformat=HTML` in einer freigegebenen Spalte ist obligatorisch. Andernfalls enthalten die Spalten keine Informationen (sie sind leer), wenn der Bericht aus Adobe Workfront exportiert wird.
* Die bedingte Formatierung wird in zusammengeführten Spalten möglicherweise nicht unterstützt.

  Es gibt die folgenden Ausnahmen:

   * Bei der Anzeige von Informationen in Workfront wird die Formatierung der ersten Spalte beibehalten und die Formatierung für alle anderen Spalten wird ignoriert, wenn die Spalten, aus denen eine zusammengeführte Spalte besteht, unterschiedliche Formatierungen aufweisen.
   * Beim Exportieren der Ansicht in eine PDF-Datei gilt die bedingte Formatierung für die erste Spalte einer zusammengeführten Spalte.
   * Beim Exportieren der Ansicht in eine Excel-Datei werden zusammengeführte Spalten als separate Spalten angezeigt. Die einzelnen Spalten zeigen auch ihre jeweiligen bedingten Formatierungsregeln an.

* Spalten mit der **viewalias** -Attribut kann die Anzahl der Spalten begrenzen, die Sie zusammenführen können. Vermeiden Sie die Verwendung der **viewalias** -Attribut. Wenn Sie die Variable **viewalias** -Attribut in einer Spalte angeben, stellen Sie sicher, dass es sich um das letzte Element handelt, das in der Spalte aufgeführt ist.

* Wenn Sie eine Liste mit gemeinsamen Spalten in ein Excel- oder Tabulator-Format exportieren, werden diese Spalten in der exportierten Datei getrennt.

* Wenn eine oder beide Spalten eine `tile` Typ ein, wird automatisch ein Zeilenumbruch in die zusammengeführte Spalte eingefügt. Beispielsweise sind Textfelder mit Formatierung `tile` Typfelder. In diesem Fall gibt es einen Zeilencode von `type=tile` beim Anzeigen der Spalten im Textmodus.

## Zusammenführen von Daten aus zwei Spalten ohne Zeilenumbruch

Sie können die Daten aus mehreren separaten Spalten zusammenführen, um sie in einer Spalte ohne Umbrüche oder Leerzeichen zwischen den Werten der einzelnen Spalten anzuzeigen.

>[!TIP]
>
>Dieser Ansatz wird empfohlen, wenn Sie zwei Spalten zusammenführen, die nie einen Wert für denselben Datensatz gleichzeitig anzeigen können. Beispielsweise können in einem Arbeitselement-Bericht die Spalten &quot;Problemname&quot;und &quot;Aufgabenname&quot;ohne Zeilenumbruch zusammengeführt werden, da ein Arbeitselement nie einen Problemnamen und einen Aufgabennamen gleichzeitig haben kann. Ein Arbeitselement kann in Workfront entweder ein Problem oder eine Aufgabe sein.

Gehen Sie dazu folgendermaßen vor:

1. Fügen Sie im Textmodus für eine Ansicht den folgenden Text zur ersten Spalte hinzu, die Sie zusammenführen möchten:

   `sharecol=true`

   Wenn Sie die ersten beiden Spalten einer Liste oder eines Berichts zusammenführen, steht Workfront jeder Textzeile voran, die Informationen über das Objekt in der ersten Spalte mit `column.0.` und die Textzeilen, die Informationen über die zweite Spalte mit `column.1.` .

   Sie müssen der Spaltennummer der ersten Spalte die Nummer dieser Spalte voranstellen. Die Spaltenzählung beginnt immer mit der Spalte ganz links in der Liste oder im Bericht, die als `column.0.`.

   Wenn Sie mehr als eine Spalte freigeben, stellen Sie sicher, dass Sie die Spaltennummer in den Codezeilen hinzufügen, die die Freigabeinformationen für jede Spalte enthalten.

   **Beispiel:** Im Folgenden finden Sie den Textmoduscode für eine zusammengeführte Spalte, die drei separate Spalten enthält, beginnend mit der zweiten Spalte der Liste. Die zusammengeführten Werte sind &quot;Projektname&quot;, &quot;Geplantes Startdatum&quot;und &quot;Name des Projekteigentümers&quot;. Zwischen den drei Werten gibt es keinen Umbruch:

   `column.1.valuefield=name`

   `column.1.valueformat=HTML`

   `column.1.sharecol=true`

   `column.2.valuefield=plannedStartDate`

   `column.2.valueformat=atDate`

   `column.2.sharecol=true`

   `column.3.valuefield=owner:name`

   `column.3.valueformat=HTML`

![](assets/shared-column-no-line-breaks-350x142.png)

1. Klicken **Speichern**, dann **Ansicht speichern**.

## Zusammenführen von Daten aus zwei Spalten mit einem Zeilenumbruch

Führen Sie die folgenden Schritte aus, um die Daten aus mehreren Spalten zusammenzuführen und in einer gemeinsamen Spalte mit einem Zeilenumbruch zwischen den Werten der einzelnen Spalten anzuzeigen:

1. Fügen Sie zwischen den beiden Spalten, die Sie zusammenführen möchten, eine dritte Spalte hinzu.

   >[!TIP]
   >
   >* Die Spalten, die Sie zusammenführen möchten, müssen nebeneinander liegen.
   >* Sie müssen auf die erste Spalte klicken, die Sie zusammenführen möchten.

1. Klicken **In den Textmodus wechseln** und fügen Sie in der mittleren Spalte, die Sie in Schritt 1 hinzugefügt haben, den folgenden Code hinzu:

   `value=<br>`

   `valueformat=HTML`

   `width=1`

   `sharecol=true`


1. Fügen Sie der ersten Spalte den folgenden Text hinzu:

   `sharecol=true`

   Wenn Sie die ersten beiden Spalten einer Liste oder eines Berichts zusammenführen, steht Workfront jeder Textzeile voran, die Informationen über das Objekt in der ersten Spalte mit `column.0.`, die Spalte mit den Informationen, die für `column.1.`und die Textzeilen, die Informationen über die zweite Spalte mit `column.2.`.

   Wenn sich die kombinierte Spalte in der Mitte der Ansicht befindet, werden die Spalten entsprechend ihrer Position in der Ansicht nummeriert. Die Spaltenzählung beginnt immer mit der Spalte ganz links in der Liste oder im Bericht, die als `column.0.`.

   Wenn Sie mehr als eine Spalte freigeben, stellen Sie sicher, dass Sie die Spaltennummer in den Codezeilen hinzufügen, die die Freigabeinformationen enthalten.

   **Beispiel:** Im Folgenden finden Sie den Textmoduscode für eine freigegebene Spalte, die den Projektnamen, das geplante Startdatum und den Namen des Projektinhabers mit einem Zeilenumbruch enthält. Die freigegebene Spalte ist die zweite Spalte einer Projektansicht.


   `column.1.displayname=Project_StartDate_Owner`

   `column.1.sharecol=true`

   `column.1.textmode=true`

   `column.1.valuefield=name`

   `column.1.valueformat=HTML`

   `column.2.value=<br>`

   `column.2.width=1`

   `column.2.valueformat=HTML`

   `column.2.sharecol=true`

   `column.3.valuefield=plannedStartDate`

   `column.3.valueformat=atDate`

   `column.3.sharecol=true`

   `column.4.value=<br>`

   `column.4.width=1`

   `column.4.valueformat=HTML`

   `column.4.sharecol=true`

   `column.5.textmode=true`

   `column.5.valuefield=owner:name`

   `column.5.valueformat=HTML`


   ![](assets/shared-column-with-line-breaks-350x199.png)


1. Klicken **Speichern**, dann **Ansicht speichern**.
