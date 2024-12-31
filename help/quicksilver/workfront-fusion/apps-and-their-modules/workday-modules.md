---
filename: workday-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: Workday-Module
description: In einem Adobe Workfront Fusion-Szenario können Sie Workflows automatisieren, die verwenden [!DNL Workday] und sie mit mehreren Anwendungen und Services von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 535573e0-b6ad-43a2-b7cb-ed32d1dc8d16
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1030'
ht-degree: 1%

---

# [!DNL Workday]

In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die [!DNL Workday] verwenden, und sie mit mehreren Anwendungen und Services von Drittanbietern verbinden.

Anweisungen zum Erstellen eines Szenarios finden Sie unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## Voraussetzungen

Um die [!DNL Workday]-Module zu verwenden, müssen Sie:

* Ein [!DNL Workday] Konto haben.

* Erstellen Sie eine OAuth-Anwendung in [!DNL Workday]. Anweisungen hierzu finden Sie in der [!DNL Workday].

## Workday-API-Informationen

Der Workday-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td>https://&#123;&#123;connection.servicesUrl&#125;&#125;/api</td> 
  </tr>
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.6.4</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Workday] mit [!DNL Workfront Fusion] verbinden

1. Klicken Sie in einem [!DNL Workfront Fusion] Modul [!UICONTROL Hinzufügen] neben dem Feld [!UICONTROL Verbindung]

2. Füllen Sie die folgenden Felder aus:

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Verbindungsname]</p>
                </td>
                <td>Einen Namen für die Verbindung eingeben</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Workday-Host]</td>
                <td>Geben Sie die Adresse Ihres [!DNL Workday]-Hosts ohne <code>https://</code> ein. Beispiel: <code>mycompany.workday.com</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Services URL]</td>
                <td>Geben Sie die Adresse Ihrer [!DNL Workday] Webservices ohne <code>https://</code> ein. Beispiel: <code>mycompany-services.workday.com</code>.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Mandantenname]</td>
                <td>Geben Sie den Mandanten für dieses [!DNL Workday] ein. Ihr Mandant ist die Kennung Ihres Unternehmens und ist in der URL zu sehen, mit der Sie sich bei Workday anmelden. Beispiel: Im <code>https://www.myworkday.com/mycompany</code> Adresse wird der Mandant <code>mycompany</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Client-ID]</td>
                <td>Geben Sie die Client-ID für die [!DNL Workday] ein, die diese Verbindung verwendet. Dies erhalten Sie, wenn Sie das Programm in [!DNL Workday] erstellen.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Client-Geheimnis]</td>
                <td>Geben Sie das Client-Geheimnis für die [!DNL Workday]-Anwendung ein, die diese Verbindung verwendet. Dies erhalten Sie, wenn Sie das Programm in [!DNL Workday] erstellen.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Sitzungs-Timeout (Min.)]</td>
                <td >Geben Sie die Anzahl der Minuten ein, nach denen Ihr Autorisierungs-Token abläuft.</td>
            </tr>
        </tbody>
    </table>


3. Klicken Sie [!UICONTROL Fortfahren], um die Verbindung zu speichern und zum Modul zurückzukehren

## [!DNL Workday] Module und ihre Felder

Beim Konfigurieren [!DNL Workday] Module zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service weitere [!DNL Workday] angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Aktion](#action)

* [Suchen](#search)


### Aktion

* [[!UICONTROL Datensatz erstellen]](#create-a-record)

* [[!UICONTROL Löschen eines Datensatzes]](#delete-a-record)

* [[!UICONTROL Erstellen eines benutzerdefinierten API-Aufrufs]](#make-a-custom-api-call)

* [[!UICONTROL Aktualisieren eines Datensatzes]](#update-a-record)


#### [!UICONTROL Datensatz erstellen]

Dieses Aktionsmodul erstellt einen einzelnen Datensatz in [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL-Verbindung]</td>
            <td>Anweisungen zum Verbinden Ihres [!DNL Workday]-Kontos mit Workfront Fusion finden Sie unter <a href="#Connect" class="MCXref xre[!DNL ]f" >Verbinden von [!DNL Workday] mit [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Datensatztyp]</td>
            <td>Wählen Sie den Typ des Datensatzes aus, den Sie erstellen möchten.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>Geben Sie die ID des Datensatzes ein, den Sie erstellen möchten, oder ordnen Sie sie zu.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Unterressourcen-ID]</td>
            <td >Geben Sie die ID der Unterressource ein, die Sie erstellen möchten, oder mappen Sie sie.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL Löschen eines Datensatzes]

Dieses Aktionsmodul löscht einen einzelnen Datensatz in [!DNL Workday].

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL-Verbindung]</td>
            <td>Anweisungen zum Verbinden Ihres [!DNL Workday]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#Connect" class="MCXref xre[!DNL ]f" >Verbinden von [!DNL Workday] mit [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Datensatztyp]</td>
            <td>Wählen Sie den Typ des Datensatzes aus, den Sie löschen möchten.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Spezifischer Datensatztyp]</td>
            <td>Wählen Sie den spezifischen Typ des Datensatzes aus, den Sie löschen möchten. Diese basieren auf dem von Ihnen ausgewählten Datensatztyp.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Unterressourcen-ID]</td>
            <td>Geben Sie die ID der Teilressource ein, die Sie löschen möchten, oder mappen Sie sie.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >Geben Sie die ID des Datensatzes ein, den Sie löschen möchten, oder mappen Sie sie.</td>
        </tr>
    </tbody>
</table>


### [!UICONTROL Erstellen eines benutzerdefinierten API-Aufrufs]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Workday]-API durchführen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von den anderen [!DNL Workday] nicht durchgeführt werden kann.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

Das Modul gibt den Status-Code zusammen mit den Kopfzeilen und dem Hauptteil des API-Aufrufs zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Connection]</p> </td> 
            <td>Anweisungen zum Verbinden Ihres [!DNL Workday]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#Connect" class="MCXref xre[!DNL ]f" >Verbinden von [!DNL Workday] mit [!DNL Workfront Fusion]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Geben Sie einen Pfad relativ zu <code style="color: #ff1493;">https://&lt;tenantHostname>/api/&lt;serviceName>/&lt;version>/&lt;tenant></code> ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Methode]</td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-Anfragemethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Kopfzeilen]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL body]</td> 
   <td> <p>Fügen Sie den Hauptteil des Inhalts für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Wenn Sie bedingte Anweisungen wie <code>if</code> in Ihrer JSON-Datei verwenden, setzen Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aktualisieren eines Datensatzes]

Dieses Aktionsmodul aktualisiert einen einzelnen Datensatz in [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL-Verbindung]</td>
            <td>Anweisungen zum Verbinden Ihres [!DNL Workday]-Kontos mit Workfront Fusion finden Sie unter <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] to Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">Datensatztyp</td>
            <td>Wählen Sie den Typ des Datensatzes aus, den Sie aktualisieren möchten[!UICONTROL ].</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>Geben Sie die ID des Datensatzes ein, den Sie aktualisieren möchten, oder mappen Sie sie.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Unterressourcen-ID]</td>
            <td >Geben Sie die ID der Unterressource ein, die Sie aktualisieren möchten, oder mappen Sie sie.</td>
        </tr>
    </tbody>
</table>

### Suchen

* [[!UICONTROL Datensatz lesen]](#read-a-record)

* [[!UICONTROL Einträge auflisten]](#list-records)


#### [!UICONTROL Datensatz lesen]

Dieses Aktionsmodul liest einen einzelnen Datensatz.

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL-Verbindung]</td>
            <td>Anweisungen zum Verbinden Ihres [!DNL Workday]-Kontos mit Workfront Fusion finden Sie unter <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] to Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Datensatztyp]</td>
            <td>Wählen Sie den Typ des Datensatzes aus, den Sie löschen möchten.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Spezifischer Datensatztyp]</td>
            <td>Wählen Sie den Datensatztyp aus, den Sie lesen möchten. Diese basieren auf dem von Ihnen ausgewählten Datensatztyp.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >Geben Sie die ID des Datensatzes ein, den Sie löschen möchten, oder mappen Sie sie.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL Einträge auflisten]

Dieses Suchmodul ruft eine Liste von Datensätzen des angegebenen Typs ab.

<table style="table-layout:auto"> 
      <col/>
      <col/>
      <tbody>
          <tr>
              <td role="rowheader">[!UICONTROL-Verbindung]</td>
              <td>Anweisungen zum Verbinden Ihres [!DNL Workday]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#Connect" class="MCXref xref" >Verbinden von [!DNL Workday] mit [!DNL Workfront Fusion]</a></td>
          </tr>
          <tr>
              <td  role="rowheader">[!UICONTROL Datensatztyp]</td>
              <td>Wählen Sie den Typ des Datensatzes aus, den Sie abrufen möchten.</td>
          </tr>
          <tr>
              <td role="rowheader">[!UICONTROL Limit]</td>
              <td >
                  <p>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus abrufen soll, oder mappen Sie sie.</p>
              </td>
          </tr>
      </tbody>
  </table>
