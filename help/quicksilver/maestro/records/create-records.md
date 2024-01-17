---
title: Datensätze erstellen
description: In Adobe Maestro ist ein Datensatz eine Instanz eines Datensatztyps. Sie müssen Datensatztypen erstellen, bevor Sie einzelne Datensätze erstellen können.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c7de4b1f-674b-424b-af64-a6df62fb738f
source-git-commit: 5f3d5c93c2fc721dda2dd04adac22190ef6a3f29
workflow-type: tm+mt
source-wordcount: '1091'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Datensätze erstellen

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Maestro, ein neues Angebot von Adobe Workfront.
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist. Sie müssen Workfront-Kunde sein, um Maestro-Funktionen verwenden zu können.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

In Adobe Maestro ist ein Datensatz eine Instanz eines Datensatztyps.

Folgende Datensätze stehen zur Verfügung:

* **Betriebsaufzeichnungen**: Sie stellen arbeitsbezogene Objekte dar. Beispielsweise können Sie für einen Betriebsdatensatz mit dem Namen &quot;Kampagne&quot;Datensätze wie &quot;Monatlicher Newsletter&quot;oder &quot;Sommerverkauf&quot;benannt haben.
* **Taxonomiedatensätze**: Sie stellen Attribute dar, die betrieblichen Datensätzen zugeordnet werden können. Beispielsweise können Sie für einen Taxonomiedatensatz mit dem Namen &quot;Kanal&quot;Taxonomien wie &quot;E-Mail&quot;, &quot;Social Media&quot;oder &quot;Werbung&quot;benannt haben.

Das Erstellen von Betriebsdatensätzen ist mit dem Erstellen von Taxonomiedatensätzen oder Taxonomien identisch.

Sie können Datensätze in Maestro erstellen, indem Sie einen der folgenden Schritte ausführen:

* Erstellen Sie sie manuell für Maestro-Datensatztypen
* Verbinden Sie sie mit Maestro-Datensätzen aus Drittanbieteranwendungen.
* Erstellen Sie Datensätze durch Kopieren und Einfügen von Informationen aus einer externen Liste.

In diesem Artikel wird beschrieben, wie Sie Maestro-Datensätze erstellen können. Informationen zum Verwalten von Datensätzen in der Tabellen- oder Timeline-Ansicht finden Sie in den folgenden Artikeln:

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

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Datensätze durch manuelles Hinzufügen zu einem Datensatztyp erstellen <!--in a record type table (I don't think you can create them elsewhere right now)-->

Sie können Datensätze in der Tabellenansicht einer Seite vom Typ Datensatz erstellen.

{#step1-to-maestro}

Der zuletzt aufgerufene Arbeitsbereich wird standardmäßig geöffnet. Informationen zum Erstellen von Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](../architecture/create-workspaces.md).
1. Klicken Sie auf eine Karte vom Typ Datensatz. Informationen zum Erstellen eines Datensatztyps finden Sie unter [Erstellen von Datensatztypen](../architecture/create-record-types.md).

   Die Seite mit dem Datensatztyp wird in der Ansicht geöffnet, auf die Sie zuletzt zugegriffen haben. Standardmäßig wird eine Seite vom Typ Datensatz in der Tabellenansicht geöffnet.
Alle Datensätze des ausgewählten Typs werden in der Tabellenansicht angezeigt.

1. (Bedingt) Wenn die Seite mit dem Datensatztyp nicht in der Tabellenansicht geöffnet wird, klicken Sie auf die Schaltfläche **Ansicht** und wählen Sie entweder ein vorhandenes **Tabellenansicht** ![](assets/table-view-icon.png) oder klicken Sie **Ansicht erstellen > Tabelle** , um eine Tabellenansicht zu erstellen.

1. Um neue Datensätze hinzuzufügen, klicken Sie auf **Neu &lt; Name des Datensatztyps >** in der letzten Zeile der Tabelle

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

1. (Optional) Verwenden Sie die folgenden Tastaturbefehle, um das Hinzufügen neuer Datensätze rückgängig zu machen oder wiederherzustellen:

   * STRG + Z ( ⌘ + Z für Mac) zum Rückgängigmachen einer Änderung
   * STRG + Umschalt + Z ( ⌘ + Umschalt + Z für Mac) zum Wiederholen einer Änderung

## Erstellen von Datensätzen durch Verbinden mit einer anderen Anwendung

Sie können Datensätze aus anderen Anwendungen importieren, indem Sie sie mit Maestro verknüpften Datensätzen verknüpfen. Dadurch wird ein Maestro-Record-Typ für das angeschlossene Objekt der Drittanbieteranwendung erstellt. Datensätze, die Sie mit den ursprünglichen Maestro-Datensätzen verbinden, werden in der Tabellenansicht des mit der Drittanbieteranwendung verbundenen Objekts Maestro record type angezeigt.

1. Erstellen Sie einen Maestro-Record-Typ, wie im Abschnitt [Erstellen von Datensatztypen](../architecture/create-record-types.md).

1. Erstellen Sie Maestro-Datensätze für den Datensatztyp, den Sie im vorherigen Schritt erstellt haben. Weitere Informationen finden Sie im Abschnitt . [Datensätze durch manuelles Hinzufügen zu einem Datensatztyp erstellen](#create-records-by-manually-adding-them-to-a-record-type) in diesem Artikel.

1. Erstellen Sie eine Verbindung zu einem Objekttyp aus einer Drittanbieteranwendung für den von Ihnen erstellten Maestro-Datensatztyp. Weitere Informationen finden Sie unter [Datensatztypen verbinden](../architecture/connect-record-types.md).

1. Fügen Sie den oben erstellten Maestro-Datensätzen Datensätze aus der Drittanbieteranwendung hinzu, indem Sie das verknüpfte Datensatzfeld verwenden, das Sie im vorherigen Schritt erstellt haben. Weitere Informationen finden Sie unter [Datensätze verbinden](../records/connect-records.md).

   Die folgenden Elemente werden in Maestro erstellt:

   * Ein schreibgeschützter Maestro-Record-Typ, der sich auf den von Ihnen im Feld für den verbundenen Datensatz verknüpften Drittanbieter-Record-Typ bezieht.

     Wenn Sie beispielsweise einen Maestro-Record-Typ mit Workfront-Projekten verknüpfen, wird im selben Arbeitsbereich ein schreibgeschützter Datensatz mit dem Namen &quot;Workfront projects&quot;erstellt.
   * Schreibgeschützte Datensätze auf der Seite des Drittanbieter-Datensatztyps. Die aus der Drittanbieteranwendung importierten Datensätze bleiben schreibgeschützt und können nur in der Originalanwendung aktualisiert werden.

## Datensätze durch Kopieren und Einfügen von Informationen aus einer externen Liste erstellen

1. Erstellen Sie in Maestro Datensätze in der Tabellenansicht, wie im Abschnitt beschrieben. [Datensätze durch manuelles Hinzufügen zu einem Datensatztyp erstellen](#create-records-by-manually-adding-them-to-a-record-type) in diesem Artikel.

   Stellen Sie sicher, dass die Maestro-Tabellenansicht über die Spalten (oder Felder) verfügt, die mit den neuen Datensatzinformationen gefüllt werden sollen.

1. Klicks **Neu &lt; Name des Datensatztyps >** in der letzten Zeile der Tabelle, um der Tabelle so viele neue Zeilen hinzuzufügen, wie Ihre neuen Datensätze sein sollen.

   Fügen Sie der Tabellenansicht beispielsweise 10 Zeilen hinzu, wenn Sie die Informationen für 10 neue Datensätze aus einer anderen Anwendung einfügen möchten.

1. Erstellen Sie in einer anderen Anwendung eine Liste von Datensätzen, die Sie in Maestro importieren möchten.

   Sie können beispielsweise eine Excel-Tabelle verwenden, um Ihre Liste zu erstellen.

   Die Liste sollte Informationen im Tabellenformat enthalten.

   >[!TIP]
   >
   > Die Spalten der Liste sollten Informationen für die vorhandenen Felder enthalten, die Sie in Maestro haben.
   >
   > Vergewissern Sie sich, dass die gewünschten Felder bereits in Maestro erstellt wurden und dass die Informationen in Ihrem Blatt im richtigen Format angezeigt werden, das dem der Felder in Maestro entspricht.

1. Wählen Sie in der Drittanbieteranwendung mehrere Zeilen und Spalten aus und fügen Sie dann die Informationen in die Tabellenansicht des Datensatztyps ein, beginnend mit dem ersten neuen Datensatz.

   Die folgenden Informationen werden in Maestro importiert:

   * Die Zeilen enthalten die neuen Datensätze
   * Die Spalten enthalten Informationen zu den Feldern der Datensätze.
