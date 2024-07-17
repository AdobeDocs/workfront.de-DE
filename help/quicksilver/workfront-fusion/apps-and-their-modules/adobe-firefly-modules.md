---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Adobe Firefly-Module
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die [!DNL Adobe Firefly] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 1e131c27-571d-4099-9243-69572bdb3f5a
source-git-commit: 7013302a6ba903b410ed1fa8948a195083004eb9
workflow-type: tm+mt
source-wordcount: '1301'
ht-degree: 0%

---

# [!DNL Adobe Firefly] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Adobe Firefly] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p><p>Oder</p><p>Aktuell: [!UICONTROL Arbeit] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuell: Keine [!DNL Workfront Fusion] Lizenzanforderung.</p>
   <p>Oder</p>
   <p>Veraltet: Beliebig </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Neu:</p> <ul><li>[!UICONTROL Select] oder [!UICONTROL Prime] [!DNL Workfront] Plan: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben.</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] ist enthalten.</li></ul>
   <p>Oder</p>
   <p>Aktuell: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] kaufen.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Bevor Sie den Connector [!DNL Adobe Firefly] verwenden können, müssen Sie sicherstellen, dass die folgenden Voraussetzungen erfüllt sind:

* Sie müssen über ein aktives [!DNL Adobe Firefly] -Konto verfügen.

## Erstellen einer Verbindung zu [!DNL Adobe Firefly]

So erstellen Sie eine Verbindung für Ihre [!DNL Adobe Firefly] -Module:

1. Klicken Sie neben dem Feld Verbindung auf **[!UICONTROL Hinzufügen]** .

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
        <td>Wählen Sie aus, ob Sie eine Verbindung zu einer Produktions- oder Nicht-Produktionsumgebung herstellen möchten.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Typ]</td>
        <td>Wählen Sie aus, ob Sie eine Verbindung zu einem Dienstkonto oder einem persönlichen Konto herstellen möchten.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client-ID]</td>
        <td>Geben Sie Ihre [!UICONTROL Adobe] [!UICONTROL Client ID] ein. Dies finden Sie im [!UICONTROL Credentials]-Detailabschnitt des [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Geben Sie Ihren [!DNL Adobe] [!UICONTROL Client Secret] ein. Dies finden Sie im [!UICONTROL Credentials]-Detailabschnitt des [!DNL Adobe Developer Console]</td>
        </tr>
      </tbody>
    </table>

1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu speichern und zum Modul zurückzukehren.

## [!DNL Adobe Firefly] Module und ihre Felder

Wenn Sie [!DNL Adobe Firefly] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Adobe Firefly] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Benutzerdefinierte API-Aufrufe durchführen

Dieses Aktionsmodul führt einen benutzerdefinierten Aufruf an die Firefly-API durch.

Bestimmte verfügbare APIs finden Sie unter [Adobe Firefly-API](https://developer.adobe.com/firefly-services/docs/firefly-api/) in der Adobe Developer-Dokumentation.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Firefly] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Firefly]</a> .</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Geben Sie einen Pfad relativ zu <code>https://firefly-api-enterprise-stage.adobe.io/</code> ein.</p>
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
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### Bild erweitern

Dieses Aktionsmodul erweitert ein Bild, optional mit Inhalt aus einer von Ihnen angegebenen Eingabeaufforderung.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Firefly]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eingabeaufforderung]</td> 
   <td>Geben Sie eine Eingabeaufforderung für den Inhalt ein, mit dem Sie das Bild erweitern möchten, oder ordnen Sie ihn zu. Wenn keine Eingabeaufforderung angegeben wird, wird das Bild mit Inhalten erweitert, die mit dem Originalbild übereinstimmen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anzahl der Varianten]</td> 
   <td>Geben Sie eine Zahl zwischen 1 und 4 ein. Das Modul generiert diese Anzahl erweiterter Bildvarianten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Erweitertes Bildformat]</td> 
   <td>Wählen Sie das Dateiformat aus, als das erweiterte Bild gespeichert werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td>  <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen der Bilddatei und die Bilddatei (Daten) der Quelldatei zu.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Größe]</td> 
   <td>Wählen Sie die Größe aus, die das erweiterte Bild aufweisen soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seed]</td> 
   <td>Geben Sie eine Ganzzahl ein oder ordnen Sie sie zu. Sie können dieses Samen in einem anderen Modul Bild erweitern verwenden, um ein ähnliches Bild mit unterschiedlichen Stilen zu generieren. </td> 
  </tr> 
 </tbody> 
</table>

## Bild ausfüllen

Dieses Aktionsmodul füllt den maskierten Bereich eines Bildes, optional mit Inhalt aus einer von Ihnen angegebenen Eingabeaufforderung.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Firefly]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eingabeaufforderung]</td> 
   <td>Geben Sie eine Eingabeaufforderung für den Inhalt ein, mit dem Sie das Bild ausfüllen möchten, oder ordnen Sie ihn zu. Wenn keine Eingabeaufforderung angegeben wird, wird das Bild mit Inhalten gefüllt, die dem Originalbild entsprechen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anzahl der Varianten]</td> 
   <td>Geben Sie eine Zahl zwischen 1 und 4 ein. Das Modul generiert diese Anzahl an ausgefüllten Bildvarianten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bildformat ausgefüllt]</td> 
   <td>Wählen Sie das Dateiformat aus, in dem das ausgefüllte Bild gespeichert werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bild]</td> 
   <td>  <p> Klicken Sie auf <b>Bild hinzufügen</b>. Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie die Bild- und Bilddaten der Quelldatei zu.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mask]</td> 
   <td>  <p> Klicken Sie auf <b>Maske hinzufügen</b>. Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen der Mask-Datei und die Maskierungsdaten der Quelldatei zu. Die Datei Maske stellt die benutzerdefinierte Maske dar, die mit dem generierten Inhalt gefüllt wird.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Größe]</td> 
   <td>Wählen Sie die Größe aus, die das ausgefüllte Bild aufweisen soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seeds]</td> 
   <td>Klicken Sie für jedes Bild, das vom Modul generiert wird, auf <b>Element hinzufügen<b> und geben Sie eine Ganzzahl ein oder ordnen Sie sie zu. Sie können dieses Samen in einem anderen Modul Bild erweitern verwenden, um ein ähnliches Bild mit unterschiedlichen Stilen zu generieren. Die Anzahl der hinzugefügten Samen muss dem Feld Anzahl der Varianten entsprechen.</td> 
  </tr> 
 </tbody> 
</table>

## Bild generieren

Dieses Aktionsmodul generiert und erstellt ein Bild basierend auf einer von Ihnen angegebenen Eingabeaufforderung. Sie können auch ein optionales Referenzbild bereitstellen. Das generierte Bild entspricht dem Stil des Referenzbilds.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Firefly]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Eingabeaufforderung]</td> 
   <td>Geben Sie eine Eingabeaufforderung für das Bild ein, das Sie erstellen möchten, oder ordnen Sie es zu. Weitere Details in der Eingabeaufforderung ermöglichen Ihnen mehr Kontrolle darüber, was im Bild angezeigt wird.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anzahl der Varianten]</td> 
   <td>Geben Sie eine Zahl zwischen 1 und 4 ein. Das Modul generiert diese Anzahl an Bildvarianten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Generiertes Bildformat]</td> 
   <td>Wählen Sie das Dateiformat aus, als das erweiterte Bild gespeichert werden soll. Wenn Sie "Standard"auswählen, ist das Dateiformat "JPEG", wenn kein Referenzbild bereitgestellt wird. Wenn ein Referenzbild angegeben wird, entspricht das Dateiformat des generierten Bildes dem Referenzbild.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td>  <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen der Referenzbilddatei und die Referenzbilddatei (Daten) der Quelldatei zu. Das generierte Bild wird so erstellt, dass es dem Stil des Referenzbilds entspricht.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vorgaben]</td> 
   <td>Wenn Sie einen Vorgabenstil verwenden möchten, klicken Sie auf Element hinzufügen und geben Sie den gewünschten Stil ein oder ordnen Sie ihn zu.<p>Eine Liste der Vorgabenstile finden Sie unter <a href="https://developer.adobe.com/firefly-services/docs/firefly-api/guides/concepts/styles/" >Bildmodellstile</a> in der Adobe-Entwicklerdokumentation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Negative Eingabeaufforderung]</td> 
   <td>Geben Sie im generierten Inhalt die Wörter ein, die Sie vermeiden möchten, oder ordnen Sie sie zu. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content class]</td> 
   <td>Wählen Sie aus, ob das generierte Bild eher wie ein Foto oder eher wie eine erstellte Kunst sein soll. <ul><li><b>Foto</b><p>Geben Sie Werte für die Perspektive, die Verschlusszeit (in Sekunden) und das Sichtfeld (in Millimetern) ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seed]</td> 
   <td>Geben Sie eine Ganzzahl ein oder ordnen Sie sie zu. Sie können dieses Samen in einem anderen Modul Bild erweitern verwenden, um ein ähnliches Bild mit unterschiedlichen Stilen zu generieren. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Größe]</td> 
   <td>Wählen Sie die Größe aus, die das generierte Bild erhalten soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stärke]</td> 
   <td>Geben Sie eine Ganzzahl ein oder ordnen Sie sie zu, die die Intensität darstellt, mit der das generierte Bild dem Stil des Vorgabenstils oder des Referenzbilds entspricht. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL visuelle Intensität</td> 
   <td>Geben Sie eine Ganzzahl ein oder ordnen Sie sie zu, die die Gesamtintensität der vorhandenen visuellen Eigenschaften des Fotos darstellt. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Locale]</td> 
   <td>Wenn ein Gebietsschema angegeben wird, generiert das Modul Inhalte, die für das angegebene Gebietsschema relevanter sind. <p>Das Gebietsschema muss im Sprachcode nach ISO 639-1 und in der Region nach ISO 3166-1 angegeben werden.</p><p> Beispiel: <code>en-US</code></p></td> 
  </tr> 
 </tbody> 
</table>
