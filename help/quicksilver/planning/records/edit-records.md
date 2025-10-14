---
title: Datensätze bearbeiten
description: Datensatzinformationen können in Adobe Workfront Planning bearbeitet werden. Sie müssen Datensatztypen erstellen, bevor Sie Datensätze erstellen und bearbeiten können.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 7d37481fc5b468f6f8ea1fce6ccd7ae064f00251
workflow-type: tm+mt
source-wordcount: '2764'
ht-degree: 0%

---


# Datensätze bearbeiten

<!--keep the choice values information in yellow till Jan 2026-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Datensatzinformationen können in Adobe Workfront Planning bearbeitet werden, indem die Werte der Felder bearbeitet werden, die mit den Datensätzen verknüpft sind.

Sie müssen Datensatztypen erstellen, bevor Sie Datensätze erstellen und bearbeiten können.

Weitere Informationen finden Sie [Datensatztypen erstellen](/help/quicksilver/planning/architecture/create-record-types.md).

Weitere Informationen zum Erstellen von Datensätzen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).

&lt;!— Erwähnen Sie hier, dass die Felder in der Detailansicht mit denen in der Tabellenansicht übereinstimmen — dieser Artikel ist mit der Liste Datensatzansichten verwalten verlinkt, um auf diese Informationen zu verweisen—>

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produkte</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront-Planung<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Plan*</p></td> 
   <td> 
<p>Einer der folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning ist nicht für ältere Workfront-Pläne verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td> 
   <td> 
<p>Beliebig </p> 
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen erhalten Sie von Ihrem Workfront Account Manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Um auf Workfront Planning zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td> <p>Standard</p> 
   <p>Workfront Planning ist nicht für ältere Workfront-Lizenzen verfügbar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>  <p>Beitragen oder höhere Berechtigungen für einen Arbeitsbereich und Datensatztyp </a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr>

</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Überlegungen zum Bearbeiten von Datensätzen

* Sie können von Ihnen erstellte oder von anderen erstellte Datensätze bearbeiten, wenn Sie über Berechtigungen für den Arbeitsbereich verfügen.
* Datensatzfelder können aus den folgenden Bereichen bearbeitet werden:

   * Vorschau des Datensatzes in einer Datensatzansicht
   * Die Detailseite des Datensatzes
   * Inline, in einer Tabellenansicht.
   * <span class="preview"> Die Kalender- und Timeline-Ansicht bei der Größenänderung <!--or dragging and dropping--> Datensätze. Dadurch werden die Daten der Datensätze aktualisiert.</span>

* Wenn ein(e) Benutzende(r) einen Datensatz in einer Ansicht bearbeitet, sind die Änderungen sofort in allen Ansichten und auf den Datensatzseiten für alle anderen Benutzenden sichtbar.

* Die folgenden Feldtypen werden automatisch aktualisiert und Sie können ihre Werte nicht manuell bearbeiten:
   * Verknüpfte Felder aus anderen Datensätzen
   * Felder vom Typ Formel
   * Systemfelder (Erstellt von, Erstellt am, Zuletzt geändert von, Zuletzt geändert am)
* Wenn die angezeigten Datensätze mit anderen Datensätzen verknüpft sind, spiegeln die neuen Informationen der Datensätze, die Sie bearbeiten, die verknüpften Datensätze wider.
* Einträge können nicht stapelweise bearbeitet werden. <!--this will probably change-->
* URLs werden nur dann als Links in einzeiligen Textfeldtypen erkannt, wenn sie mit dem Folgenden beginnen: http://, https://, ftp:// oder www. .
* Sie können jedem Datensatz ein Cover-Bild hinzufügen. Das Bild ist für jeden Datensatz eindeutig und gilt nicht für alle Datensätze gleichzeitig.
* Sie können die Reihenfolge der Felder auf einer Datensatzseite bearbeiten und ein Titelbild für einen Datensatz hinzufügen. Weitere Informationen finden Sie unter [Seitenlayout für Einträge verwalten](/help/quicksilver/planning/records/manage-the-record-page.md).

## Datensätze bearbeiten

Sie können einen Datensatz aus den folgenden Bereichen bearbeiten:

* [Die Tabellenansicht](#edit-a-record-inline-in-the-table-view-of-a-record-type)
* [Die Zeitleisten -Ansicht](#edit-a-record-in-the-timeline-view-of-a-record-type)
* [Die Kalenderansicht](#edit-a-record-in-the-calendar-view-of-a-record-type)
* [Vorschau des Datensatzes in einer Ansicht](#edit-a-record-from-the-records-preview-in-a-view)
* [Die Seite des Datensatzes](#edit-a-record-from-the-records-page)
* [Ein Workfront-Objekt im Planungsabschnitt](#edit-a-record-from-a-workfront-object-in-the-planning-section)

Um die Daten der Datensätze zu bearbeiten, gehen Sie wie folgt vor:

* [Ändern Sie die Größe der Balken der Datensätze in der Zeitleisten- und Kalenderansicht]

### Bearbeiten eines Datensatzes inline in der Tabellenansicht eines Datensatztyps

Wenn Sie Datensätze in der Tabellenansicht bearbeiten, gibt es einen Hinweis darauf, welches Feld von anderen Benutzern zum Zeitpunkt der Anzeige des Datensatzes bearbeitet wird.

Weitere Informationen finden Sie unter [Verwalten von Datensatzansichten](/help/quicksilver/planning/views/manage-record-views.md).

Wenn Sie in einer Gruppierung oder Untergruppierung nach dem letzten Datensatz einen neuen Datensatz hinzufügen, aktualisiert Workfront automatisch die in den Gruppierungen enthaltenen Felder für die neuen Datensätze. Sie können diese Felder bei Bedarf manuell bearbeiten, und die Datensätze können aus der Gruppierung entfernt werden.

Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensätze Sie bearbeiten möchten

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.
1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. (Bedingt) Klicken Sie auf die Registerkarte einer Tabellenansicht oder klicken Sie auf **+ Ansicht** um eine Tabellenansicht zu erstellen. Die Tabellenansicht sollte die Standardansicht sein, es sei denn, Sie haben den Datensatztyp beim letzten Zugriff in einer anderen Ansicht angezeigt.

   Die mit dem ausgewählten Datensatztyp verknüpften Datensätze werden in der Tabellenansicht angezeigt.
1. Klicken Sie in die Zeile eines Datensatzes, um Informationen über den Datensatz inline zu bearbeiten.

   ![Datensatzabsatzfeld mit Formatierungstabellenansicht bearbeiten](assets/edit-record-paragraph-field-with-formatting-table-view.png)

   >[!TIP]
   >
   >  Informationen für die folgenden Felder können nicht bearbeitet werden, da sie schreibgeschützt sind und von Workfront automatisch aktualisiert werden:
   >  
   >  * Verknüpfte Felder, die durch Verbinden von Datensatztypen erstellt werden. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Felder der folgenden Typen: Erstellt von, Erstellt am, Zuletzt geändert von, Zuletzt geändert am, Formelfelder.

1. (Optional und bedingt) Verwenden Sie beim Bearbeiten eines Felds vom Typ Absatz die folgenden Formatierungsoptionen **Rich-Text**:

   * Fett
   * Kursiv
   * Unterstreichen
   * Link hinzufügen
   * Aufzählungsliste hinzufügen
   * Nummerierte Liste hinzufügen

   ![Rich-Text-Symbolleiste im Absatzfeld](assets/rich-text-toolbar-on-paragraph-field.png)

1. (Optional) Doppelklicken Sie auf ein Feld Verbundener Datensatz , um einem anderen Datensatz verbundene Datensätze oder Objekte hinzuzufügen. Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).
1. Drücken Sie **Eingabetaste** auf der Tastatur oder klicken Sie außerhalb einer Zeile, um Ihre Änderungen zu speichern. Die Änderungen werden automatisch gespeichert. Ein **Gespeichert**-Indikator wird kurz in der oberen rechten Ecke der Tabellenansicht angezeigt, um anzuzeigen, dass die Änderungen gespeichert wurden.


1. (Optional) Führen Sie einen der folgenden Schritte aus, um Informationen von einem Feld in ein anderes zu kopieren und einzufügen:

   * Kopieren Sie einen oder mehrere vorhandene Werte eines Felds und fügen Sie sie dann in ein Feld desselben Typs in einem anderen Datensatz ein.
   * Klicken Sie auf die Spaltenüberschrift einer Spalte, um sie auszuwählen, und kopieren Sie sie. Klicken Sie dann auf die Spaltenüberschrift einer anderen Spalte, und fügen Sie den Inhalt der kopierten Spalte ein. Die Spalten müssen ähnliche Feldtypen enthalten.
   * Klicken Sie bei gedrückter Umschalttaste auf mehrere Zeilen in einer Tabelle, kopieren Sie die Informationen in die ausgewählten Zeilen, klicken Sie dann auf eine andere Zeile und fügen Sie die ausgewählten Informationen in die neue Zeile und die folgenden Zeilen ein.
   * Kopieren Sie die Informationen aus einer Zelle, wählen Sie dann mehrere Zellen aus und fügen Sie dieselben Informationen in mehrere Zellen ein. Sie können mehrere Zellen auswählen und dieselben Informationen in mehrere Zellen aus benachbarten Zeilen und Spalten einfügen.
   * Wählen Sie die untere rechte Ecke einer vorhandenen Zelle aus, die die Informationen enthält, die Sie kopieren möchten, und ziehen Sie sie dann per Drag-and-Drop über die angrenzenden Zellen, in die Sie dieselben Informationen einfügen möchten. Alle Zellen müssen dieselbe Art von Informationen enthalten.

     ![Ziehbare untere rechte Ecke für Kopieren und Einfügen in die Tabellenansicht](assets/dragable-lower-right-corner-for-copy-paste-in-table-view.png)


   * Kopieren Sie eine oder mehrere Zellen aus einer externen Quelle (z. B. einer Excel-Datei) und fügen Sie sie dann in einen der folgenden Feldtypen ein:

      * Workfront Planning-Verbindungsfelder.
      * Personenfelder. Es werden nur Felder mit einem Wert unterstützt.

     Es ist nicht möglich, Informationen aus einer externen Quelle zu kopieren und in andere Feldtypen, einschließlich Workfront- oder AEM Assets-Verbindungsfeldern, einzufügen.

   >[!NOTE]
   >
   >Beachten Sie Folgendes:
   >
   >* Verwenden Sie die folgenden Tastaturbefehle zum Kopieren und Einfügen von Informationen:
   >   * Kopieren: STRG + C (⌘ + C für Mac)
   >   * Einfügen: STRG + V (⌘ + V für Mac)
   >
   >* Feldwerte können nicht kopiert und in die Datensatzseite eingefügt werden. Diese Funktion wird nur in der Tabellenansicht eines Datensatztyps unterstützt.
   >* Feldwerte für die folgenden Feldtypen können nicht kopiert und eingefügt werden:
   >
   >    * Suchfelder, die beim Verbinden von Datensatztypen erstellt werden. Sie können verknüpfte Datensatzfelder kopieren und einfügen. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
   >    * Felder der folgenden Typen: Erstellt von, Erstellt am, Zuletzt geändert von, Zuletzt geändert am

1. (Optional) Verwenden Sie die folgenden Tastaturbefehle, um das Bearbeiten oder Kopieren und Einfügen von Datensatzinformationen rückgängig zu machen oder wiederherzustellen:

   * STRG + Z (⌘ + Z für Mac), um eine Änderung rückgängig zu machen
   * Strg+Umsch+Z (⌘+Umschalt+Z für Mac) zum Wiederherstellen einer Änderung

   >[!TIP]
   >
   >    Sie können die Tastaturbefehle mehrmals hintereinander verwenden, um mehrere Änderungen rückgängig zu machen.

1. (Optional) Fügen Sie einem Datensatz eine Miniaturansicht hinzu. Weitere Informationen finden Sie unter [Hinzufügen einer Miniaturansicht zu einem Datensatz](/help/quicksilver/planning/records/add-thumbnails-to-records.md).


### Bearbeiten eines Datensatzes in der Zeitleisten-Ansicht eines Datensatztyps

<!--add another step about drag and drop here when that is available-->

1. Öffnen Sie die Seite „Datensatztyp“ in einer Zeitleisten -Ansicht. Weitere Informationen finden Sie unter [Verwalten der Zeitleisten-Ansicht](/help/quicksilver/planning/views/manage-the-timeline-view.md).

1. <span class="preview">Bewegen Sie den Mauszeiger über die Enden der Leiste eines Datensatzes und klicken Sie, ziehen Sie den Rand per Drag-and-Drop an ein anderes Datum. Dadurch wird automatisch das Start- oder Enddatum des Datensatzes aktualisiert.</span>

   <span class="preview">![Leiste am linken Ende der Zeitleisten-Ansicht, um die Größe zu ändern](assets/left-end-bar-handle-to-resize-timeline-view.png)</span>

1. <span class="preview">Klicken Sie auf eine Datensatzleiste, halten Sie sie gedrückt und ziehen Sie sie dann an eine andere Position, um ihre Zeitleiste und Daten zu aktualisieren. Das Start- und Enddatum des Datensatzes werden automatisch aktualisiert.</span>

1. Klicken Sie auf die Leiste eines Datensatzes, um seinen Detailbereich zu öffnen und alle Felder zu bearbeiten.

   Weitere Informationen finden Sie [&#x200B; Abschnitt „Bearbeiten eines Datensatzes aus der Vorschau des Datensatzes in einer Ansicht](#edit-a-record-from-the-records-preview-in-a-view) in diesem Artikel.

### Bearbeiten eines Datensatzes in der Kalenderansicht eines Datensatztyps

<!--add another step about drag and drop here when that is available-->

1. Öffnen Sie die Seite „Datensatztyp“ in einer Kalenderansicht. Weitere Informationen finden Sie unter [Verwalten der Kalenderansicht](/help/quicksilver/planning/views/manage-the-calendar-view.md).
1. <span class="preview">(Bedingt) Bewegen Sie den Mauszeiger in der Kalenderansicht über die Enden der Leiste eines Datensatzes und klicken Sie dann auf, ziehen Sie die Ränder und legen Sie sie an einem anderen Datum ab. Dadurch wird automatisch das Start- oder Enddatum des Datensatzes aktualisiert.</span>

   <span class="preview">![Leiste am linken Ende der Kalenderansicht, deren Größe geändert werden soll](assets/left-end-bar-handle-to-resize-calendar-monthly-view.png)</span>

1. <span class="preview">Klicken Sie auf eine Datensatzleiste, halten Sie sie gedrückt und ziehen Sie sie dann an eine andere Position, um ihre Zeitleiste und Daten zu aktualisieren. Das Start- und Enddatum des Datensatzes werden automatisch aktualisiert.</span>

1. Klicken Sie auf die Leiste eines Datensatzes, um seinen Detailbereich zu öffnen und alle Felder zu bearbeiten.

   Weitere Informationen finden Sie [&#x200B; Abschnitt „Bearbeiten eines Datensatzes aus der Vorschau des Datensatzes in einer Ansicht](#edit-a-record-from-the-records-preview-in-a-view) in diesem Artikel.

### Bearbeiten eines Datensatzes aus der Datensatzvorschau in einer Ansicht

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensätze Sie bearbeiten möchten

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. Klicken Sie in einer beliebigen Ansicht auf den Datensatz

   Oder

   Klicken Sie in der Tabellenansicht auf das Symbol **Details öffnen** ![Detailsymbol öffnen im Feld „Tabellenname](assets/open-details-icon-in-table-name-field.png) in der ersten Spalte. Die Vorschau des Datensatzes wird in der Ansicht geöffnet.

   ![Detailfeld](assets/details-box.png)

1. (Optional) Klicken Sie auf das **Mehr**-Menü rechts neben dem Datensatztitel und klicken Sie dann auf **Umbenennen**. Dadurch wird das Feld aktualisiert, das als Datensatztitel angezeigt wird.

   Der Titel des Datensatzes ist das primäre Feld des Datensatzes, wenn er in einer Tabellenansicht angezeigt wird. Weitere Informationen finden Sie unter [Übersicht über Primäre Felder](/help/quicksilver/planning/fields/primary-field-overview.md).

1. Beginnen Sie mit der Bearbeitung der Feldinformationen in der Vorschau des Datensatzes.

   >[!TIP]
   >
   >  Informationen für die folgenden Felder können nicht bearbeitet werden, da sie schreibgeschützt sind und von Workfront automatisch aktualisiert werden:
   >  
   >  * Nachschlagen von Feldern aus anderen Datensätzen, die durch Verbinden von Datensatztypen erstellt werden. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Felder der folgenden Typen: Erstellt von, Erstellt am, Zuletzt geändert von, Zuletzt geändert am, Formelfelder.

1. (Optional) Klicken Sie auf **Cover hinzufügen**, um dem Datensatz ein Cover-Bild hinzuzufügen. Weitere Informationen finden Sie unter [Hinzufügen eines Cover-Bildes zu einem Datensatz](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md).

1. (Optional) Bewegen Sie den Mauszeiger über das Miniaturansichtssymbol und klicken Sie dann auf **Mehr** ![Mehr Menü](assets/more-menu.png) > **Miniaturansicht bearbeiten**, um ein Miniaturbild hinzuzufügen. Weitere Informationen finden Sie unter [Hinzufügen einer Miniaturansicht zu einem Datensatz](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

   Workfront speichert Ihre Änderungen automatisch.

1. (Optional) Klicken Sie auf **Echtzeitindikator** ![Echtzeitindikatorsymbol](assets/real-time-indicator-icon.png) in der rechten oberen Ecke des Vorschaufelds des Datensatzes und aktivieren Sie dann die Einstellung **Mitarbeiter anzeigen**, um die Felder hervorzuheben, die von anderen Personen in Echtzeit bearbeitet werden.

   In diesem Bereich werden die Namen und Avatare aller Benutzer angezeigt, die gleichzeitig auf den Datensatz zugreifen.

   Wenn die Einstellung deaktiviert ist, werden die Avatare und Namen im Bereich der Echtzeitanzeige aufgelistet und die Felder, die bearbeitet werden, werden nicht hervorgehoben.

   ![Erweitertes Feld für die Datensatzvorschau der Echtzeit-Anzeige](assets/real-time-indicator-expanded-record-preview-box.png)

1. (Optional) Klicken Sie auf das **Export**-Menü ![Export-Symbol auf der Seite mit &#x200B;](assets/export-icon-in-record-details-page.png) Datensatzdetails), um die Datensatzdetails zu exportieren. Weitere Informationen finden Sie [Exportieren der Details eines Datensatzes](/help/quicksilver/planning/records/export-the-record-page.md).

1. (Optional) Klicken Sie auf **In neuer Registerkarte öffnen** Symbol ![Details in einer neuen Registerkarte öffnen](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in der oberen rechten Ecke der Datensatzvorschau, um die Seite des Datensatzes in einer neuen Registerkarte zu öffnen. Fahren Sie mit der Bearbeitung des Datensatzes fort[&#x200B; wie im Abschnitt Bearbeiten eines Datensatzes auf der Seite des Datensatzes &#x200B;](#edit-a-record-from-the-records-page) diesem Artikel beschrieben.

### Bearbeiten eines Datensatzes auf der Datensatzseite

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensätze Sie bearbeiten möchten

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. Führen Sie einen der folgenden Schritte aus:

   * Greifen Sie in jeder Ansicht auf die Vorschau des Datensatzes zu, wie im Abschnitt [Bearbeiten eines Datensatzes aus der Vorschau des Datensatzes in einer Ansicht](#edit-a-record-from-the-records-preview-in-a-view) in diesem Artikel beschrieben, und klicken Sie dann auf das Symbol **In neuer Registerkarte öffnen** ![Details in einem neuen Registerkartensymbol öffnen](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> in der oberen rechten Ecke der Datensatzvorschau, um die Seite des Datensatzes in einer neuen Registerkarte zu öffnen.

   * Bewegen Sie in **Tabellenansicht** den Mauszeiger über den Namen eines Datensatzes und klicken Sie dann auf das **Mehr** Menü ![Mehr](assets/more-menu.png) und dann auf **Ansicht**

     ![Kontextmenü für Datensatzzeile](assets/contextual-menu-for-record-row.png)

     Die Datensatzseite wird geöffnet.

     ![Detailseite](assets/details-page.png)

1. (Optional) Klicken Sie auf das **Mehr**-Menü rechts neben dem Datensatztitel und klicken Sie dann auf **Umbenennen**. Dadurch wird das Feld aktualisiert, das als Datensatztitel angezeigt wird.

   Der Titel des Datensatzes ist das primäre Feld des Datensatzes, wenn er in einer Tabellenansicht angezeigt wird. Weitere Informationen finden Sie unter [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md).

1. Klicken Sie auf ein bearbeitbares Feld auf der Datensatzseite, um es zu bearbeiten.

   >[!TIP]
   >
   >  Informationen für die folgenden Felder können nicht bearbeitet werden, da sie schreibgeschützt sind und von Workfront automatisch aktualisiert werden:
   >  
   >  * Verknüpfte Felder, die durch Verbinden von Datensatztypen erstellt werden. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Felder der folgenden Typen: Erstellt von, Erstellt am, Zuletzt geändert von, Zuletzt geändert am, Formelfelder.

1. (Optional) Klicken Sie auf das Informationssymbol rechts neben einem Feld, in dem es angezeigt wird, um die Beschreibung eines Felds anzuzeigen.
1. (Optional) Klicken Sie auf **Cover hinzufügen**, um dem Datensatz ein Cover-Bild hinzuzufügen

   Oder

   Bewegen Sie den Mauszeiger über das vorhandene Cover-Bild und klicken Sie dann auf das **Mehr** Menü ![Mehr &#x200B;](assets/more-menu.png) > **Hochladen**, um ein neues Cover-Bild für den Datensatz hinzuzufügen.

   Weitere Informationen finden Sie unter [Hinzufügen eines Cover-Bildes zu einem Datensatz](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md).

1. (Optional) Bewegen Sie den Mauszeiger über eine vorhandene Miniaturansicht oder das Symbol **Miniaturansicht** ![Miniaturansicht aufzeichnen auf der Detailseite](assets/record-thumbnail-icon-on-details-page.png) und klicken Sie dann auf das Menü **Mehr** Menü ![Mehr](assets/more-menu.png) > **Miniaturansicht bearbeiten**, um eine Miniaturansicht für den Datensatz hinzuzufügen.

   Weitere Informationen finden Sie unter [Hinzufügen einer Miniaturansicht zu einem Datensatz](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

   Workfront speichert Ihre Änderungen automatisch.

1. (Optional) Klicken Sie auf das Symbol **Echtzeitanzeige** ![Echtzeitanzeige](assets/real-time-indicator-icon.png) in der rechten oberen Ecke der Datensatzseite und aktivieren Sie dann die Einstellung **Mitarbeiter anzeigen**, um die Felder hervorzuheben, die von anderen Personen in Echtzeit bearbeitet werden.

   In diesem Bereich werden die Namen und Avatare aller Benutzer angezeigt, die gleichzeitig auf den Datensatz zugreifen.

   Wenn die Einstellung deaktiviert ist, werden die Avatare und Namen im Bereich der Echtzeitanzeige aufgelistet und die Felder, die bearbeitet werden, werden nicht hervorgehoben.

   ![Das erweiterte Feld für die Datensatzvorschau der Echtzeitanzeige](assets/real-time-indicator-expanded-record-preview-box.png)

1. (Optional) Klicken Sie auf das **Export**-Menü ![Export-Symbol auf der Seite mit &#x200B;](assets/export-icon-in-record-details-page.png) Datensatzdetails), um die Datensatzdetails zu exportieren. Weitere Informationen finden Sie [Exportieren der Details eines Datensatzes](/help/quicksilver/planning/records/export-the-record-page.md).


## Bearbeiten eines Datensatzes aus einem Workfront-Objekt im Planungsabschnitt

Nachdem Sie Datensätze mit Workfront-Objekten verbunden haben, können Sie Workfront-Planungsdatensätze in Workfront im Planungsabschnitt des Objekts bearbeiten.

Weitere Informationen finden Sie unter [Verwalten von Datensatzverbindungen aus Workfront-Objekten](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

<div class="preview">

## Bearbeiten von Einfach- oder Mehrfachauswahl-Feldeinstellungen beim Aktualisieren ihrer Werte

<!--some of this information is also available in Edit fields article - update both when necessary-->

Wenn Sie Informationen in einem Ein- oder Mehrfachauswahlfeld aktualisieren, können Sie dem Feld neue Auswahlmöglichkeiten hinzufügen, ohne das Feld bearbeiten zu müssen.

>[!IMPORTANT]
>
>Die in diesem Abschnitt beschriebene Funktion ist nur in der Tabellenansicht verfügbar. Sie ist nicht in anderen Bereichen verfügbar, in denen Einzel- oder Mehrfachauswahlfelder angezeigt werden.

**BEISPIEL**

Möglicherweise verfügen Sie über ein Feld mit einer einzigen Auswahl namens Status , in dem die Optionen Neu und Geschlossen verfügbar sind, und Sie möchten eine Auswahl für einen Status In Bearbeitung hinzufügen. Sie können die Auswahl hinzufügen, indem Sie einen der folgenden Schritte ausführen:

* Bearbeiten des Felds. Weitere Informationen finden Sie unter [Felder bearbeiten](/help/quicksilver/planning/fields/edit-fields.md)
* Hinzufügen einer neuen Option beim Bearbeiten des Datensatzes in der Tabellenansicht, wie unten beschrieben.

So fügen Sie beim Bearbeiten eines Datensatzes einem vorhandenen Auswahlfeld eine neue Auswahl hinzu:

1. Wechseln Sie zu einer Seite vom Typ Datensatz und öffnen Sie die Tabellenansicht.
1. Fügen Sie das Einzel- oder Mehrfachauswahlfeld, dem Sie eine Auswahl hinzufügen möchten, in der Tabellenansicht als neue Spalte hinzu. Weitere Informationen finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).
1. Beginnen Sie mit der Inline-Bearbeitung des Felds, indem Sie auf die Zelle für das Feld doppelklicken.
1. Geben Sie den Namen der Auswahl ein, die Sie hinzufügen möchten, und klicken Sie dann auf **Auswahl hinzufügen**.

   ![Auswahl im Einzelauswahlfeld in der Tabellenansicht hinzufügen](assets/add-choice-in-table-view-for-single-select-field.png)

   Die neue Auswahl wird sofort zum Feld für die Einzelauswahl hinzugefügt.

   <!--<span class="preview">A new choice value is also added to each choice. You can use the choice values in API calls or other integrations. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md). </span>-->

</div>
