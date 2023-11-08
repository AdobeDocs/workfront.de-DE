---
title: Übersicht über Adobe Maestro
description: Adobe Maestro ist ein neues Angebot von Adobe Workfront. Sie können vollständig anpassbare Arbeitsbereiche erstellen, um Workflows zu definieren, die den Anforderungen jeder Organisationseinheit in Ihrem Unternehmen entsprechen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: b1d6e0b3-e6d4-46d1-a6a2-4b8b73f7d3f7
source-git-commit: 324ad45b52dafa96c2854f1fec1172b88643bdc2
workflow-type: tm+mt
source-wordcount: '1845'
ht-degree: 1%

---

# Übersicht über Adobe Maestro

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

<!--see the separate article I wrote to have the PMs vet it for this: https://adobe-my.sharepoint.com/personal/alinaw_adobe_com/_layouts/15/doc.aspx?sourcedoc={79f94807-3d73-4015-afc0-5c016fc63cfc}&action=edit-->

<!--all the links are hidden for now, so I can share this with customer zero. Activate the links before making this public. -->

<!-- remove the references to closed beta from the entire article-->

<!--update the video in the IMPORTANT below, when we have something better, especially after Open Beta - remove it-->

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Maestro, ein neues Angebot von Adobe.
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>[Videodemonstration von Adobe Maestro anzeigen](https://video.tv.adobe.com/v/3424253/){target=_blank}

## Einführung in Adobe Maestro

Adobe Maestro ist ein neues Angebot von Adobe Workfront. Maestro soll umfassende Einblicke in die operativen Details einer Organisation gewinnen und wichtige Geschäftsfragen in jeder Phase des Lebenszyklus der Arbeitsverwaltung beantworten.

Teams und Führungskräfte benötigen klare Antworten auf Fragen wie:

* Wie viele Kampagnen führen wir in EMEA für das 4. Quartal durch?
* Gibt es Zielgruppenüberschneidungen zwischen gleichzeitigen Kampagnen?
* Wie gut laufen die Sensibilisierungsprogramme derzeit?
* Wie sehen die Assets für eine bestimmte Kampagne aus? Welche von ihnen müssen noch genehmigt werden?

Um diese Fragen zu beantworten, braucht Führungskräfte eine Lösung, die einen ganzheitlichen Überblick über alle Arbeitsschritte von der Planung über die Ausführung bis zur Messung der Ergebnisse liefert. Derzeit verfügen Unternehmen über Tools, die einige Teile des Prozesses abdecken können, aber viele verfügen nicht über gute Verbindungen zu allen Phasen der Arbeit und können auch keine zuverlässigen Ergebnisse liefern.

Im Folgenden finden Sie einige der wichtigsten Funktionen von Maestro:

* Lösung des Problems der Verwaltung der Arbeit in allen Phasen und für alle am Arbeitsprozess beteiligten Akteure.
* Passen Sie Ihre Workflows vollständig an, indem Sie entscheiden, welche Objekttypen (oder Datensatztypen) Ihr Unternehmen verwendet, und konfigurieren Sie, wie diese Objekte miteinander verknüpft werden.
* Relation zu Objektarten aus anderen Systemen, Erstellung eines kohärenten Frameworks für alle Ihre Prozesse.

## Zugriff erforderlich für die Verwendung von Maestro während des geschlossenen Betaprogramms

>[!IMPORTANT]
>
>Derzeit gibt es keine Zugriffsebenen oder Berechtigungen, die mit Benutzern oder den Informationen in Maestro verknüpft sind. Alle Benutzer können alle Informationen, die andere Benutzer Maestro hinzufügen, anzeigen, bearbeiten und löschen.

Weitere Informationen zum erforderlichen Zugriff für die Verwendung von Maestro finden Sie unter [Adobe Maestro-Zugriffsübersicht](../maestro/access/access-overview.md).

<!-- hidden the table after I moved the content to the Access overview article: 

You must have the following access to use Adobe Maestro: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader">Access level</td>
   <td> <p>Any</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see <a href="../maestro/access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

************* Activate note when going to GA: 

>[!NOTE]
>
>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). 
-->

## Maestro-Terminologie

Maestro ist zwar Teil von Workfront, bietet aber auch proprietäre Konzepte und Terminologie. Stellen Sie sicher, dass Sie mit den Maestro-Konzepten vertraut sind, bevor Sie mit der Einrichtung von Maestro für Ihr Unternehmen beginnen.

Das Framework für Maestro ist vollständig anpassbar. Sie können alle Datensatztypen, ihre Attribute und alle mit ihnen verknüpften Felder entsprechend den Anforderungen Ihrer Organisation erstellen.

Im Folgenden finden Sie die wichtigsten Maestro-Objekte und -Konzepte:

* **Arbeitsbereich**: Eine Sammlung von Datensatztypen und Taxonomien, die den betrieblichen Lebenszyklus eines bestimmten Unternehmens definieren. Ein Arbeitsbereich ist der Arbeitsbereich einer Organisationseinheit.

  Eine Workfront-Instanz kann über maximal 1.000 Arbeitsbereiche verfügen.

  ![](assets/marketing-workspace-with-record-type-taxonomies-opening-page.png)

  Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](../maestro/architecture-and-fields/create-workspaces.md).

* **Record Type**: Der Maestro-Hauptobjekttyp.

  Im Gegensatz zu Workfront, wo die Objekttypen vordefiniert sind, können Sie in Maestro eigene Objekttypen erstellen.

  Beispielsweise sind in Workfront die Objektarten &quot;Programm&quot;, &quot;Portfolio&quot;, &quot;Projekt&quot;, &quot;Aufgabe&quot;oder &quot;Problem&quot;bereits erstellt.

  In Maestro können Sie alle Datensatztypen erstellen, die den Workflows Ihres Unternehmens entsprechen. Später können Sie definieren, wie sich die Datensatztypen untereinander oder mit Formularabhängigkeiten verhalten.

  Weitere Informationen finden Sie unter [Übersicht über die Betriebsdatentypen und -taxonomien](../maestro/architecture-and-fields/overview-of-record-types-and-taxonomies.md).

  Maestro verfügt über die folgenden Datensatztypen:

   * **Betriebsdatentyp**: Ein Datensatztyp, der strategische Pläne, Initiativen oder ausgeführte Arbeiten darstellt.

     ![](assets/operational-record-type-blank.png)

     Beispielsweise kann Campaign, Activity, Programm operationelle Datensatztypen sein.

     Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](../maestro/architecture-and-fields/create-record-types.md).

   * **Taxonomie**: Ein Record Type, der Attribute über einen operationellen Record erfasst.

     ![](assets/taxonomy-record-type-blank.png)

     Obwohl das Erstellen von Taxonomien mit dem Erstellen von operationellen Datensatztypen identisch ist, unterscheidet Maestro zwischen einem operationellen Datensatztyp und einem Taxonomiedatensatstyp. Ziel von Taxonomien ist es, die operationellen Datensatztypen zu verbessern. <!--this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.-->

     Beispielsweise können Datensatztypen vom Typ Zielgruppe, Region oder Adresse vom Typ Taxonomie sein.

     Weitere Informationen finden Sie unter [Erstellen von Taxonomiedatensatztypen](../maestro/architecture-and-fields/create-a-taxonomy.md).

* **Datensatz**: Eine Instanz eines Maestro-Datensatztyps. Ein Datensatz kann sich auf einen operationellen Datensatztyp oder auf eine Taxonomie beziehen.

  ![](assets/records-highlighted-in-campaign-record-type-list.png)
  ![](assets/records-highlighted-in-region-taxonomy-type-list.png)

  Nachdem Sie einem Arbeitsbereich einen Datensatztyp hinzugefügt haben, können Sie damit beginnen, Datensätze dieses Typs auf der Seite des Datensatztyps hinzuzufügen.

  Beispielsweise kann &quot;Campaign&quot;ein operativer Record-Typ sein und &quot;Summer Campaign for EMEA&quot;ist ein Datensatz vom Typ &quot;Campaign Record&quot;

  Oder

  &quot;Region&quot;ist ein Datensatz vom Typ Taxonomie, während &quot;Nord- und Südamerika&quot;oder &quot;EMEA - Mitteleuropa&quot;Taxonomie-Datensätze sind.

  Weitere Informationen finden Sie unter [Datensätze erstellen](../maestro/records/create-records.md).

* **Workspace-Vorlage**: Sie können einen Arbeitsbereich mit vordefinierten Vorlagen erstellen. Sie können die vordefinierten Datensatztypen, Taxonomien und Felder, die in einer Vorlage enthalten sind, verwenden oder eigene hinzufügen.

  ![](assets/workspaces-page-with-templates-thumbnails.png)

  Maestro enthält eine Workspace-Vorlage für Vertrieb, Marketing und Produktverwaltung .

  Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](../maestro/architecture-and-fields/create-workspaces.md).

* **Felder**: Felder sind Attribute, die Sie zu Betriebs- oder Taxonomiedatensatztypen hinzufügen können, die Informationen zum Datensatztyp enthalten. <!--check the shot below, "Connection" needs to be in lowercase-->

  ![](assets/drop-down-list-of-record-fields.png)

  Überlegungen zu Maestro-Feldern:

   * Die Felder, die Sie für einen Datensatztyp hinzufügen, werden automatisch allen Datensätzen dieses Typs zugeordnet und können zum Erfassen von Daten zu diesen Datensätzen verwendet werden.

   * Felder werden in der Tabellenansicht als Spalten angezeigt, die auf eine Seite vom Typ Datensatz angewendet werden. Sie werden auch auf der Detailseite des Datensatzes angezeigt.

   * Felder sind für einen Datensatztyp eindeutig und werden nicht von einem Datensatztyp zum anderen übertragen.

   * Maestro-Felder können vollständig angepasst werden und sind nur in Maestro verfügbar. Sie können nicht über Workfront auf Maestro-Felder zugreifen.

  Weitere Informationen finden Sie unter [Felder erstellen](../maestro/architecture-and-fields/create-fields.md)

  Ein neuer operationeller Datensatztyp ist standardmäßig mit den folgenden vordefinierten Feldern verknüpft:

   * Name
   * Beschreibung
   * Startdatum
   * Enddatum
   * Status

  Ein neuer Taxonomie-Record-Typ ist standardmäßig mit einem Namensfeld verknüpft.

  Sie können benutzerdefinierte Felder der folgenden Typen erstellen:

   * Einzeiliger Text
   * Absatz
   * Mehrfachauswahl
   * Einzelauswahl
   * Datum
   * Zahl
   * Prozentsatz
   * Währung
   * Kontrollkästchen
   * Personen
   * Erstellt von
   * Erstellungsdatum
   * Zuletzt geändert von
   * Zuletzt geändert am

* **Verknüpfte Datensatztypen**, **Verknüpfte Datensätze**, und **Verknüpfte Datensatzfelder**: Sie können eine Verbindung zwischen den folgenden Entitäten herstellen:

   * Zwei Maestro-Record-Typen
   * Ein Maestro-Record-Typ und ein Workfront-Projekt-, Programm-, Portfolio-, Unternehmens- oder Gruppenobjekttyp.

  ![](assets/new-connection-tab-with-workfront-option.png)

  Nachdem Sie eine Verbindung zwischen den Datensatztypen hergestellt haben, können Sie einzelne Datensätze dieser Typen miteinander verbinden. Die Verbindung zwischen den Datensätzen wird als verknüpftes Datensatzfeld angezeigt.

* **Verknüpfte Felder** (oder Suchfelder): Nachdem Sie die Verbindung zwischen zwei Datensatztypen hergestellt und einzelne Datensätze miteinander verknüpft haben, können Sie auf die Felder der verknüpften Datensätze in dem Datensatz verweisen, aus dem Sie eine Verbindung herstellen.

  ![](assets/add-lookup-fields-modal.png)

  Informationen zum Verknüpfen von Datensatztypen und Datensätzen sowie zum Erstellen verknüpfter Felder finden Sie in den folgenden Artikeln:

   * [Datensatztypen verbinden](../maestro/architecture-and-fields/connect-record-types.md)
   * [Datensätze verbinden](../maestro/records/connect-records.md)

<!--not yet:* Fields are reusable across Record Types.  -->

* **Ansichten**: Datensätze werden unter der jeweiligen Datensatztyp-Seite in verschiedenen Ansichten angezeigt.

  ![](assets/view-types-drop-down-from-record-type-list.png)

  Ansichten enthalten personalisierte Einstellungen eines bestimmten Ansichtstyps, z. B. die Liste der Felder (Spalten), eine Liste von Datensätzen (Zeilen), ihre Reihenfolge (Sortierung), einen angewendeten oder anwendbaren Filter und eine Gruppierung.

  Im Folgenden finden Sie Ansichtstypen, die Sie auf die Seite vom Typ Datensatz anwenden können:

   * **Tabellenansicht**: Zeigt Datensätze und deren Felder im Tabellenformat an. Die Tabellenzeilen enthalten die einzelnen Datensätze und die Spalten die Datensatzfelder. Dies ist die Standardansicht.

     ![](assets/table-view-example.png)

   * **Timeline-Ansicht**: Zeigt Datensätze mit mindestens zwei Datumsfeldern in einer chronologischen Zeitleiste an.

     ![](assets/grouping-applied-in-timeline-view.png)

  Weitere Informationen finden Sie unter [Verwalten von Datensatzansichten](../maestro/views/manage-record-views.md).


## Maestro-Objektbeschränkungen

Die folgende Tabelle zeigt die Einschränkungen für die Anzahl der Objekte, die Sie in Maestro erstellen können. Die Einschränkungen können sich ändern, wenn wir in die nächsten Phasen der Entwicklung von Maestro eintreten.

| Maestro-Objekt | Limit |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
| Anzahl der Arbeitsbereiche für eine Workfront-Instanz | 1,000 |
| Anzahl der Datensatztypen für einen Arbeitsbereich | 1.000 (dies umfasst Taxonomien für den Arbeitsbereich oder Objekte, die Sie aus Drittanbieteranwendungen importieren) |
| Datensatzanzahl für einen Datensatztyp | 10,000 |
| Anzahl der Felder für einen Datensatztyp oder eine Taxonomie | 500 |
| Anzahl der Zeichen für ein Textfeld | 1.000 Zeichen |
| Dateigröße, die Sie in eine Datensatztyp-Tabelle einfügen können | 1MB |
| Dateigröße, die Sie über die API für eine Datentyptabelle importieren können | 1.5MB |
| Die Rate, mit der API-Anfragen gestellt werden können | 200 Anfragen pro Minute |
| Größe der CSV-Datei, die Sie in eine Tabelle importieren können | 5MB |

## Maestro für Benutzer in Ihrer Workfront-Instanz aktivieren

Ihr Unternehmen muss sich im geschlossenen Betaprogramm von Adobe Maestro anmelden, bevor Sie auf Maestro zugreifen können. Wenden Sie sich an Ihren Kundenbetreuer, um Informationen zur Anmeldung im Beta-Programm zu erhalten.

Weitere Informationen zur Gewährung des Zugriffs auf Maestro und zur Ermöglichung der Verwendung durch andere finden Sie unter [Zugriff auf Adobe Maestro gewähren](../maestro/access/grant-access.md).

<!--hidden this after moved it to a separate article

After your organization has been enrolled in the Maestro beta program, you can add the Maestro area for other users by using a layout template. 

To share the Maestro area using a layout template: 

1. Log in to Workfront as a system administrator.  

1. Add the Maestro icon to the Main Menu using a Layout Template. For information, see [Customize the Main Menu using a layout template](../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md). 

1. Assign the  layout template to the users that you want to have access to Maestro.For information, see [Assign users to a layout template](../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

    All users who can access Maestro in their Main Menu can start creating workspaces, records types, records, and fields.  
  -->


## Suchen Sie Maestro

Stellen Sie sicher, dass Ihr Unternehmen Zugriff auf Maestro erhalten hat und dass Ihr System- oder Gruppenadministrator den Bereich Maestro zu Ihrem Hauptmenü hinzugefügt hat.

Suchen nach Maestro:

1. Melden Sie sich bei Adobe Workfront an.

1. Klicken Sie auf **Hauptmenü** ![](assets/main-menu-workfront.png) in der oberen rechten Ecke oder klicken Sie auf das **Hauptmenü** ![](assets/main-menu-shell.png) oben links, falls verfügbar.

1. Klicks **Maestro** ![](assets/maestro-icon.png).

   Der Arbeitsbereich von Maestro wird geöffnet.

1. (Optional und empfohlen) Fahren Sie mit einigen der folgenden Aktionen fort, um Ihre Arbeitsstruktur in Maestro zu erstellen:

   1. Erstellen Sie einen neuen Arbeitsbereich oder verwenden Sie eine Vorlage.

   1. Fügen Sie dem neuen Arbeitsbereich Datensatztypen hinzu.

   1. Fügen Sie den neuen Arbeitsbereichen Taxonomien hinzu.

   1. Klicken Sie auf den Namen eines Datensatztyps, um die Datensatzseite zu öffnen. Die Datensatzseite wird standardmäßig in der Tabellenansicht geöffnet.

   1. Passen Sie die Tabellenansicht an, indem Sie einen der folgenden Schritte ausführen:

      * Fügen Sie dem Datensatztyp weitere Felder hinzu, indem Sie auf die Schaltfläche **+** in der oberen rechten Ecke. Die Spalten in der Ansicht sind Felder, die mit dem Datensatztyp verknüpft sind.
      * Hinzufügen von Datensätzen durch Klicken auf **+** in der linken unteren Ecke. Die Zeilen in der Ansicht sind eindeutige Datensätze des ausgewählten Datensatztyps.
      * Klicks **Filter** , um die angezeigten Informationen auf der Seite vom Typ Datensatz zu filtern.

   1. Klicken Sie auf den Namen eines Datensatzes, um weitere Informationen auf der Detailseite des Datensatzes anzuzeigen.

   1. Erstellen Sie eine Timeline-Ansicht aus dem **Ansicht** Dropdown-Menü in der oberen rechten Ecke der Seite vom Typ Datensatz.

   1. Passen Sie die Timeline-Ansicht an, indem Sie Filter, Gruppierungen oder Einstellungen aktualisieren.

## Derzeit in Maestro verfügbare Funktionen

Die folgende Tabelle zeigt die wichtigsten Funktionen, die in Maestro verfügbar sein werden, und einen Zeitplan ihrer Verfügbarkeit. Die Liste enthält nicht alle Funktionen.

| Funktion | Jetzt verfügbar | In Kürze verfügbar | Forschung |
|----------------------------------------------------|:-----------------------------:|:--------------------------------:|:----------------:|
| Erstellen von Arbeitsbereichen | ✓ |                                  |                  |
| Erstellen von operationellen Datensatztypen | ✓ |                                  |                  |
| Erstellen von Taxonomien | ✓ |                                  |                  |
| Erstellen einzelner, benannter Datensätze und Taxonomien | ✓ |                                  |                  |
| Benutzerdefinierte Datensatzfelder erstellen | ✓ |                                  |                  |
| Importieren von Datensatztypen und Feldern mithilfe einer Excel- oder CSV-Datei | ✓ |                                  |                  |
| Link-Datensätze | ✓ |                                  |                  |
| Datensätze in einer Tabelle anzeigen | ✓ |                                  |                  |
| Anzeigen von Datensätzen in einer Timeline | ✓ |                                  |                  |
| Datensätze filtern | ✓ |                                  |                  |
| Gruppieren von Datensätzen in der Timeline-Ansicht | ✓ |                                  |                  |
| Gruppieren von Datensätzen in der Tabellenansicht | ✓ |                                 |                  |
| Sortieren von Datensätzen in der Tabellenansicht | ✓ |                                 |                  |
| Sortieren von Datensätzen in der Timeline-Ansicht |                               | ✓ |                  |
| Sortieren von Gruppierungen in der Tabellenansicht |                               | ✓ |                  |
| Sortieren von Gruppierungen in der Timeline-Ansicht |                               | ✓ |                  |
| Arbeitsbereiche verbinden |                               | ✓ |                  |
| Maestro-Datensätze und Taxonomien verbinden | ✓ |
| In der Tabellenansicht nach Datensätzen suchen | ✓ |   |
| Verbinden von Maestro-Datensätzen mit Workfront-Projekten, -Programmen, -Portfolios, -Unternehmen, -Gruppen | ✓ |                                 |                  |
| Seite mit Datensatzdetails | ✓ |                                  |                  |
| Layout der Seite mit den Datensatzdetails aktualisieren |                               | ✓ |                  |
| Zugriffsebenen und Berechtigungen | | ✓ |  |
| Anfragen senden |                               |                                  | ✓ |
| Kreativbeschreibung |                               |                                  | ✓ |
| Farbe und Symbol eines Datensatzes anpassen | ✓ |                                  |                 |
<!--
Add another row for Rich text formatting:


|     Rich Text formatting for Paragraph fields                                 |      ✓                         |                                  |                 |
-->

## Maestro-Release-Aktivität

Wir veröffentlichen regelmäßig neue Funktionen für Maestro. Eine aktuelle Liste der veröffentlichten Funktionen finden Sie unter [Adobe Maestro-Release-Aktivität](../maestro/release-activity.md).

<!--moved the contents of this whole section to its own article: release-activity.md, in the same folder

This section lists the features and patches that have been released after the launch of the Maestro closed beta program, on May 22, 2023. 

The features are released weekly and are listed in the order of their release, with the most recent first. Customers who are participating in the Maestro closed beta program can access all features in their Preview and Production environments. 

### Week of September 4, 2023

#### Connect Maestro records with Workfront companies and groups

Preview and production: September 5, 2023  

You can now connect a Maestro record with Workfront companies and groups. You must first create a connection between a Maestro record type and the Workfront companies and groups object types. Then, you can connect a single Maestro record of the selected record type to individual Workfront companies and groups.  

Consider the following:  

* You must create a connection between Maestro record types and Workfront companies and groups for each Workspace.  

* You cannot connect taxonomy record types with Workfront object types. 

* You can connect multiple Maestro records to the same Workfront company or group, and multiple companies or groups to the same Maestro record.  

* You cannot edit companies or groups in Maestro. All company or group changes performed in Workfront are visible in Maestro, when reviewing the Maestro linked records.  

#### URL support for single-line text fields 

Preview and production: September 7, 2023 

For better visibility when working with links in the Table view, we have added support for URLs in single-line text fields. Using URLs to other websites or external drives when updating a single-line text field, now identifies them as links and allows you to click them from the table.  

### Week of August 28, 2023

#### Field visibility menu for the Table View toolbar

Preview and production: August 31, 2023

To display the right information on a given set of records, especially if you intend to share the view with others who need to see some but not all fields of a record type, you can now select which fields (or columns) to display and which to hide in the Table view.  

You can hide or show individual fields, from each header of the field columns, or you can manage all fields of the record type from a setting in the table view toolbar.  

### Week of August 21, 2023

#### Connect Maestro records to programs and portfolios 

Preview and production: August 24, 2023

You can now connect a Maestro record with Workfront programs and portfolios. You must first create a connection between a Maestro record type and a program or portfolio which creates a connected field. Then, you can connect any Maestro records from all other record types within the same workspace to specific programs and portfolios which will create a read-only Workfront Program or Workfront Portfolio record type in the same workspace. Consider the following:

* Workfront connector record types are unique for each workspace. 
* You can connect multiple Maestro records to the same Workfront program or portfolio, and multiple programs and portfolios to the same Maestro record. 
* You cannot edit programs and portfolios in Maestro. All program and portfolio changes performed in Workfront are visible in Maestro, when reviewing the linked records. 

#### New sorting functionality for the table view

Preview and production: August 24, 2023

You can now sort records in the table view of a record type page. 
The following capabilities are now available: 

* Sorting at the table-level, where you can sort by multiple fields at the same time. 
* Sorting at the column or field-level, where you can sort by an individual field at a time.

#### Improvements to the timeline view: new look-and-feel for groupings and the Compact/ Standard view switch

Preview and production: August 24, 2023

We have introduced the following improvements to the timeline view: 

* You can now display the timeline view in the following modes:

    * Standard: Displays records in separate lines.
    * Compact: Display the records whose dates don't intersect on the same line. 

* We have changed the look-and-feel of the grouping lines in the timeline view to display above the timeline of the records they contain. Prior to this improvement, the grouping lines displayed across the entire length of the timeline.

### Week of August 14, 2023

#### Reorder columns in the table view

You can now reorder columns in the Maestro table view. Consider the following when reordering columns: 

* The Name field is always the first field in the table view of a record type page 

* You cannot move the Name field to another position 

* The Name field is frozen and is not part of the horizontal scroll. 

#### Horizontal scroll for timeline view

You can now scroll horizontally in the timeline view of a record type. 

### Week of August 7, 2023

#### Import record types from an Excel file 

Preview and production: August 10, 2023

You can now import an Excel file to create record types in a workspace. The sheets of the file become the record types, and the columns of the file become their respective fields.  

#### Improved experience for connecting record types and projects 

Preview and production: August 10, 2023

We have improved the way you connect record types, including connecting to Workfront projects. As part of this improvement, we made the following changes when adding a field for a record type from the table view:  

* Removed the Relationship-type field from the "New field" tab.  

* Add a "New connection" tab where you can directly select the record or object type you want to connect to, eliminating the need for a Relationship-type field. 

### Week of July 10, 2023

#### Update the appearance of a record type

Preview and production: July 13, 2023

You can now select a custom icon for a record type, as well as a custom color for the record type icon.  

#### New Checkbox field type

Preview and production: July 13, 2023 

You can now add a Checkbox field type to Maestro record types. You can use the Checkbox field type to add a single checkbox option to a record. You can use this field to indicate a specific attribute or status for that particular record. For example, you can use it as a flag for tracking completion, approval, or any other binary attribute for each record.  

### Week of June 26, 2023

#### Quick activation of the contextual menu in a table

Preview and production: June 28, 2023
 
We have enabled the ability to activate the contextual menu by right-clicking anywhere in a record row, when viewing the records in the table view or a record type. You can now quickly view, delete, or copy a link to the record's Details page when you access the contextual menu from anywhere in the table view of a record type. Prior to this enhancement, the contextual menu was accessible only from the More menu in the Name column of a record.  

### Week of June 19, 2023

#### Record field names are unique

We have introduced a requirement now that the field names of a Maestro record type should have unique names. Fields that belong to different record types do not have to have unique names.  

### Week of June 5, 2023

#### Connect Maestro records with Workfront projects

Preview and production: June 5, 2023

You can now connect a Maestro record with Workfront projects. You must first create a connector Maestro record type to establish the connection between Maestro records and Workfront projects. Then, you can connect any Maestro records from all other record types to the connector record using the Relationship field. Consider the following:

* You must have a connector record type for Workfront for each Workspace. 
* You can connect multiple Maestro records to the same Workfront project, and multiple projects to the same Maestro record. 
* You cannot edit projects in Maestro. All project changes performed in Workfront are visible in Maestro, when reviewing the linked records. 

### Week of May 29, 2023

#### Two-date requirement for creating a Timeline view

Preview and production: May 31, 2023  

You must have at least two date fields associated with a record type in order to create a Timeline view. 
-->
