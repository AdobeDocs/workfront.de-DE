---
title: Erstellen von Datensatztypen
description: Datensatztypen sind die Objekttypen der Adobe Workfront-Planung. In der Workfront-Planung können Sie benutzerdefinierte Datensatztypen erstellen, die die im Lebenszyklus Ihres Unternehmens benötigten Arbeitselemente illustrieren.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ed1c4954-b338-4865-a7a9-5ba0192e7b37
source-git-commit: f713e8fa72c98b6df2509e71acd7080d4df46a3a
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->
<!--this is linked to the UI in an empty workspace screen-->

# Erstellen von Datensatztypen

{{planning-important-intro}}

Datensatztypen sind die Objekttypen der Adobe Workfront-Planung. In der Workfront-Planung können Sie benutzerdefinierte Datensatztypen erstellen, die die im Lebenszyklus Ihres Unternehmens benötigten arbeitsbezogenen Elemente veranschaulichen.

Weitere Informationen zu Datensatztypen finden Sie unter [Übersicht über Datensatztypen](/help/quicksilver/planning/architecture/overview-of-record-types.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Workfront-Planung anzuzeigen.

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
   <td> Adobe Workfront
   </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-Abkommen</p></td>
   <td>
<p>Ihr Unternehmen muss in der Phase des frühen Zugriffs für die Workfront-Planung eingeschrieben sein </p>
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
   <p>Aktuell: Plan</p>
   Oder
   <p>Neu: Standard </p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfigurationen auf Zugriffsebene</p></td>
   <td> <p>Für die Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Ihr Workfront- oder Gruppenadministrator muss den Planungsbereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Berechtigungen für einen Arbeitsbereich verwalten</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Überlegungen zum Erstellen von Datensatztypen

* Sie können Datensatztypen in einem Arbeitsbereich wie folgt erstellen:

   * Automatisch:
      * Wenn Sie einen Arbeitsbereich mit einer Vorlage erstellen.

        Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

     <!--* When you import them using an Excel or CSV file. 

            >[!IMPORTANT]
            >
            >This functionality has been temporarily removed since March 21, 2024. It will be enabled at a later date.-->

     <!--this should not ne known anymore: * When you add objects from another application to a linked record field of a record. This creates a read-only record type in Workfront Planning which is connected to object types from the original application. 
        For information about connecting record types with object types from another application, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md).
        For information about connecting objects with records, see [Connect records](/help/quicksilver/planning/records/connect-records.md). -->
   * Manuell:

      * Von Grund auf neu.

        In diesem Artikel wird beschrieben, wie Sie neue Datensatztypen erstellen.

* Sie können Datensatztypen innerhalb eines Abschnitts und von einem Abschnitt eines Arbeitsbereichs in einen anderen verschieben. Es ist nicht möglich, Datensatztypen von einem Arbeitsbereich in einen anderen zu verschieben.

## Erstellen von Datensatztypen mithilfe einer Workspace-Vorlage

Sie können Datensatztypen automatisch erstellen, wenn Sie einen Arbeitsbereich mithilfe einer Workfront-Planungsvorlage erstellen. Jede Vorlage enthält Beispieldatensatztypen.

Wenn Sie einen Arbeitsbereich aus einer Vorlage erstellen, sind die Datensatztypen in den folgenden Abschnitten gruppiert:

* Betriebsdatentypen
* Taxonomien

Sie können Datensatztypen manuell sowohl in den Abschnitten &quot;Operative Datensatztypen&quot;als auch &quot;Taxonomien&quot;hinzufügen.

Informationen zum Erstellen von Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

Informationen dazu, welche Datensatztypen in den einzelnen Vorlagen enthalten sind, finden Sie unter [Liste der Workspace-Vorlagen](/help/quicksilver/planning/architecture/workspace-templates.md).

## Erstellen eines neuen Datensatztyps

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, in dem Sie einen Datensatztyp erstellen möchten.

   Oder

   Erweitern Sie in einem Arbeitsbereich den nach unten zeigenden Pfeil rechts neben einem vorhandenen Arbeitsbereichnamen, suchen Sie nach einem Arbeitsbereich und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.
1. (Optional) Klicken Sie auf **Abschnitt hinzufügen** , um einen neuen Abschnitt zum Arbeitsbereich hinzuzufügen.
1. Klicken Sie auf **Hinzufügen des Datensatztyps**.

   Das Feld Datensatztyp hinzufügen wird geöffnet.
   <!--1. (Conditional) When creating record types by importing an Excel or CSV file is enabled, click **From scratch**. Otherwise, the **Add record type** box opens. -->

   ![](assets/add-record-type-box-with-appearance-options.png)

1. Aktualisieren Sie die folgenden Informationen:

   * Ersetzen Sie &quot;Untitled record type&quot;durch den Namen Ihres künftigen Datensatztyps. <!--did they bring back the field label here and did they rename it to "Name"-->
   * **Beschreibung**: Fügen Sie weitere Informationen zum Datensatztyp hinzu.
   * Wählen Sie eine Farbe und Form für das dem Datensatztyp zugeordnete Symbol aus. Gehen Sie wie folgt vor:
      * Wählen Sie eine Farbe aus, um Ihren neuen Datensatztyp zu identifizieren. Dies ist die Farbe des Symbols für den Datensatztyp. Graustufen ist standardmäßig ausgewählt.
      * Wählen Sie ein Symbol aus der Liste aus oder geben Sie den Namen eines Symbols ein, um zu beschreiben, was es darstellt, und wählen Sie es dann aus, wenn es angezeigt wird. Dies ist das Symbol des Datensatztyps. Standardmäßig ist ein Dateisymbol ausgewählt.

1. Klicken Sie auf **Erstellen**.

   Die Karte vom Typ Datensatz wird dem ausgewählten Bereich und Arbeitsbereich hinzugefügt.
Die Beschreibung des Datensatztyps wird auf der Karte angezeigt.

   ![](assets/record-type-card-with-description.png)

1. (Optional) Bewegen Sie den Mauszeiger über die Karte des Datensatztyps, klicken Sie oben rechts auf das Symbol **Mehr** ![](assets/more-menu.png) und klicken Sie dann auf **Bearbeiten** , um Informationen zum Datensatztyp zu ändern.
1. (Optional) Klicken Sie auf die Karte vom Typ Datensatz , um die Seite vom Typ Datensatz zu öffnen.

   ![](assets/operational-record-type-blank.png)

   Die Seite vom Typ Datensatz wird standardmäßig in der Tabellenansicht angezeigt. Die Spalten der Tabelle sind Felder, die mit dem neuen Datensatztyp verknüpft sind. Jede Zeile ist ein eindeutiger Datensatz, den Sie hinzufügen müssen.

   <!--TIP: If you import a record type from an Excel or CSV file, records are also imported.-->

   Standardmäßig werden die folgenden Felder in den Tabellenansichtsspalten eines operationellen Datensatztyps angezeigt:

   * Name
   * Beschreibung
   * Startdatum
   * Enddatum
   * Status

1. (Optional) Aktualisieren Sie den Namen des Datensatztyps in der Kopfzeile der Seite

   Oder

   Klicken Sie auf das Symbol **Mehr** ![](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und klicken Sie auf **Bearbeiten** , um ihn umzubenennen oder die Informationen darüber zu ändern. Weitere Informationen finden Sie unter [Bearbeiten von Datensatztypen](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Optional) Klicken Sie auf **+ Neuer Datensatz** , um Datensätze des ausgewählten Datensatztyps hinzuzufügen. Weitere Informationen finden Sie unter [Datensätze erstellen](/help/quicksilver/planning/records/create-records.md).
1. (Optional) Klicken Sie oben rechts in der Tabelle auf das Symbol **+** , um dem Datensatztyp weitere Felder hinzuzufügen.

   Weitere Informationen zum Erstellen von Feldern finden Sie unter [Felder erstellen](/help/quicksilver/planning/fields/create-fields.md).

1. (Optional) Klicken Sie in der Kopfzeile auf den nach links zeigenden Pfeil neben dem Namen des Datensatztyps, um zum ausgewählten Arbeitsbereich zurückzukehren.

1. (Optional) Klicken Sie im Arbeitsbereich auf eine Karte vom Typ Datensatz, um den Datensatztyp per Drag-and-Drop an eine gewünschte Stelle zu ziehen oder in einen anderen Bereich zu verschieben.

   Die Änderungen werden automatisch gespeichert.

   Weitere Informationen zum Hinzufügen von Datensätzen, zum Löschen oder Bearbeiten von Datensatztypen oder zum Aktualisieren der Ansicht auf der Seite mit dem Datensatztyp finden Sie in den folgenden Artikeln:

   * [Datensätze erstellen](/help/quicksilver/planning/records/create-records.md)
   * [Löschen von Datensatztypen](/help/quicksilver/planning/architecture/delete-record-types.md)
   * [Datensatztypen bearbeiten](/help/quicksilver/planning/architecture/edit-record-types.md)
   * [Ansichten von Datensätzen verwalten](/help/quicksilver/planning/views/manage-record-views.md)

<!--
## Create record types by importing an Excel or CSV file

>[!IMPORTANT]
>
>This functionality has been temporarily removed since March 21, 2024. It will be enabled at a later date.

Consider the following when importing record types using an Excel or CSV file: 

* Each sheet of the Excel file becomes a record type. 
* The columns of each sheet become the fields associated with each record type. 
* Fields are unique for their respective record types. 
* Each row in each sheet becomes a unique record associated with its respective record type. 
* Each sheet of the Excel file should not exceed the following: 
    * 50,000 rows
    * 500 columns
* The Excel file should not be larger than 5MB.
* Empty sheets are not supported. 

To import record types using an Excel file: 

{{step1-to-planning}}

1. Click the workspace where you want to create record types, 

    Or

    From a workspace, expand the downward-pointing arrow to the right of an existing workspace name, search for a workspace, then select it when it displays in the list.
1. Click **Add record type**. 
1. Click **Excel/CSV**.
1. Drag and drop an Excel or CSV file previously saved on your computer, or click **Select a CSV or Excel file** to browse for one. 
1. Click **Review your data**.
    
    The Preview and edit box displays with the following information: 

    * The names of the sheets or of the future record types display in the left panel. Workfront Planning selects an icon and a color for each new record type by default.
    * The first sheet or record type is selected and the names of the fields associated with it display as the column headers. The type of each field is selected by default. 
    * Each row represents a new record. Only the first 10 records display in the Preview and edit box. 

    ![](assets/preview-and-edit-box.png)

1. (Optional) Click the name of each sheet in the left panel to review the information it contains. 

    >[!NOTE]
    >
    >    Sheets that are empty are not supported and are dimmed. 


1. (Optional) Click the **Select sheets to import** drop-down menu and deselect the sheets that you don't want to import. 

    ![](assets/select-sheets-to-import-drop-down-with-unselected.png)

    Sheets you deselected display with a gray background. 

1. Click **Import** when you are ready to import your file. 

    The following information imports in to Workfront Planning:

    * New record types
    * New fields associated with each record type
    * New records associated with each record type

    You can start managing fields and records on the record types pages. 
    
    Everyone with access to Workfront Planning can now view and edit the imported record types and their information.-->

