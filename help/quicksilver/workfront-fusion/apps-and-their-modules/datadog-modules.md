---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connector
navigation-topic: apps-and-their-modules
title: Datenmodulen
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die Datadog verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: a0b4352d-a1ce-4459-a58e-71de860b8a90
source-git-commit: 27fb07b7b19bab25bb7ee925e722ccace3bea628
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 1%

---

# [!DNL Datadog] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Datadog] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

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

Um [!DNL Datadog] -Module zu verwenden, müssen Sie über ein [!DNL Datadog] -Konto verfügen.

## Daten-API-Informationen

Der Datadog-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>1,0,11</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Datadog] mit [!DNL Workfront Fusion] verbinden {#connect-datadog-to-workfront-fusion}

### API-Schlüssel und Anwendungsschlüssel abrufen {#retrieve-your-api-key-and-application-key}

Um Ihr [!DNL Datadog]-Konto mit [!DNL Workfront Fusion] zu verbinden, müssen Sie einen API-Schlüssel und einen Anwendungsschlüssel aus Ihrem [!DNL Datadog]-Konto abrufen.

1. Melden Sie sich bei Ihrem [!DNL Datadog] -Konto an.
1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL Integrationen]** und dann auf **[!UICONTROL APIs]**.
1. Klicken Sie im Hauptbildschirm auf **[!UICONTROL API-Schlüssel]**.
1. Bewegen Sie den Mauszeiger über die lilafarbene Leiste, um den API-Schlüssel anzuzeigen.
1. Kopieren Sie den API-Schlüssel an einen sicheren Speicherort.
1. Klicken Sie im Hauptbildschirm auf **[!UICONTROL Anwendungsschlüssel]**.
1. Bewegen Sie den Mauszeiger über die lilafarbene Leiste, um den Anwendungsschlüssel anzuzeigen.
1. Kopieren Sie den Anwendungsschlüssel an einen sicheren Speicherort.

### Erstellen einer Verbindung zu [!DNL Datadog] in [!DNL Workfront Fusion]

Sie können eine Verbindung zu Ihrem [!DNL Datadog]-Konto direkt in einem [!UICONTROL Datadog] -Modul erstellen.

1. Klicken Sie in einem beliebigen [!UICONTROL Datadog]-Modul neben dem Feld [!UICONTROL Verbindung] auf **[!UICONTROL Hinzufügen]** .
1. Füllen Sie die Felder des Moduls wie folgt aus:

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Verbindungstyp]</td> 
      <td> <p> Wählen Sie die Option [!UICONTROL [!DNL Datadog] Application] aus, um vollen Zugriff auf die [!DNL Datadog] -API zu erhalten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Verbindungsname]</td> 
      <td> <p> Geben Sie einen Namen für die Verbindung ein.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Domain] </td> 
      <td> <p>Wählen Sie die Domäne aus, mit der Sie eine Verbindung herstellen möchten (USA oder EU).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API-Schlüssel]</td> 
      <td> <p> Geben Sie Ihren [!DNL Datadog] API-Schlüssel ein. </p> <p>Anweisungen zum Abrufen des API-Schlüssels finden Sie unter <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">Abrufen des API-Schlüssels und des Anwendungsschlüssels</a> in diesem Artikel.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Anwendungsschlüssel]</td> 
      <td> <p> Geben Sie Ihren [!DNL Datadog] Anwendungsschlüssel ein. </p> <p>Anweisungen zum Abrufen des Anwendungsschlüssels finden Sie unter <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">Abrufen des API-Schlüssels und des Anwendungsschlüssels</a> in diesem Artikel.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

## [!DNL Datadog] Module und ihre Felder

Wenn Sie [!DNL Datadog] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Datadog] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Aktionen

* [[!UICONTROL POST-Timeseries-Punkte]](#post-timeseries-points)
* [[!UICONTROL API-Aufruf durchführen]](#make-an-api-call)

#### [!UICONTROL POST-Timeseries-Punkte]

Mit dem -Modul können Sie Zeitreihendaten posten, die auf den Dashboards von [!DNL Datadog] dargestellt werden können.

Der Grenzwert für komprimierte Payloads beträgt 3,2 Megabytes (3200000) und 62 Megabytes (62914560) für dekomprimierte Payloads.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Datadog]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Datadog] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Serie]</td> 
   <td> <p>Fügen Sie Zeitreihen hinzu, die Sie an [!DNL Datadog] senden möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Metrik]</strong> </p> <p>Geben Sie den Namen der Zeitreihen ein.</p> </li> 
     <li> <p><strong>[!UICONTROL Type]</strong> </p> <p>Wählen Sie den Typ der Metrik aus.</p> </li> 
     <li> <p><strong>[!UICONTROL Interval]</strong> </p> <p> Wenn der Typ der Metrik Rate oder Zählung ist, definieren Sie das entsprechende Intervall.</p> </li> 
     <li> <p><strong>[!UICONTROL Points]</strong> </p> <p>Fügen Sie Punkte hinzu, die sich auf eine Metrik beziehen.</p> <p>Dies ist ein JSON-Array von Punkten. Jeder Punkt hat das Format: <code>[[POSIX_timestamp, numeric_value], ...] </code></p> <p>Hinweis:  <p>Der Zeitstempel muss in Sekunden angegeben werden.</p> <p>Der Zeitstempel muss aktuell sein. Aktuell ist definiert als nicht mehr als 10 Minuten in der Zukunft oder mehr als 1 Stunde in der Vergangenheit.</p> <p> Das numerische Wertformat sollte ein Gleitkommawert sein.</p> </p> <p>Dieses Feld muss mindestens 1 Element enthalten.</p> </li> 
     <li> <p><strong>[!UICONTROL Host]</strong> </p> <p>Geben Sie den Namen des Hosts ein, der die Metrik erzeugt hat.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL API-Aufruf durchführen]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten API-Aufruf ausführen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Datadog]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Datadog] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Geben Sie einen Pfad relativ zu <code>https://api.datadoghq.com/api/</code> ein. Beispiel:<code> /v1/org</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode]</td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
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

**Beispiel:** Der folgende API-Aufruf gibt alle Dashboards in Ihrem [!DNL Datadog] -Konto zurück:

URL: `/v1/dashboard`

Methode: `GET`

![](assets/datadog-api-example.png)

Das Ergebnis finden Sie in der Ausgabe des Moduls unter Bundle > Hauptteil > Dashboards.

In unserem Beispiel wurden drei Dashboards zurückgegeben:

![](assets/datadog-api-response-example.png)
