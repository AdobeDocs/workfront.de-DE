---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: Partnermodule
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: e4dc9588-334a-41a3-85d1-996cb819c3fa
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 0%

---

# [!DNL Bynder]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Bynder-Module](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/bynder-modules.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die [!DNL Bynder] verwenden, und sie mit mehreren Anwendungen und Services von Drittanbietern verbinden.

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

Um [!DNL Bynder]-Module verwenden zu können, müssen Sie über ein [!DNL Bynder]-Konto verfügen.

## Binder-API-Informationen

Der Binder-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API-Version</td> 
   <td> v4 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.25.21</td> 
  </tr>
 </tbody> 
 </table>

## Verbinden von [!DNL Bynder] mit Workfront Fusion  {#connect-bynder-to-workfront-fusion}

* [Erstellen einer Verbindung zu [!DNL Bynder] von [!DNL Workfront Fusion]](#create-a-connection-to-bynder-from-workfront-fusion)
* [Generieren einer [!UICONTROL Client-ID] und [!UICONTROL Client-Geheimnis] in [!DNL Bynder] (optional)](#generate-a-client-id-and-client-secret-in-bynder-optional)

### Erstellen einer Verbindung zu [!DNL Bynder] aus [!DNL Workfront Fusion]

Sie können direkt aus einem [!DNL Bynder]-Modul heraus eine Verbindung von [!DNL Workfront Fusion] zu Ihrem [!DNL Bynder]-Konto erstellen.

1. Klicken Sie in einem [!DNL Bynder] Modul **[!UICONTROL Hinzufügen]** neben dem Feld [!UICONTROL Verbindung].
1. Wählen Sie die [!DNL Bynder] Domain aus, mit der Sie eine Verbindung herstellen möchten.
1. (Optional) Klicken Sie auf **[!UICONTROL Erweiterte Einstellungen]** und geben Sie dann Ihre [!UICONTROL Client-ID] und [!UICONTROL Client-Geheimnis] ein.

   Anweisungen zum Generieren der Client-ID und des Client-Geheimnisses finden Sie unter [Generieren einer Client-ID und eines Client-Geheimnisses in [!DNL Bynder] (optional)](#generate-a-client-id-and-client-secret-in-bynder-optional) in diesem Artikel.

1. Geben [!UICONTROL  im Fenster &quot;]&quot; Ihren Benutzernamen (E-Mail-Adresse) und Ihr Passwort ein.
1. Klicken Sie **[!UICONTROL Fortfahren]**, um die Verbindung zu erstellen, und kehren Sie zum Modul zurück.

### Generieren einer [!UICONTROL Client-ID] und [!UICONTROL Client-]) in [!DNL Bynder] (optional)

Wenn Sie eine Verbindung mit der Client-ID und dem Client-Geheimnis erstellen möchten, können Sie sie aus Ihrem [!DNL Bynder]-Konto generieren. Die Client-ID und der geheime Client-Schlüssel werden beim Erstellen einer App in [!DNL Bynder] generiert.

Anweisungen zum Erstellen einer App in [!DNL Bynder] finden Sie unter [OAuth 2.0-](https://developer-docs.bynder.com/api/authentication-oauth2-oauth-apps/)) in der [!DNL Bynder].

>[!NOTE]
>
>Geben Sie beim Erstellen der App in [!DNL Bynder] Folgendes als `redirect uri` ein:
>
>`https://app.workfrontfusion.com/oauth/cb/workfront-bynder`

## [!DNL Bynder] Module und ihre Felder

Beim Konfigurieren [!DNL Bynder] Module zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service weitere [!DNL Bynder] angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Aktionen](#actions)
* [Suchvorgänge](#searches)
* [Trigger](#triggers)

### Aktionen

* [[!UICONTROL Benutzerdefinierter API-Aufruf]](#custom-api-call)
* [[!UICONTROL Asset-Metadaten lesen]](#read-asset-metadata)
* [[!UICONTROL Aktualisieren von Asset-Metadaten]](#update-asset-metadata)
* [[!UICONTROL Hinzufügen von Assets zu einer Sammlung]](#add-assets-to-a-collection)
* [[!UICONTROL Entfernen von Assets aus der Sammlung]](#remove-assets-from-collection)
* [[!UICONTROL Hinzufügen eines Tags zu Assets]](#add-a-tag-to-assets)
* [[!UICONTROL Entfernen eines Tags] aus Assets](#remove-a-tag-from-assets)
* [[!UICONTROL Asset herunterladen]](#download-asset)
* [[!UICONTROL Asset hochladen]](#upload-asset)

#### [!UICONTROL Benutzerdefinierter API-Aufruf]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Bynder]-API durchführen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von den anderen [!DNL Bynder] nicht durchgeführt werden kann.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

Das Modul gibt einen Status-Code zusammen mit den Kopfzeilen und dem Hauptteil des API-Aufrufs zurück.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Bynder]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Bynder] mit [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Geben Sie einen Pfad relativ zu <code>https://{your-bynder-domain}/api/{api-version}/</code> ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Methode]</td> 
   td&gt; <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anfragemethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Kopfzeilen]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
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

#### [!UICONTROL Asset-Metadaten lesen]

Dieses Aktionsmodul liest die Metadaten eines Assets.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Bynder]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Bynder] mit [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-ID]</td> 
   <td>Geben Sie die ID des Assets ein, für das Sie Metadaten abrufen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabepaket für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aktualisieren von Asset-Metadaten]

Dieses Aktionsmodul aktualisiert die Metadaten eines vorhandenen Assets.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Bynder]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Bynder] mit [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-ID]</td> 
   <td>Geben Sie die ID des Assets ein, für das Sie Metadaten aktualisieren möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Felder]</td> 
   <td> <p>Wählen Sie die Felder aus, für die Sie Informationen eingeben möchten, und geben Sie dann die Informationen, mit denen Sie die Metadaten aktualisieren möchten, in diese Felder ein oder ordnen Sie sie zu. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Metaproperties]</p> </td> 
   <td>Wählen Sie die Optionen aus, die Sie aktualisieren möchten, und geben Sie dann die Informationen in diese Eigenschaften ein oder ordnen Sie sie ihnen zu. Metaeigenschaften sind Informationen über das Asset, die keine bestimmten Felder im Asset darstellen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Hinzufügen von Assets zu einer Sammlung]

Dieses Aktionsmodul fügt ein oder mehrere Assets zu einer Sammlung hinzu.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Bynder]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Bynder] mit [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Sammlungs-ID]</td> 
   <td> <p>Geben Sie die ID der Sammlung ein, der Sie Assets hinzufügen möchten, oder mappen Sie sie.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-IDs]</td> 
   <td> <p>Klicken Sie für jedes Asset, das Sie der Sammlung hinzufügen möchten, auf <strong>[!UICONTROL Element hinzufügen]</strong> und geben Sie dann die Asset-ID ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Entfernen von Assets aus der Sammlung]

Dieses Aktionsmodul entfernt ein oder mehrere Assets aus einer Sammlung.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Bynder]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Bynder] mit [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Sammlungs-ID]</td> 
   <td> <p>Geben Sie die ID der Sammlung ein, aus der Sie Assets entfernen möchten, oder mappen Sie sie.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-IDs]</td> 
   <td> <p>Klicken Sie für jedes Asset, das Sie aus der Sammlung entfernen möchten, auf <strong>[!UICONTROL Element hinzufügen]</strong> und geben Sie dann die Asset-ID ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Hinzufügen eines Tags zu Assets]

Hinzufügen eines Tags zu einem oder mehreren Assets

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Bynder]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Bynder] mit [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tag-ID]</td> 
   <td> <p>Geben Sie die ID des Tags ein, das Sie zu Assets hinzufügen möchten, oder ordnen Sie sie zu.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-IDs]</td> 
   <td> <p>Klicken Sie für jedes Asset, das Sie mit einem Tag versehen möchten, auf <strong>[!UICONTROL Element hinzufügen]</strong> und geben Sie dann die Asset-ID ein bzw. mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Entfernen eines Tags aus Assets]

Entfernen eines Tags aus einem oder mehreren Assets

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Bynder]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Bynder] mit [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tag-ID]</td> 
   <td> <p>Geben Sie die ID des Tags ein, das Sie aus Assets entfernen möchten, oder ordnen Sie sie zu.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-IDs]</td> 
   <td> <p>Klicken Sie für jedes Asset, aus dem Sie ein Tag entfernen möchten, auf <strong>[!UICONTROL Element hinzufügen]</strong> und geben Sie dann die Asset-ID ein bzw. mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Asset herunterladen]

Dieses Aktionsmodul lädt ein einzelnes Asset herunter.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Bynder]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Bynder] mit [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-ID]</td> 
   <td>Geben Sie die ID des Assets ein, das Sie herunterladen möchten, oder mappen Sie sie.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-Version]</td> 
   <td> <p>Geben Sie die Version des Assets ein, das Sie herunterladen möchten, oder ordnen Sie sie zu. Um die neueste Version des Assets herunterzuladen, lassen Sie das Feld leer.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Asset hochladen]

Dieses Aktionsmodul lädt ein einzelnes Asset hoch.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Bynder]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Bynder] mit [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Speichern unter]</td> 
   <td> <p>Wählen Sie aus, wie Sie die hochgeladene Datei speichern möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Neues Asset]</strong> </p> <p>Wählen Sie die Felder und Metaeigenschaften aus, für die Sie Informationen eingeben möchten, und geben Sie dann die Informationen in diese Felder ein.</p> <p>Geben Sie die ID der Marke ein, die Sie für das hochgeladene Asset verwenden möchten, oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Neue Asset-Version]</strong> </p> <p>Geben Sie die ID des Assets ein, für das Sie eine neue Version hochladen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</td> 
  </tr> 
 </tbody> 
</table>

### Suchvorgänge

* [[!UICONTROL Eintrag auflisten]](#list-record)
* [[!UICONTROL Nach Assets suchen]](#search-for-assets)

#### [!UICONTROL Eintrag auflisten]

Dieses Suchmodul ruft alle Elemente eines bestimmten Typs ab.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Bynder]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Bynder] mit [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Datensatztyp]</td> 
   <td> <p>Wählen Sie den Typ des aufzulistenden Datensatzes aus.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Alle Sammlungen lesen]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Informationen über alle Tags lesen]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Alle Assets einer Sammlung lesen]</strong> </p> <p>Geben Sie die ID der Sammlung ein, für die Sie Assets auflisten möchten, oder ordnen Sie sie zu.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Felder aus, die Sie in die Ausgabe des Moduls aufnehmen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Assets ein, die das Modul bei jedem Ausführungszyklus des Szenarios zurückgeben soll, oder mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Nach Assets suchen]

Dieses Suchmodul sucht anhand der von Ihnen angegebenen Kriterien nach Assets.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Bynder]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Bynder] mit [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Kriterien]</td> 
   <td> <p>Geben Sie die Suchkriterien ein. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL-Feld]</strong> </p> <p>Wählen Sie das Feld aus, das Sie für Ihre Suche verwenden möchten</p> </li> 
     <li> <p><strong>[!UICONTROL Logischer Operator]</strong> </p> <p>Wählen Sie den Operator aus, den Sie für Ihre Suche verwenden möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL value]</strong> </p> <p>Geben Sie den Wert, nach dem im ausgewählten Feld gesucht werden soll, ein oder ordnen Sie ihn zu. Der Werttyp sollte mit dem Datentyp des ausgewählten Felds übereinstimmen. </p> <p>Weitere Informationen zu Datentypen finden Sie unter <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Elementdatentypen in [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ergebnissatz]</td> 
   <td>Wählen Sie aus, ob das erste übereinstimmende Asset oder alle übereinstimmenden Assets zurückgegeben werden sollen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sortieren nach]</td> 
   <td> <p>Wählen Sie das Feld aus, nach dem Sie sortieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sortierrichtung]</td> 
   <td> <p>Wählen Sie aus, ob auf- oder absteigend sortiert werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Felder aus, die Sie in die Ausgabe des Moduls aufnehmen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Assets ein, die das Modul bei jedem Ausführungszyklus des Szenarios zurückgeben soll, oder mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Trigger

#### [!UICONTROL Überwachen von Assets]

Dieses Trigger-Modul startet ein Szenario, wenn ein Asset erstellt oder aktualisiert wird.

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL-Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Bynder]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Bynder] mit [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Event type</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select whether you want to start the scenario when a new asset is created or when an existing asset is updated.</td>
   --> 
  </tr> 
  <tr>
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL-Sammlungen]</td>
   <td> <p>Wählen Sie die Sammlung aus, die Sie auf neue Assets überwachen möchten. Um alle Sammlungen zu sehen, lassen Sie dieses Feld leer.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Outputs</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the fields that you want to include in the output.</td>
   --> 
  </tr> 
  <tr> 
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Limit]</td>

<td> <p>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul bei jedem Ausführungszyklus des Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>
