---
title: Kalenderansicht verwalten
description: Sie können Datensätze und ihre Felder in einer Kalenderansicht anzeigen. Dieser Artikel beschreibt, wie Sie eine Kalenderansicht erstellen und eine vorhandene bearbeiten oder löschen können.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: 5d326776b9c5b4d9d24e802375df4630508c8bd0
workflow-type: tm+mt
source-wordcount: '1776'
ht-degree: 5%

---

# Kalenderansicht verwalten

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

Auf der Seite Datensatztyp können Sie Datensätze und ihre Felder in einer Kalenderansicht anzeigen.

Weitere Informationen zu Adobe Workfront Planning-Ansichten und deren Verwaltung finden Sie unter [Verwalten von Datensatzansichten](/help/quicksilver/planning/views/manage-record-views.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<p>Beliebiges Workfront und beliebiges Planungspaket</p>
<p>Beliebiger Workflow und beliebiges Planungspaket</p>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p> Standard zum Erstellen und Löschen von Ansichten</p>
   <p>Mitwirkender oder höher zum Aktualisieren von Ansichtselementen</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten der Berechtigungen für eine Ansicht</p>  
   <p>Anzeigeberechtigungen für eine Ansicht, um die Anzeigeeinstellungen vorübergehend zu ändern oder zu duplizieren</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> Benutzenden mit einer Light- oder Contributor-Lizenz muss eine Layout-Vorlage zugewiesen werden, die Planning enthält.
   <p>Für Standardbenutzer und Systemadministratoren sind die Planungsbereiche standardmäßig aktiviert.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

<!--Old:
 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
    <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard to create and delete views</p>
   <p>Contributor or higher to update view elements</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings or to duplicate it</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>

</tbody> 
</table> -->

## Verwalten einer Kalenderansicht {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

Beachten Sie Folgendes:

* Eine Kalenderansicht kann nur erstellt werden, wenn mindestens zwei Datumsfelder mit einem Datensatztyp verknüpft sind. Wenn Sie ein oder kein Datumsfeld mit einem Datensatztyp verknüpft haben, ist die Option Kalenderansicht abgeblendet.

  Sie können aus Datensatzdatumsfeldern auswählen oder Datumsfelder aus verbundenen Datensatz- oder Objekttypen nachschlagen.
* Die folgenden Szenarien sind vorhanden:

   * Wenn sowohl das Start- als auch das Enddatum keine Werte haben, werden die Datensätze nicht im Kalender angezeigt
   * Wenn das Start- oder Enddatum keinen Wert hat, wird der Datensatz als eintägiges Ereignis angezeigt
   * Wenn das Startdatum nach dem Enddatum liegt, wird der Datensatz nicht im Kalender angezeigt.

Verwalten einer Kalenderansicht:

1. Wechseln Sie zur Seite „Datensatztyp“, für die Sie den Kalender anzeigen möchten.
1. Erstellen Sie eine Kalenderansicht, wie im Artikel [Verwalten von Datensatzansichten](/help/quicksilver/planning/views/manage-record-views.md) beschrieben.

   ![Beispiel für Kalenderansicht](assets/calendar-view-example.png)

   Die Datensätze, die mit dem ausgewählten Datensatztyp verknüpft sind, werden als Balken in einem Kalender angezeigt. Standardmäßig entspricht die Farbe der Balken der Farbe des Datensatzsymbols.

1. Führen Sie einen der folgenden Schritte aus, um durch den Kalender zu navigieren:

   * Klicken Sie auf die Symbole links und rechts oben im Kalender oder verwenden Sie den horizontalen Bildlauf, um im Kalender vor- und rückwärts zu blättern.
   * Klicken **oben** auf „Heute“, um den Kalender auf das heutige Datum zu zentrieren.
   * Wählen Sie eine der folgenden Optionen aus dem Dropdown-Menü Zeitrahmen aus, um die Zeitinkremente zu aktualisieren:

      * **Monat**: Datensätze werden in einem monatlichen Kalender angezeigt.

      * **Woche**: Die Datensätze werden in den folgenden Bereichen angezeigt:

         * Datensätze, die sich über mehrere Tage erstrecken, werden oben im Kalender angezeigt.
         * Datensätze, die einen Tag oder weniger dauern, werden in der unteren Hälfte der Kalenderansicht angezeigt. Wenn Sie ausgewählt haben, die Stunde des Start- und Enddatums anzuzeigen, wird der Datensatz zum entsprechenden Zeitpunkt innerhalb des Tages angezeigt, an dem er auftritt.

1. (Optional) Klicken Sie auf das **Vollbildsymbol**-Symbol ![Vollbildsymbol öffnen](assets/open-full-screen-icon.png) um die Ansicht im Vollbildmodus zu öffnen. Klicken Sie dann auf das **Vollbildsymbol beenden**-Symbol ![Vollbildsymbol beenden](assets/exit-full-screen-icon.png) oder auf der Tastatur auf Esc , um den Vollbildmodus zu verlassen.

1. Führen Sie einen der folgenden Schritte aus, um Datensätze in der Kalenderansicht zu erstellen oder ihre Daten zu bearbeiten:

   * Doppelklicken Sie auf eine beliebige Stelle im Kalender, um einen Datensatz zu erstellen.

     Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).

   * Klicken Sie auf den linken oder rechten Rand einer Datensatzleiste und ziehen Sie sie dann per Drag-and-Drop an eine neue Position. Wenn Sie die Größe der Balken der Datensätze ändern, werden das Start- oder Enddatum sofort aktualisiert.

   * Ziehen Sie die Datensatzleisten per Drag-and-Drop, um ihre Position und ihr Datum zu aktualisieren. Durch Verschieben der Datensatzbalken wird das Start- und Enddatum sofort aktualisiert.

     Weitere Informationen finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

1. Aktualisieren Sie die folgenden Ansichtselemente wie in den folgenden Unterabschnitten beschrieben:
   * [Filter](#add-filters)
   * [Zeilenhöhe](#modify-row-height)
   * [Einstellungen](#edit-the-calendar-view-settings)

   <!--* [Grouping](#add-grouping)-->
   <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### Filter hinzufügen

Mithilfe von Filtern können Sie die Informationsmenge reduzieren, die auf dem Bildschirm angezeigt wird.

Beachten Sie beim Arbeiten mit Filtern in der Kalenderansicht Folgendes:

<!-- this list is almost identical to the one for the table view - update both-->

* Die Filter, die Sie für eine Kalenderansicht erstellen, funktionieren unabhängig von den Filtern in jeder anderen Ansicht, die auf denselben Datensatztyp angewendet wird.

* Die Filter sind für die ausgewählte Ansicht eindeutig. Auf zwei Kalenderansichten desselben Datensatztyps können unterschiedliche Filter angewendet werden.

* Zwei Benutzer, die dieselbe Kalenderansicht betrachten, sehen denselben Filter, der derzeit angewendet wird.

* Die Filter, die Sie für eine Kalenderansicht erstellen, können nicht benannt werden.

* Das Entfernen von Filtern entfernt sie von allen, die auf denselben Datensatztyp zugreifen wie Sie und die dieselbe Ansicht anzeigen wie Sie.

* Sie können nach verbundenen Datensatzfeldern oder Suchfeldern filtern.

* Sie können nach Suchfeldern filtern, die mehrere Werte anzeigen.

So fügen Sie einen Filter zu einer Kalenderansicht hinzu:

1. Erstellen Sie eine Kalenderansicht für eine Datensatztypseite, wie im Artikel [Verwalten von Datensatzansichten](/help/quicksilver/planning/views/manage-record-views.md) beschrieben.
1. Wählen Sie eine Kalenderansicht aus und klicken Sie dann **Filter** in der Kalendersymbolleiste.
1. Klicken Sie **Bedingung hinzufügen** und fügen Sie die folgenden Informationen hinzu:

   * **Feld auswählen**, um nach einem Feld zu suchen und es aus der Liste auszuwählen

   * **Wählen Sie eine Option** oder einen Filtermodifikator), um festzulegen, welche Art von Bedingung das Feld erfüllen muss

     In der folgenden Tabelle werden die verfügbaren Modifikatoren für jeden Feldtyp angezeigt.

     <table>
        <thead>
        <tr>
            <th><b>Feldtyp</b></th>
            <th><b>Modifikatoren</b></th>
        </tr>
        </thead>
        <tbody>
        <tr>
            <td>Einzeilig, Absatz, Formel </td>
            <td><p>Enthält</p>
            <p>Enthält nicht</p>
            <p>Ist</p>
            <p>Ist nicht</p>
            <p>Ist leer</p>
            <p>Ist nicht leer</p></td>
        </tr>
        <tr><td>Einzelauswahl</td>
            <td><p>Ist</p>
            <p>Ist nicht</p>
            <p>Ist ein beliebiges von</p>
            <p>Ist keines von</p>
            <p>Ist leer</p>
            <p>Ist nicht leer</p></td>
        </tr>
        <tr>
            <td>Mehrfachauswahl, Personen</td>
            <td><p>Hat eines von</p>
            <p>Hat alle von</p>
            <p>Ist genau</p>
            <p>Hat keines von</p>
            <p>Ist leer</p>
            <p>Ist nicht leer</p></td>
        </tr>
        <tr>
            <td>Zahl, Prozentsatz, Währung</td>
            <td><p>=</p>
            <p>≠</p>
            <p> &lt; </p>
            <p>&gt;</p>
            <p>≤</p>
            <p>≥</p>
            <p>Ist leer</p>
            <p>Ist nicht leer</p></td>
        </tr>
        <tr>
            <td>Datum</td>
            <td><p>Ist</p>
            <p>Ist nicht</p>
            <p>Ist nach</p>
            <p>Ist vor</p>
            <p>Ist zwischen</p><p>Ist nicht zwischen</p>
            <p>Ist leer</p><p>Ist nicht leer</p></td>
        </tr>

     <tr>
            <td>Kontrollkästchen</td>
            <td><p>Ist</p>
        </tr>
        </tbody>
        </table>

   * Einen Wert für das ausgewählte Feld auswählen.

   ![Tabellenansicht der Filter-Benutzeroberfläche](assets/filter-ui-table-view.png)

   Es gibt keine Begrenzung dafür, wie viele Filterbedingungen Sie hinzufügen können.

1. (Optional) Klicken Sie auf **Bedingung hinzufügen**, um eine weitere Filteroption hinzuzufügen, und wiederholen Sie die obigen Schritte. Die Anzahl der angewendeten Filter wird links neben dem Symbol Filter angezeigt.
1. Klicken Sie auf die folgenden Operatoren, um anzugeben, wie die Filterbedingungen verbunden werden und angewendet werden sollen:

   * **AND**: Alle angegebenen Bedingungen müssen erfüllt sein.
   * **OR**: Jede der angegebenen Bedingungen muss erfüllt sein. Dies ist die Standardoption.

   1. (Optional) Fügen Sie zusätzliche Operatoren **AND** oder **OR** zwischen mehreren Bedingungsgruppierungen hinzu.

      ![Mehrstufige Filter in Ansichten](assets/multi-tiered-filters-in-views.png)

   Die Liste der Datensätze wird automatisch gefiltert.  <!--at this time, you can't name and save the filter - but will this change?!-->
   <!-- asked on the task for the simple filters whether there is a limitation for how many statements a filter can have?!-->

1. (Optional) Klicken Sie auf das Symbol **x**, um eine Filterbedingung zu entfernen.
1. (Optional) Klicken Sie auf **Filter**, um das Feld „Filter“ zu schließen. <!--right now you cannot "clear all" for filters, but this might come later-->


### Zeilenhöhe ändern

Sie können die Zeilenhöhe einer Kalenderzelle ändern, um die Anzahl der in jeder Zelle angezeigten Datensatzleisten zu erhöhen oder zu verringern.

Die Anzahl der im Kalender angezeigten Datensätze hängt von der Anzahl der Felder ab, die in den Balken der Datensätze angezeigt werden.

>[!TIP]
>
>Diese Einstellung ist nur verfügbar, wenn der Kalender nach Monat angezeigt wird.


1. Erstellen Sie eine Kalenderansicht für eine Datensatztypseite, wie im Artikel [Verwalten von Datensatzansichten](/help/quicksilver/planning/views/manage-record-views.md) beschrieben.
1. (Bedingt) Zeigen Sie die Kalenderansicht nach Monat an und klicken Sie dann auf **Zeilenhöhe** in der Kalendersymbolleiste.
1. Wählen Sie aus den folgenden Optionen:

   <table>
    <thead>
    <tr>
        <th><b>Zeilenhöhenoption</b></th>
        <th><b>Standardmäßige maximale Anzahl von Datensätzen</b></th>
    </tr>
    </thead>
    <tbody>
    <tr>
        <td>Kurz</td>
        <td><p>Enthält:</p>

   <ul><li>2 Datensätze mit 1 Feld</li>
    <li>1 Datensatz mit mehr als 1 Feld</li></ul>
        </td>
    </tr>
    <tr><td>Standard</td>
        <td><p>Enthält:</p>

   <ul><li>4 Datensätze mit 1 Feld</li>
    <li>2 Datensätze mit mehr als 1 Feld</li></ul>
        </td>
    </tr>
    <tr>
        <td>Mittel</td>
        <td><p>Enthält:</p>

   <ul><li>8 Datensätze mit 1 Feld</li>
    <li>4 Datensatz mit mehr als 1 Feld</li></ul>
        </td>
    </tr>
    <tr>
        <td>Groß</td>
        <td><p>Enthält:</p>

   <ul><li>12 Datensätze mit 1 Feld</li>
    <li>6 Datensatz mit mehr als 1 Feld</li></ul>
        </td>
    </tr>
    <tr>
        <td>An Inhalt anpassen</td>
        <td><p>Alle Datensätze sind sichtbar, bis zu 500 Datensätze</p></td>
    </tr>
    </tbody>
    </table>

1. (Optional) Klicken Sie auf **Mehr**, wenn Datensätze im Kalender nicht sichtbar sind.

</span>

### Bearbeiten der Einstellungen für die Kalenderansicht

Aktualisieren Sie die Einstellungen der Kalenderansicht, um anzugeben, welche Informationen in der Ansicht angezeigt werden.

1. Erstellen Sie eine Kalenderansicht für einen Datensatztyp, wie im Artikel [Verwalten von Datensatzansichten](/help/quicksilver/planning/views/manage-record-views.md) beschrieben.
1. Klicken Sie auf **Einstellungen**.
1. Klicken Sie **linken Bereich auf** Datum und Uhrzeit) und wählen Sie dann ein **Startdatum** und ein **Enddatum** aus, die im Kalender angezeigt werden sollen. Sie können das standardmäßige Start- und Enddatum oder ein beliebiges verfügbares Datumsfeld auswählen.

   Die Balken, die die Datensätze darstellen, beginnen an dem Datum, das Sie als Startdatum angeben, und enden an dem Datum, das dem Enddatum entspricht.

   >[!NOTE]
   >
   >* Datensätze, die keine Werte für das Start- oder Enddatum haben oder deren Startdatum nach dem Enddatum liegt, werden nicht in der Kalenderansicht angezeigt.
   >
   >* Wenn Sie zusätzliche Datensätze mithilfe der Option Aufschlüsselung anzeigen, sind das Start- und Enddatum die Daten des Hauptdatensatzes. Start- und Enddatum für die verbundenen Datensätze in diesem Bereich können nicht ausgewählt werden.

1. Klicken Sie **linken** auf „Balkenstil“, um anzugeben, welche Informationen in den Datensatzleisten angezeigt werden sollen.

   Das primäre Feld (oder der Titel) des Datensatzes, wie in der Tabellenansicht des Datensatzes definiert, ist standardmäßig ausgewählt.
   <!--adjust this when the primary field is released??-->

1. (Optional und bedingt) Wenn Sie den Datensätzen Miniaturen hinzugefügt haben, wählen Sie die Option **Miniatur**, um das mit den Datensätzen verknüpfte Bild in der Datensatzleiste anzuzeigen.

   >[!NOTE]
   >
   >    Sie müssen zunächst Miniaturen in der Tabellenansicht hinzufügen, bevor Sie sie in der Kalenderansicht anzeigen können. Weitere Informationen finden Sie unter [Hinzufügen einer Miniaturansicht zu einem Datensatz](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

1. Klicken Sie **Feld hinzufügen**, klicken Sie dann in das Feld **Suchfelder** und klicken Sie auf das Feld, das Sie hinzufügen möchten.

   >[!TIP]
   >
   >   * Sie müssen die Felder erstellen, bevor Sie sie den Datensatzleisten hinzufügen können.
   > 
   >   * Es muss mindestens ein Feld ausgewählt sein. **Name** ist standardmäßig ausgewählt.
   >
   >   * Sie können bis zu 5 Felder hinzufügen.

   Eine Vorschau davon, wie die Balken im Kalender aussehen werden, wird auf der rechten Seite angezeigt.

   ![Abschnitt „Balkenstil“ in den Einstellungen der Kalenderansicht](assets/bar-style-section-in-calendar-view-settings-with-preview.png)

1. Klicken Sie **linken** auf „Farbe“, um die Farben der Datensätze im Kalender anzupassen.

   ![Farbbedienfeld in den Einstellungen für die Kalenderansicht](assets/color-panel-on-calendar-view-settings.png)

1. Wählen **im Abschnitt Datensatzfarbe festlegen** eine der folgenden Optionen aus, um eine Farbe für die Datensätze festzulegen:

   * **Datensatztyp**: Die Farbe der Datensatzleisten im Kalender entspricht der Farbe des ausgewählten Datensatztyps. Dies ist die Standardoption.
   * **Feldwerte**: Die Farbe der Datensätze entspricht der Farbe eines von Ihnen angegebenen Felds.
   * **Keine**: Die Datensätze werden in einem weißen Balken angezeigt.

1. (Bedingt) Wenn Sie **Feldwerte** für die Datensatzfarben ausgewählt haben, wählen Sie ein Feld aus dem Dropdown-Menü **Übereinstimmung der Datensatzfarbe mit** aus.

   ![Dropdown-Menü zur Feldauswahl für die Kalenderansicht](assets/field-selector-drop-down-menu-calendar-view.png)

   Nur Felder mit farbcodierten Optionen werden im Dropdown-Menü angezeigt.

   Beispielsweise können Felder mit Mehrfachauswahl oder Einzelauswahl farbcodierte Optionen haben.

   Wenn Sie kein Feld mit farbcodierten Optionen für den ausgewählten Datensatztyp haben, ist diese Option abgeblendet.


1. Klicken Sie auf **Speichern**.

   Die Datensätze werden in der Kalenderansicht mit den von Ihnen ausgewählten Spezifikationen angezeigt.