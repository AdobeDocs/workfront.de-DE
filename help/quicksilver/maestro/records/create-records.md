---
title: Datensätze erstellen
description: Bei Verwendung der Planungsfunktionen von Adobe Workfront ist ein Datensatz eine Instanz eines Datensatztyps. Sie müssen Datensatztypen erstellen, bevor Sie einzelne Datensätze erstellen können. Das Erstellen von Taxonomiedatensätzen ist mit dem Erstellen von Betriebsdatensätzen identisch.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: b795ceccb3f72eb64269062823199be9c8511860
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Datensätze erstellen

{{maestro-important-intro}}

In den Planungsfunktionen von Adobe Workfront ist ein Datensatz eine Instanz eines Datensatztyps.

Folgende Datensätze stehen zur Verfügung:

* **Betriebsaufzeichnungen**: Sie stellen arbeitsbezogene Objekte dar. Beispielsweise können Sie für einen Betriebsdatensatz mit dem Namen &quot;Kampagne&quot;Datensätze wie &quot;Monatlicher Newsletter&quot;oder &quot;Sommerverkauf&quot;benannt haben.
* **Taxonomiedatensätze**: Sie stellen Attribute dar, die betrieblichen Datensätzen zugeordnet werden können. Beispielsweise können Sie für einen Taxonomiedatensatz mit dem Namen &quot;Kanal&quot;Taxonomien wie &quot;E-Mail&quot;, &quot;Social Media&quot;oder &quot;Werbung&quot;benannt haben.

Das Erstellen von Betriebsdatensätzen ist mit dem Erstellen von Taxonomiedatensätzen identisch.

Sie können Datensätze anhand einer der folgenden Methoden erstellen:

* Erstellen Sie sie manuell für Datensatztypen
  <!-- not possible anymore: * Connect them to records from other applications-->
* Erstellen Sie Datensätze durch Kopieren und Einfügen von Informationen aus einer externen Liste.

In diesem Artikel wird beschrieben, wie Sie Datensätze erstellen können. Informationen zum Verwalten von Datensätzen in der Tabellen- oder Timeline-Ansicht finden Sie in den folgenden Artikeln:

* [Tabellenansicht verwalten](/help/quicksilver/maestro/views/manage-the-table-view.md)
* [Verwalten der Timeline-Ansicht](/help/quicksilver/maestro/views/manage-the-timeline-view.md)

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
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td>
   <td>
   <p>Alle</p> 
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

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Datensätze durch manuelles Hinzufügen zu einem Datensatztyp erstellen <!--in a record type table (I don't think you can create them elsewhere right now)-->

Sie können Datensätze in der Tabellenansicht einer Seite vom Typ Datensatz erstellen.

Informationen zum Bearbeiten von Datensatzinformationen finden Sie unter [Datensätze bearbeiten](/help/quicksilver/maestro/records/edit-records.md).

{#step1-to-maestro}

Der zuletzt aufgerufene Arbeitsbereich wird standardmäßig geöffnet. Informationen zum Erstellen von Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture/create-workspaces.md).
1. Klicken Sie auf eine Karte vom Typ Datensatz. Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](../architecture/create-record-types.md).

   Die Seite mit dem Datensatztyp wird in der Ansicht geöffnet, auf die Sie zuletzt zugegriffen haben. Standardmäßig wird eine Seite vom Typ Datensatz in der Tabellenansicht geöffnet.
Alle Datensätze des ausgewählten Typs werden in der Tabellenansicht angezeigt.

1. (Bedingt) Wenn die Seite mit dem Datensatztyp nicht in der Tabellenansicht geöffnet wird, klicken Sie auf die Schaltfläche **Ansicht** und wählen Sie entweder ein vorhandenes **Tabellenansicht** ![](assets/table-view-icon.png) oder klicken Sie **Ansicht erstellen > Tabelle** , um eine Tabellenansicht zu erstellen.

<!--Replace the above with this when we release the tabbed views: 
1. (Conditional) If the record type page does not open in the table view, click the tab of a table view, or click **+ View** to create a table view. -->

1. Um neue Datensätze hinzuzufügen, klicken Sie auf **Neuer Datensatz** in der letzten Zeile der Tabelle

   Oder

   Klicks **Umschalt + Eingabetaste** auf der Tastatur von einer beliebigen Spalte oder Zeile der Tabelle aus. Hierdurch wird eine leere Zeile angezeigt.

   ![](assets/adding-a-new-campaign-in-table-row.png)

1. Beginnen Sie mit der Eingabe von Informationen in die neue Zeile zum neuen Datensatz.

   >[!NOTE]
   >
   >  * Es gibt keine Pflichtfelder für Datensätze. Es wird jedoch empfohlen, einen Namen für den Datensatz hinzuzufügen, da es hilfreich ist, Datensätze beim Verknüpfen von Datensätzen miteinander zu identifizieren.
   >
   >  * Felder, die auf andere Datensatztypen oder berechnete Felder verweisen, sind schreibgeschützte Felder.

1. Fügen Sie weitere Informationen zu den einzelnen Zeilen hinzu und klicken Sie auf **Eingabe** auf der Tastatur, um Ihre Änderungen zu speichern.

<!--Or 
    
    Click the new record's name or the **Open details** icon ![](assets/open-details-icon-in-table-name-field.png) to the left of the record name. The **Details** box opens in the table. 

      >[!TIP]
      >
      >    You can access the Details box only from the name field of the record when the Name field is a primary field. 

  1. Start editing the record's information in the Details box. Workfront automatically saves your changes. 
  1. (Optional) Click the **Open in new tab** icon ![](assets/open-details-in-a-new-tab-icon.png) in the upper-right corner of the Details box to open the record's **Details** page in a new tab. Continue editing the record on the Details page.
    -->

1. (Optional) Verwenden Sie die folgenden Tastaturbefehle, um das Hinzufügen neuer Datensätze rückgängig zu machen oder wiederherzustellen:

   * STRG + Z ( ⌘ + Z für Mac) zum Rückgängigmachen einer Änderung
   * STRG + Umschalt + Z ( ⌘ + Umschalt + Z für Mac) zum Wiederholen einer Änderung

<!-- this is not possible anymore: 

## Create records by connecting them from another application

You can import records from other applications by linking them to existing records. This creates a linked record for the other application's connected object. 

1. Create a record type, as described in the [Create record types](../architecture/create-record-types.md).

1. Create records for the record type you created in the previous step. For information, see the section [Create records by manually adding them to a record type](#create-records-by-manually-adding-them-to-a-record-type) in this article. 

1. Create a connection to an object type from another application for the record type you created. For information, see [Connect record types](../architecture/connect-record-types.md).

1. Add objects from another application to the records you created above using the linked record field you created in the previous step. For information, see [Connect records](../records/connect-records.md). 

    The following items are created in Maestro:

    * A read-only Maestro record type that refers to the other application's record type you linked to in the connected record field. 

      For example, if you connect a Maestro record type to Workfront project, a read-only record type named "Workfront project" is created in the same workspace. You can access the read-only Workfront record types from the table view of the Maestro records you're linking from. 
   
-->

## Datensätze durch Kopieren und Einfügen von Informationen aus einer externen Liste erstellen

1. Erstellen Sie Datensätze in der Tabellenansicht, wie im Abschnitt beschrieben. [Datensätze durch manuelles Hinzufügen zu einem Datensatztyp erstellen](#create-records-by-manually-adding-them-to-a-record-type) in diesem Artikel.

   Stellen Sie sicher, dass die Tabellenansicht über die Spalten (oder Felder) verfügt, die mit den neuen Datensatzinformationen gefüllt werden sollen.

1. Klicks **Neu &lt; Name des Datensatztyps >** in der letzten Zeile der Tabelle, um der Tabelle so viele neue Zeilen hinzuzufügen, wie Ihre neuen Datensätze sein sollen.

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
