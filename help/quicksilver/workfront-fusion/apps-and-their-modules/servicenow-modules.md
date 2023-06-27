---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: ServiceNow-Module
description: In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL ServiceNow], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.
author: Becky
feature: Workfront Fusion
exl-id: b362cd8b-06b3-4f4c-b405-a2afc24abddb
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1613'
ht-degree: 1%

---

# [!DNL ServiceNow]-Module

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL ServiceNow], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.

Informationen zum Erstellen eines Szenarios finden Sie unter [Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Ältere Lizenzanforderungen: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderungen: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Ältere Produktanforderungen: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Verwendung [!DNL ServiceNow] -Module, müssen Sie über eine [!DNL ServiceNow] -Konto.

## Verbinden [!DNL ServiceNow] nach [!DNL Workfront Fusion]

So erstellen Sie eine Verbindung für Ihre [!DNL ServiceNow] -Module:

1. Klicken **[!UICONTROL Hinzufügen]** neben dem [!UICONTROL Verbindung] bei der Konfiguration des ersten [!DNL ServiceNow] -Modul.
1. Geben Sie Folgendes ein:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Verbindungsname]</p> </td> 
      <td>Geben Sie einen Namen für die neue [!DNL ServiceNow] connection</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Benutzername]</p> </td> 
      <td>Geben Sie Ihre [!DNL ServiceNow] Benutzername.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Kennwort]</p> </td> 
      <td>Geben Sie Ihr ServiceNow-Kennwort ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Instanz]</p> </td> 
      <td> <p>Geben Sie die Adresse Ihres [!DNL ServiceNow] Konto ohne <code>https://</code> (gewöhnlich <code>&lt;company>.service-now.com</code>).</p> </td> 
     </tr> 
    </tbody> 
   </table>

## [!UICONTROL ServiceNow] Module und ihre Felder

Bei der Konfiguration [!DNL ServiceNow] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL ServiceNow] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>Wenn ein benutzerdefinierter Datensatz in einem &quot;[!UICONTROL Record Type]&quot;, kann es einige Zeit dauern, die benutzerdefinierten Felder zu laden.
>
>Wenn keine benutzerdefinierten Datensätze vorhanden sind, ist das Dropdown-Menü leer.

* [[!UICONTROL Aufnahmen ansehen]](#watch-records)
* [[!UICONTROL Benutzerspezifischer API-Aufruf]](#custom-api-call)
* [[!UICONTROL Datensatz lesen]](#read-a-record)
* [[!UICONTROL Deaktivieren eines Benutzers]](#deactivate-a-user)
* [[!UICONTROL Anlage herunterladen]](#download-an-attachment)
* [[!UICONTROL Hochladen eines Anhangs]](#upload-an-attachment)
* [[!UICONTROL Datensatz erstellen]](#create-a-record)
* [[!UICONTROL Datensatz aktualisieren]](#update-a-record)
* [[!UICONTROL Datensatz löschen]](#delete-a-record)
* [[!UICONTROL Datensätze suchen]](#search-for-records)

### [!UICONTROL Aufnahmen ansehen]

Dieses Trigger-Modul aktiviert ein Szenario, wenn ein Datensatz erstellt oder aktualisiert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres ServiceNow-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] nach [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabellenart]</td> 
   <td>Wählen Sie aus, ob es sich bei der zu überwachenden Tabelle um eine benutzerdefinierte Tabelle oder eine Standardtabelle handelt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Wählen Sie den Typ des Datensatzes aus, den Sie sehen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>Wählen Sie den Typ der Werte aus, die angezeigt werden sollen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td>Wählen Sie die Felder aus, die das Modul ausgeben soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Wählen Sie aus, ob Sie neue Datensätze oder aktualisierte Datensätze anzeigen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Benutzerspezifischer API-Aufruf]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL ServiceNow] API. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von der anderen nicht durchgeführt werden kann [!DNL ServiceNow] Module.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres ServiceNow-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] nach [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Relative URL von [!UICONTROL]</td> 
   <td> <p>Geben Sie die Adresse auf dem Webserver ein, mit der das Modul interagieren soll.</p> <p>Sie können eine relative URL eingeben. Das bedeutet, dass Sie das Protokoll nicht einbeziehen müssen (z. B. <code>http://</code>) am Anfang. Dies legt dem Webserver nahe, dass die Interaktion auf dem Server stattfindet.</p> <p>Beispiel: <code>[!DNL /api/conversations].create</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode]</td> 
   td&gt; <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Notiz:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensatz lesen]

Dieses Aktionsmodul liest eine [!DNL ServiceNow] -Datensatz mithilfe der System-ID.

Das Modul gibt alle mit dem Datensatz verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres ServiceNow-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] nach [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>Eindeutige Eingabe oder Zuordnung [!DNL ServiceNow] Kennung des Datensatzes, den das Modul lesen soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabellenart]</td> 
   <td>Wählen Sie aus, ob sich der zu lesende Datensatz in einer benutzerdefinierten Tabelle oder einer Standardtabelle befindet.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Wählen Sie den Typ [!DNL ServiceNow] notieren, dass das Modul gelesen werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>Wählen Sie den Typ der Werte aus, die angezeigt werden sollen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td>Wählen Sie die Felder aus, die das Modul ausgeben soll.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Deaktivieren eines Benutzers]

Dieses Aktionsmodul deaktiviert einen Benutzer in [!DNL ServiceNow] unter Verwendung der System-ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres ServiceNow-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] nach [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User System ID]</td> 
   <td> Eindeutige Eingabe oder Zuordnung [!DNL ServiceNow] Kennung des Benutzers, den das Modul deaktivieren soll.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Anlage herunterladen]

Dieses Aktionsmodul lädt eine Anlage in einem [!DNL ServiceNow] aufzeichnen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres ServiceNow-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] nach [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anlagensystem-ID]</td> 
   <td> Eindeutige Eingabe oder Zuordnung [!DNL ServiceNow] Kennung des Anhangs, den das Modul herunterladen soll.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Hochladen eines Anhangs]

Dieses Aktionsmodul lädt eine Anlage in eine [!DNL ServiceNow] aufzeichnen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres ServiceNow-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] nach [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabellenname]</td> 
   <td>Geben Sie den Namen der Tabelle ein oder ordnen Sie sie zu, in die Sie den Anhang hochladen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL System-ID]</td> 
   <td>Eindeutige Eingabe oder Zuordnung [!DNL ServiceNow] Kennung des Systems, in das Sie den Anhang hochladen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dateiname]</td> 
   <td>Geben Sie einen Namen für den Anhang ein oder ordnen Sie ihn zu</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dateiinhalt]</td> 
   <td>Geben Sie die Datei ein oder ordnen Sie sie zu, in die Sie hochladen möchten [!DNL ServiceNow].</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensatz erstellen]

Dieses Aktionsmodul erstellt eine neue [!DNL ServiceNow] aufzeichnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres ServiceNow-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] nach [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabellenart]</td> 
   <td>Wählen Sie aus, ob Sie einen Datensatz in einer benutzerdefinierten Tabelle oder einer Standardtabelle erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Wählen Sie den Typ [!DNL ServiceNow] notieren, dass das Modul erstellt werden soll. Sie können dann die verfügbaren Felder für diesen Datensatztyp ausfüllen.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensatz aktualisieren]

Dieses Aktionsmodul erstellt eine neue [!DNL ServiceNow] aufzeichnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres ServiceNow-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] nach [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>Eindeutige Eingabe oder Zuordnung [!DNL ServiceNow] Kennung des Datensatzes, den das Modul aktualisieren soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabellenart]</td> 
   <td>Wählen Sie aus, ob sich der zu aktualisierende Datensatz in einer benutzerdefinierten Tabelle oder einer Standardtabelle befindet.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Wählen Sie den Typ [!DNL ServiceNow] notieren, dass das Modul aktualisiert werden soll. Sie können dann die verfügbaren Felder für diesen Datensatztyp ausfüllen.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensatz löschen]

Dieses Aktionsmodul löscht einen Vorfall oder einen Benutzer.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres ServiceNow-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] nach [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Wählen Sie aus, ob Sie einen Vorfall oder einen Benutzer löschen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL System-ID]</td> 
   <td>Eindeutige Eingabe oder Zuordnung [!DNL ServiceNow] Kennung des Datensatzes, den das Modul löschen soll.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensätze suchen]

Dieses Modul sucht nach Datensätzen anhand von von Ihnen ausgewählten Kriterien.

Das Modul gibt alle mit dem Datensatz verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres ServiceNow-Kontos mit [!DNL Workfront Fusion], siehe <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL ServiceNow] nach [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tabellenart]</td> 
   <td>Wählen Sie aus, ob es sich bei der zu suchenden Tabelle um eine benutzerdefinierte Tabelle oder eine Standardtabelle handelt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>Wählen Sie den Typ des Datensatzes aus, nach dem Sie suchen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Result set]</td> 
   <td>Wählen Sie aus, ob das Modul alle Datensätze zurückgeben soll, die den Kriterien entsprechen, oder nur den ersten Datensatz, der mit ihm übereinstimmt. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl der Datensätze]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suchtyp]</td> 
   <td> <p>Wählen Sie die Art der Suche aus, die das Modul ausführen soll</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Erweiterte Abfrage]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Suchabfrage]</p> <p>Geben Sie die benutzerdefinierte Suchabfrage ein. Informationen über [!DNL ServiceNow] benutzerdefinierte Suchabfragen, siehe <a href="https://docs.servicenow.com/bundle/orlando-platform-user-interface/page/use/common-ui-elements/reference/r_OpAvailableFiltersQueries.html">Dokumentation zur ServiceNow-Abfrage</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Simple]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Suchkriterien]</p> <p>Geben Sie die Kriterien ein, nach denen das Modul suchen soll. Weitere Informationen zum Einrichten von Suchfiltern finden Sie unter <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Hinzufügen eines Filters zu einem Szenario in Adobe Workfront Fusion</a>.</p> </li> 
       <li> <p>[!UICONTROL Sortieren nach]</p> <p>Geben Sie an, nach welchem Feld das Modul Ergebnisse sortieren soll und ob sie auf- oder absteigend sortiert werden sollen.</p> </li> 
      </ul> </li> 
    </ul> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>Wählen Sie den Typ der Werte aus, die angezeigt werden sollen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td>Wählen Sie die Felder aus, die das Modul ausgeben soll.</td> 
  </tr> 
 </tbody> 
</table>
