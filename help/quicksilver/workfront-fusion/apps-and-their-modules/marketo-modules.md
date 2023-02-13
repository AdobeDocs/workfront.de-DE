---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Marketo-Module
description: In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Marketo], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.
author: Becky
feature: Workfront Fusion
exl-id: 7f6dace5-ab50-45da-a926-1a8919057f7b
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2014'
ht-degree: 0%

---

# [!DNL Marketo]-Module

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Marketo], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.

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

Verwendung [!DNL Marketo] -Module, müssen Sie über eine [!DNL Marketo] -Konto.

## Verbinden [!DNL Marketo] zu Workfront Fusion {#connect-marketo-to-workfront-fusion}

Sie können eine Verbindung zu Ihrem [!DNL Marketo] direkt von innen aus [!DNL Marketo] -Modul.

1. In jeder [!DNL Marketo] Modul, klicken Sie auf **[!UICONTROL Hinzufügen]** neben dem [!UICONTROL Verbindung] -Feld.
1. Geben Sie Ihre [!DNL Marketo] Konto oder [!DNL Marketo] [!UICONTROL Munchkin] Kennung. Dies ist der eindeutige Teil der Basis-URL oder des Endpunkts, der Ihrem Konto zugewiesen ist und über den Sie auf [!DNL Marketo] über [!UICONTROL REST] API. Anweisungen zum Auffinden finden Sie unter [Basis-URL](https://developers.marketo.com/rest-api/base-url/) im [!DNL Marketo] Dokumentation.
1. Geben Sie Ihre [!UICONTROL Client-ID] und [!UICONTROL Client-Geheimschlüssel]. Anweisungen zur Lokalisierung finden Sie unter [Authentifizierung](https://developers.marketo.com/rest-api/authentication/) im [!DNL Marketo] Dokumentation.
1. Klicken **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

## [!DNL Marketo] Module und ihre Felder

Bei der Konfiguration [!DNL Marketo] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Marketo] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Trigger

* [[!UICONTROL Aufnahmen ansehen]](#watch-records)
* [[!UICONTROL Ereignisse überwachen (Sofort)]](#watch-events-instant)

#### [!UICONTROL Aufnahmen ansehen]

Dieses Trigger-Modul startet ein Szenario, wenn ein Datensatz erstellt oder aktualisiert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Marketo] Konto [!DNL Workfront Fusion], siehe <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Marketo] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ des Datensatzes aus, den Sie erstellen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Aktivität]</strong> </p> <p>Wählen Sie den Aktivitätstyp aus, den Sie sehen möchten. </p> <p>Das Modul überwacht nur auf neue Aktivitäten.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Lead]</strong> </p> <p>Wählen Sie aus, ob Sie nach neuen, aktualisierten Datensätzen, neuen und aktualisierten Datensätzen oder spezifischen Feldaktualisierungen suchen möchten. Wenn Sie bestimmte Feldaktualisierungen anzeigen möchten, wählen Sie das Feld aus, das das Modul überwachen soll.</p> </li> 
     <li> <p><strong>[!UICONTROL Programm]</strong> </p> <p>Wählen Sie aus, ob Sie nach neuen, aktualisierten oder sowohl neuen als auch aktualisierten Datensätzen suchen möchten.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabebundle für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ereignisse überwachen (Sofort)]

Dieses Trigger-Modul startet ein Szenario, wenn ein Datensatz erstellt oder aktualisiert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Webhook]</p> </td> 
   <td> <p>Geben Sie den Webhook ein, den das Modul verwenden soll.</p> <p>Weitere Informationen zu Webhooks finden Sie unter <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Sofortige Trigger (Webhooks) in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL Benutzerspezifischer API-Aufruf]](#custom-api-call)
* [[!UICONTROL Datensatz erstellen]](#create-a-record)
* [[!UICONTROL Datensatz aktualisieren]](#update-a-record)
* [[!UICONTROL Datei herunterladen]](#download-a-file)
* [[!UICONTROL Datei hochladen]](#upload-a-file)
* [[!UICONTROL Datensatz lesen]](#read-a-record)
* [[!UICONTROL Leads zu einer Liste hinzufügen]](#add-leads-to-a-list)
* [[!UICONTROL Leads aus einer Liste entfernen]](#remove-leads-from-a-list)
* [[!UICONTROL Eine Kampagne planen]](#schedule-a-campaign)
* [[!UICONTROL Programm kopieren]](#copy-a-program)

#### [!UICONTROL Benutzerspezifischer API-Aufruf]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Marketo] API. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von der anderen nicht durchgeführt werden kann [!DNL Marketo] Module.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Marketo] Konto [!DNL Workfront Fusion], siehe <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Marketo] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Geben Sie einen Pfad relativ zu ein <code>https://{your-base-url}.mktorest.com/</code>.</td> 
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
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Notiz:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, mit denen das Modul während der verschiedenen Ausführungszyklen eines Szenarios arbeiten soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datensatz erstellen]

Dieses Aktionsmodul erstellt einen neuen Datensatz in [!DNL Marketo]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Marketo] Konto [!DNL Workfront Fusion], siehe <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Marketo] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ des Datensatzes aus, den Sie erstellen möchten.</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Ordner]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL Programm]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Felder zur Zuordnung auswählen]</td> 
   <td>Wenn Sie ein Unternehmen oder einen Lead erstellen, wählen Sie die Felder aus, für die Sie bei der Erstellung des neuen Datensatzes Werte festlegen möchten, und geben Sie dann Werte für diese Felder ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Programmtyp]</td> 
   <td>Wenn Sie ein Programm erstellen, wählen Sie den Typ des Programms aus, das Sie erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Programmkanal] </td> 
   <td>Wenn Sie ein Programm erstellen, wählen Sie den Programmkanal aus, in dem Sie das Programm erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner] / [!UICONTROL Programmname]</td> 
   <td>Wenn Sie einen Ordner oder ein Programm erstellen, geben Sie einen Namen für den neuen Datensatz ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beschreibung]</td> 
   <td> <p>Wenn Sie einen Ordner oder ein Programm erstellen, geben Sie eine Beschreibung für den neuen Datensatz ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parent Folder ID]</td> 
   <td>Wenn Sie einen Ordner oder ein Programm erstellen, geben Sie die ID des übergeordneten Ordners ein oder ordnen Sie sie zu, in dem Sie den neuen Datensatz erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kosten]</td> 
   <td>Wenn Sie ein Programm erstellen, fügen Sie Kosten hinzu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td>Wenn Sie ein Programm erstellen, fügen Sie beliebige Tags hinzu</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datensatz aktualisieren]

Dieses Aktionsmodul aktualisiert einen vorhandenen Datensatz mithilfe seiner ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Marketo] Konto [!DNL Workfront Fusion], siehe <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Marketo] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ des Datensatzes aus, den Sie erstellen möchten.</p> 
    <ul> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL Programm]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Company] / [!UICONTROL Lead] / [!UICONTROL Programm-ID]</td> 
   <td>Geben Sie die Kennung des Datensatzes ein, den Sie aktualisieren möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Felder zur Zuordnung auswählen]</td> 
   <td>Wenn Sie ein Unternehmen oder Lead aktualisieren, wählen Sie die Felder aus, für die Werte aktualisiert werden sollen, und geben Sie dann Werte für diese Felder ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Programmname]</td> 
   <td>Wenn Sie ein Programm aktualisieren, geben Sie einen neuen Namen für das Programm ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beschreibung]</td> 
   <td> <p>Wenn Sie ein Programm aktualisieren, geben Sie eine neue Beschreibung für das Programm ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Startdatum]</td> 
   <td>Wenn Sie ein Programm aktualisieren, geben Sie ein neues Startdatum für das Programm ein oder ordnen Sie es zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enddatum]</td> 
   <td>Wenn Sie ein Programm aktualisieren, geben Sie ein neues Enddatum für das Programm ein oder ordnen Sie es zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kosten]</td> 
   <td>Wenn Sie ein Programm aktualisieren, fügen Sie Kosten hinzu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td>Wenn Sie ein Programm aktualisieren, fügen Sie beliebige Tags hinzu</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei herunterladen]

Dieses Aktionsmodul lädt mithilfe der Datei-ID eine Datei herunter.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Marketo] Konto [!DNL Workfront Fusion], siehe <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Marketo] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datei-ID]</td> 
   <td>Ordnen Sie die ID der Datei zu, die Sie herunterladen möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei hochladen]

Dieses Aktionsmodul lädt eine neue Datei in [!UICONTROL Marketo].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Marketo] Konto [!DNL Workfront Fusion], siehe <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Marketo] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner-ID]</td> 
   <td>Geben Sie die Kennung des Ordners ein, in dem sich die neue Datei befinden soll, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beschreibung]</td> 
   <td>Geben Sie eine Beschreibung für die hochgeladene Datei ein.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datensatz lesen]

Dieses Aktionsmodul liest Informationen zu einem Datensatz mithilfe seiner ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Marketo] Konto [!DNL Workfront Fusion], siehe <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Marketo] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ des Datensatzes aus, den Sie erstellen möchten.</p> 
    <ul> 
     <li> <p>[!UICONTROL Campaign]</p> </li> 
     <li> <p>[!UICONTROL Company]</p> </li> 
     <li> <p>[!UICONTROL Lead]</p> </li> 
     <li> <p>[!UICONTROL Liste]</p> </li> 
     <li> <p>[!UICONTROL Programm]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td>Wählen Sie die Informationen aus, die im Ausgabebundle für dieses Modul enthalten sein sollen. Die Felder sind je nach ausgewähltem [!UICONTROL Record Type] verfügbar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL &lt;object&gt; ID]</td> 
   <td>Geben Sie die ID des Objekts ein, über das Sie Informationen abrufen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leads zu einer Liste hinzufügen]

Dieses Aktionsmodul fügt mithilfe der Lead-ID eine oder mehrere Leads zu einer Liste hinzu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Marketo] Konto [!DNL Workfront Fusion], siehe <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Marketo] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listen-ID]</td> 
   <td>Geben Sie die ID der Liste ein oder ordnen Sie sie zu, in der Sie Leads hinzufügen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lead-IDs]</td> 
   <td> <p>Klicken Sie für jeden Lead, den Sie der Liste hinzufügen möchten, auf <b>[!UICONTROL Hinzufügen]</b>eingeben oder die Kennung des Leads zuordnen, den Sie hinzufügen möchten. Sie können bis zu 300 Leads hinzufügen, damit das Modul zur Liste hinzugefügt wird.</p> <p>Klicken Sie auf den Umschalter Zuordnung , um eine vorhandene Sammlung von Leads zuzuordnen, die Sie der Liste hinzufügen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Leads aus einer Liste entfernen]

Dieses Aktionsmodul entfernt mithilfe der Lead-ID eine oder mehrere Leads aus einer Liste.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Marketo] Konto [!DNL Workfront Fusion], siehe <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Marketo] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Listen-ID]</td> 
   <td>Geben Sie die ID der Liste ein oder ordnen Sie sie zu, in der Sie Leads entfernen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Lead-IDs]</td> 
   <td> <p>Klicken Sie für jeden Lead, den Sie aus der Liste entfernen möchten, auf <b>[!UICONTROL Hinzufügen]</b>eingeben oder die Kennung des Leads zuordnen, den Sie entfernen möchten. Sie können bis zu 300 Leads hinzufügen, damit das Modul aus der Liste entfernt wird. </p> <p>Klicken Sie auf den Umschalter Zuordnung , um eine vorhandene Sammlung von Leads zuzuordnen, die Sie aus der Liste entfernen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eine Kampagne planen]

Dieses Aktionsmodul plant eine vorhandene Kampagne für ein bestimmtes Datum.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Marketo] Konto [!DNL Workfront Fusion], siehe <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Marketo] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Campaign ID]</td> 
   <td>Geben Sie die Kennung der Kampagne ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Zeitplan für das Datum]</p> </td> 
   <td>Wählen Sie das Datum aus, an dem die Kampagne laufen soll. Wenn dieses Feld leer gelassen wird, wird die Kampagne fünf Minuten nach Beginn des Szenarios ausgeführt.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Programm kopieren]

Dieses Aktionsmodul erstellt eine Kopie eines Programms unter Verwendung der Kennung des bestehenden Programms.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Marketo] Konto [!DNL Workfront Fusion], siehe <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Marketo] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vorhandene Programm-ID]</td> 
   <td>Geben Sie die Kennung des Programms ein, das Sie kopieren möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Neuer Programmname]</p> </td> 
   <td> <p>Geben Sie einen Namen für das neue Programm ein oder ordnen Sie ihn zu</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner-ID]</td> 
   <td>Geben Sie die Kennung des Ordners ein, in dem sich das neue Programm befinden soll, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

### Suchvorgänge

* [[!UICONTROL Auflisten von Datensätzen]](#list-records)
* [[!UICONTROL Suchdatensätze]](#update-a-record)

#### [!UICONTROL Auflisten von Datensätzen]

Dieses Aktionsmodul ruft alle Datensätze eines bestimmten Typs ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Marketo] Konto [!DNL Workfront Fusion], siehe <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Marketo] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ des Datensatzes aus, den Sie auflisten möchten.</p> 
    <ul> 
     <li> <p>[!UICONTROL Alle Kampagnen lesen]</p> </li> 
     <li> <p>[!UICONTROL Alle Programme lesen]</p> </li> 
     <li> <p>[!UICONTROL Alle Leads lesen] </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Field]</td> 
   <td>Wenn Sie ausgewählt haben, Leads abzurufen, wählen Sie aus, ob Sie Leads aus einer Liste oder aus einem Programm abrufen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td>Wählen Sie die Informationen aus, die im Ausgabebundle für dieses Modul enthalten sein sollen. Die Felder sind je nach ausgewähltem [!UICONTROL Record Type] verfügbar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suchdatensätze]

Dieses Suchmodul ruft eine Liste von Datensätzen ab, die bestimmten Suchkriterien entsprechen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Marketo] Konto [!DNL Workfront Fusion], siehe <a href="#connect-marketo-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Marketo] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den zu suchenden Datensatztyp aus.</p> 
    <ul> 
     <li> <p>[!UICONTROL Kampagnen]</p> </li> 
     <li> <p>[!UICONTROL Leads]</p> </li> 
     <li> <p>[!UICONTROL Programme]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Field]</p> </td> 
   <td> <p>Wählen Sie aus, ob Sie nach Name, Programmname oder Workspace-Name suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Werte]</td> 
   <td>Klicken Sie für jeden Wert, nach dem Sie suchen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie den Wert ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output]</td> 
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabebundle für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>
