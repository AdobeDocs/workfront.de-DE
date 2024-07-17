---
filename: airtable-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Airtable Module
description: Adobe Workfront Fusion erfordert zusätzlich zu einer Adobe Workfront-Lizenz eine Adobe Workfront Fusion-Lizenz.
author: Becky
feature: Workfront Fusion
exl-id: 1d78e0db-9a77-437d-a72f-88fb256981c0
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '1862'
ht-degree: 1%

---

# Airtable Module


Mit dem [!DNL Airtable] -Connector für [!DNL Adobe Workfront Fusion] können Sie ein Szenario starten, das auf Ereignissen in Ihrem [!DNL Airtable]-Konto basiert, Datensätze erstellen, hochladen und aktualisieren, Datensätze suchen und benutzerdefinierte API-Aufrufe an die Airtable-API richten.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Sie müssen über ein Airtable-Konto verfügen, um die Funktionalität dieses Artikels nutzen zu können.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see the tutorial .</p>
-->

## Verbinden von Airtable mit Workfront Fusion {#connect-airtable-to-workfront-fusion}

<!--

1. Log in to your Airtable account.
1. Open your account overview and generate the API key.
-->
1. Öffnen Sie Workfront Fusion und das Dialogfeld **Verbindung erstellen** des gewünschten Moduls.
1. Geben Sie einen Namen für die Verbindung ein.
1. (Optional) Klicken Sie auf Erweiterte Einstellungen anzeigen und geben Sie Ihre Airtable Client ID und den Client Secret ein.
1. Klicken Sie auf die Schaltfläche **Weiter** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

## Airtable Module und ihre Felder

### Datensätze

* [Erstellen eines Datensatzes](#create-a-record)
* [Einen Datensatz löschen](#delete-a-record)
* [Datensatz abrufen](#get-a-record)
* [Suchdatensätze](#search-records)
* [Datensatz aktualisieren](#update-a-record)
* [Datensatz hochladen](#upsert-a-record)
* [Aufnahmen ansehen](#watch-records)
* [Antworten ansehen](#watch-responses)
* [API-Aufruf](#make-an-api-call)

#### Datensatz erstellen {#create-a-record}

Dieses Aktionsmodul erstellt einen neuen Datensatz.

Sie geben die Daten an, die im Datensatz gespeichert werden sollen.

Das Modul gibt alle mit dem Datensatz verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Verbindung </td> 
   <td> <p>Anweisungen zum Verbinden Ihres Airtable-Kontos mit Workfront Fusion finden Sie in diesem Artikel unter <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Verbinden von Airtable mit Workfront Fusion</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>Basis </td> 
   <td> <p>Wählen Sie die Basis aus, zu der der neue Datensatz gehören soll.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabelle </td> 
   <td> <p>Wählen Sie die Tabelle aus, zu der der neue Datensatz gehören soll.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Datensatz</p> </td> 
   <td> <p>Geben Sie die Werte für den neuen Datensatz ein. Die verfügbaren Felder basieren auf der von Ihnen ausgewählten Tabelle.</p> <!--<p>For more information on field types, search for "Supported field types" in the Airtable documentation.</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>Multiple lines of text, which may contain "mention tokens", for example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong> : Add the attachment. Airtable will download the file from the provided <code>url</code> and keep its own copy of it. If the File name field is left empty, Airtable generates the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05 (ISO 8601 formatted date)</li> 
     <li>Phone number:</li> 
     <li><strong>Emails</strong>: A valid email address.</li> 
     <li><strong>URL</strong>: A valid URL (for example, airtable.com or https://airtable.com/universe).</li> 
     <li><strong>Number</strong>: Enter a number.</li> 
     <li><strong>Currency</strong>: Currency value.</li> 
     <li><strong>Percent</strong>: A percentage value. Must be higher than or equal to 0.</li> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation. </li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs will be reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>Smart-Links</td> 
   <td> <p>Aktivieren Sie diese Option, um Namen anstelle von Datensatz-IDs für Felder einzugeben, die mit einer anderen Tabelle verknüpft sind. Der Datensatz wird automatisch in der verknüpften Tabelle erstellt, wenn keine Übereinstimmung vorliegt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Datensatz löschen {#delete-a-record}

Dieses Aktionsmodul löscht einen bestimmten Datensatz.

Sie geben die Kennung und die Speicherorte des Datensatzes an.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Verbindung </td> 
   <td> <p>Anweisungen zum Verbinden Ihres Airtable-Kontos mit Workfront Fusion finden Sie in diesem Artikel unter <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Verbinden von Airtable mit Workfront Fusion</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>Basis </td> 
   <td> <p>Wählen Sie die Basis aus, die den zu löschenden Datensatz enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabelle </td> 
   <td> <p>Wählen Sie die Tabelle aus, die den zu löschenden Datensatz enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>Datensatz-ID</td> 
   <td> <p>Geben Sie die eindeutige Airtable ID des Datensatzes ein oder ordnen Sie sie zu, den das Modul löschen soll. Sie können die ID beispielsweise mithilfe des Moduls Suchdatensätze abrufen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Datensatz abrufen {#get-a-record}

Dieses Aktionsmodul ruft Datensatzdetails ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Verbindung </td> 
   <td> <p>Anweisungen zum Verbinden Ihres Airtable-Kontos mit Workfront Fusion finden Sie in diesem Artikel unter <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Verbinden von Airtable mit Workfront Fusion</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>Basis </td> 
   <td> <p>Wählen Sie die Basis aus, die die Tabelle mit dem Datensatz enthält, den Sie abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabelle</td> 
   <td> <p> Wählen Sie die Tabelle aus, die den Datensatz enthält, für den Sie Details abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>Datensatz-ID</td> 
   <td> <p> Geben Sie die Kennung des Datensatzes ein oder ordnen Sie ihn zu, für den Sie Details abrufen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Suchdatensätze {#search-records}

Dieses Suchmodul sucht nach Datensätzen in einem Objekt in Airtable, die mit der von Ihnen angegebenen Suchabfrage übereinstimmen.

Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Verbindung </td> 
   <td> <p>Anweisungen zum Verbinden Ihres Airtable-Kontos mit Workfront Fusion finden Sie in diesem Artikel unter <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Verbinden von Airtable mit Workfront Fusion</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>Basis </td> 
   <td> <p>Wählen Sie die Basis aus, nach der Sie nach Datensätzen suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabelle </td> 
   <td> <p>Wählen Sie die Tabelle aus, nach der Sie nach Datensätzen suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Formel</p> </td> 
   <td> <p>Eine Formel zum Filtern von Datensätzen. Die Formel wird für jeden Datensatz ausgewertet. Wenn das Ergebnis nicht <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code> oder <code>#Error!</code> ist, wird der Datensatz in die Antwort aufgenommen.</p> <p>In Kombination mit dem <code>view</code> werden nur Datensätze in dieser Ansicht zurückgegeben, die der Formel entsprechen.</p> <p>Um beispielsweise nur Datensätze einzuschließen, für die der Name nicht leer ist, geben Sie Folgendes an:<code> NOT({Name} = '')</code></p> <p>Weitere Informationen finden Sie in der Dokumentation zur Airtable-Unterstützung unter Informationen zu Formularfelderverweisen.</p> </td> 
  </tr> 
  <tr> 
   <td>Sortieren </td> 
   <td> <p>Wählen Sie die Sortierrichtung und das Feld aus, nach dem die Ergebnisse sortiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>Anzeigen </td> 
   <td> <p>Wählen Sie die Ansicht aus, nach der Sie nach Datensätzen suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>Limit</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Datensatz aktualisieren {#update-a-record}

Dieses Aktionsmodul aktualisiert einen bestimmten Datensatz.

Sie geben die Kennung des Datensatzes und die neuen Daten an, die darin enthalten sein sollen.

Das Modul gibt alle mit dem Datensatz verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Verbindung </td> 
   <td> <p>Anweisungen zum Verbinden Ihres Airtable-Kontos mit Workfront Fusion finden Sie in diesem Artikel unter <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Verbinden von Airtable mit Workfront Fusion</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>Basis </td> 
   <td> <p>Wählen Sie die Basis aus, die den zu aktualisierenden Datensatz enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabelle </td> 
   <td> <p>Wählen Sie die Tabelle aus, die den zu aktualisierenden Datensatz enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>Datensatz-ID </td> 
   <td> <p>Geben Sie die eindeutige Airtable ID des Datensatzes ein oder ordnen Sie sie zu, den das Modul aktualisieren soll. Sie können die ID beispielsweise mithilfe des Moduls Suchdatensätze abrufen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Datensatz</p> </td> 
   <td> <p>Geben Sie die Werte für den neuen Datensatz ein. Die verfügbaren Felder hängen von der ausgewählten Tabelle ab.</p> <!--<p>In order to delete the content of the field, use the erase function. </p>  <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><strong>Phone number</strong>: A telephone number, for example, (415) 555-9876.</li> 
     <li><strong>Email</strong>valid email address.</li> 
     <li><strong>URL</strong>: lid URL such as airtable.com or https://airtable.coiverse.</li> 
     <li><strong>Number</strongnter a number.</li> 
     <li><strong>Currency</stro Currency value.</li> 
     <li><strong>Percent</stronA percentage value; must be equal to or more than 0i> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>Smart-Links</td> 
   <td> <p>Geben Sie Namen anstelle von Datensatz-IDs zu Feldern ein, die mit einer anderen Tabelle verknüpft sind. Der Datensatz wird automatisch in der verknüpften Tabelle erstellt, wenn keine Übereinstimmung vorliegt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Datensatz aktualisieren

Dieses Aktionsmodul aktualisiert oder fügt einen bestimmten Datensatz hinzu.

Sie geben die Kennung des Datensatzes und die neuen Daten an, die darin enthalten sein sollen.

Das Modul gibt alle mit dem Datensatz verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Verbindung </td> 
   <td> <p>Anweisungen zum Verbinden Ihres Airtable-Kontos mit Workfront Fusion finden Sie in diesem Artikel unter <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Verbinden von Airtable mit Workfront Fusion</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>Basis </td> 
   <td> <p>Wählen Sie die Basis aus, die den zu aktualisierenden Datensatz enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabelle </td> 
   <td> <p>Wählen Sie die Tabelle aus, die den zu aktualisierenden Datensatz enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>Datensatz-ID </td> 
   <td> <p>Wenn Sie einen Datensatz aktualisieren, geben Sie die eindeutige Airtable ID des Datensatzes ein oder ordnen Sie sie zu, den das Modul aktualisieren soll. Sie können die ID beispielsweise mithilfe des Moduls Suchdatensätze abrufen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Datensatz</p> </td> 
   <td> <p>Geben Sie die Werte für den neuen Datensatz ein. Die verfügbaren Felder hängen von der ausgewählten Tabelle ab.</p> <!-- <p>In order to delete the content of the field, use the erase function. </p>  <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><strong>Phone number</strong>: A telephone number, for example, (415) 555-9876.</li> 
     <li><strong>Email</strong>valid email address.</li> 
     <li><strong>URL</strong>: lid URL such as airtable.com or https://airtable.coiverse.</li> 
     <li><strong>Number</strongnter a number.</li> 
     <li><strong>Currency</stro Currency value.</li> 
     <li><strong>Percent</stronA percentage value; must be equal to or more than 0i> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>Smart-Links</td> 
   <td> <p>Geben Sie Namen anstelle von Datensatz-IDs zu Feldern ein, die mit einer anderen Tabelle verknüpft sind. Der Datensatz wird automatisch in der verknüpften Tabelle erstellt, wenn keine Übereinstimmung vorliegt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Aufnahmen ansehen {#watch-records}

Dieses Trigger-Modul startet ein Szenario, wenn ein Datensatz in der angegebenen Tabelle erstellt oder aktualisiert wird.

>[!NOTE]
>
>Um dieses Modul verwenden zu können, muss in Ihrer Tabelle das Feld Erstellte Zeit oder Letzte Änderungszeit erstellt werden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Verbindung </td> 
   <td> <p>Anweisungen zum Verbinden Ihres Airtable-Kontos mit Workfront Fusion finden Sie in diesem Artikel unter <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Verbinden von Airtable mit Workfront Fusion</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>Basis </td> 
   <td> <p>Wählen Sie die Basis aus, die Sie auf neue Datensätze achten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>Tabelle </td> 
   <td> <p>Wählen Sie die Tabelle aus, die Sie auf neue Datensätze achten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Trigger-Konfiguration</p> </td> 
   <td> <p>Trigger</p> <p>Ein <code>Created Time</code> - oder <code>Last Modified Time</code> -Feld zum Sortieren von Datensätzen. Wenn Ihr Schema kein <code>Created Time</code> - oder <code>Last Modified Time</code> -Feld enthält, müssen Sie eines erstellen. </p> <p>Beschriftungsfeld</p> <p>Ein Feld, das als Beschriftung für einen Datensatz verwendet wird, z. B. im Dialogfeld Festlegen, wo der Datensatz gestartet werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td>Limit</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios überwachen soll.</p> </td> 
  </tr> 
  <tr> 
   <td>Anzeigen</td> 
   <td> <p>Wählen Sie die Ansicht aus, die Sie verwenden möchten.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Formel</p> </td> 
   <td> <p>Eine Formel zum Filtern von Datensätzen. Die Formel wird für jeden Datensatz ausgewertet. Wenn das Ergebnis nicht <code>0</code>, <code>false</code>, <code>""</code>, <code>NaN</code>, <code>[]</code> oder <code>#Error!</code> ist, wird der Datensatz in die Antwort aufgenommen.</p> <p>In Kombination mit dem <code>view</code> werden nur Datensätze in dieser Ansicht zurückgegeben, die der Formel entsprechen.</p> <p>Um beispielsweise nur Datensätze einzuschließen, für die der Name nicht leer ist, geben Sie Folgendes an:<code> NOT({Name} = '')</code></p> <p>Weitere Informationen finden Sie in der Dokumentation zur Airtable-Unterstützung in den Informationen zu Formularfelderverweisen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Antworten ansehen

Dieses Trigger-Modul startet ein Szenario, wenn ein Formular gesendet wird.

>[!NOTE]
>
>Diese Funktion ist nur für zahlungspflichtige Airtable Pro Plan verfügbar.

Die Webhook-URL muss in Workfront Fusion generiert und dann zur Formularkonfiguration in Airtable hinzugefügt werden.

1. Fügen Sie das Modul Neue Antworten überwachen zu Ihrem Workfront Fusion-Szenario hinzu.
1. Erstellen und kopieren Sie die Webhook-URL.

   Anweisungen finden Sie unter [Instant Trigger (Webhooks) in Adobe Workfront Fusion](../../workfront-fusion/webhooks/instant-triggers-webhooks.md).

1. Melden Sie sich bei Ihrem Airtable-Konto an.
1. Öffnen Sie die Basis und die Tabelle, die Sie für das Formular verwenden möchten, und erstellen Sie eine Formularansicht.
1. Legen Sie das Formular nach Bedarf fest, scrollen Sie nach unten in das Formular und aktivieren Sie die Option Zu URL umleiten , nachdem das Formular gesendet wurde.
1. Geben Sie die in Schritt 2 generierte Webhook-URL in das angezeigte Dialogfeld ein und fügen Sie ?record_id={record_id} direkt nach der Webhook-URL hinzu, um die Datensatz-ID in die Ausgabe des Moduls einzuschließen. Klicken Sie dann auf Speichern. Die resultierende URL sieht beispielsweise wie folgt aus:
1. Gehen Sie zurück zu Ihrem Workfront Fusion-Szenario und führen Sie das Modul Antworten überwachen nur aus, um Felder von Airtable zu laden und diese Felder den anderen Modulen zuzuordnen.
1. Senden Sie das Formular in Airtable, wobei die Option Zu URL umleiten, nachdem das Formular gesendet wurde aktiviert ist und die Webhook-URL hinzugefügt wurde (Schritt 6 oben).

   Das Modul Überwachungsantworten wird ausgelöst und die gewünschten Daten werden geladen.

1. Fügen Sie das Modul Airtable > Get a Record (Datensatz abrufen) direkt nach dem Modul Airtable > Watch Responses hinzu und ordnen Sie die record_id dem Feld Record ID zu.

Jetzt wird jedes Mal, wenn das Formular gesendet wird, das Modul &quot;Antworten überwachen&quot;in Ihrem Workfront Fusion-Szenario ausgelöst und das Modul &quot;Datensatz abrufen&quot;gibt die gesendeten Formulardaten zurück.

#### API-Aufruf

#### Benutzerspezifischer API-Aufruf

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Airtable] -API durchführen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von anderen [!DNL Airtable] -Modulen nicht ausgeführt werden kann.

Die Aktion basiert auf dem von Ihnen angegebenen Entitätstyp (Allocadia-Objekttyp).

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Verbindung</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres Airtable-Kontos mit Workfront Fusion finden Sie in diesem Artikel unter <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Verbinden von Airtable mit Workfront Fusion</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Geben Sie einen Pfad relativ zu <code>https://api.airtable.com/}</code> ein. Beispiel: <code>v0/{base}/{table}</code> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Methode</td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Kopfzeilen</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Abfragezeichenfolge</td> 
   <td> <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines Schlüssels und Werts hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Text</td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
