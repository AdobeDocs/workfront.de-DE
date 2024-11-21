---
filename: workday-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Workday-Module
description: In einem Adobe Workfront Fusion-Szenario können Sie Workflows automatisieren, die [!DNL Workday] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 535573e0-b6ad-43a2-b7cb-ed32d1dc8d16
source-git-commit: 27fb07b7b19bab25bb7ee925e722ccace3bea628
workflow-type: tm+mt
source-wordcount: '1030'
ht-degree: 1%

---

# [!DNL Workday] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Workday] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## Voraussetzungen

Um die [!DNL Workday] -Module zu verwenden, müssen Sie:

* Verwenden Sie ein [!DNL Workday] -Konto.

* Erstellen Sie eine OAuth-Anwendung in [!DNL Workday]. Anweisungen finden Sie in der Dokumentation zu [!DNL Workday] .

## Workday-API-Informationen

Der Workday-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td>https://{connection.servicesUrl}/api</td> 
  </tr>
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.6.4</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Workday] mit [!DNL Workfront Fusion] verbinden

1. Klicken Sie in einem beliebigen [!DNL Workfront Fusion]-Modul neben dem Feld [!UICONTROL Verbindung] auf [!UICONTROL Hinzufügen] .

2. Füllen Sie die folgenden Felder aus:

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Verbindungsname]</p>
                </td>
                <td>Geben Sie einen Namen für die Verbindung ein</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Workday Host]</td>
                <td>Geben Sie die Adresse Ihres [!DNL Workday]-Hosts ohne <code>https://</code> ein. Beispiel: <code>mycompany.workday.com</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Services URL]</td>
                <td>Geben Sie die Adresse Ihrer [!DNL Workday] Webdienste ohne <code>https://</code> ein. Beispiel: <code>mycompany-services.workday.com</code>.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Mandantenname]</td>
                <td>Geben Sie den Mandanten für dieses [!DNL Workday]-Konto ein. Ihr Mandant ist die Kennung Ihres Unternehmens und kann in der URL angezeigt werden, die Sie zum Anmelden bei Workday verwenden. Beispiel: In der Adresse <code>https://www.myworkday.com/mycompany</code> ist der Mandant <code>mycompany</code>.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Client-ID]</td>
                <td>Geben Sie die Client-ID für die [!DNL Workday] -Anwendung ein, die diese Verbindung verwendet. Sie erhalten dies beim Erstellen der Anwendung in [!DNL Workday].</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Client Secret]</td>
                <td>Geben Sie das Client-Geheimnis für die [!DNL Workday]-Anwendung ein, die diese Verbindung verwendet. Sie erhalten dies beim Erstellen der Anwendung in [!DNL Workday].</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Sitzungs-Timeout (min)]</td>
                <td >Geben Sie die Anzahl der Minuten ein, nach denen Ihr Autorisierungstoken abläuft.</td>
            </tr>
        </tbody>
    </table>


3. Klicken Sie auf [!UICONTROL Weiter] , um die Verbindung zu speichern und zum Modul zurückzukehren.

## [!DNL Workday] Module und ihre Felder

Wenn Sie [!DNL Workday] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Workday] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Aktion](#action)

* [Suchen](#search)


### Aktion

* [[!UICONTROL Erstellen eines Datensatzes]](#create-a-record)

* [[!UICONTROL Datensatz löschen]](#delete-a-record)

* [[!UICONTROL Erstellen eines benutzerdefinierten API-Aufrufs]](#make-a-custom-api-call)

* [[!UICONTROL Datensatz aktualisieren]](#update-a-record)


#### [!UICONTROL Erstellen eines Datensatzes]

Dieses Aktionsmodul erstellt einen einzelnen Datensatz in [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Verbindung]</td>
            <td>Anweisungen zum Verbinden Ihres [!DNL Workday]-Kontos mit Workfront Fusion finden Sie unter <a href="#Connect" class="MCXref xre[!DNL ]f" >Verbinden [!DNL Workday] mit [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Record Type]</td>
            <td>Wählen Sie den Typ des Datensatzes aus, den Sie erstellen möchten.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>Geben Sie die Kennung des Datensatzes ein oder ordnen Sie ihn zu.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Subresource ID]</td>
            <td >Geben Sie die Kennung der zu erstellenden Unterressource ein oder ordnen Sie sie zu.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL Datensatz löschen]

Dieses Aktionsmodul löscht einen einzelnen Datensatz in [!DNL Workday].

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Verbindung]</td>
            <td>Anweisungen zum Verbinden Ihres [!DNL Workday]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#Connect" class="MCXref xre[!DNL ]f" >Verbinden [!DNL Workday] mit [!DNL Workfront Fusion]</a>.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Record Type]</td>
            <td>Wählen Sie den Typ des Datensatzes aus, den Sie löschen möchten.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Spezifischer Datensatztyp]</td>
            <td>Wählen Sie den spezifischen Datensatztyp aus, den Sie löschen möchten. Diese basieren auf dem gewählten Datensatztyp.</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Subresource ID]</td>
            <td>Geben Sie die Kennung der zu löschenden Unterressource ein oder ordnen Sie sie zu.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >Geben Sie die Kennung des Datensatzes ein, den Sie löschen möchten, oder ordnen Sie sie zu.</td>
        </tr>
    </tbody>
</table>


### [!UICONTROL Erstellen eines benutzerdefinierten API-Aufrufs]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Workday] -API durchführen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von anderen [!DNL Workday] -Modulen nicht ausgeführt werden kann.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

Das Modul gibt den Status-Code zusammen mit den Kopfzeilen und dem Text des API-Aufrufs zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Connection]</p> </td> 
            <td>Anweisungen zum Verbinden Ihres [!DNL Workday]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#Connect" class="MCXref xre[!DNL ]f" >Verbinden [!DNL Workday] mit [!DNL Workfront Fusion]</a>.</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Geben Sie einen Pfad relativ zu <code style="color: #ff1493;">https://&lt;tenantHostname>/api/&lt;serviceName>/&lt;version>/&lt;tenant></code> ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode]</td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"name":"something-urgent"}</code></p> </td> 
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

#### [!UICONTROL Datensatz aktualisieren]

Dieses Aktionsmodul aktualisiert einen einzelnen Datensatz in [!DNL Workday].

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Verbindung]</td>
            <td>Anweisungen zum Verbinden Ihres [!DNL Workday]-Kontos mit Workfront Fusion finden Sie unter <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] mit Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">Datensatztyp</td>
            <td>Wählen Sie den zu aktualisierenden Datensatztyp t[!UICONTROL ] aus.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>Geben Sie die Kennung des Datensatzes ein, den Sie aktualisieren möchten, oder ordnen Sie sie zu.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Subresource ID]</td>
            <td >Geben Sie die Kennung der zu aktualisierenden Unterressource ein oder ordnen Sie sie zu.</td>
        </tr>
    </tbody>
</table>

### Suchen

* [[!UICONTROL Datensatz lesen]](#read-a-record)

* [[!UICONTROL Listeneinträge]](#list-records)


#### [!UICONTROL Datensatz lesen]

Dieses Aktionsmodul liest einen einzelnen Datensatz.

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Verbindung]</td>
            <td>Anweisungen zum Verbinden Ihres [!DNL Workday]-Kontos mit Workfront Fusion finden Sie unter <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] mit Workfront Fusion]</a></td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Record Type]</td>
            <td>Wählen Sie den Typ des Datensatzes aus, den Sie löschen möchten.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Spezifischer Datensatztyp]</td>
            <td>Wählen Sie den gewünschten Datensatztyp aus. Diese basieren auf dem gewählten Datensatztyp.</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >Geben Sie die Kennung des Datensatzes ein, den Sie löschen möchten, oder ordnen Sie sie zu.</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL Listeneinträge]

Dieses Suchmodul ruft eine Liste von Datensätzen des angegebenen Typs ab.

<table style="table-layout:auto"> 
      <col/>
      <col/>
      <tbody>
          <tr>
              <td role="rowheader">[!UICONTROL Verbindung]</td>
              <td>Anweisungen zum Verbinden Ihres [!DNL Workday]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#Connect" class="MCXref xref" >Verbinden [!DNL Workday] mit [!DNL Workfront Fusion]</a></td>
          </tr>
          <tr>
              <td  role="rowheader">[!UICONTROL Record Type]</td>
              <td>Wählen Sie den Typ des Datensatzes aus, den Sie abrufen möchten.</td>
          </tr>
          <tr>
              <td role="rowheader">[!UICONTROL Limit]</td>
              <td >
                  <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen des Szenarios abrufen soll.</p>
              </td>
          </tr>
      </tbody>
  </table>
