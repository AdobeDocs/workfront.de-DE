---
filename: creative-cloud-libraries-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Creative Cloud-Bibliotheksmodule
description: Mit den [!DNL Adobe Workfront Fusion Adobe Creative Cloud] Bibliotheksmodulen können Sie ein Szenario starten, wenn ein Element oder eine Bibliothek erstellt oder aktualisiert wird. Sie können auch Elemente hochladen, abrufen, archivieren, auflisten oder die [!DNL Adobe Creative Cloud Libraries] API aufrufen.
author: Becky
feature: Workfront Fusion
exl-id: 8affa34b-803d-48a5-a986-9fbe0cb8c8f5
source-git-commit: 103a4a7b58048678739d6125c042503458ae3722
workflow-type: tm+mt
source-wordcount: '1338'
ht-degree: 0%

---

# Adobe Creative Cloud-Bibliotheksmodule

Mit den Modulen [!DNL Adobe Workfront Fusion] [!DNL Adobe Creative Cloud Libraries] können Sie ein Szenario starten, wenn ein Element oder eine Bibliothek erstellt oder aktualisiert wird. Sie können auch Elemente hochladen, abrufen, archivieren, auflisten oder die [!DNL Adobe Creative Cloud Libraries] -API aufrufen.

Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!IMPORTANT]
>
>Die Erstellung von Verbindungen ist derzeit nicht im Creative Cloud Libraries-Connector verfügbar. Bestehende Verbindungen funktionieren erwartungsgemäß.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
      <td>
        <p>[!UICONTROL Pro] oder höher</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] license*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p>
      </td>
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

## Voraussetzungen

Um [!DNL Adobe Creative Cloud Libraries] -Module zu verwenden, müssen Sie über ein [!UICONTROL Adobe Creative Cloud] -Konto verfügen.

## [!UICONTROL Adobe Creative Cloud-Bibliotheksmodule] und ihre Felder

Wenn Sie die Module [!UICONTROL Adobe Creative Cloud-Bibliotheken] konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Adobe Creative Cloud Libraries] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


* [Elemente](#elements)

* [Bibliotheken](#libraries)

* [Sonstige](#other)


### Elemente

* [[!UICONTROL Ein Element archivieren]](#archive-an-element)

* [[!UICONTROL Element abrufen]](#get-an-element)

* [[!UICONTROL Listenelemente]](#list-elements)

* [[!UICONTROL Hochladen eines Elements]](#upload-an-element)

* [!UICONTROL [Neues Element in Bibliothek ansehen]](#watch-new-element-in-library)

* [[!UICONTROL Aktualisierte Elemente ansehen]](#watch-updated-elements)


#### [!UICONTROL Ein Element archivieren]

Dieses Aktionsmodul archiviert ein Element aus einer Bibliothek.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Wählen Sie eine bestehende Creative Cloud Libraries-Verbindung aus. Die Erstellung von Verbindungen ist derzeit nicht im Creative Cloud Libraries-Connector verfügbar. Bestehende Verbindungen funktionieren erwartungsgemäß.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Bibliotheks-ID]</td>
      <td >Wählen Sie die Bibliothek aus, die das Element enthält, das Sie archivieren möchten.</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL Element ID]</td>
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
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Wählen Sie eine bestehende Creative Cloud Libraries-Verbindung aus. Die Erstellung von Verbindungen ist derzeit nicht im Creative Cloud Libraries-Connector verfügbar. Bestehende Verbindungen funktionieren erwartungsgemäß.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Bibliotheks-ID]</td>
      <td >Wählen Sie die Bibliothek aus, die das Element enthält, das Sie abrufen möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Element ID]</td>
      <td>Geben Sie die ID des Elements ein oder ordnen Sie sie zu.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selector]</td>
      <td>
        <p>Wählen Sie den Informationstyp aus, den das Modul zurückgibt. </p>
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
            <p><b>[!UICONTROL Darstellungen]</b>
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
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Wählen Sie eine bestehende Creative Cloud Libraries-Verbindung aus. Die Erstellung von Verbindungen ist derzeit nicht im Creative Cloud Libraries-Connector verfügbar. Bestehende Verbindungen funktionieren erwartungsgemäß.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Bibliotheks-ID]</td>
      <td >Wählen Sie die Bibliothek aus, aus der Sie Elemente auflisten möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Reihenfolge nach]</td>
      <td>Wählen Sie aus, ob die Ergebnisse nach Namen oder nach dem letzten Änderungsdatum des Elements sortiert werden sollen.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Typ]</td>
      <td >Geben Sie einen MIME-Typ ein, um die Ergebnisse auf die mit dem angegebenen MIME-Typ identifizierten Elemente zu beschränken. Beispiel: <code>string</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selector]</td>
      <td>
        <p>Wählen Sie den Informationstyp aus, den das Modul zurückgibt. </p>
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
            <p><b>[!UICONTROL Darstellungen]</b>
            </p>
            <p>Eine reduzierte Liste von Assets, die mit dem Bibliothekselement verknüpft sind</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Hochladen eines Elements]

Dieses Aktionsmodul lädt ein kleines Datei-Asset in eine vorhandene Bibliothek hoch. Die maximale Dateigröße beträgt 1 GB.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Wählen Sie eine bestehende Creative Cloud Libraries-Verbindung aus. Die Erstellung von Verbindungen ist derzeit nicht im Creative Cloud Libraries-Connector verfügbar. Bestehende Verbindungen funktionieren erwartungsgemäß.</td>
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
            <p>Der API-Aufruf wird synchron verarbeitet. Die Antwort wird nach Abschluss der Verarbeitung bereitgestellt (es sei denn, der Aufruf erfolgt mit einer Zeitüberschreitung.)</p>
          </li>
          <li>
            <p><b>[!UICONTROL async]</b>
            </p>
            <p>Die asynchrone Monitorantwort wird sofort zurückgegeben und die Anforderungsverarbeitung erfolgt asynchron. Der Aufruf ist für die Abfrage des Endpunkts bis zum Abschluss verantwortlich.</p>
          </li>
          <li>
            <p><b>[!UICONTROL sync,async]</b> (Standard)</p>
            <p>Die synchrone Verarbeitung der Anfrage wird versucht. Wenn die Verarbeitung 5.000 ms überschreitet, wird die Antwort des asynchronen Monitors zurückgegeben. Die Überwachungs-URL sollte abgerufen werden, bis die Anfrage abgeschlossen ist.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type File]</td>
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
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Wählen Sie eine bestehende Creative Cloud Libraries-Verbindung aus. Die Erstellung von Verbindungen ist derzeit nicht im Creative Cloud Libraries-Connector verfügbar. Bestehende Verbindungen funktionieren erwartungsgemäß.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Bibliotheks-ID]</td>
      <td >Wählen Sie die Bibliothek aus, die Sie auf aktualisierte Elemente achten möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td>
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
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Wählen Sie eine bestehende Creative Cloud Libraries-Verbindung aus. Die Erstellung von Verbindungen ist derzeit nicht im Creative Cloud Libraries-Connector verfügbar. Bestehende Verbindungen funktionieren erwartungsgemäß.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Bibliotheks-ID]</td>
      <td >Wählen Sie die Bibliothek aus, die Sie auf neue Elemente achten möchten.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td>
    </tr>
  </tbody>
</table>

### Bibliotheken

* [[!UICONTROL Neue Bibliotheken ansehen]](#watch-new-libraries)

* [[!UICONTROL Aktualisierte Bibliotheken ansehen]](#watch-updated-libraries)


#### [!UICONTROL Neue Bibliotheken ansehen]

Dieses Trigger-Modul startet ein Szenario, wenn eine neue Bibliothek erstellt wird.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Wählen Sie eine bestehende Creative Cloud Libraries-Verbindung aus. Die Erstellung von Verbindungen ist derzeit nicht im Creative Cloud Libraries-Connector verfügbar. Bestehende Verbindungen funktionieren erwartungsgemäß.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL Aktualisierte Bibliotheken ansehen]

Dieses Trigger-Modul startet ein Szenario, wenn eine bestehende Bibliothek aktualisiert wird.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Wählen Sie eine bestehende Creative Cloud Libraries-Verbindung aus. Die Erstellung von Verbindungen ist derzeit nicht im Creative Cloud Libraries-Connector verfügbar. Bestehende Verbindungen funktionieren erwartungsgemäß.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td>
    </tr>
  </tbody>
</table>

### Sonstige

#### [!UICONTROL API-Aufruf durchführen]

Dieses Modul führt einen benutzerdefinierten API-Aufruf an die [!DNL Adobe Creative Cloud Libraries] -API durch.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td> <p>Anweisungen zum Verbinden Ihres Adobe Creative Cloud-Kontos mit Workfront Fusion finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe Workfront Fusion - Grundlegende Anweisungen</a>.</p>
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
      <td role="rowheader">[!UICONTROL Methode]</td>
      <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Header]</td>
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
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
       <tr>
      <td role="rowheader">[!UICONTROL Hochladen eines Verlaufsdokuments]</td>
      <td>
      <p>Wenn Sie ein Verlaufsdokument hochladen möchten, geben Sie die Quelldatei für das Dokument ein, das Sie hochladen möchten.</p>
      <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p>
    </td>
    </tr>

</tbody>
</table>
