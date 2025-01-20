---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: Adobe Workfront-Planungsmodule
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 892fdaf3-935e-4e66-a01c-9e9b6e0daf3e
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1207'
ht-degree: 0%

---

# [!DNL Adobe Workfront Planning]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Adobe Workfront-Planungsmodule](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-planning-modules.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Mit den [!DNL Adobe Workfront Planning]-Modulen können Sie einen Trigger erstellen, wenn in Workfront Planning Ereignisse eintreten. Sie können auch Datensätze erstellen, lesen, aktualisieren und löschen oder einen benutzerdefinierten API-Aufruf an Ihr [!DNL Adobe Workfront Planning]-Konto durchführen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td>
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td> 
   <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!DNL Adobe Workfront] [!UICONTROL Select] oder [!UICONTROL Prime] verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen. [!DNL Workfront Fusion] ist im [!DNL Workfront] [!UICONTROL Ultimate] enthalten.</p>
   <p>Oder</p>
   <p>Legacy-Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Informationen zur Adobe Workfront Planning-API

Der Adobe Workfront Planning-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td>https://&lbrace;&lbrace;connection.host&rbrace;&rbrace;/maestro/api/&lbrace;&lbrace;common.maestroApiVersion&rbrace;&rbrace;/</td> 
  </tr>
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.13.7</td> 
  </tr>
 </tbody> 
 </table>

## Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]

Sie können direkt aus einem [!DNL Workfront Fusion]-Modul heraus eine Verbindung zu Ihrem [!DNL Workfront Planning]-Konto herstellen.

1. Klicken Sie in einem beliebigen [!DNL Adobe Workfront Planning] auf **[!UICONTROL Hinzufügen]** neben dem Feld Verbindung .

1. Füllen Sie die folgenden Felder aus:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Verbindungsname]</td>
          <td>
            <p>Geben Sie einen Namen für diese Verbindung ein.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Umgebung]</td>
          <td>Wählen Sie aus, ob Sie eine Verbindung zu einer Produktions- oder Nicht-Produktionsumgebung herstellen.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Typ]</td>
          <td>Wählen Sie aus, ob Sie eine Verbindung zu einem Service-Konto oder einem persönlichen Konto herstellen möchten.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client-ID]<p>(Optional)</p></td>
          <td>Geben Sie Ihre [!DNL Adobe] [!UICONTROL Client ID] ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client-Geheimnis]<p>(Optional)</p></td>
          <td>Geben Sie Ihren [!DNL Adobe] [!UICONTROL Client Secret] ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL-Authentifizierungs-URL]<p>(Optional)</p></td>
          <td>Geben Sie die URL ein, die Ihre Workfront-Instanz zur Authentifizierung dieser Verbindung verwenden soll. <p>Der Standardwert ist <code>https://oauth.my.workfront.com/integrations/oauth2</code>.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Host-Präfix]</td>
          <td>Geben Sie Ihr Host-Präfix ein.<p>Der Standardwert ist <code>origin-</code>.</p>
        </tr>
      </tbody>
    </table>
1. Klicken Sie **[!UICONTROL Fortfahren]**, um die Verbindung zu speichern und zum Modul zurückzukehren.

## [!DNL Adobe Workfront Planning] Module und ihre Felder

### Trigger

#### Ereignisse ansehen

Dieses Trigger-Modul startet ein Szenario, wenn ein Datensatz, ein Datensatztyp oder ein Arbeitsbereich in Workfront Planning erstellt, aktualisiert oder gelöscht wird.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>Wählen Sie den Webhook aus, den Sie verwenden möchten, oder klicken Sie auf Hinzufügen , um einen neuen zu erstellen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning] finden Sie unter <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Objekttyp]</td>
      <td>Wählen Sie aus, ob Datensätze, Datensatztypen oder Arbeitsbereiche überwacht werden sollen.</td>
    </tr>
     <tr data-mc-conditions=""> 
      <td> <p>[!UICONTROL Ereignisfilter]</p> </td> 
      <td> <p>Sie können Filter festlegen, um nur nach Datensätzen zu suchen, die die von Ihnen ausgewählten Kriterien erfüllen.</p> <p>Geben Sie für jeden Filter das Feld ein, das vom Filter ausgewertet werden soll, den Operator und den Wert, den der Filter zulassen soll. Sie können mehr als einen Filter verwenden, indem Sie AND-Regeln hinzufügen.</p> <p>Hinweis: Filter in vorhandenen [!DNL Workfront]-Webhooks können nicht bearbeitet werden. Um verschiedene Filter für [!DNL Workfront] Ereignisabonnements einzurichten, entfernen Sie den aktuellen Webhook und erstellen Sie einen neuen.</p> <p>Weitere Informationen zu Ereignisfiltern finden Sie unter <a href="/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-modules" class="MCXref xref">Ereignisabonnementfilter in den Modulen [!DNL Workfront] &gt; [!UICONTROL Ereignisse beobachten</a> im Artikel Workfront-Module .</p> </td> 
     </tr> 
    <tr>
      <td role="rowheader">[!UICONTROL zu überwachende Objekte]</td>
      <td>Wählen Sie aus, ob Sie auf neue Nachrichten achten möchten. Aktualisierte, neue und aktualisierte oder gelöschte Datensätze.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Von dieser Verbindung vorgenommene Aktualisierungen ausschließen]</p>
      </td>
      <td>Aktivieren Sie diese Option, um zu verhindern, dass das Szenario ausgelöst wird, wenn eine Änderung durch die von diesem Modul verwendete Verbindung vorgenommen wird. Dadurch wird verhindert, dass eine weitere Instanz des Szenarios ausgelöst wird, wenn dieses Szenario eine auslösende Aktion ausführt.</td> 
      </tr>
  </tbody>
</table>

### Aktionen

* [Datensatztyp löschen](#delete-a-record-type)
* [Erstellen eines benutzerdefinierten KI-Aufrufs](#make-a-custom-api-call)

#### Datensatztyp löschen

Dieses Aktionsmodul löscht einen einzelnen Datensatztyp in Workfront Planning anhand seiner ID.

>[!WARNING]
>
>Durch das Löschen eines Datensatztyps in Workfront Planning werden auch alle Datensätze in der Datensatztyptabelle gelöscht.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning] finden Sie unter <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]</a> in diesem Artikel.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Datensatztyp-ID]</p>
      </td>
      <td>Geben Sie die ID des Felds ein, das Sie löschen möchten, oder ordnen Sie sie zu.</td> 
      </tr>
  </tbody>
</table>

#### Erstellen eines benutzerdefinierten API-Aufrufs

Dieses Modul führt einen benutzerdefinierten API-Aufruf an die [!DNL Adobe Workfront Planning]-API durch.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning] finden Sie unter <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]</a> in diesem Artikel.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL]</p>
      </td>
      <td>
        <p>Pfad eingeben für <code>https://(YOUR_WORKFRONT_DOMAIN)/maestro/api/</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL-Methode]</p>
      </td>
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anfragemethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL-Kopfzeilen]</td>
      <td>
        <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p>
        <p>Beispiel: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] Fügt automatisch Autorisierungskopfzeilen hinzu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Abfragezeichenfolge]  </td>
      <td>
        <p>Klicken Sie für jedes Schlüssel/Wert-Paar, das Sie der Abfragezeichenfolge hinzufügen möchten, auf <b>Element hinzufügen</b> und geben Sie den Schlüssel und den Wert ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL body]</td>
   <td> <p>Fügen Sie den Hauptteil des Inhalts für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Wenn Sie bedingte Anweisungen wie <code>if</code> in Ihrer JSON-Datei verwenden, setzen Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

<!--
### Searches

#### Search records

This action module retrieves a list of records based on criteria you specify.

-->

### Nicht kategorisiert


#### Erstellen eines Datensatzes

Diese Aktion erstellt in Workfront Planning einen einzigen Datensatz.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning] finden Sie unter <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]</a> in diesem Artikel.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Datensatztyp-ID]</p>
      </td>
      <td>Geben Sie den Typ des Datensatzes ein, den Sie erstellen möchten, oder ordnen Sie ihn zu. Die verfügbaren Datensatztypen basieren auf Ihrem Workfront Planning-Konto.</td> 
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

### Löschen eines Datensatzes

Dieses Aktionsmodul löscht den angegebenen Datensatz in Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning] finden Sie unter <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]</a> in diesem Artikel.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Datensatz-ID]</p>
      </td>
      <td>Geben Sie die ID des Datensatzes ein, den Sie löschen möchten, oder mappen Sie sie.</td> 
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

Dieses Aktionsmodul ruft einen einzelnen Datensatz aus [!DNL Adobe Workfront Planning] ab, angegeben durch die Kennung.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning] finden Sie unter <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datensatz-ID]</td>
      <td>Geben Sie die ID des Datensatzes ein, den Sie abrufen möchten, oder ordnen Sie sie zu.</td>
    </tr>
  </tbody>
</table>

### Datensätze nach Datensatztyp abrufen

Dieses Aktionsmodul ruft alle Datensätze des angegebenen Typs ab.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning] finden Sie unter <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Wählen Sie den Arbeitsbereich aus, der die abzurufenden Datensätze enthält, oder ordnen Sie ihn zu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datensatztyp]</td>
      <td>Wählen Sie den Typ des Datensatzes aus, den Sie abrufen möchten.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximale Anzahl der zurückgegebenen Datensätze]</p>
      </td>
      <td>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</td> 
  </tbody>
</table>

### Datensatztypen abrufen

Dieses Aktionsmodul ruft eine Liste von Datensatztypen in einem [!DNL Adobe Workfront Planning] ab.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning] finden Sie unter <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]</a> in diesem Artikel.</td>
    </tr>
  </tbody>
</table>

### Eintrag aktualisieren

Diese Aktion aktualisiert einen einzelnen Datensatz in Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning] finden Sie unter <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Workfront Planning]</a> in diesem Artikel.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Datensatz-ID]</p>
      </td>
      <td>Geben Sie den Typ des Datensatzes ein, den Sie aktualisieren möchten, oder ordnen Sie ihn zu. Die verfügbaren Datensatztypen basieren auf Ihrem Workfront Planning-Konto.</td> 
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
