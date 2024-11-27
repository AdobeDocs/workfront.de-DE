---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Microsoft Dynamics 365 Finanz- und Betriebsmodule
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die Microsoft Dynamics 365 Finance and Operations verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
source-git-commit: 130437dd44db5db2a94914fb0e42fd35a7c14291
workflow-type: tm+mt
source-wordcount: '995'
ht-degree: 0%

---

# [!DNL Microsoft Dynamics 365 Finance and Operations modules]

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Microsoft Dynamics 365] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

>[!NOTE]
>
>Der [!DNL Microsoft Dynamics 365 Finance and Operations]-Connector unterstützt [!DNL Dynamics 365] nicht.
>
>Informationen zu Microsoft Dynamics 365-Modulen finden Sie unter [[!DNL Microsoft Dynamics 365 modules]](/help/quicksilver/workfront-fusion/apps-and-their-modules/microsoft-dynamics-365-modules.md).

Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Verbindung erstellen

So erstellen Sie eine Verbindung für Ihre Microsoft Dynamics 365 Finance- und Operations-Module:

1. Klicken Sie in einem beliebigen Microsoft Dynamics 365 Finance and Operations-Modul neben dem Feld Connection auf **[!UICONTROL Add]** .

1. Füllen Sie die folgenden Felder aus:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Verbindungstyp]</td>
        <td>
          <p>Wählen Sie aus, ob Sie eine standardmäßige Dynamics Finance- und Operations-Verbindung oder eine Verbindung mit einem Autorisierungscode erstellen.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Verbindungsname]</td>
        <td>
          <p>Geben Sie einen Namen für diese Verbindung ein.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client-ID]</td>
        <td>Geben Sie Ihre Dynamics Finance- und Operations-Client-ID [!UICONTROL] ein.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Geben Sie Ihren Dynamics Finance- und Operations-Client-Geheimnis ein. </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Mandantenkennung]</td>
        <td>Geben Sie Ihre Dynamics Finance- und Operations-Mandanten-ID ein.</td>
        </tr>
        <tr>
        <td role="rowheader">Ressource</td>
        <td>Geben Sie die URL Ihres Dynamics Finance- und Operations-Kontos ein (ohne https://)</td>
        </tr>
      </tbody>
    </table>

1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu speichern und zum Modul zurückzukehren.



## Microsoft Dynamics 365 Finanz- und Betriebsmodule und ihre Felder

>[!IMPORTANT]
>
>Die über die F&amp;O-API von Dynamics 365 verfügbaren Datenentitäten können je nach Instanz variieren. Wenn Sie nicht sicher sind, welche Entitäten über die API verfügbar sind, sollten Sie die Entitäten in Ihrer Instanz mithilfe des Endpunkts &quot;Daten&quot;durchsuchen. Der Endpunkt &quot;data&quot;in Dynamics 365 Finance and Operations ist die Stamm-URL für den Zugriff auf OData-Dienste. Mit diesem Endpunkt können Sie mithilfe von Standard-OData-Protokollen mit verschiedenen vom System offen gelegten Datenentitäten interagieren.
>
>Sie können diese Entitäten mit dem benutzerdefinierten API-Aufrufmodul abrufen.
>
><!--For more information -->



### Entitätselement erstellen

Dieses Aktionsmodul erstellt ein neues Entitätselement in Microsoft Dynamics 365 Finance and Operations.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Verbindung]</td>
    <td> <p>Anweisungen zum Verbinden von Microsoft Dynamics 365 Finance and Operations mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection" class="MCXref xref">Erstellen einer Verbindung</a> .</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entity]</td>
     <td>Geben Sie den Entitätstyp Dynamics Finance and Operations ein oder ordnen Sie ihn zu, den Sie erstellen möchten.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Body]</td>
     <td> <p>Geben Sie einen JSON-Hauptteil ein oder ordnen Sie ihn zu, der die Daten enthält, die Sie in das neue Entitätselement aufnehmen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>



### Entitätselement löschen

Dieses Aktionsmodul löscht ein Entitätselement aus Dynamics Finance and Operations. Das Element wird durch seine Primären Schlüsselfelder identifiziert.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Verbindung]</td>
    <td> <p>Anweisungen zum Verbinden von Microsoft Dynamics 365 Finance and Operations mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection" class="MCXref xref">Erstellen einer Verbindung</a> .</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entity]</td>
     <td>Geben Sie den Entitätstyp Dynamics Finance and Operations ein oder ordnen Sie ihn zu, den Sie löschen möchten.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Primäre Schlüsselfelder]</td>
     <td> Die Primären Schlüsselfelder identifizieren das Element. Klicken Sie für jedes Primärschlüsselfeld, das Sie bereitstellen möchten, auf "<b>Element hinzufügen</b>"und geben Sie den eindeutigen Schlüssel und Wert ein oder ordnen Sie ihn zu, die dieses Element identifizieren. </td> 
  </tr> 
 </tbody> 
</table>

### Benutzerdefinierte API-Aufrufe durchführen

Dieses Aktionsmodul führt einen benutzerdefinierten Aufruf an die Dynamics Finance- und Operations-API durch.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
    <td> <p>Anweisungen zum Verbinden von Microsoft Dynamics 365 Finance and Operations mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection" class="MCXref xref">Erstellen einer Verbindung</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Geben Sie einen Pfad relativ zu Ihrer Dynamics Finance- und Operations-URL ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode]</td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu. Dadurch wird der Inhaltstyp der Anforderung bestimmt.</p> <p>Beispiel:<code> {"Content-type":"application/json"}</code></p> <p>Hinweis: Wenn Fehler auftreten und es schwierig ist, ihren Ursprung zu bestimmen, sollten Sie die Kopfzeilen auf Grundlage der [!DNL Workfront] -Dokumentation ändern. Wenn Ihr benutzerspezifischer API-Aufruf einen 422-HTTP-Anforderungsfehler zurückgibt, versuchen Sie, einen <code>"Content-Type":"text/plain"</code> -Header zu verwenden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"name":"something-urgent"}</code></p> <p>Tipp: Es wird empfohlen, Informationen nicht als Abfrageparameter, sondern über den JSON-Hauptteil zu senden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>



### Entitätselement lesen

Dieses Aktionsmodul gibt Daten von einem Entitätselement zurück. Das Element wird durch seine Primären Schlüsselfelder identifiziert.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Verbindung]</td>
    <td> <p>Anweisungen zum Verbinden von Microsoft Dynamics 365 Finance and Operations mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection" class="MCXref xref">Erstellen einer Verbindung</a> .</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entity]</td>
     <td>Geben Sie den Entitätstyp Dynamics Finance and Operations ein oder ordnen Sie ihn zu, den Sie lesen möchten.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Primäre Schlüsselfelder]</td>
     <td> Die Primären Schlüsselfelder identifizieren das Element. Klicken Sie für jedes Primärschlüsselfeld, das Sie bereitstellen möchten, auf "<b>Element hinzufügen</b>"und geben Sie den eindeutigen Schlüssel und Wert ein oder ordnen Sie ihn zu, die dieses Element identifizieren. </td> 
  </tr> 
 </tbody> 
</table>

### Entitätselement aktualisieren

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Verbindung]</td>
    <td> <p>Anweisungen zum Verbinden von Microsoft Dynamics 365 Finance and Operations mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#create-a-connection" class="MCXref xref">Erstellen einer Verbindung</a> .</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Entity]</td>
     <td>Geben Sie den Entitätstyp Dynamics Finance and Operations ein oder ordnen Sie ihn zu, den Sie aktualisieren möchten.</td> 
  </tr>  
  <tr> 
    <td>[!UICONTROL Primäre Schlüsselfelder]</td>
     <td> Die Primären Schlüsselfelder identifizieren das Element. Klicken Sie für jedes Primärschlüsselfeld, das Sie bereitstellen möchten, auf "<b>Element hinzufügen</b>"und geben Sie den eindeutigen Schlüssel und Wert ein oder ordnen Sie ihn zu, die dieses Element identifizieren. </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Body]</td>
     <td> <p>Geben Sie einen JSON-Hauptteil ein oder ordnen Sie ihn zu, der die Daten enthält, die Sie in das neue Entitätselement aufnehmen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Suchen

Dieses Suchmodul gibt Ergebnisse basierend auf von Ihnen angegebenen Kriterien zurück.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihrer [!DNL Workfront]-App mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-workfront-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Workfront] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Entity]</td> 
   <td>Geben Sie den Entitätstyp Dynamics Finance and Operations ein oder ordnen Sie ihn zu, den Sie suchen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Suchkriterien]</td> 
   <td> <p>Geben Sie das Feld, nach dem Sie suchen möchten, den Operator, den Sie in Ihrer Abfrage verwenden möchten, und den Wert ein, nach dem Sie im Feld suchen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Sortieren nach</td> 
   <td> <p>Geben Sie das Feld ein oder ordnen Sie es zu, nach dem die Ergebnisse sortiert werden sollen.</p> </td> 
  </tr> 
 </tbody> 
</table>


<!--

### List All

This module lists all records for a given entity.  The item is identified by its Primary key fields.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>[!UICONTROL Connection]</td>
    <td> <p>For instructions about connecting Microsoft Dynamics 365 Finance and Operations to [!DNL Workfront Fusion], see <a href="#create-a-connection" class="MCXref xref">Create a connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Record Type]</td>
     <td>Choose the Dynamics Finance and Operations entity type that you want the module to list.</td> 
  </tr> 
  <tr> 
    <td>[!UICONTROL Outputs]</td>
     <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Watch Record

This trigger module starts a scenario when a record of the given type is created or updated.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
    <td> <p>For instructions about connecting Microsoft Dynamics 365 Finance and Operations to [!DNL Workfront Fusion], see <a href="#create-a-connection" class="MCXref xref">Create a connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td> <p>Select the type of [!DNL Workfront] record that you want the module to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Enter the field that you want to search by, the operator you want to use in your query, and the value that you are searching for in the field.</p> <p>Note: Do not use <code>username </code>in your search criteria. Including <code>username </code>in an API query to [!DNL Workfront] logs the user into Workfront, and the search will not be successful.</p> <p>Note: <code>In</code> and <code>NotIn</code>work with arrays. The inputs should be in array format.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->
