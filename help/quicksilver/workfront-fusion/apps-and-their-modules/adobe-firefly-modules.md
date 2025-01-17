---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: Adobe Firefly-Module
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 1e131c27-571d-4099-9243-69572bdb3f5a
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1369'
ht-degree: 0%

---

# [!DNL Adobe Firefly]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Adobe Firefly-Module](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/adobe-firefly-modules.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die [!DNL Adobe Firefly] verwenden, und sie mit mehreren Anwendungen und Services von Drittanbietern verbinden.

Anweisungen zum Erstellen eines Szenarios finden Sie unter [Erstellen eines Szenarios](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: [!UICONTROL Standard]</p><p>Oder</p><p>Aktuell: [!UICONTROL Work] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] Lizenz **</td> 
   <td>
   <p>Aktuell: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy: Beliebig </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Neu:</p> <ul><li>[!UICONTROL Select] oder [!UICONTROL Prime] [!DNL Workfront] Plan: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] kaufen.</li><li>[!UICONTROL Ultimate] [!DNL Workfront]: [!DNL Workfront Fusion] ist enthalten.</li></ul>
   <p>Oder</p>
   <p>Aktuell: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Bevor Sie den [!DNL Adobe Firefly]-Connector verwenden können, müssen Sie sicherstellen, dass die folgenden Voraussetzungen erfüllt sind:

* Sie müssen über ein aktives [!DNL Adobe Firefly] verfügen.

## Adobe Campaign-API-Informationen

Der Adobe Campaign-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.4.24</td> 
  </tr>
 </tbody> 
 </table>

## Erstellen einer Verbindung zu [!DNL Adobe Firefly]

So erstellen Sie eine Verbindung für Ihre [!DNL Adobe Firefly]:

1. Klicken Sie **[!UICONTROL Hinzufügen]** neben dem Feld Verbindung auf.

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
        <td role="rowheader">[!UICONTROL Client-ID]</td>
        <td>Geben Sie Ihre [!UICONTROL Adobe] [!UICONTROL Client ID] ein. Dies finden Sie im Abschnitt mit den [!UICONTROL-Anmeldeinformationen] im [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client-Geheimnis]</td>
        <td>Geben Sie Ihren [!DNL Adobe] [!UICONTROL Client Secret] ein. Dies finden Sie im Abschnitt mit den [!UICONTROL-Anmeldeinformationen] im [!DNL Adobe Developer Console].</td>
        </tr>
      </tbody>
    </table>

1. Klicken Sie **[!UICONTROL Fortfahren]**, um die Verbindung zu speichern und zum Modul zurückzukehren.

## [!DNL Adobe Firefly] Module und ihre Felder

Beim Konfigurieren [!DNL Adobe Firefly] Module zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service weitere [!DNL Adobe Firefly] angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Erstellen eines benutzerdefinierten API-Aufrufs

Dieses Aktionsmodul führt einen benutzerdefinierten Aufruf an die Firefly-API durch.

Spezifische verfügbare APIs finden Sie unter [Adobe Firefly-API](https://developer.adobe.com/firefly-services/docs/firefly-api/) in der Dokumentation zu Adobe Developer.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
      <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Firefly] finden Sie unter <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Firefly]</a> in diesem Artikel.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Geben Sie einen Pfad relativ zu <code>https://firefly-api-enterprise-stage.adobe.io/</code> ein.</p>
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
      <td role="rowheader">[!UICONTROL body]</td>
   <td> <p>Fügen Sie den Hauptteil des Inhalts für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Wenn Sie bedingte Anweisungen wie <code>if</code> in Ihrer JSON-Datei verwenden, setzen Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### Bild erweitern

Dieses Aktionsmodul erweitert ein Bild, optional mit Inhalten aus einer von Ihnen angegebenen Eingabeaufforderung.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie unter <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Firefly]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prompt]</td> 
   <td>Geben Sie eine Eingabeaufforderung für den Inhalt ein, mit dem Sie das Bild erweitern möchten, oder ordnen Sie sie zu. Wenn keine Eingabeaufforderung angezeigt wird, wird das Bild mit Inhalten erweitert, die dem Originalbild entsprechen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anzahl der Varianten]</td> 
   <td>Geben Sie eine Zahl zwischen 1 und 4 ein. Das Modul generiert diese Anzahl von erweiterten Bildvarianten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Erweitertes Bildformat]</td> 
   <td>Wählen Sie das Dateiformat aus, in dem das erweiterte Bild gespeichert werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td>  <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Bilddateinamen und die Bilddatei (Daten) der Quelldatei zu.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Größe]</td> 
   <td>Wählen Sie die Größe aus, die das erweiterte Bild haben soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL seed]</td> 
   <td>Ganzzahl eingeben oder zuordnen. Sie können denselben Startwert in einem anderen Modul zum Erweitern eines Bildes verwenden, um ein ähnliches Bild mit verschiedenen Stilen zu generieren. </td> 
  </tr> 
 </tbody> 
</table>

## Bild ausfüllen

Dieses Aktionsmodul füllt den maskierten Bereich eines Bildes aus, optional mit Inhalten aus einer von Ihnen angegebenen Eingabeaufforderung.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie unter <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Firefly]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prompt]</td> 
   <td>Geben Sie eine Eingabeaufforderung für den Inhalt ein, mit dem Sie das Bild ausfüllen möchten, oder mappen Sie sie. Wenn keine Eingabeaufforderung angezeigt wird, wird das Bild mit Inhalten gefüllt, die dem Originalbild entsprechen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anzahl der Varianten]</td> 
   <td>Geben Sie eine Zahl zwischen 1 und 4 ein. Das Modul generiert diese Anzahl von ausgefüllten Bildvarianten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Gefülltes Bildformat]</td> 
   <td>Wählen Sie das Dateiformat aus, in dem das ausgefüllte Bild gespeichert werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bild]</td> 
   <td>  <p> Klicken Sie <b>Bild hinzufügen</b>. Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Bilddateinamen und die Bilddaten der Quelldatei zu.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Maske]</td> 
   <td>  <p> Klicken Sie <b>Maske hinzufügen</b>. Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen der Quelldatei und die Maskendaten der Quelldatei zu. Die Maskendatei stellt die benutzerdefinierte Maske dar, die mit generierten Inhalten gefüllt wird.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Größe]</td> 
   <td>Wählen Sie die Größe aus, in der das Bild ausgefüllt werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Seeds]</td> 
   <td>Klicken Sie für jedes Bild, das das Modul generiert, auf <b>Element hinzufügen<b> und geben Sie eine Ganzzahl ein oder mappen Sie sie. Sie können denselben Startwert in einem anderen Modul zum Erweitern eines Bildes verwenden, um ein ähnliches Bild mit verschiedenen Stilen zu generieren. Die Anzahl der hinzugefügten Testadressen muss der Anzahl der Varianten im Feld entsprechen.</td> 
  </tr> 
 </tbody> 
</table>

## Bild erzeugen

Dieses Aktionsmodul generiert ein - und -Bild basierend auf einer von Ihnen angegebenen Eingabeaufforderung. Sie können auch ein optionales Referenzbild angeben. Das generierte Bild entspricht dem Stil des Referenzbilds.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie unter <a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Firefly]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Prompt]</td> 
   <td>Geben Sie eine Eingabeaufforderung für das Bild ein, das Sie erstellen möchten, oder ordnen Sie sie zu. Weitere Details in der Eingabeaufforderung ermöglichen Ihnen mehr Kontrolle darüber, was im Bild angezeigt wird.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anzahl der Varianten]</td> 
   <td>Geben Sie eine Zahl zwischen 1 und 4 ein. Das Modul generiert diese Anzahl von Bildvarianten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Generiertes Bildformat]</td> 
   <td>Wählen Sie das Dateiformat aus, in dem das erweiterte Bild gespeichert werden soll. Wenn Sie Standard auswählen, wird das Dateiformat JPEG, wenn kein Referenzbild angegeben wird. Wenn ein Referenzbild bereitgestellt wird, ist das Dateiformat des generierten Bildes mit dem Referenzbild identisch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td>  <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen der Referenzbilddatei und die Referenzbilddatei (Daten) der Quelldatei zu. Das generierte Bild wird entsprechend dem Stil des Referenzbilds erstellt.</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Vorgaben]</td> 
   <td>Wenn Sie einen Vorgabestil verwenden möchten, klicken Sie auf Element hinzufügen und geben Sie den gewünschten Stil ein, oder ordnen Sie ihn zu.<p>Eine Liste der Vorgabestile finden Sie unter <a href="https://developer.adobe.com/firefly-services/docs/firefly-api/guides/concepts/style-presets/" >Bildmodellstile</a> in der Adobe-Entwicklerdokumentation.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Negative Eingabeaufforderung]</td> 
   <td>Geben Sie die Wörter ein, die Sie im generierten Inhalt vermeiden möchten, oder ordnen Sie sie zu. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inhaltsklasse]</td> 
   <td>Wählen Sie aus, ob das generierte Bild mehr wie ein Foto oder eher wie erstellte Kunst aussehen soll. <ul><li><b>Foto</b><p>Geben Sie Werte für Blende, Verschlusszeit (in Sekunden) und Sichtfeld (in Millimetern) ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL seed]</td> 
   <td>Ganzzahl eingeben oder zuordnen. Sie können denselben Startwert in einem anderen Modul zum Erweitern eines Bildes verwenden, um ein ähnliches Bild mit verschiedenen Stilen zu generieren. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Größe]</td> 
   <td>Wählen Sie die Größe aus, in der das generierte Bild angezeigt werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Strength]</td> 
   <td>Geben Sie eine Ganzzahl ein, die die Intensität darstellt, mit der das generierte Bild dem Stil des Vorgabenstils oder Referenzbilds entspricht, oder mappen Sie sie. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sehstärke]</td> 
   <td>Geben Sie eine Ganzzahl ein, die die Gesamtintensität der vorhandenen visuellen Eigenschaften des Fotos darstellt, oder mappen Sie sie. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Locale]</td> 
   <td>Wenn ein Gebietsschema bereitgestellt wird, generiert das Modul Inhalte, die für das angegebene Gebietsschema relevanter sind. <p>Das Gebietsschema muss im ISO-639-1-Sprachcode und in der ISO-3166-1-Region angegeben werden.</p><p> Beispiel: <code>en-US</code></p></td> 
  </tr> 
 </tbody> 
</table>
