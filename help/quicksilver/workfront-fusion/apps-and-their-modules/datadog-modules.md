---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connector
navigation-topic: apps-and-their-modules
title: Datadog-Module
description: In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die Datadog verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: a0b4352d-a1ce-4459-a58e-71de860b8a90
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 1%

---

# [!DNL Datadog]-Module

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Datadog], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Verwendung [!DNL Datadog] -Module, müssen Sie über eine [!DNL Datadog] -Konto.

## Verbinden [!DNL Datadog] nach [!DNL Workfront Fusion] {#connect-datadog-to-workfront-fusion}

### API-Schlüssel und Anwendungsschlüssel abrufen {#retrieve-your-api-key-and-application-key}

Um eine Verbindung herzustellen [!DNL Datadog] Konto [!DNL Workfront Fusion] Sie müssen einen API-Schlüssel und einen Anwendungsschlüssel von Ihrem [!DNL Datadog] -Konto.

1. Melden Sie sich bei Ihrer [!DNL Datadog] -Konto.
1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL Integrationen]** Klicken Sie auf **[!UICONTROL APIs]**.
1. Klicken Sie im Hauptbildschirm auf **[!UICONTROL API-Schlüssel]**.
1. Bewegen Sie den Mauszeiger über die lilafarbene Leiste, um den API-Schlüssel anzuzeigen.
1. Kopieren Sie den API-Schlüssel an einen sicheren Speicherort.
1. Klicken Sie im Hauptbildschirm auf **[!UICONTROL Anwendungsschlüssel]**.
1. Bewegen Sie den Mauszeiger über die lilafarbene Leiste, um den Anwendungsschlüssel anzuzeigen.
1. Kopieren Sie den Anwendungsschlüssel an einen sicheren Speicherort.

### Erstellen Sie eine Verbindung zu [!DNL Datadog] in [!DNL Workfront Fusion]

Sie können eine Verbindung zu Ihrem [!DNL Datadog] direkt in einer [!UICONTROL Datadog] -Modul.

1. In jeder [!UICONTROL Datadog] Modul, klicken Sie auf **[!UICONTROL Hinzufügen]** neben dem [!UICONTROL Verbindung] -Feld.
1. Füllen Sie die Felder des Moduls wie folgt aus:

<table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Verbindungstyp]</td> 
      <td> <p> [!UICONTROL auswählen [!DNL Datadog] Application]-Option, um vollen Zugriff auf [!DNL Datadog] API.</p> </td> 
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
      <td> <p> Geben Sie Ihre [!DNL Datadog] API-Schlüssel. </p> <p>Anweisungen zum Abrufen des API-Schlüssels finden Sie unter <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">API-Schlüssel und Anwendungsschlüssel abrufen</a> in diesem Artikel.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Anwendungsschlüssel]</td> 
      <td> <p> Geben Sie Ihre [!DNL Datadog] Anwendungsschlüssel. </p> <p>Anweisungen zum Abrufen des Anwendungsschlüssels finden Sie unter <a href="#retrieve-your-api-key-and-application-key" class="MCXref xref">API-Schlüssel und Anwendungsschlüssel abrufen</a> in diesem Artikel.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

## [!DNL Datadog] Module und ihre Felder

Bei der Konfiguration [!DNL Datadog] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Datadog] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Aktionen

* [[!UICONTROL POST-Zeitpunkte]](#post-timeseries-points)
* [[!UICONTROL API-Aufruf durchführen]](#make-an-api-call)

#### [!UICONTROL POST-Zeitpunkte]

Mit dem -Modul können Sie Zeitreihendaten posten, auf denen Diagramme erstellt werden können [!DNL Datadog]Dashboards.

Der Grenzwert für komprimierte Payloads beträgt 3,2 Megabytes (3200000) und 62 Megabytes (62914560) für dekomprimierte Payloads.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Datadog] Konto [!DNL Workfront Fusion], siehe <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Datadog] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Serie]</td> 
   <td> <p>Zeitreihen hinzufügen, an die Sie senden möchten [!DNL Datadog].</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Metrik]</strong> </p> <p>Geben Sie den Namen der Zeitreihen ein.</p> </li> 
     <li> <p><strong>[!UICONTROL Typ]</strong> </p> <p>Wählen Sie den Typ der Metrik aus.</p> </li> 
     <li> <p><strong>[!UICONTROL Interval]</strong> </p> <p> Wenn der Typ der Metrik Rate oder Zählung ist, definieren Sie das entsprechende Intervall.</p> </li> 
     <li> <p><strong>[!UICONTROL Points]</strong> </p> <p>Fügen Sie Punkte hinzu, die sich auf eine Metrik beziehen.</p> <p>Dies ist ein JSON-Array von Punkten. Jeder Punkt hat das Format: <code>[[POSIX_timestamp, numeric_value], ...] </code></p> <p>Notiz:  <p>Der Zeitstempel muss in Sekunden angegeben werden.</p> <p>Der Zeitstempel muss aktuell sein. Aktuell ist definiert als nicht mehr als 10 Minuten in der Zukunft oder mehr als 1 Stunde in der Vergangenheit.</p> <p> Das numerische Wertformat sollte ein Gleitkommawert sein.</p> </p> <p>Dieses Feld muss mindestens 1 Element enthalten.</p> </li> 
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
   <td> <p>Anweisungen zum Verbinden der [!DNL Datadog] Konto [!DNL Workfront Fusion], siehe <a href="#connect-datadog-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Datadog] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Geben Sie einen Pfad relativ zu ein <code>https://api.datadoghq.com/api/</code>. Beispiel:<code> /v1/org</code>.</td> 
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
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Notiz:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Beispiel:** Der folgende API-Aufruf gibt alle Dashboards in Ihrer [!DNL Datadog] Konto:

URL: `/v1/dashboard`

Methode: `GET`

![](assets/datadog-api-example.png)

Das Ergebnis finden Sie in der Ausgabe des Moduls unter Bundle > Hauptteil > Dashboards.

In unserem Beispiel wurden drei Dashboards zurückgegeben:

![](assets/datadog-api-response-example.png)
