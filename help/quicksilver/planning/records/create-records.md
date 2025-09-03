---
title: Erstellen von Datensätzen
description: Bei Verwendung von Adobe Workfront Planning ist ein Datensatz eine Instanz eines Datensatztyps. Sie können in Workfront Planning für jeden Datensatztyp eindeutige Datensätze erstellen, indem Sie diese manuell zur Tabellenansicht hinzufügen, aus einer Liste importieren, duplizieren oder beim Verbinden mit anderen Datensätzen erstellen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 4e295b4fdbbde7439567ef2a4f4383ad8dea738c
workflow-type: tm+mt
source-wordcount: '2814'
ht-degree: 0%

---


# Erstellen von Datensätzen

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

In Adobe Workfront Planning ist ein Datensatz eine Instanz eines Datensatztyps.

Sie können Datensätze wie folgt erstellen:

* [Verwenden Sie die Schaltfläche Neuer Datensatz oder Datensatz anfragen in einer beliebigen Datensatztypansicht.](#create-records-using-the-new-record-or-request-record-button-from-any-record-type-view)
* [Fügen Sie sie inline über die Tabellenansicht vom Typ Datensatz hinzu](#create-records-by-adding-them-inline-from-the-record-type-table-view)

<div class="preview">

* [Fügen Sie sie in der Zeitleisten-Ansicht des Datensatztyps hinzu](#create-records-by-adding-them-in-the-record-type-timeline-view)

</div>

<!--
<div class="preview">

* [Add them in the record type calendar view](#create-records-by-adding-them-in-the-record-type-calendar-view)

</div>
-->

* [Kopieren und Einfügen einer Liste von Datensätzen aus einer externen Liste](#create-records-by-copying-and-pasting-them-from-an-external-list)
* [Duplizieren von Datensätzen aus einer Tabellenansicht](#create-records-by-duplicating-them)
* [Aus anderen Datensätzen verbinden](#create-records-as-you-connect-them)
* [Senden eines Anfrageformulars an einen Datensatztyp](#create-records-by-submitting-a-request-form-to-a-record-type)
* [Informationen aus einer CSV- oder Excel-Datei importieren](#create-records-by-importing-records-from-a-csv-or-excel-file)
* [Automatisierungen verwenden](#create-records-by-using-automations)

Informationen zum Verwalten von Datensätzen in der Tabellen- oder Zeitleisten -Ansicht finden Sie in den folgenden Artikeln:

* [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md)
* [Zeitleisten-Ansicht verwalten](/help/quicksilver/planning/views/manage-the-timeline-view.md)

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
   <td> Standard
   <p>Workfront Planning ist nicht für ältere Workfront-Lizenzen verfügbar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p> 
   <p>Bearbeiten Sie den Zugriff in Workfront für die Objekttypen, die Sie erstellen möchten (Projekte, Programme und Portfolios), während Sie die Datensätze mit ihnen verbinden. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td> <p>Tragen Sie Berechtigungen oder höhere Berechtigungen zum Arbeitsbereich und Datensatztyp bei, dem Sie Datensätze hinzufügen möchten. </p>
   <p>Zeigen Sie Berechtigungen für den Arbeitsbereich und den Datensatztyp an oder erhöhen Sie diese, um Datensätze mithilfe der Schaltfläche Datensatz anfragen auf der Datensatzseite zu erstellen</p>
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>
   <p>Verwalten Sie Berechtigungen für Workfront-Objekte (Portfolios), um untergeordnete Objekte (Projekte) hinzuzufügen.</p>
   </td> 
  </tr>

</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen von Datensätzen mithilfe der Schaltfläche Neuer Datensatz oder Datensatz anfragen in einer beliebigen Datensatztypansicht

Benutzende mit der Berechtigung Anzeigen für den Arbeitsbereich und den Datensatztyp können Datensätze nur mithilfe der Schaltfläche Datensatz anfordern auf der Seite Datensatztyp erstellen.

Benutzende mit den Berechtigungen Beitragen und Verwalten für den Arbeitsbereich und den Datensatztyp können mithilfe der Schaltfläche Neuer Datensatz auf der Seite Datensatztyp Datensätze erstellen.


>[!IMPORTANT]
>
>Ein Workspace-Manager muss ein Anfrageformular für den Datensatztyp erstellen, damit Benutzer mit der Berechtigung Anzeigen Datensätze mithilfe eines Anfrageformulars hinzufügen können. Andernfalls können Benutzer mit Anzeigeberechtigung keine Datensätze erstellen.

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in dem Sie Datensätze hinzufügen möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz. Weitere Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

   Die Seite Datensatztyp wird in der Ansicht geöffnet, auf die Sie zuletzt zugegriffen haben. Standardmäßig wird eine Seite mit dem Datensatztyp in der Tabellenansicht geöffnet.
Alle Datensätze des ausgewählten Typs werden in der Ansicht angezeigt.

1. (Bedingt) Klicken Sie in einer beliebigen Ansicht in der oberen rechten Ecke Ihres Bildschirms auf eines der folgenden Elemente, je nach den Berechtigungen für den Arbeitsbereich und den Datensatztyp:

   * Klicken Sie **Neuer Datensatz**, wenn Sie für den Arbeitsbereich und den Datensatztyp die Berechtigung Beitragen oder eine höhere Berechtigung haben

     Oder

   * Klicken Sie **Datensatz anfordern**, wenn Sie über Anzeigeberechtigungen für den Arbeitsbereich und den Datensatztyp verfügen.

1. (Bedingt) Wenn Sie auf **Neuer Datensatz** geklickt haben, führen Sie folgende Schritte aus:

   1. Klicken Sie auf eine der folgenden Möglichkeiten, um einen Datensatz zu erstellen, und klicken Sie dann auf **Weiter**:

      * **Manuell hinzufügen**. Das Vorschaufeld des Datensatzes wird geöffnet.\
        Fügen Sie Informationen über den Datensatz hinzu, wie im Abschnitt [Erstellen von Datensätzen durch Hinzufügen inline über die Tabellenansicht des Datensatztyps](#create-records-by-adding-them-inline-from-the-record-type-table-view) in diesem Artikel beschrieben, beginnend mit Schritt 6. <!--insure this stays accurate-->
      * **Aus Datei hochladen**
Fügen Sie Datensätze hinzu, wie im Artikel [Erstellen von Datensätzen durch Importieren von Informationen aus einer CSV- oder Excel-Datei](/help/quicksilver/planning/records/import-file-to-create-records.md) beschrieben, beginnend mit Schritt 6. <!--ensure this stays accurate-->
      * **Anforderung einreichen**
Das Anfrageformular des Datensatztyps wird geöffnet.

        Ein Workspace-Manager muss ein Anfrageformular erstellen, um einen Datensatz mithilfe eines Anfrageformulars hinzufügen zu können.

        >[!TIP]
        >
        >Einige Datensatztypen können mehrere Formulare aufweisen. Klicken Sie auf eines, um es zu öffnen.

        Fügen Sie den Datensatz hinzu, wie im Artikel [Senden von Adobe Workfront-Planungsanfragen zum Erstellen von Datensätzen](/help/quicksilver/planning/requests/submit-requests.md) beschrieben, beginnend mit Schritt 6. <!--ensure this stays accurate-->

      ![Drei Möglichkeiten zum Erstellen des Datensatzauswahl-Modals](assets/three-ways-to-create-records-choice-modal.png)

1. (Bedingt) Wenn Sie auf **Eintrag anfragen** klicken, führen Sie folgende Schritte aus:

   1. (Bedingt) Wenn der Datensatztyp über mehr als ein Anfrageformular verfügt, klicken Sie auf eines, um es auszuwählen.
   2. Fahren Sie mit dem Hinzufügen von Informationen im Formular fort, um den Datensatz zu erstellen, wie im Artikel [Senden von Adobe Workfront-Planungsanfragen zum Erstellen von Datensätzen](/help/quicksilver/planning/requests/submit-requests.md) beschrieben, beginnend mit Schritt 6. <!--ensure this stays accurate-->

1. (Bedingt) Überprüfen Sie die neuen Datensätze.

   Je nachdem, wie Sie den Datensatz hinzugefügt haben, können einige der folgenden Probleme auftreten:

   * Ein neuer Datensatz wird dem Datensatztyp hinzugefügt, es sei denn, Sie haben sich dafür entschieden, ihn über ein Anfrageformular mit einem Genehmigungsprozess hinzuzufügen. Die Genehmigung muss von allen genehmigenden Personen erteilt werden, bevor der Datensatz erstellt wird.
   * Mehrere Datensätze werden dem Datensatztyp hinzugefügt, wenn Sie Datensätze mithilfe einer CSV- oder Excel-Tabelle hinzugefügt haben.
   * Eine neue Anfrage wird auf der Registerkarte Planung im Bereich Workfront-Anfragen hinzugefügt, wenn Sie die Anfrage durch Senden eines Anfrageformulars hinzugefügt haben.

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    The following items are created in Workfront Planning:

    * A read-only record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Planning record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Planning records you're linking from. 
   
-->

## Erstellen Sie Datensätze, indem Sie sie inline über die Tabellenansicht des Datensatztyps hinzufügen

Sie können Datensätze in der Tabellenansicht einer Datensatztypseite erstellen, indem Sie sie inline hinzufügen.

Informationen zum Bearbeiten von Datensatzinformationen finden Sie unter [Bearbeiten von Datensätzen](/help/quicksilver/planning/records/edit-records.md).

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in dem Sie Datensätze hinzufügen möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz. Weitere Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

   Die Seite Datensatztyp wird in der Ansicht geöffnet, auf die Sie zuletzt zugegriffen haben. Standardmäßig wird eine Seite mit dem Datensatztyp in der Tabellenansicht geöffnet.
Datensätze des ausgewählten Typs werden in der Ansicht angezeigt.

1. (Bedingt) Führen Sie in der Tabellenansicht einen der folgenden Schritte aus:

   * Klicken Sie **Neuer Datensatz** in der letzten Zeile der Tabelle oder nach dem letzten Datensatz in einer Gruppierung

     >[!TIP]
     >
     >Wenn Sie in einer Gruppierung oder Untergruppierung nach dem letzten Datensatz einen neuen Datensatz hinzufügen, füllt Workfront automatisch die in den Gruppierungen enthaltenen Felder. Sie können diese Felder bei Bedarf manuell bearbeiten, und die Datensätze können aus der Gruppierung entfernt werden.

   * Klicken Sie **einer beliebigen Spalte oder Zeile** Tabelle auf der Tastatur auf „Umschalt+Eingabe“. Dadurch wird eine leere Zeile unter dem Datensatz hinzugefügt, von dem aus Sie beginnen.
   * Bewegen Sie den Mauszeiger über das Primärfeld eines Datensatzes und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) rechts neben dem Feld und dann auf **Datensatz oben einfügen** oder **Datensatz unten einfügen**.

   ![Hinzufügen einer neuen Kampagne in der Tabellenzeile](assets/adding-a-new-campaign-in-table-row.png)

   Workfront lädt für jeden neuen Datensatz automatisch eine Miniaturansicht hoch. Sie können diese Bilder später ändern. Weitere Informationen finden Sie [Hinzufügen eines Cover-Bildes zu einem Datensatz](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md).

   Der Tabelle wird ein neuer Datensatz hinzugefügt.

1. Klicken Sie auf das primäre Feld des neuen Datensatzes

   Oder

   Klicken Sie auf **Details öffnen**-Symbol ![Details öffnen“ im Feld ](assets/open-details-icon-in-table-name-field.png)Tabellenname“ links neben dem Datensatznamen.

   Das Vorschaufeld wird in der Tabelle geöffnet.

1. Beginnen Sie mit der Eingabe von Informationen über den neuen Datensatz in die Felder, die Sie im Vorschaufeld sehen.

   >[!NOTE]
   >
   >  * Es gibt keine Pflichtfelder für Datensätze. Es wird jedoch empfohlen, Informationen für das Primärfeld eines Datensatzes hinzuzufügen, da es hilfreich ist, Datensätze zu identifizieren, wenn Datensätze miteinander verknüpft werden. Weitere Informationen zu Primärfeldern finden Sie unter [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md) und [Übersicht über Primäre Felder](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * Felder, die auf andere Datensatztypen oder berechnete Felder verweisen, sind schreibgeschützt.

1. (Bedingt) Fügen Sie beim Hinzufügen von Datensätzen in der Tabelle vor dem Öffnen des Vorschaufelds des Datensatzes weitere Informationen in jeder Zeile hinzu und klicken Sie dann auf der Tastatur auf **Eingabetaste** um die Änderungen zu speichern.

   Oder

   Klicken Sie auf den Namen des neuen Datensatzes oder auf das Symbol **Details öffnen** ![Detailsymbol öffnen im Feld &quot;](assets/open-details-icon-in-table-name-field.png)&quot; links neben dem Datensatznamen, um das Vorschaufeld zu öffnen und die Datensatzinformationen im Detailbereich zu bearbeiten.

   >[!TIP]
   >
   >Sie können auf das Symbol **Details öffnen** nur über das Namensfeld des Datensatzes zugreifen, wenn das Namensfeld ein primäres Feld ist.

1. (Optional) Klicken Sie im Vorschaufeld des Datensatzes auf das Symbol **In neuer Registerkarte öffnen** ![Details in einer neuen Registerkarte öffnen](assets/open-details-in-a-new-tab-icon.png) in der oberen rechten Ecke, um die Seite des Datensatzes in einer neuen Registerkarte zu öffnen. Bearbeitung des Datensatzes auf der Datensatzseite fortsetzen. Weitere Informationen finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

   Workfront speichert Ihre Änderungen automatisch.

1. (Optional) Schließen Sie das Vorschaufeld oder klicken Sie auf den Rückwärtspfeil links neben dem Datensatznamen, wenn Sie die Seite des Datensatzes geöffnet haben.

1. (Optional) Verwenden Sie in der Tabellenansicht die folgenden Tastaturbefehle, um das Hinzufügen neuer Datensätze oder deren Informationen rückgängig zu machen oder wiederherzustellen, wenn Sie sie in der Tabellenansicht hinzufügen:

   * STRG + Z (⌘ + Z für Mac), um eine Änderung rückgängig zu machen
   * Strg+Umsch+Z (⌘+Umschalt+Z für Mac) zum Wiederherstellen einer Änderung


<div class="preview">

## Erstellen von Datensätzen durch Hinzufügen in der Zeitleisten-Ansicht vom Datensatztyp

Sie können Datensätze in der Zeitleisten-Ansicht einer Datensatztypseite erstellen, indem Sie in die Zeitleiste doppelklicken.

Weitere Informationen zum Erstellen einer Zeitleistenansicht finden Sie unter [Verwalten der Zeitleistenansicht](/help/quicksilver/planning/views/manage-the-timeline-view.md).

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in dem Sie Datensätze hinzufügen möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite Datensatztyp wird in der Ansicht geöffnet, auf die Sie zuletzt zugegriffen haben.

1. Klicken Sie, um zuerst eine Zeitleisten-Ansicht zu öffnen oder eine Zeitleisten-Ansicht zu erstellen.

   >[!NOTE]
   >
   >Sie können eine Zeitleisten -Ansicht nur erstellen, wenn mindestens zwei Datumsfelder mit dem Datensatztyp verknüpft sind.
1. Doppelklicken Sie auf eine beliebige Stelle in der Zeitleiste.

   Ein neues Eintragsfeld wird geöffnet. <!--might need a new screen shot for Production - might add a title etc-->

   ![Neues Datensatzfeld in der Timeline mit unbenannter Datensatzleiste](assets/new-record-small-box-on-timeline.png)
1. Aktualisieren Sie die folgenden Informationen:

   * **Name**: Geben Sie den Namen des Datensatzes ein. Wenn Sie es leer lassen, benennt Workfront es **mit &quot;**&quot;.

     >[!TIP]
     >
     >Wenn Sie den Namen des Datensatzes in den Datensatzleisten entsprechend den Zeitleisteneinstellungen anzeigen, ist der Name nicht in der Datensatzleiste sichtbar, wenn er leer gelassen wird.

   * **Datensatzdatumsfelder**: Aktualisieren Sie die Daten des Datensatzes.

     Die Namen der Datumsfelder werden entsprechend den Feldern angepasst, die zum Zeitpunkt der Erstellung der Zeitleisten-Ansicht für das Start- und Enddatum ausgewählt wurden.

     Standardmäßig sind Datumswerte vorab ausgewählt, je nachdem, wie Sie die Zeitleisten -Ansicht anzeigen. Die folgenden Szenarien sind vorhanden:

      * Nach **Jahr**: Das Start- und Enddatum des Datensatzes erstrecken sich über einen Monat.
      * Nach **Quartal**: Das Start- und Enddatum des Datensatzes erstrecken sich über eine Woche.
      * Nach **Monat**: Das Start- und Enddatum des Datensatzes erstrecken sich über drei Tage.

1. (Optional) Klicken Sie auf eines der folgenden Symbole:

   * **Erweitern** ![Symbol „Erweitern](assets/expand-icon.png), um die Datensatzdetails im Vorschaufenster zu öffnen.
   * **Löschen** ![Löschen-Symbol](assets/delete-icon.png), um den Datensatz zu löschen.
   * **Schließen** ![Schließen-Symbol](assets/close-icon.png), um das neue Datensatzfeld zu schließen.

   Der Datensatz wird sofort zur Zeitleiste sowie zur Tabellen- und Kalenderansicht hinzugefügt, es sei denn, Sie haben auf das Symbol **Löschen** geklickt.
   <!--1. (Optional) Hover over one of the record bar's margins in the timeline, then drag and drop the ends of the bar to a different date. This automatically changes the start and end date of the record. 
    For information, see [Edit records](/help/quicksilver/planning/records/edit-records.md).-->

1. (Optional) Klicken Sie auf die Datensatzleiste in der Zeitleiste, um das Detailfenster des Datensatzes zu öffnen und seine Informationen zu aktualisieren, zu löschen oder Kommentare hinzuzufügen.

   >[!TIP]
   >
   >Standardmäßig verknüpft Workfront den Datensatz mit einer Miniaturansicht und einem Titelbild.
   >
   >Die Miniaturansicht wird nur in der Zeitleisten -Ansicht angezeigt, wenn sie in den Einstellungen der Ansicht aktiviert ist.

</div>

<!--

<div class="preview">

## Create records by adding them in the record type calendar view

You can create records in the calendar view of a record type page, by double-clicking anywhere on the calendar. 

For information about creating a calendar view, see [Manage the calendar view](/help/quicksilver/planning/views/manage-the-calendar-view.md).

{{step1-to-planning}}
  
1. Click the workspace where you want to add records.

    The workspace opens and the record types display as cards.

1. Click a record type card. 

    The record type page opens in the view that you last accessed. 

1. Click to open a calendar view, or create a calendar view.

    >[!NOTE]
    >
    >You can create a calendar view only if there are at least two date fields associated with the record type.
1. Double-click anywhere on the calendar. 

    A new record box opens. (********might need a new screen shot for Production - might add a title etc*********ALSO CHECK IF THE SAME ONE NEEDS REPLACING FOR TIMELINE?????)

    ![New record box on calendar with unnamed record bar](assets/new-record-small-box-on-calendar.png)

1. Update the following information:

    * **Name**: Enter the name of the record. If you leave it empty, Workfront names it **Untitled** by default. 
    
        >[!TIP]
        >
        >If you display the Name of the record in the record bars according to the calendar settings, the name is not visible in the record bar if left empty. 

    * **Record date fields**: Update the dates of the record. 
        
        The names of the date fields are customized according to the fields selected for the Start and End dates when the calendar view was created.

        By default, date values are preselected depending on how you display the calendar view. The following scenarios exist:

        * By **Month**: The record start and end dates span one day.
        * By **Week**: The record start and end dates span two days.

1. (Optional) Click one of the following icons: 

    * **Expand** ![Expand icon](assets/expand-icon.png) to open the record details in the preview window. 
    * **Delete** ![Delete icon](assets/delete-icon.png) to delete the record.
    * **Close**  ![Close icon](assets/close-icon.png) to close the new record box. 

    The record is added to the calendar as well as to the table and timeline views immediately, unless you clicked the **Delete** icon. 
1. (Optional and conditional) Choose **Month** from the upper-corner dropdown menu, hover over one of the record bar's margins in the calendar, then drag and drop the ends of the bar to a different date. This automatically changes the start and end date of the record. 

    For information, see [Edit records](/help/quicksilver/planning/records/edit-records.md).
1. (Optional) Click the record bar in the calendar to open the record's details window and update its information, delete it, or add comments. 

    >[!TIP]
    >
    >By default, Workfront associates the record with a thumbnail and a cover image.
    >
    >The thumbnail displays in the calendar view only when it is enabled in the Settings of the view. 

    (*********when this is available in both monthly and weekly, add more steps to show resizing the timeline and dragging and dropping the record in the calendar*******)

    </div> -->


## Erstellen von Datensätzen durch Kopieren und Einfügen aus einer externen Liste

1. Beginnen Sie mit der Erstellung von Datensätzen in der Tabellenansicht, wie im Abschnitt [Erstellen von Datensätzen durch manuelles Hinzufügen zu einem Datensatztyp](#create-records-by-manually-adding-them-to-a-record-type) in diesem Artikel beschrieben.

   Stellen Sie sicher, dass die Tabellenansicht über die Spalten (oder Felder) verfügt, die Sie mit den neuen Datensatzinformationen füllen möchten.

1. Klicken Sie **Neu &lt; Name des Datensatztyps >** in der letzten Zeile der Tabelle, um der Tabelle so viele neue Zeilen hinzuzufügen, wie Sie möchten.

   Fügen Sie beispielsweise 10 Zeilen zur Tabellenansicht hinzu, wenn Sie die Informationen für 10 neue Datensätze aus einer anderen Anwendung einfügen möchten.

1. Erstellen Sie in einem anderen Programm eine Liste von Datensätzen, die Sie importieren möchten.

   Sie können beispielsweise eine Excel-Tabelle verwenden, um Ihre Liste zu erstellen.

   Die Liste sollte Informationen in tabellarischer Form enthalten.

   >[!TIP]
   >
   > Die Spalten der Liste sollten Informationen zu den vorhandenen Feldern enthalten, die Sie in Workfront haben.
   >
   > Stellen Sie sicher, dass Sie die gewünschten Felder bereits in Workfront erstellt haben und dass die Informationen im Blatt im richtigen Format angezeigt werden, das dem Format der einzelnen Felder in Workfront entspricht.

1. Wählen Sie in einer anderen Anwendung mehrere Zeilen und Spalten aus und fügen Sie dann die Informationen in die Tabellenansicht „Datensatztyp“ ein, beginnend mit dem ersten neuen Datensatz.

   Die folgenden Informationen werden in den Workfront Planning-Bereich importiert:

   * Die Zeilen enthalten die neuen Datensätze
   * Die Spalten füllen Informationen für die Felder der Datensätze aus.

## Erstellen von Datensätzen durch Duplizieren

Informationen zum Duplizieren von Datensätzen finden Sie unter [Duplizieren von Datensätzen](/help/quicksilver/planning/records/copy-or-duplicate-records.md).

## Datensätze erstellen, während Sie sie verbinden

Sie können die folgenden Objekttypen erstellen, während Sie sie aus anderen Datensätzen verbinden:

* Workfront-Planungsdatensätze
* Workfront-Objekte

In diesem Abschnitt wird beschrieben, wie Sie Workfront Planning-Datensätze erstellen, während Sie sie mit anderen Datensätzen verbinden.

>[!NOTE]
>
>Das Erstellen von Workfront-Projekten und -Portfolios beim Verbinden mit Workfront-Planungsdatensätzen ähnelt dem Erstellen von Planungsdatensätzen beim Verbinden aus anderen Datensätzen.
>
>Informationen zum Erstellen von Workfront-Objekten in Workfront Planning finden Sie unter [Erstellen von Workfront-Objekten in Workfront Planning beim Verbinden mit Datensätzen](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md).

Sie müssen über Folgendes verfügen, bevor Sie neue Datensätze hinzufügen können, indem Sie sie mit vorhandenen Datensätzen verbinden:

* Verbundene Datensatztypen Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
* Einträge.
* Die richtigen Zugriffsberechtigungen in Workfront Planning und Workfront, wie im Abschnitt [Zugriffsanforderungen“ in ](#access-requirements) Artikel beschrieben.

So erstellen Sie Datensätze, während Sie sie mit anderen Datensätzen verbinden:

1. Verbinden Sie Workfront-Planungsdatensätze, wie im Artikel [Verbinden von Datensätzen](/help/quicksilver/planning/records/connect-records.md) beschrieben. Sie können Datensätze aus den folgenden Bereichen verbinden:

   * Ein Verbindungsfeld in den folgenden Bereichen von Workfront Planning:

      * Die Tabellenansicht
      * Die Detailseite oder das Vorschaufeld eines Datensatzes

   * Ein Verbindungsfeld im Abschnitt Planung eines Projekts, Portfolios oder Programms in Workfront.

     Weitere Informationen finden Sie unter [Verwalten von Datensatzverbindungen aus Workfront-Objekten](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

1. (Bedingt) Wenn Sie beim Versuch, eine Verbindung herzustellen, einen Datensatz nicht finden können, klicken Sie auf **+ Hinzufügen**

   oder
Geben Sie einen Namen ein und klicken Sie dann auf **+ Hinzufügen**. Auf die Schaltfläche **+ Hinzufügen** folgt der Name des Datensatztyps, mit dem Sie eine Verbindung herstellen. Beispiel: „Hinzufügen von Marken“, wenn eine Marke zu einer bestehenden Kampagne hinzugefügt wird. Der eingegebene Name folgt auch der Schaltfläche Hinzufügen .

   ![Schaltfläche „Hinzufügen“ zum Erstellen von Datensätzen im hervorgehobenen Kontext](assets/add-button-to-create-records-in-context-highlighted.png)

   Der Datensatz wird erstellt und dem verbundenen Datensatzfeld hinzugefügt.

   >[!IMPORTANT]
   >
   >* Sie können nur Projekte, Portfolios und Programme in Workfront erstellen, wenn Sie sie über einen Datensatz verbinden.
   >
   >* Sie können keine Gruppen oder Unternehmen erstellen, wenn Sie sie über einen Datensatz in Workfront Planning verbinden.
   > 

1. (Optional) Wechseln Sie zur Tabellenansicht des Datensatztyps, dessen Datensatz Sie erstellt haben. Ein neuer Datensatz wird in der letzten Zeile der Ansicht angezeigt.
1. (Optional) Mit dem Hinzufügen von Informationen für den neuen Datensatz in der Tabellenansicht beginnen
oder
Klicken Sie auf den Namen, um die Detailseite zu öffnen und dort Informationen hinzuzufügen.

## Erstellen von Datensätzen durch Senden eines Anforderungsformulars an einen Datensatztyp

Nachdem jemand ein Anfrageformular für einen Datensatztyp erstellt und einen Link dazu für Sie freigegeben hat, können Sie eine Anfrage senden, die einen Datensatz für diesen Datensatztyp erstellt.

Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Sowohl Workfront-Benutzer als auch externe Benutzer Ihres Unternehmens können Anfragen an Planning-Datensatztypen senden und Datensätze erstellen, wenn sie einen Link zum Anfrageformular haben.

Weitere Informationen finden Sie unter [Senden von Adobe Workfront-Planungsanfragen zum Erstellen von Datensätzen](/help/quicksilver/planning/requests/submit-requests.md).

## Erstellen von Datensätzen beim Importieren von Datensatztypen aus einer CSV- oder Excel-Datei

Sie können Datensätze importieren, wenn Sie Datensatztypen mithilfe einer CSV- oder Excel-Datei importieren.

Weitere Informationen finden Sie [Datensatztypen erstellen](/help/quicksilver/planning/architecture/create-record-types.md).

## Erstellen von Datensätzen durch Importieren von Datensätzen aus einer CSV- oder Excel-Datei

Sie können Datensätze für vorhandene Datensatztypen importieren, wenn Sie Informationen aus einer CSV- oder Excel-Datei importieren.

Weitere Informationen finden Sie unter [Erstellen von Datensätzen durch Importieren von Informationen aus einer CSV- oder Excel-Datei](/help/quicksilver/planning/records/import-file-to-create-records.md).

## Erstellen von Datensätzen mithilfe von Automatisierungen

Sie können Automatisierungen in Workfront Planning konfigurieren, die Datensätze erstellen, wenn sie aktiviert sind, sobald sie aus einem Planungsdatensatz ausgelöst werden. Die erstellten Datensätze werden automatisch mit den Datensätzen verbunden, für die Sie die Automatisierung auslösen.

Sie können die Automatisierung auf der Seite des Datensatzes in Workfront Planning konfigurieren und aktivieren. Der verknüpfte Datensatz, der erstellt wird, wird in das Feld „Verbunden“ des Datensatztyps eingefügt, von dem aus die Automatisierung ausgeführt wird.

Weitere Informationen finden Sie unter [Erstellen von Objekten mithilfe von Adobe Workfront Planning-Datensatzautomatisierungen](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).



