---
title: Datensätze bearbeiten
description: Sie können Datensatzinformationen in Adobe Maestro bearbeiten. Sie müssen Datensatztypen erstellen, bevor Sie mit der Erstellung und Bearbeitung von Datensätzen beginnen können.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: d9a8af627c8d3da4a7625cd5180bfca69da43b3d
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 1%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Datensätze bearbeiten

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Maestro, ein neues Angebot von Adobe Workfront.
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist. Sie müssen Workfront-Kunde sein, um Maestro-Funktionen verwenden zu können.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

Sie können Datensatzinformationen in Adobe Maestro bearbeiten. Sie müssen Datensatztypen erstellen, bevor Sie mit der Erstellung und Bearbeitung von Datensätzen beginnen können.
Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](../architecture/create-record-types.md).

&lt;!— Erwähnen Sie hier, dass die Felder in der Detailansicht mit denen in der Tabellenansicht identisch sind. Dieser Artikel ist über die Option Datensatzansichten verwalten verknüpft, um auf diese Informationen zu verweisen.—>

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produkt</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-Abkommen</p></td>
   <td>
<p>Ihr Unternehmen muss am Adobe Maestro Closed-Beta-Programm teilnehmen. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Abo</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td>
   <td>
   <p>Alle</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> <p>Es gibt keine Zugriffskontrollen für Maestro </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Beitragen oder höhere Berechtigungen zu einem Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Maestro-Bereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## Überlegungen zum Bearbeiten von Datensätzen

* Sie können von Ihnen oder einem anderen Benutzer erstellte Datensätze bearbeiten. <!--will change with access levels-->
* Felder, die mit anderen Datensätzen oder Feldern verknüpft sind, die Berechnungen enthalten, können nicht bearbeitet werden.
* Wenn die angezeigten Datensätze mit anderen Datensätzen verknüpft sind, werden die neuen Informationen der von Ihnen bearbeiteten Datensätze in den verknüpften Datensätzen angezeigt.
* Datensätze können nicht stapelweise bearbeitet werden. <!--this will probably change-->
* URLs werden nur dann als Links in einzeiligen Textfeldtypen erkannt, wenn sie mit den folgenden Begriffen beginnen: http://, https://, ftp:// oder www. .
* Sie können beim Bearbeiten eines Felds vom Typ &quot;Absatz&quot;die folgenden Rich-Text-Formatierungsoptionen verwenden:

   * Fett
   * Kursiv
   * Unterstreichen
   * Link hinzufügen
   * Liste mit Aufzählungszeichen hinzufügen
   * Nummerierte Liste hinzufügen

## Datensätze bearbeiten

Sie können einen Datensatz aus den folgenden Bereichen bearbeiten:

* [Auf der Detailseite eines Datensatzes](#edit-a-record-from-the-records-details-page)
* [Aus der Tabellenansicht eines Datensatztyps](#edit-a-record-from-the-table-view-of-a-record-type)

### Datensatz auf der Detailseite des Datensatzes bearbeiten

{{step1-to-maestro}}

Der Arbeitsbereich, auf den Sie zuletzt zugreifen, wird geöffnet.

1. (Optional) Klicken Sie auf den nach unten zeigenden Pfeil rechts neben dem Workspace-Namen, um den Arbeitsbereich auszuwählen, dessen Datensätze Sie aktualisieren möchten.
1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie in der Tabellenansicht auf den Namen eines Datensatzes.
   * Bewegen Sie in der Tabellenansicht den Mauszeiger über den Namen eines Datensatzes und klicken Sie auf die Schaltfläche **Mehr** Menü ![](assets/more-menu.png)Klicken Sie auf **Ansicht**

     ![](assets/contextual-menu-for-record-row.png)
   * Klicken Sie in einer Timeline-Ansicht auf eine Datensatzleiste.

   Der Datensatz **Details** Seite geöffnet.

1. Klicken Sie auf **Mehr** Menü ![](assets/more-menu.png) rechts neben dem Datensatznamen klicken Sie auf **Bearbeiten**

   Oder

   Klicken Sie auf der Detailseite in ein beliebiges bearbeitbares Feld, um die Informationen zu bearbeiten.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

1. Klicks **Änderungen speichern**. <!--logged a bug for this - this needs to be "Save"-->

### Datensatz in der Tabellenansicht eines Datensatztyps bearbeiten

{#step1-to-maestro}

Der zuletzt aufgerufene Arbeitsbereich wird geöffnet.

1. (Optional) Klicken Sie auf den nach unten zeigenden Pfeil rechts neben dem Workspace-Namen, um den Arbeitsbereich auszuwählen, dessen Datensätze Sie aktualisieren möchten.
1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. (Bedingt) Aus der **Ansicht** Dropdown-Menü in der oberen rechten Ecke der Tabelle auswählen Sie eine **Verzeichnis** anzeigen. Dies sollte die Standardansicht sein, es sei denn, Sie haben den Datensatztyp in der Timeline-Ansicht angezeigt, als Sie zuletzt darauf zugegriffen haben.

   Die mit dem ausgewählten Datensatztyp verknüpften Datensätze werden in der Tabellenansicht angezeigt.
1. Klicken Sie in die Zeile eines Datensatzes, um Informationen über den Datensatz inline zu bearbeiten.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)
1. Presse **Eingabe** auf der Tastatur oder klicken Sie außerhalb einer Zeile, um Ihre Änderungen zu speichern. Die Änderungen werden automatisch gespeichert. In der oberen rechten Ecke der Tabellenansicht wird eine Anzeige zum Speichern der Änderungen kurz angezeigt.

   >[!NOTE]
   >
   >  Sie können Informationen für die folgenden Felder nicht bearbeiten, da sie schreibgeschützt sind und Workfront sie automatisch aktualisiert:
   >  
   >  * Verknüpfte Felder, die durch Verbinden von Datensatztypen erstellt werden. Weitere Informationen finden Sie unter [Datensatztypen verbinden](../architecture/connect-record-types.md).
   >  * Felder der folgenden Typen: Erstellt von, Erstellungsdatum, Letzte Änderung durch, Datum der letzten Änderung


1. (Optional) Kopieren Sie einen oder mehrere vorhandene Werte eines Felds und fügen Sie sie dann in ein Feld desselben Typs in einen anderen Datensatz ein. Klicken Sie dann auf **Eingabe** auf der Tastatur, um Ihre Änderungen zu speichern.

   >[!NOTE]
   >
   >Beachten Sie Folgendes:
   >
   >* Es ist nicht möglich, Informationen aus anderen Quellen als einem Maestro-Feld des gleichen Typs zu kopieren wie das Feld, in das Sie die Informationen einfügen.
   >
   >* Sie können keine Feldwerte kopieren und in den Detailbereich eines Datensatzes einfügen. Diese Funktion wird nur in der Tabellenansicht eines Datensatztyps unterstützt.
   >* Für die folgenden Feldtypen können Sie keine Feldwerte kopieren und einfügen:
   >
   >
   >    * Verknüpfte Felder, die durch Verbinden von Datensatztypen erstellt werden. Sie können verknüpfte Datensatzfelder kopieren und einfügen. Weitere Informationen finden Sie unter [Datensatztypen verbinden](../architecture/connect-record-types.md).
   >    * Felder der folgenden Typen: Erstellt von, Erstellungsdatum, Letzte Änderung durch, Datum der letzten Änderung

1. (Optional) Verwenden Sie die folgenden Tastaturbefehle, um die Bearbeitung oder das Kopieren und Einfügen von Datensatzinformationen rückgängig zu machen oder wiederherzustellen:

   * STRG + Z ( ⌘ + Z für Mac) zum Rückgängigmachen einer Änderung
   * STRG + Umschalt + Z ( ⌘ + Umschalt + Z für Mac) zum Wiederholen einer Änderung
<!--
1. (Optional) Add a thumbnail to a record. For information, see [Add a thumbnail to a record](/help/quicksilver/maestro/records/add-thumbnail-to-a-record.md). -->
