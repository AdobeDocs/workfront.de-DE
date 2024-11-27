---
title: Datensätze erstellen
description: Bei Verwendung der Adobe Workfront-Planung ist ein Datensatz eine Instanz eines Datensatztyps. In der Workfront-Planung können Sie für jeden Datensatztyp eindeutige Datensätze erstellen, indem Sie diese manuell zur Tabellenansicht hinzufügen, aus einer Liste importieren, duplizieren oder erstellen, während Sie ihn mit anderen Datensätzen verbinden.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: d962d60294295dd1f3771d1f0b737c9d1f03dfef
workflow-type: tm+mt
source-wordcount: '1617'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Datensätze erstellen

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Versionen für die Produktion sind in der Produktionsumgebung dieselben Funktionen auch für Kunden verfügbar, die schnelle Versionen aktiviert haben. </span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md) </span>.

{{planning-important-intro}}

In der Adobe Workfront-Planung ist ein Datensatz eine Instanz eines Datensatztyps.

Sie können Datensätze anhand einer der folgenden Methoden erstellen:

* [Hinzufügen von Datensätzen auf der Seite &quot;Record Type&quot;in der Tabellenansicht](#create-records-by-adding-them-to-a-record-type-in-a-record-type-table)
* [Datensätze aus einer externen Liste kopieren und einfügen](#create-records-by-copying-and-pasting-them-from-an-external-list)
* [Datensätze aus einer Tabellenansicht duplizieren](#create-records-by-duplicating-them)
* [Erstellen Sie Datensätze, während Sie sie mit anderen Datensätzen verbinden](#create-records-as-you-connect-them)
* [Erstellen Sie sie, indem Sie ein Anfrageformular an einen Datensatztyp senden](#create-records-by-submitting-a-request-form-to-a-record-type)
* <span class="preview">[Erstellen von Datensätzen beim Import von Datensatztypen aus einer CSV- oder Excel-Datei](#create-records-when-importing-record-types-from-a-csv-or-excel-file)</span>


Informationen zum Verwalten von Datensätzen in der Tabellen- oder Timeline-Ansicht finden Sie in den folgenden Artikeln:

* [Tabellenansicht verwalten](/help/quicksilver/planning/views/manage-the-table-view.md)
* [Verwalten der Timeline-Ansicht](/help/quicksilver/planning/views/manage-the-timeline-view.md)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Workfront-Planung anzuzeigen.

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
   <p> Produkte</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront-Planung<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Plan*</p></td> 
   <td> 
<p>Die folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Erstklassig</li> 
<li>Ultimativ</li></ul> 
<p>Die Workfront-Planung ist für veraltete Workfront-Pläne nicht verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td> 
   <td> 
<p>Alle </p> 
<p>Weitere Informationen zu den Funktionen der einzelnen Workfront-Planungspläne erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Die Workfront-Instanz Ihres Unternehmens muss in das Adobe Unified Experience integriert sein, damit Sie auf alle Funktionen der Workfront-Planung zugreifen können.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td> Standard
   <p>Für ältere Workfront-Lizenzen ist die Workfront-Planung nicht verfügbar.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Für die Adobe Workfront-Planung gibt es keine Zugriffssteuerungselemente</p> 
   <p>Bearbeiten Sie den Zugriff in Workfront für die Objekttypen, die Sie erstellen möchten (Projekte und Portfolios), während Sie die Datensätze mit ihnen verbinden. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td> <p>Verwalten Sie Berechtigungen für den Arbeitsbereich, dem Sie Datensätze hinzufügen möchten. </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p>
   <p>Verwalten Sie Berechtigungen für Workfront-Objekte (Portfolios), um untergeordnete Objekte (Projekte) hinzuzufügen.</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen von Datensätzen durch Hinzufügen zu einem Datensatztyp in einer Tabelle vom Typ Datensatz

Sie können Datensätze in der Tabellenansicht einer Seite vom Typ Datensatz erstellen.

Informationen zum Bearbeiten von Datensatzinformationen finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in den Sie Datensätze hinzufügen möchten.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden als Karten angezeigt.

1. Klicken Sie auf eine Karte vom Typ Datensatz. Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

   Die Seite mit dem Datensatztyp wird in der Ansicht geöffnet, auf die Sie zuletzt zugegriffen haben. Standardmäßig wird eine Seite vom Typ Datensatz in der Tabellenansicht geöffnet.
Alle Datensätze des ausgewählten Typs werden in der Ansicht angezeigt.

1. (Bedingt) Führen Sie je nach angezeigter Ansicht einen der folgenden Schritte aus:

   * In der Tabellenansicht:

      * Klicken Sie in der letzten Zeile der Tabelle auf **Neuer Datensatz** .

      * Klicken Sie in einer beliebigen Spalte oder Zeile der Tabelle auf die Tastenkombination **Umschalt + Eingabetaste**. Dadurch wird eine leere Zeile unter dem Datensatz hinzugefügt, aus dem Sie beginnen.
      * Bewegen Sie den Mauszeiger über das Primärfeld eines Datensatzes, klicken Sie auf das Menü **Mehr** Menü ![](assets/more-menu.png) rechts neben dem Feld und klicken Sie dann auf **Datensatz über** einfügen oder **Datensatz unter** einfügen .

     ![](assets/adding-a-new-campaign-in-table-row.png)

   * Aus jeder Sicht:

      * Klicken Sie oben rechts auf der Seite auf **Neuer Datensatz** . Das Vorschaufeld für Datensätze wird geöffnet.

     Workfront lädt automatisch eine Miniaturansicht und ein Titelbild in jeden neuen Datensatz hoch. Sie können diese Bilder später ändern. Weitere Informationen finden Sie in den folgenden Artikeln:

      * [Hinzufügen eines Titelbilds zu einem Datensatz](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md)
      * [Hinzufügen einer Miniaturansicht zu einem Datensatz](/help/quicksilver/planning/records/add-thumbnails-to-records.md)

1. Geben Sie in die im Vorschaufenster angezeigten Felder Informationen zum neuen Datensatz ein.

   >[!NOTE]
   >
   >  * Es gibt keine Pflichtfelder für Datensätze. Es wird jedoch empfohlen, Informationen für das primäre Feld eines Datensatzes hinzuzufügen, da es beim Verknüpfen von Datensätzen hilfreich ist, Datensätze zu identifizieren. Weitere Informationen zu Primärfeldern finden Sie unter [Tabellenansicht verwalten](/help/quicksilver/planning/views/manage-the-table-view.md) und [Übersicht über Primäre Felder](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * Felder, die auf andere Datensatztypen oder berechnete Felder verweisen, sind schreibgeschützte Felder.

1. (Bedingt) Wenn Sie Datensätze in die Tabelle einfügen, fügen Sie weiterhin Informationen zu jeder Zeile hinzu und klicken Sie dann auf der Tastatur auf **Enter** , um Ihre Änderungen zu speichern.

   Oder

   Klicken Sie auf den Namen des neuen Datensatzes oder auf das Symbol **Details öffnen** ![](assets/open-details-icon-in-table-name-field.png) links neben dem Datensatznamen. Eine Vorschau mit den detaillierten Informationen des Datensatzes wird in der Tabelle geöffnet.

   >[!TIP]
   >
   >Sie können nur dann auf das Symbol **Details öffnen** zugreifen, wenn das Feld &quot;Name&quot;ein primäres Feld ist.

1. Bearbeiten Sie die Datensatzinformationen in der Vorschau des Datensatzes. Workfront speichert Ihre Änderungen automatisch.
1. (Optional) Klicken Sie oben rechts in der Vorschau des Datensatzes auf das Symbol **In neuer Registerkarte öffnen** ![](assets/open-details-in-a-new-tab-icon.png) , um die Seite des Datensatzes in einer neuen Registerkarte zu öffnen. Bearbeiten Sie den Datensatz auf der Datensatzseite weiter. Weitere Informationen finden Sie unter [Datensätze bearbeiten](/help/quicksilver/planning/records/edit-records.md).

1. (Optional) Verwenden Sie die folgenden Tastaturbefehle, um das Hinzufügen neuer Datensätze oder ihrer Informationen rückgängig zu machen oder wiederherzustellen, wenn Sie sie in der Tabellenansicht hinzufügen:

   * STRG + Z ( ⌘ + Z für Mac) zum Rückgängigmachen einer Änderung
   * STRG + Umschalt + Z ( ⌘ + Umschalt + Z für Mac) zum Wiederholen einer Änderung

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

## Datensätze durch Kopieren und Einfügen aus einer externen Liste erstellen

1. Beginnen Sie mit der Erstellung von Datensätzen in der Tabellenansicht, wie im Abschnitt [Erstellen von Datensätzen beschrieben, indem Sie sie manuell zu einem Datensatztyp hinzufügen](#create-records-by-manually-adding-them-to-a-record-type) in diesem Artikel.

   Stellen Sie sicher, dass die Tabellenansicht über die Spalten (oder Felder) verfügt, die mit den neuen Datensatzinformationen gefüllt werden sollen.

1. Klicken Sie in der letzten Zeile der Tabelle auf **Neu &lt; Name des Datensatztyps >** , um der Tabelle so viele neue Zeilen hinzuzufügen, wie die neuen Datensätze sein sollen.

   Fügen Sie der Tabellenansicht beispielsweise 10 Zeilen hinzu, wenn Sie die Informationen für 10 neue Datensätze aus einer anderen Anwendung einfügen möchten.

1. Erstellen Sie in einer anderen Anwendung eine Liste von Datensätzen, die Sie importieren möchten.

   Sie können beispielsweise eine Excel-Tabelle verwenden, um Ihre Liste zu erstellen.

   Die Liste sollte Informationen im Tabellenformat enthalten.

   >[!TIP]
   >
   > Die Spalten der Liste sollten Informationen zu den in Workfront vorhandenen Feldern enthalten.
   >
   > Vergewissern Sie sich, dass die gewünschten Felder bereits in Workfront erstellt wurden und dass die Informationen in Ihrem Arbeitsblatt im richtigen Format angezeigt werden, das dem der Felder in Workfront entspricht.

1. Wählen Sie in einer anderen Anwendung mehrere Zeilen und Spalten aus und fügen Sie dann die Informationen in die Tabellenansicht des Datensatztyps ein, beginnend mit dem ersten neuen Datensatz.

   Die folgenden Informationen werden in den Workfront-Planungsbereich importiert:

   * Die Zeilen enthalten die neuen Datensätze
   * Die Spalten enthalten Informationen zu den Feldern der Datensätze.

## Datensätze durch Duplizierung erstellen

Informationen zum Duplizieren von Datensätzen finden Sie unter [Duplizieren von Datensätzen](/help/quicksilver/planning/records/copy-or-duplicate-records.md).

## Erstellen von Datensätzen während der Verbindung

Sie können Datensätze oder Workfront-Objekte erstellen, während Sie sie mit anderen Datensätzen verbinden.

Sie müssen über Folgendes verfügen, bevor Sie neue Datensätze oder Workfront-Objekte hinzufügen können, indem Sie sie aus vorhandenen Datensätzen verbinden:

* Verbundene Datensatztypen. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
* Verbundene Datensätze. Weitere Informationen finden Sie unter [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md).
* Die korrekten Zugriffs- und Zugriffsberechtigungen in Workfront Planning und Workfront, wie im Abschnitt [Zugriffsanforderungen](#access-requirements) in diesem Artikel beschrieben.

>[!NOTE]
>
>Das Erstellen von Workfront-Projekten und -Portfolios während Sie sie mit Workfront-Planungsdatensätzen verbinden, ähnelt dem Erstellen von Datensätzen für die Planung , während Sie sie mit anderen Datensätzen verbinden.

So erstellen Sie Datensätze, während Sie sie aus anderen Datensätzen verbinden:

1. Beginnen Sie mit dem Verbinden von Workfront-Planungsprotokollen, wie im Artikel [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md) beschrieben.
1. (Bedingt) Wenn Sie beim Versuch, einen Datensatz aus dem verbundenen Datensatzfeld eines anderen Datensatzes hinzuzufügen, keinen Eintrag finden können, suchen Sie nach einem Datensatz und klicken Sie auf **+ Hinzufügen**. Auf die Schaltfläche **+ Hinzufügen** folgt der Name des Datensatztyps, aus dem Sie eine Verbindung herstellen.

   ![](assets/add-button-to-create-records-in-context-highlighted.png)

   Der Datensatz wird erstellt und dem Feld des verbundenen Datensatzes hinzugefügt.

   >[!IMPORTANT]
   >
   >* Sie können nur Projekte und Portfolios in Workfront erstellen, wenn Sie sie aus einem Datensatz verbinden.
   >
   >* Sie können keine Programme, Gruppen oder Unternehmen erstellen, wenn Sie sie aus einem Datensatz in der Workfront-Planung verbinden.
   >
   >* Sie können ein Projekt nicht aus einer Vorlage erstellen, wenn Sie Projekte durch Verbinden aus einem Datensatz erstellen. Sie müssen dem neuen Projekt manuell Aufgaben und Projektinformationen oder eine Vorlage hinzufügen, nachdem Sie sie zum Datensatz hinzugefügt haben.

1. (Optional) Rufen Sie die Tabellenansicht des Datensatztyps auf, dessen Datensatz Sie erstellt haben. In der letzten Zeile der Ansicht wird ein neuer Datensatz angezeigt.
1. (Optional) Beginnen Sie mit dem Hinzufügen von Informationen für den neuen Datensatz in der Tabellenansicht.
Oder
Klicken Sie auf seinen Namen, um die Detailseite zu öffnen und dort Informationen hinzuzufügen.

## Erstellen von Datensätzen durch Senden eines Anfrageformulars an einen Datensatztyp

Nachdem ein Benutzer ein Anfrageformular für einen Datensatztyp erstellt und einen Link mit Ihnen geteilt hat, können Sie eine Anfrage senden, die einen Datensatz für diesen Datensatztyp erstellt.

Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anforderungsformulars in der Adobe Workfront-Planung](/help/quicksilver/planning/requests/create-request-form.md).

Sowohl Workfront-Benutzer als auch externe Benutzer Ihrer Organisation können Anfragen an die Planung von Datensatztypen senden und Datensätze erstellen, sofern sie über eine Verknüpfung mit dem Anfrageformular verfügen.

Weitere Informationen finden Sie unter [Planungsanfragen zur Erstellung von Datensätzen mit Adobe Workfront senden](/help/quicksilver/planning/requests/submit-requests.md).

<div class="preview">

## Erstellen von Datensätzen beim Import von Datensatztypen aus einer CSV- oder Excel-Datei

Datensätze können beim Import von Datensatztypen mithilfe einer CSV- oder Excel-Datei importiert werden.

Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

</div>