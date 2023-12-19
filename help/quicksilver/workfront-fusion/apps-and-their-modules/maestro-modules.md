---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Adobe Maestro-Module
description: Mit dem [!DNL Adobe Maestro] -Module, können Sie eine [!DNL Adobe Workfront Fusion] Szenario basierend auf Ereignissen in Ihrer [!DNL Adobe] Maestro-Konto, erstellen, lesen oder aktualisieren Vereinbarungen und andere Datensätze, suchen nach Datensätzen anhand von von Ihnen festgelegten Kriterien und laden Dokumente hoch.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: fe0c867b218879c1d0d969112eb62878782a40ad
workflow-type: tm+mt
source-wordcount: '1007'
ht-degree: 0%

---

# [!DNL Adobe Maestro] Module

Mit dem [!DNL Adobe Maestro] -Modulen können Sie ein Szenario Trigger haben, wenn Ereignisse in Maestro auftreten. Sie können auch Datensätze erstellen, lesen, aktualisieren und löschen oder einen benutzerdefinierten API-Aufruf an Ihre [!DNL Adobe Maestro] -Konto.

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
   <td>
   <p>Aktuelle Lizenzanforderungen: nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Erstellen Sie eine Verbindung zu [!DNL Adobe Maestro]

Sie können eine Verbindung zu Ihrem [!DNL Maestro] direkt in einer [!DNL Workfront Fusion] -Modul.

1. In jeder [!DNL Maestro] App-Modul, klicken Sie auf **[!UICONTROL Hinzufügen]** neben dem [!UICONTROL Verbindung] ankreuzen.
1. Geben Sie einen Namen für diese Verbindung ein.
1. Wählen Sie aus, ob Sie eine Verbindung zu einer Produktionsumgebung oder einer Nicht-Produktionsumgebung herstellen möchten.
1. Wählen Sie aus, ob Sie eine Verbindung zu einem Dienstkonto oder einem persönlichen Konto herstellen möchten.
1. Klicks **[!UICONTROL SAML-Anmeldung]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

## [!DNL Adobe Maestro] Module und ihre Felder

### Ereignisse beobachten

Dieses Trigger-Modul startet ein Szenario, wenn ein Datensatz, ein Datensatztyp oder ein Arbeitsbereich in Maestro erstellt, aktualisiert oder gelöscht wird.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>Wählen Sie den Webhook aus, den Sie verwenden möchten, oder klicken Sie auf Hinzufügen , um einen neuen zu erstellen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Maestro], siehe <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Maestro]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Objekttyp]</td>
      <td>Wählen Sie aus, ob Sie Datensätze, Datensatztypen oder Arbeitsbereiche anzeigen möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Objekte ansehen]</td>
      <td>Wählen Sie aus, ob Sie nach neuen Optionen suchen möchten. aktualisierte, neue und aktualisierte oder gelöschte Datensätze.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Von dieser Verbindung vorgenommene Aktualisierungen ausschließen]</p>
      </td>
      <td>Aktivieren Sie diese Option, um zu verhindern, dass das Szenario ausgelöst wird, wenn die von diesem Modul verwendete Verbindung eine Änderung vornimmt. Dadurch wird verhindert, dass eine andere Instanz des Szenarios ausgelöst wird, wenn dieses Szenario eine auslösende Aktion ausführt.</td> 
      </tr>
  </tbody>
</table>

### Löschen eines Datensatztyps

Dieses Aktionsmodul löscht einen einzelnen Datensatztyp in Maestro anhand seiner ID.

>[!WARNING]
>
>Beim Löschen eines Datensatztyps in Maestro werden auch alle Datensätze aus der Tabelle &quot;Record Type&quot;gelöscht.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Maestro], siehe <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Maestro]</a> in diesem Artikel.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Datensatz-Typ-ID]</p>
      </td>
      <td>Geben Sie die Kennung des Felds ein, das Sie löschen möchten, oder ordnen Sie sie zu.</td> 
      </tr>
  </tbody>
</table>

### Benutzerdefinierte API-Aufrufe durchführen

Dieses Modul führt einen benutzerdefinierten API-Aufruf an die [!DNL Adobe Maestro] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Maestro], siehe <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Maestro]</a> in diesem Artikel.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Geben Sie einen Pfad relativ zu https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/ ein.</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL API-Version]</p>
      </td>
      <td>
        <p>Wählen Sie die API-Version aus, die Sie verwenden möchten. Wenn Sie keine Version auswählen, wird standardmäßig die neueste Version verwendet.</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL API Path override]</p>
      </td>
      <td>
        <p>Geben Sie einen Pfad relativ zu https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/ ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Methode]</p>
      </td>
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Header]</td>
      <td>
        <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p>
        <p>Beispiel: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] fügt automatisch Autorisierungskopfzeilen hinzu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Abfragezeichenfolge]  </td>
      <td>
        <p>Klicken Sie für jedes Schlüssel/Wert-Paar, das Sie zur Abfragezeichenfolge hinzufügen möchten, auf <b>Element hinzufügen</b> und geben Sie den Schlüssel und den Wert ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

<!--

### Delete a field

This action module deletes a single field in Maestro by its ID.

>[!WARNING]
>
>Deleting a field in Maestro deletes it and any data in it from every object of that record type in Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the record type you want to delete.</td> 
      </tr>
  </tbody>
</table>

### Get a field 


This action module retrieves a single field in Maestro by its ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the field you want to delete.</td> 
      </tr>
  </tbody>
</table>

-->

### Datensatz erstellen

Diese Aktion erstellt einen einzelnen Datensatz in Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Maestro], siehe <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Maestro]</a> in diesem Artikel.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Datensatz-Typ-ID]</p>
      </td>
      <td>Geben Sie den zu erstellenden Datensatztyp ein oder ordnen Sie ihn zu. Verfügbare Datensatztypen basieren auf Ihrem Maestro-Konto.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>Andere Felder</p>
      </td>
      <td>Diese Felder basieren auf dem von Ihnen ausgewählten Datensatztyp.</td> 
      </tr>
     <tr>
  </tbody>
</table>

### Datensatz löschen

Dieses Aktionsmodul löscht den angegebenen Datensatz in Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Maestro], siehe <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Maestro]</a> in diesem Artikel.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Datensatz-ID]</p>
      </td>
      <td>Geben Sie die Kennung des Datensatzes ein, den Sie löschen möchten, oder ordnen Sie sie zu.</td> 
      </tr>
  </tbody>
</table>

<!--

### Get all records

This action module retrieves all records from an [!DNL Adobe Maestro] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned records]</p>
      </td>
      <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
      </tr>
  </tbody>
</table>

-->

### Datensatz abrufen

Dieses Aktionsmodul ruft einen einzelnen Datensatz aus [!DNL Adobe Maestro], angegeben durch die Kennung.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Maestro], siehe <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Maestro]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datensatz-ID]</td>
      <td>Geben Sie die Kennung des Datensatzes ein oder ordnen Sie ihn zu.</td>
    </tr>
  </tbody>
</table>

### Abrufen von Datensätzen nach Datensatztyp

Dieses Aktionsmodul ruft alle Datensätze des angegebenen Typs ab.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Maestro], siehe <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Maestro]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Wählen Sie den Arbeitsbereich aus oder ordnen Sie ihn zu, der die abzurufenden Datensätze enthält.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record Type]</td>
      <td>Wählen Sie den Typ des Datensatzes aus, den Sie abrufen möchten.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximale Anzahl an zurückgegebenen Datensätzen]</p>
      </td>
      <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td> 
  </tbody>
</table>

### Abrufen von Datensatztypen

Dieses Aktionsmodul ruft eine Liste von Datensatztypen in einer [!DNL Adobe Maestro] -Konto.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Maestro], siehe <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Maestro]</a> in diesem Artikel.</td>
    </tr>
  </tbody>
</table>

### Datensatz aktualisieren

Diese Aktion aktualisiert einen einzelnen Datensatz in Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Maestro], siehe <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Maestro]</a> in diesem Artikel.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Datensatz-ID]</p>
      </td>
      <td>Geben Sie den zu aktualisierenden Datensatztyp ein oder ordnen Sie ihn zu. Verfügbare Datensatztypen basieren auf Ihrem Maestro-Konto.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>Andere Felder</p>
      </td>
      <td>Diese Felder basieren auf dem von Ihnen ausgewählten Datensatztyp.</td> 
      </tr>
     <tr>
  </tbody>
</table>

### Suchdatensätze

Dieses Aktionsmodul ruft anhand der von Ihnen angegebenen Kriterien eine Liste von Datensätzen ab.

>[!NOTE]
>
>Dieses Modul befindet sich im Bau.

