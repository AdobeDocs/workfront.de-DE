---
filename: creative-cloud-libraries-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Creative Cloud-Bibliotheksmodule
description: Mit den  [!DNL Adobe Workfront Fusion Adobe Creative Cloud] -Bibliotheksmodulen können Sie ein Szenario starten, wenn ein Element oder eine Bibliothek erstellt oder aktualisiert wird. Sie können Elemente auch hochladen, abrufen, archivieren oder auflisten oder die API  [!DNL Adobe Creative Cloud Libraries] .
author: Becky
feature: Workfront Fusion
exl-id: 8affa34b-803d-48a5-a986-9fbe0cb8c8f5
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1359'
ht-degree: 0%

---

# Adobe Creative Cloud-Bibliotheksmodule

Mit den [!DNL Adobe Workfront Fusion] [!DNL Adobe Creative Cloud Libraries] können Sie ein Szenario starten, wenn ein Element oder eine Bibliothek erstellt oder aktualisiert wird. Sie können auch Elemente hochladen, abrufen, archivieren oder auflisten oder die [!DNL Adobe Creative Cloud Libraries]-API aufrufen.

Anweisungen zum Erstellen eines Szenarios finden Sie unter [Erstellen eines Szenarios](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!IMPORTANT]
>
>Die Verbindungserstellung ist derzeit nicht im Creative Cloud Libraries-Connector verfügbar. Vorhandene Verbindungen funktionieren erwartungsgemäß.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
      <td>
        <p>[!UICONTROL Pro] oder höher</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td>
      <td>
        <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p>
      </td>
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

## Voraussetzungen

Um [!DNL Adobe Creative Cloud Libraries]-Module verwenden zu können, müssen Sie über ein [!UICONTROL Adobe Creative Cloud]-Konto verfügen.

## Informationen zur Adobe Creative Cloud Libraries-API

Der Adobe Creative Cloud Libraries-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td>https://cc-libraries.adobe.io/api/v1</td> 
  </tr>
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.1.7</td> 
  </tr>
 </tbody> 
 </table>

## [!UICONTROL Adobe Creative Cloud-], -Module und ihre Felder

Beim Konfigurieren von [!UICONTROL Adobe Creative Cloud Libraries]-Modulen zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service weitere [!DNL Adobe Creative Cloud Libraries] angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


* [Elemente](#elements)

* [Bibliotheken](#libraries)

* [Sonstige](#other)


### Elemente

* [[!UICONTROL Element archivieren]](#archive-an-element)

* [[!UICONTROL Element abrufen]](#get-an-element)

* [[!UICONTROL Listenelemente]](#list-elements)

* [[!UICONTROL Element hochladen]](#upload-an-element)

* [!UICONTROL [Neues Element in Bibliothek ansehen]](#watch-new-element-in-library)

* [[!UICONTROL Aktualisierte Elemente ansehen]](#watch-updated-elements)


#### [!UICONTROL Element archivieren]

Dieses Aktionsmodul archiviert ein Element aus einer Bibliothek.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Eine bestehende Creative Cloud Libraries-Verbindung auswählen. Die Verbindungserstellung ist derzeit nicht im Creative Cloud Libraries-Connector verfügbar. Vorhandene Verbindungen funktionieren erwartungsgemäß.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Bibliotheks-ID]</td>
      <td >Wählen Sie die Bibliothek aus, die das zu archivierende Element enthält.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL Element-ID]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">Wählen Sie das Element aus, das Sie archivieren möchten.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Element abrufen]

Dieses Aktionsmodul gibt ein einzelnes Element aus einer Bibliothek zurück.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Eine bestehende Creative Cloud Libraries-Verbindung auswählen. Die Verbindungserstellung ist derzeit nicht im Creative Cloud Libraries-Connector verfügbar. Vorhandene Verbindungen funktionieren erwartungsgemäß.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Bibliotheks-ID]</td>
      <td >Wählen Sie die Bibliothek aus, die das abzurufende Element enthält.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Element-ID]</td>
      <td>Geben Sie die ID des Elements ein, das Sie abrufen möchten, oder ordnen Sie sie zu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL-Auswahl]</td>
      <td>
        <p>Wählen Sie den Typ der Informationen aus, die das Modul zurückgibt. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Standard]</b>
            </p>
            <p>Basisdaten</p>
          </li>
          <li>
            <p><b>[!UICONTROL Details]</b>
            </p>
            <p>Alle verfügbaren Daten</p>
          </li>
          <li>
            <p><b>[!UICONTROL-Darstellungen]</b>
            </p>
            <p>Eine reduzierte Liste von Assets, die mit dem Bibliothekselement verknüpft sind</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Listenelemente]

Dieses Aktionsmodul ruft eine Liste von Elementen in einer Bibliothek ab.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Eine bestehende Creative Cloud Libraries-Verbindung auswählen. Die Verbindungserstellung ist derzeit nicht im Creative Cloud Libraries-Connector verfügbar. Vorhandene Verbindungen funktionieren erwartungsgemäß.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Bibliotheks-ID]</td>
      <td >Wählen Sie die Bibliothek aus, aus der Sie Elemente auflisten möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Sortieren nach]</td>
      <td>Wählen Sie aus, ob die Ergebnisse nach Namen oder nach dem letzten Änderungsdatum des Elements sortiert werden sollen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Typ]</td>
      <td >Geben Sie einen MIME-Typ ein, um die Ergebnisse auf Elemente zu beschränken, die mit dem angegebenen MIME-Typ identifiziert werden. Beispiel: <code>string</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL-Auswahl]</td>
      <td>
        <p>Wählen Sie den Typ der Informationen aus, die das Modul zurückgibt. </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Standard]</b>
            </p>
            <p>Basisdaten</p>
          </li>
          <li>
            <p><b>[!UICONTROL Details]</b>
            </p>
            <p>Alle verfügbaren Daten</p>
          </li>
          <li>
            <p><b>[!UICONTROL-Darstellungen]</b>
            </p>
            <p>Eine reduzierte Liste von Assets, die mit dem Bibliothekselement verknüpft sind</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Element hochladen]

Dieses Aktionsmodul lädt ein kleines Datei-Asset in eine vorhandene Bibliothek hoch. Die maximale Dateigröße beträgt 1 GB.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Eine bestehende Creative Cloud Libraries-Verbindung auswählen. Die Verbindungserstellung ist derzeit nicht im Creative Cloud Libraries-Connector verfügbar. Vorhandene Verbindungen funktionieren erwartungsgemäß.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Bibliotheks-ID]</td>
      <td >Wählen Sie die Bibliothek aus, aus der Sie Elemente auflisten möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Aufrufmodus]</td>
      <td>
        <p>Wählen Sie den Verarbeitungsmodus aus, mit dem dieser Anforderungsprozess aufgerufen werden soll.</p>
        <ul>
          <li>
            <p><b>[!UICONTROL sync]</b>
            </p>
            <p>Der API-Aufruf wird synchron verarbeitet. Die Antwort wird bereitgestellt, wenn die Verarbeitung abgeschlossen ist (es sei denn, der Aufruf überschreitet das Zeitlimit.)</p>
          </li>
          <li>
            <p><b>[!UICONTROL async]</b>
            </p>
            <p>Die Antwort des asynchronen Monitors wird sofort zurückgegeben, und die Anforderungsverarbeitung erfolgt asynchron. Der aufrufende Benutzer ist dafür verantwortlich, den Endpunkt bis zum Abschluss abzufragen.</p>
          </li>
          <li>
            <p><b>[!UICONTROL sync,async]</b> (Standard)</p>
            <p>Es wird versucht, die Anfrage synchron zu verarbeiten. Wenn die Verarbeitung mehr als 5000 ms dauert, wird die Antwort des asynchronen Monitors zurückgegeben. Die Monitor-URL sollte abgefragt werden, bis die Anfrage abgeschlossen ist.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Typdatei]</td>
      <td >Geben Sie den MIME-Typ der hochgeladenen Datei ein oder ordnen Sie ihn zu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Source-Datei]</td>
      <td>
        <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Neues Element in Bibliothek ansehen]

Dieses Trigger-Modul startet ein Szenario, wenn ein Element zu einer Bibliothek hinzugefügt wird.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Eine bestehende Creative Cloud Libraries-Verbindung auswählen. Die Verbindungserstellung ist derzeit nicht im Creative Cloud Libraries-Connector verfügbar. Vorhandene Verbindungen funktionieren erwartungsgemäß.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Bibliotheks-ID]</td>
      <td >Wählen Sie die Bibliothek aus, die Sie auf aktualisierte Elemente überwachen möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL Aktualisierte Elemente ansehen]

Dieses Trigger-Modul startet ein Szenario, wenn ein Element in einer Bibliothek aktualisiert wird.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Eine bestehende Creative Cloud Libraries-Verbindung auswählen. Die Verbindungserstellung ist derzeit nicht im Creative Cloud Libraries-Connector verfügbar. Vorhandene Verbindungen funktionieren erwartungsgemäß.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Bibliotheks-ID]</td>
      <td >Wählen Sie die Bibliothek aus, die Sie auf neue Elemente überwachen möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</td>
    </tr>
  </tbody>
</table>

### Bibliotheken

* [[!UICONTROL Neue Bibliotheken ansehen]](#watch-new-libraries)

* [[!UICONTROL Aktualisierte Bibliotheken ansehen]](#watch-updated-libraries)


#### [!UICONTROL Neue Bibliotheken ansehen]

Dieses Bibliotheksmodul startet ein Trigger, wenn eine neue Bibliothek erstellt wird.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Eine bestehende Creative Cloud Libraries-Verbindung auswählen. Die Verbindungserstellung ist derzeit nicht im Creative Cloud Libraries-Connector verfügbar. Vorhandene Verbindungen funktionieren erwartungsgemäß.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Aktualisierte Bibliotheken ansehen]

Dieses Bibliotheksmodul startet ein Trigger, wenn eine vorhandene Bibliothek aktualisiert wird.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Eine bestehende Creative Cloud Libraries-Verbindung auswählen. Die Verbindungserstellung ist derzeit nicht im Creative Cloud Libraries-Connector verfügbar. Vorhandene Verbindungen funktionieren erwartungsgemäß.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</td>
    </tr>
  </tbody>
</table>

### Sonstige

#### [!UICONTROL Erstellen eines API-Aufrufs]

Dieses Modul führt einen benutzerdefinierten API-Aufruf an die [!DNL Adobe Creative Cloud Libraries]-API durch.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden Ihres Adobe Creative Cloud-Kontos mit Workfront Fusion finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbindung zu Adobe Workfront Fusion herstellen - Grundanweisungen.</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Geben Sie einen Pfad relativ zu <code>https://cc-libraries.adobe.io/api</code> ein.</p>
    <p>Beispiel: <code>/v1/libraries</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL API-Version]</td>
      <td>
        <p>Wählen Sie die Version der [!DNL Adobe Analytics]-API aus, mit der Sie eine Verbindung herstellen möchten.</p>
      </td>
    </tr>    <tr>
      <td role="rowheader">[!UICONTROL-Methode]</td>
      <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-Anfragemethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL-Kopfzeilen]</td>
      <td>
        <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p>
        <p>Beispiel: <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion fügt die Autorisierungskopfzeilen für Sie hinzu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td>
      <td>
        <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p>
        <p>Beispiel: <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL body]</td>
   <td> <p>Fügen Sie den Hauptteil des Inhalts für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Wenn Sie bedingte Anweisungen wie <code>if</code> in Ihrer JSON-Datei verwenden, setzen Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
       <tr>
      <td role="rowheader">[!UICONTROL Vorübergehendes Dokument hochladen]</td>
      <td>
      <p>Wenn Sie ein vorübergehendes Dokument hochladen möchten, geben Sie die Quelldatei für das Dokument ein, das Sie hochladen möchten.</p>
      <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p>
    </td>
    </tr>

</tbody>
</table>
