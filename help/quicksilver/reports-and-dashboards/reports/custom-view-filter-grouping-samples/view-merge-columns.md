---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Informationen aus mehreren Spalten in einer gemeinsamen Spalte zusammenführen'
description: Sie können die Informationen, die in mehreren separaten Spalten angezeigt werden, zusammenführen und in einer gemeinsamen Spalte anzeigen.
author: Nolan
feature: Reports and Dashboards
exl-id: d4f9db12-59ce-4cfc-90dd-e611b49fafdf
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1070'
ht-degree: 0%

---

# Ansicht: Zusammenführen von Informationen aus mehreren Spalten in einer gemeinsamen Spalte

<!-- Audited: 11/2024 -->

Sie können die Informationen, die in mehreren separaten Spalten angezeigt werden, zusammenführen und in einer gemeinsamen Spalte anzeigen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Mitwirkender oder Anfrage zum Ändern einer Ansicht </p>
   <p>Standard oder Plan zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Überlegungen beim Freigeben oder Zusammenführen von Spalten

* Sie können zwei benachbarte Spalten zusammenführen und die Informationen aus jeder Spalte anzeigen, die durch einen Zeilenumbruch getrennt sind, oder Sie können die Informationen in zwei benachbarten Spalten zusammenführen, ohne ein Trennzeichen zwischen den Informationen aus jeder Spalte zu verwenden.
* Sie können die Informationen aus mehr als zwei Spalten zusammenführen, indem Sie die in diesem Artikel beschriebene Syntax auf eine bereits freigegebene Spalte und eine angrenzende Spalte anwenden.
* Die `valueformat=HTML` ist in einer freigegebenen Spalte obligatorisch. Andernfalls enthalten die Spalten keine Informationen (sie sind leer), wenn der Bericht aus Adobe Workfront exportiert wird.
* Bedingte Formatierung wird in zusammengeführten Spalten möglicherweise nicht unterstützt.

  Die folgenden Ausnahmen sind vorhanden:

   * Beim Anzeigen von Informationen in Workfront wird die Formatierung der ersten Spalte beibehalten und die Formatierung für alle anderen Spalten wird ignoriert, wenn die Spalten, aus denen eine zusammengeführte Spalte besteht, unterschiedliche Formatierungen aufweisen.
   * Beim Exportieren der Ansicht in eine PDF-Datei wird die bedingte Formatierung auf die erste Spalte in einer zusammengeführten Spalte angewendet.
   * Beim Exportieren der Ansicht in eine Excel-Datei werden zusammengeführte Spalten als separate Spalten angezeigt. Die einzelnen Spalten zeigen auch ihre jeweiligen bedingten Formatierungsregeln an.

* Spalten mit dem **viewAlias**-Attribut können die Anzahl der Spalten begrenzen, die zusammengeführt werden können. Um diese Einschränkungen zu vermeiden, vermeiden Sie die Verwendung des **viewalias**-Attributs. Wenn Sie das Attribut **viewalias** in eine Spalte einbeziehen müssen, stellen Sie sicher, dass dies das letzte in der Spalte aufgeführte Element ist.

* Wenn Sie eine Liste mit freigegebenen Spalten in ein durch Excel- oder Tabulatoren getrenntes Format exportieren, werden diese Spalten in der exportierten Datei getrennt.

* Wenn eine oder beide Spalten ein Feld vom Typ `tile` anzeigen, wird automatisch ein erzwungener Zeilenumbruch in die zusammengeführte Spalte eingefügt. Beispielsweise sind Textfelder mit Formatierung Felder vom Typ `tile`. In diesem Fall gibt es einen Zeilen-Code von `type=tile`, wenn die Spalten im Textmodus angezeigt werden.

## Zusammenführen von Daten aus zwei Spalten ohne Zeilenumbruch

Sie können die Daten aus mehreren separaten Spalten zusammenführen, um sie in einer Spalte ohne Umbrüche oder Leerzeichen zwischen den Werten aus den einzelnen Spalten anzuzeigen.

>[!TIP]
>
>Dieser Ansatz wird empfohlen, wenn Sie zwei Spalten zusammenführen, die nie gleichzeitig einen Wert für denselben Datensatz anzeigen können. Beispielsweise können in einem Arbeitsaufgabenbericht die Spalten „Anfragename“ und „Aufgabenname“ ohne Zeilenumbruch zusammengeführt werden, da ein Arbeitselement nie gleichzeitig einen Anfragenamen und einen Aufgabennamen haben kann. Ein Arbeitselement kann in Workfront entweder ein Problem oder eine Aufgabe sein.

So führen Sie Daten aus zwei Spalten ohne Zeilenumbruch zusammen:

1. Navigieren Sie zu einer Liste von Objekten.
1. Wählen Sie aus **Dropdown** Liste Ansicht eine Ansicht aus und klicken Sie dann auf das **Bearbeiten**-Symbol ![Bearbeiten](assets/edit-icon.png), um die Ansicht zu bearbeiten.
1. Wechseln Sie zur ersten Spalte, die Sie zusammenführen möchten, und klicken Sie dann auf **In Textmodus wechseln** > **Textmodus bearbeiten**.
1. Fügen Sie der ersten Spalte, die Sie zusammenführen möchten, folgenden Text hinzu:

   `sharecol=true`

   Wenn Sie die ersten beiden Spalten einer Liste oder eines Berichts zusammenführen, geht Workfront jeder Textzeile, die Informationen über das -Objekt in der ersten Spalte enthält, mit `column.0.` und den Textzeilen, die Informationen über die zweite Spalte enthalten, mit `column.1.` voran.

   Sie müssen der Spaltennummer der ersten Spalte die Nummer dieser Spalte voranstellen. Die Spaltenzählung beginnt immer mit der Spalte ganz links in der Liste oder dem Bericht, die bzw. der als `column.0.` gekennzeichnet ist.

   Wenn Sie mehr als eine Spalte gemeinsam verwenden, fügen Sie die Spaltennummer unbedingt in die Codezeilen ein, die die Freigabeinformationen für jede Spalte enthalten.


   **Beispiel:** Im Folgenden finden Sie den Textmodus-Code für eine zusammengeführte Spalte, die drei separate Spalten enthält, beginnend mit der zweiten Spalte der Liste. Die zusammengeführten Werte sind Projektname, Geplantes Startdatum und Name des Projektbesitzers. Es gibt keinen Bruch zwischen den drei Werten:

   ```
   column.1.valuefield=name
   column.1.valueformat=HTML
   column.1.sharecol=true
   column.2.valuefield=plannedStartDate
   column.2.valueformat=atDate
   column.2.sharecol=true
   column.3.valuefield=owner:name
   column.3.valueformat=HTML
   ```

   ![Freigegebene Spalte ohne Zeilenumbrüche](assets/shared-column-no-line-breaks-350x142.png)


1. Klicken Sie **Fertig** und dann **Ansicht speichern**.

## Zusammenführen von Daten aus zwei Spalten mit einem Zeilenumbruch

Führen Sie die folgenden Schritte aus, um die Daten aus mehreren Spalten zusammenzuführen und in einer gemeinsamen Spalte mit einem Zeilenumbruch zwischen den Werten jeder Spalte anzuzeigen:

1. Navigieren Sie zu einer Liste von Objekten.
1. Wählen Sie aus **Dropdown** Liste Ansicht eine Ansicht aus und klicken Sie dann auf das **Bearbeiten**-Symbol ![Bearbeiten](assets/edit-icon.png), um die Ansicht zu bearbeiten.
1. Fügen Sie zwischen den beiden Spalten, die Sie zusammenführen möchten, eine dritte Spalte hinzu.

   >[!TIP]
   >
   >* Die Spalten, die zusammengeführt werden sollen, müssen nebeneinander liegen.
   >* Sie müssen auf die erste Spalte klicken, die Sie zusammenführen möchten.

1. Klicken Sie **Wechseln Sie in den Textmodus** > **Textmodus bearbeiten** und fügen Sie den folgenden Code in der mittleren Spalte hinzu, die Sie in Schritt 1 hinzugefügt haben:

   ```
   value=<br>
   valueformat=HTML
   width=1
   sharecol=true
   ```

1. Klicken Sie auf die erste Spalte und klicken Sie **Wechseln in den Textmodus** > **Textmodus bearbeiten** und fügen Sie dann der Spalte den folgenden Text hinzu:

   `sharecol=true`

   Wenn Sie die ersten beiden Spalten einer Liste oder eines Berichts zusammenführen, geht Workfront jeder Textzeile, die Informationen über das Objekt in der ersten Spalte enthält, mit `column.0.`, der Spalte mit den Freigabeinformationen für `column.1.` und den Textzeilen, die Informationen über die zweite Spalte mit `column.2.` enthalten, voran.

   Wenn sich die kombinierte Spalte in der Mitte der Ansicht befindet, werden die Spalten entsprechend ihrer Position in der Ansicht nummeriert. Die Spaltenzählung beginnt immer mit der Spalte ganz links in der Liste oder dem Bericht, die bzw. der als `column.0.` gekennzeichnet ist.

   Wenn Sie mehr als eine Spalte gemeinsam verwenden, fügen Sie die Spaltennummer unbedingt in die Codezeilen ein, die die Freigabeinformationen enthalten.

   **Beispiel:** Im Folgenden finden Sie den Textmodus-Code für eine freigegebene Spalte, die den Projektnamen, das geplante Startdatum und den Namen des Projektbesitzers mit einem Zeilenumbruch enthält. Die Spalte Freigegeben ist die zweite Spalte einer Projektansicht.

   ```
   column.1.displayname=Project_StartDate_Owner
   column.1.sharecol=true
   column.1.textmode=true
   column.1.valuefield=name
   column.1.valueformat=HTML
   column.2.value=<br>
   column.2.width=1
   column.2.valueformat=HTML
   column.2.sharecol=true
   column.3.valuefield=plannedStartDate
   column.3.valueformat=atDate
   column.3.sharecol=true
   column.4.value=<br>
   column.4.width=1
   column.4.valueformat=HTML
   column.4.sharecol=true
   column.5.textmode=true
   column.5.valuefield=owner:name
   column.5.valueformat=HTML 
   ```

   ![Freigegebene Spalte mit Zeilenumbrüchen](assets/shared-column-with-line-breaks-350x199.png)

1. Klicken Sie **Fertig** und dann **Ansicht speichern**.
