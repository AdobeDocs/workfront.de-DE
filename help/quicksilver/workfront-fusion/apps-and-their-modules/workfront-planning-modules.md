---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Adobe Workfront-Planungsmodule
description: Mit den [!DNL Adobe Workfront Planning] Modulen können Sie ein [!DNL Adobe Workfront Fusion] Szenario starten, das auf Ereignissen in Ihrem [!DNL Adobe] Workfront-Planungskonto basiert, Vereinbarungen und andere Datensätze erstellen, lesen oder aktualisieren, nach Datensätzen anhand von von Ihnen festgelegten Kriterien suchen und Dokumente hochladen.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 892fdaf3-935e-4e66-a01c-9e9b6e0daf3e
source-git-commit: e067c5ff34c31060ca6fd392289d845f53a5ef3a
workflow-type: tm+mt
source-wordcount: '1116'
ht-degree: 0%

---

# [!DNL Adobe Workfront Planning] Module

Mit den [!DNL Adobe Workfront Planning] -Modulen können Sie ein Szenario Trigger haben, wenn Ereignisse in der Workfront-Planung auftreten. Sie können auch Einträge erstellen, lesen, aktualisieren und löschen oder einen benutzerdefinierten API-Aufruf für Ihr [!DNL Adobe Workfront Planning]-Konto ausführen.

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
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration] </p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]

Sie können eine Verbindung zu Ihrem [!DNL Workfront Planning]-Konto direkt aus einem [!DNL Workfront Fusion]-Modul erstellen.

1. Klicken Sie in einem beliebigen [!DNL Workfront Planning]-App-Modul neben dem Feld [!UICONTROL Verbindung] auf **[!UICONTROL Hinzufügen]** .
1. Geben Sie einen Namen für diese Verbindung ein.
1. Wählen Sie aus, ob Sie eine Verbindung zu einer Produktionsumgebung oder einer Nicht-Produktionsumgebung herstellen möchten.
1. Wählen Sie aus, ob Sie eine Verbindung zu einem Dienstkonto oder einem persönlichen Konto herstellen möchten.
1. Klicken Sie auf **[!UICONTROL SAML log in]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

## [!DNL Adobe Workfront Planning] Module und ihre Felder

### Ereignisse beobachten

Dieses Trigger-Modul startet ein Szenario, wenn ein Datensatz, ein Datensatztyp oder ein Arbeitsbereich in der Workfront-Planung erstellt, aktualisiert oder gelöscht wird.

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
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]</a> .</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Objekttyp]</td>
      <td>Wählen Sie aus, ob Sie Datensätze, Datensatztypen oder Arbeitsbereiche anzeigen möchten.</td>
    </tr>
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Ereignisfilter]</p> </td> 
      <td> <p>Sie können Filter festlegen, um nur Datensätze zu überwachen, die den von Ihnen ausgewählten Kriterien entsprechen.</p> <p>Geben Sie für jeden Filter das Feld, das der Filter auswerten soll, den Operator und den Wert ein, die der Filter zulassen soll. Sie können mehrere Filter verwenden, indem Sie UND-Regeln hinzufügen.</p> <p>Hinweis: Sie können keine Filter in vorhandenen [!DNL Workfront]-Webhooks bearbeiten. Um verschiedene Filter für [!DNL Workfront] -Ereignisabonnements einzurichten, entfernen Sie den aktuellen Webhook und erstellen Sie einen neuen.</p> <p>Weitere Informationen zu Ereignisfiltern finden Sie unter <a href="/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-modules" class="MCXref xref">Ereignisabonnementfilter in den Modulen [!DNL Workfront] &gt; [!UICONTROL Watch Events]</a> im Artikel Workfront-Module.</p> </td> 
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

Dieses Aktionsmodul löscht einen einzelnen Datensatztyp in der Workfront-Planung anhand seiner Kennung.

>[!WARNING]
>
>Beim Löschen eines Datensatztyps in der Workfront-Planung werden auch alle Datensätze aus der Datensatztyptabelle gelöscht.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]</a> .</td>
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

Dieses Modul führt einen benutzerdefinierten API-Aufruf an die [!DNL Adobe Workfront Planning] -API durch.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]</a> .</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Geben Sie einen Pfad relativ zu https://&amp;ltWORKFRONT_DOMAIN&gt;/attask/api/&amp;ltAPI_VERSION&gt;/ ein.</p>
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
        <p>Geben Sie einen Pfad relativ zu https://&amp;ltWORKFRONT_DOMAIN&gt;/attask/api/&amp;ltAPI_VERSION&gt;/ ein.</p>
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
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

<!--

### Delete a field

This action module deletes a single field in Workfront Planning by its ID.

>[!WARNING]
>
>Deleting a field in Workfront Planning deletes it and any data in it from every object of that record type in Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
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


This action module retrieves a single field in Workfront Planning by its ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
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

Dadurch wird ein einzelner Datensatz in der Workfront-Planung erstellt.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]</a> .</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Datensatz-Typ-ID]</p>
      </td>
      <td>Geben Sie den zu erstellenden Datensatztyp ein oder ordnen Sie ihn zu. Die verfügbaren Datensatztypen basieren auf Ihrem Workfront Planning-Konto.</td> 
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

Dieses Aktionsmodul löscht den angegebenen Datensatz in der Workfront-Planung.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]</a> .</td>
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

This action module retrieves all records from an [!DNL Adobe Workfront Planning] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
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

Dieses Aktionsmodul ruft einen einzelnen Datensatz von [!DNL Adobe Workfront Planning] ab, der durch seine Kennung angegeben wird.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]</a> .</td>
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
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]</a> .</td>
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

Dieses Aktionsmodul ruft eine Liste von Datensatztypen in einem [!DNL Adobe Workfront Planning] -Konto ab.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]</a> .</td>
    </tr>
  </tbody>
</table>

### Datensatz aktualisieren

Mit dieser Aktion wird ein einzelner Datensatz in der Workfront-Planung aktualisiert.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]</a> .</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Datensatz-ID]</p>
      </td>
      <td>Geben Sie den zu aktualisierenden Datensatztyp ein oder ordnen Sie ihn zu. Die verfügbaren Datensatztypen basieren auf Ihrem Workfront Planning-Konto.</td> 
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
