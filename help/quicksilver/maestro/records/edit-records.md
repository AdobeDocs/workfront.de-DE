---
title: Datensätze bearbeiten
description: Sie können Datensatzinformationen in den Planungsfunktionen von Adobe Workfront bearbeiten. Sie müssen Datensatztypen erstellen, bevor Sie mit der Erstellung und Bearbeitung von Datensätzen beginnen können.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: e881aa57b5175ce5b559180a2713de0c607b3b1d
workflow-type: tm+mt
source-wordcount: '1337'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Datensätze bearbeiten

{{maestro-important-intro}}

Sie können Datensatzinformationen in den Planungsfunktionen von Adobe Workfront bearbeiten, indem Sie die Werte der mit den Datensätzen verknüpften Felder bearbeiten.

Sie müssen Datensatztypen erstellen, bevor Sie mit der Erstellung und Bearbeitung von Datensätzen beginnen können.

Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](../architecture/create-record-types.md).

Informationen zum Erstellen von Datensätzen finden Sie unter [Datensätze erstellen](/help/quicksilver/maestro/records/create-records.md).

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
<p>Ihr Unternehmen muss am geschlossenen Betaprogramm für Planungsfunktionen der Adobe Workfront teilnehmen. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Abo</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td>
   <td>
   <p>Neu: Licht oder höher</p>
   Oder
   <p>Aktuell: Arbeit oder höher</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> <p>Es gibt keine Zugriffskontrollen für Adobe Workfront-Planungsfunktionen </p>  
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

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Überlegungen zum Bearbeiten von Datensätzen

* Sie können von Ihnen erstellte Datensätze oder von anderen Benutzern erstellte Datensätze bearbeiten, wenn Sie über Berechtigungen für den Arbeitsbereich verfügen.
* Sie können Datensatzfelder aus den folgenden Bereichen bearbeiten:

   * Das Feld Details eines Datensatzes aus einer Datensatzansicht.
   * Die Detailseite eines Datensatzes.
   * Inline in einer Tabellenansicht.

* Die folgenden Feldtypen werden automatisch aktualisiert und ihre Werte können nicht manuell bearbeitet werden:
   * Verknüpfte Felder anderer Datensätze
   * Felder vom Typ Formel
   * Systemfelder (erstellt von, Erstellungsdatum, Letzte Änderung durch, Datum der letzten Änderung)
* Wenn die angezeigten Datensätze mit anderen Datensätzen verknüpft sind, werden die neuen Informationen der von Ihnen bearbeiteten Datensätze in den verknüpften Datensätzen angezeigt.
* Datensätze können nicht stapelweise bearbeitet werden. <!--this will probably change-->
* URLs werden nur dann als Links in einzeiligen Textfeldtypen erkannt, wenn sie mit den folgenden Begriffen beginnen: http://, https://, ftp:// oder www. .

## Datensätze bearbeiten

Sie können einen Datensatz aus den folgenden Bereichen bearbeiten:

* [Aus der Tabellenansicht eines Datensatztyps](#edit-a-record-from-the-table-view-of-a-record-type)
* [Auf der Detailseite eines Datensatzes](#edit-a-record-from-the-records-details-page)

### Datensatz in der Tabellenansicht eines Datensatztyps inline bearbeiten

{#step1-to-maestro}

Der zuletzt aufgerufene Arbeitsbereich wird geöffnet.

1. (Optional) Klicken Sie auf den nach unten zeigenden Pfeil rechts neben dem Workspace-Namen, um den Arbeitsbereich auszuwählen, dessen Datensätze Sie aktualisieren möchten.
1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. (Bedingt) Klicken Sie auf die Registerkarte einer Tabellenansicht oder auf **+ Ansicht** , um eine Tabellenansicht zu erstellen. Die Tabellenansicht sollte die Standardansicht sein, es sei denn, Sie haben den Datensatztyp beim letzten Zugriff in einer anderen Ansicht angezeigt.

   Die mit dem ausgewählten Datensatztyp verknüpften Datensätze werden in der Tabellenansicht angezeigt.
1. Klicken Sie in die Zeile eines Datensatzes, um Informationen über den Datensatz inline zu bearbeiten.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)

   >[!NOTE]
   >
   >  Sie können Informationen für die folgenden Felder nicht bearbeiten, da sie schreibgeschützt sind und Workfront sie automatisch aktualisiert:
   >  
   >  * Verknüpfte Felder, die durch Verbinden von Datensatztypen erstellt werden. Weitere Informationen finden Sie unter [Datensatztypen verbinden](../architecture/connect-record-types.md).
   >  * Felder der folgenden Typen: Erstellt von, Erstellungsdatum, Letzte Änderung durch, Letztes Änderungsdatum, Formelfelder.

1. (Optional und bedingt) Wenn Sie ein Feld vom Typ Absatz bearbeiten, verwenden Sie Folgendes **Rich-Text** Formatierungsoptionen:

   * Fett
   * Kursiv
   * Unterstreichen
   * Link hinzufügen
   * Liste mit Aufzählungszeichen hinzufügen
   * Nummerierte Liste hinzufügen

   ![](assets/rich-text-toolbar-on-paragraph-field.png)

1. (Optional) Doppelklicken Sie auf ein Feld für einen verbundenen Datensatz, um verbundene Datensätze oder Objekte zu einem anderen Datensatz hinzuzufügen. Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/maestro/records/connect-records.md).
1. Presse **Eingabe** auf der Tastatur oder klicken Sie außerhalb einer Zeile, um Ihre Änderungen zu speichern. Die Änderungen werden automatisch gespeichert. A **Gespeichert** wird in der oberen rechten Ecke der Tabellenansicht kurz angezeigt, um zu zeigen, dass die Änderungen gespeichert wurden.


1. (Optional) Um Informationen von einem Feld in ein anderes zu kopieren und einzufügen, führen Sie einen der folgenden Schritte aus:

   * Kopieren Sie einen oder mehrere vorhandene Werte eines Felds und fügen Sie sie dann in ein Feld desselben Typs in einen anderen Datensatz ein.
   * Klicken Sie auf die Spaltenüberschrift einer Spalte, um sie auszuwählen und zu kopieren. Klicken Sie dann auf die Spaltenüberschrift einer anderen Spalte und fügen Sie den Inhalt der kopierten Spalte ein. Die Spalten müssen ähnliche Feldtypen enthalten.
   * Klicken Sie bei gedrückter Umschalt-Taste auf mehrere Zeilen in einer Tabelle, kopieren Sie die Informationen in die ausgewählten Zeilen, klicken Sie dann auf eine andere Zeile und fügen Sie die ausgewählten Informationen in die neue Zeile und die folgenden Zeilen ein.

   >[!NOTE]
   >
   >Beachten Sie Folgendes:
   >
   >* Verwenden Sie die folgenden Tastaturbefehle zum Kopieren und Einfügen von Informationen:
   >   * Kopieren: STRG + C ( ⌘ + C für Mac)
   >   * Einfügen: STRG + V ( ⌘ + V für Mac)
   >* Es ist nicht möglich, Informationen aus anderen Quellen als Datensatzfeldern des gleichen Typs zu kopieren wie aus dem Feld, in das Sie die Informationen einfügen.
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

   >[!TIP]
   >
   >    Sie können die Tastaturbefehle mehrmals hintereinander verwenden, um mehrere Änderungen rückgängig zu machen.

1. (Optional) Fügen Sie einem Datensatz eine Miniaturansicht hinzu. Weitere Informationen finden Sie unter [Hinzufügen einer Miniaturansicht zu einem Datensatz](/help/quicksilver/maestro/records/add-thumbnails-to-records.md).

### Datensatz im Feld Details des Datensatzes in einer Ansicht bearbeiten

Sie können einen Datensatz in jeder Ansicht über das Feld Details bearbeiten.

{{step1-to-maestro}}

Der Arbeitsbereich, auf den Sie zuletzt zugreifen, wird geöffnet.

1. (Optional) Klicken Sie auf den nach unten zeigenden Pfeil rechts neben dem Workspace-Namen, um den Arbeitsbereich auszuwählen, dessen Datensätze Sie aktualisieren möchten.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes.

   Oder

   Klicken Sie in der Tabellenansicht auf die **Details öffnen** icon ![](assets/open-details-icon-in-table-name-field.png) auf der linken Seite eines Datensatznamens oder klicken Sie auf einen Datensatznamen. Die **Details** wird in der Ansicht geöffnet.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >Sie können die **Details öffnen** Symbol links neben dem Feld &quot;Name&quot;eines Datensatzes in einer Tabellenansicht nur dann angezeigt, wenn das Feld &quot;Name&quot;ein primäres Feld ist.

1. Beginnen Sie mit der Bearbeitung der Feldinformationen im **Details** ankreuzen. Workfront speichert Ihre Änderungen automatisch.

1. (Optional) Klicken Sie auf die **In neuer Registerkarte öffnen** icon ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in der oberen rechten Ecke des **Details** zum Öffnen des Datensatzes **Details** in einer neuen Registerkarte. Bearbeiten Sie den Datensatz weiter wie unter [Datensatz auf der Detailseite des Datensatzes bearbeiten](#edit-a-record-from-the-records-details-page) in diesem Artikel beschrieben.

### Datensatz auf der Detailseite des Datensatzes bearbeiten

Sie können einen Datensatz auf der Detailseite bearbeiten.

{{step1-to-maestro}}

Der Arbeitsbereich, auf den Sie zuletzt zugreifen, wird geöffnet.

1. (Optional) Klicken Sie auf den nach unten zeigenden Pfeil rechts neben dem Workspace-Namen, um den Arbeitsbereich auszuwählen, dessen Datensätze Sie aktualisieren möchten.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. Führen Sie einen der folgenden Schritte aus:

   * Rufen Sie in jeder Ansicht das Feld Details auf, wie im Abschnitt [Datensatz im Feld Details des Datensatzes in einer Ansicht bearbeiten](#edit-a-record-from-the-records-details-box-in-a-view)in diesem Artikel beschrieben. Klicken Sie dann auf die **In neuer Registerkarte öffnen** icon ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in der oberen rechten Ecke des **Details** zum Öffnen des Datensatzes **Details** in einer neuen Registerkarte.

   * Aus dem **Verzeichnis** Ansicht, bewegen Sie den Mauszeiger über den Namen eines Datensatzes und klicken Sie auf die Schaltfläche **Mehr** Menü ![](assets/more-menu.png)Klicken Sie auf **Ansicht**

     ![](assets/contextual-menu-for-record-row.png)

     Der Datensatz **Details** Seite geöffnet.

     ![](assets/details-page.png)

1. Klicken Sie auf **Mehr** Menü ![](assets/more-menu.png) rechts neben dem Datensatznamen klicken Sie auf **Bearbeiten**

   Oder

   Klicken Sie auf der Detailseite in ein beliebiges bearbeitbares Feld, um die Informationen zu bearbeiten.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

1. Klicks **Änderungen speichern**.