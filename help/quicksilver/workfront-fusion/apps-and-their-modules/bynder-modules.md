---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connector
navigation-topic: apps-and-their-modules
title: Synchronisierungsmodule
description: In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Bynder], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.
author: Becky
feature: Workfront Fusion
exl-id: e4dc9588-334a-41a3-85d1-996cb819c3fa
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1616'
ht-degree: 0%

---

# [!DNL Bynder]-Module

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Bynder], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.

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

Verwendung [!DNL Bynder] -Module, müssen Sie über eine [!DNL Bynder] -Konto.

## Verbinden [!DNL Bynder] zu Workfront Fusion  {#connect-bynder-to-workfront-fusion}

* [Erstellen Sie eine Verbindung zu [!DNL Bynder] von [!DNL Workfront Fusion]](#create-a-connection-to-bynder-from-workfront-fusion)
* [Generieren Sie eine [!UICONTROL Client-ID] und [!UICONTROL Client Secret] in [!DNL Bynder] (Optional)](#generate-a-client-id-and-client-secret-in-bynder-optional)

### Erstellen Sie eine Verbindung zu [!DNL Bynder] von [!DNL Workfront Fusion]

Sie können eine Verbindung aus [!DNL Workfront Fusion] auf [!DNL Bynder] direkt in einer [!DNL Bynder] -Modul.

1. In jeder [!DNL Bynder] Modul, klicken Sie auf **[!UICONTROL Hinzufügen]** neben dem [!UICONTROL Verbindung] -Feld.
1. Wählen Sie die [!DNL Bynder] Domäne, mit der Sie eine Verbindung herstellen möchten.
1. (Optional) Klicken Sie auf **[!UICONTROL Erweiterte Einstellungen]** Geben Sie dann [!UICONTROL Client-ID] und [!UICONTROL Client Secret].

   Anweisungen zum Generieren der Client-ID und des Client-Geheimnisses finden Sie unter [Generieren einer Client-ID und eines Client-Geheimnisses in [!DNL Bynder] (Optional)](#generate-a-client-id-and-client-secret-in-bynder-optional) in diesem Artikel.

1. Im [!UICONTROL Anmeldung] eingeben, geben Sie Ihren Benutzernamen (E-Mail-Adresse) und Ihr Passwort ein.
1. Klicken **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

### Generieren Sie eine [!UICONTROL Client-ID] und [!UICONTROL Client Secret] in [!DNL Bynder] (Optional)

Wenn Sie eine Verbindung mit der Client-ID und dem Client-Geheimnis erstellen möchten, können Sie sie aus Ihrem [!DNL Bynder] -Konto. Die Client-ID und das Client-Geheimnis werden generiert, wenn Sie eine App in [!DNL Bynder].

Anweisungen zum Erstellen einer App in [!DNL Bynder], siehe [OAuth 2.0 Apps](https://developer-docs.bynder.com/api/authentication-oauth2-oauth-apps/) im [!DNL Bynder] Dokumentation.

>[!NOTE]
>
>Beim Erstellen der App in [!DNL Bynder]Geben Sie Folgendes als `redirect uri`:
>
>`https://app.workfrontfusion.com/oauth/cb/workfront-bynder`

## [!DNL Bynder] Module und ihre Felder

Bei der Konfiguration [!DNL Bynder] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Bynder] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Aktionen](#actions)
* [Suchvorgänge](#searches)
* [Trigger](#triggers)

### Aktionen

* [[!UICONTROL Benutzerspezifischer API-Aufruf]](#custom-api-call)
* [[!UICONTROL Asset-Metadaten lesen]](#read-asset-metadata)
* [[!UICONTROL Aktualisieren von Asset-Metadaten]](#update-asset-metadata)
* [[!UICONTROL Hinzufügen von Assets zu einer Sammlung]](#add-assets-to-a-collection)
* [[!UICONTROL Entfernen von Assets aus der Sammlung]](#remove-assets-from-collection)
* [[!UICONTROL Hinzufügen von Tags zu Assets]](#add-a-tag-to-assets)
* [[!UICONTROL Tag entfernen] aus Assets](#remove-a-tag-from-assets)
* [[!UICONTROL Asset herunterladen]](#download-asset)
* [[!UICONTROL Hochladen des Assets]](#upload-asset)

#### [!UICONTROL Benutzerspezifischer API-Aufruf]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Bynder] API. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von der anderen nicht durchgeführt werden kann [!DNL Bynder] Module.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

Das Modul gibt einen Statuscode sowie die Kopfzeilen und den Hauptteil des API-Aufrufs zurück.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Bynder] Konto [!DNL Workfront Fusion], siehe <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] nach [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Geben Sie einen Pfad relativ zu ein <code>https://{your-bynder-domain}/api/{api-version}/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode]</td> 
   td&gt; <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
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

#### [!UICONTROL Asset-Metadaten lesen]

Dieses Aktionsmodul liest die Metadaten eines Assets.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Bynder] Konto [!DNL Workfront Fusion], siehe <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] nach [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-ID]</td> 
   <td>Geben Sie die ID des Assets ein oder ordnen Sie sie zu, für das Sie Metadaten abrufen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabebundle für dieses Modul enthalten sein sollen.</p> </td> 
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
    <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Bynder] Konto [!DNL Workfront Fusion], siehe <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] nach [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-ID]</td> 
   <td>Geben Sie die ID des Assets ein oder ordnen Sie sie zu, für das Sie Metadaten aktualisieren möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Felder]</td> 
   <td> <p>Wählen Sie die Felder aus, für die Sie Informationen eingeben möchten, und geben Sie dann die Informationen, mit denen Sie die Metadaten aktualisieren möchten, in diese Felder ein oder ordnen Sie sie zu. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Metaeigenschaften]</p> </td> 
   <td>Wählen Sie die Optionen aus, die Sie aktualisieren möchten, und geben Sie dann die Informationen ein oder ordnen Sie sie diesen Eigenschaften zu. Metaeigenschaften sind Informationen zum Asset, die keine bestimmten Felder im Asset darstellen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Hinzufügen von Assets zu einer Sammlung]

Dieses Aktionsmodul fügt einer Sammlung mindestens ein Asset hinzu.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Bynder] Konto [!DNL Workfront Fusion], siehe <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] nach [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collection ID]</td> 
   <td> <p>Geben Sie die ID der Sammlung ein, der Sie Assets hinzufügen möchten, oder ordnen Sie sie zu.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-IDs]</td> 
   <td> <p>Klicken Sie für jedes Asset, das Sie zur Sammlung hinzufügen möchten, auf <strong>[!UICONTROL Element hinzufügen]</strong>eingeben oder die Asset-ID zuordnen.</p> </td> 
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
    <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Bynder] Konto [!DNL Workfront Fusion], siehe <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] nach [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collection ID]</td> 
   <td> <p>Geben Sie die ID der Sammlung ein oder ordnen Sie sie zu, in der Sie Assets entfernen möchten.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-IDs]</td> 
   <td> <p>Klicken Sie für jedes Asset, das Sie aus der Sammlung entfernen möchten, auf <strong>[!UICONTROL Element hinzufügen]</strong>eingeben oder die Asset-ID zuordnen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Hinzufügen von Tags zu Assets]

Tag zu einem oder mehreren Assets hinzufügen

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Bynder] Konto [!DNL Workfront Fusion], siehe <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] nach [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tag-ID]</td> 
   <td> <p>Geben Sie die ID des Tags ein oder ordnen Sie sie zu Assets zu.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-IDs]</td> 
   <td> <p>Klicken Sie für jedes Asset, das Sie taggen möchten, auf <strong>[!UICONTROL Element hinzufügen]</strong>eingeben oder die Asset-ID zuordnen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Entfernen von Tags aus Assets]

Entfernen eines Tags aus einem oder mehreren Assets

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Bynder] Konto [!DNL Workfront Fusion], siehe <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] nach [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tag-ID]</td> 
   <td> <p>Geben Sie die ID des Tags ein oder ordnen Sie sie zu, das Sie aus Assets entfernen möchten.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-IDs]</td> 
   <td> <p>Klicken Sie für jedes Asset, aus dem Sie ein Tag entfernen möchten, auf <strong>[!UICONTROL Element hinzufügen]</strong>eingeben oder die Asset-ID zuordnen.</p> </td> 
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
    <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Bynder] Konto [!DNL Workfront Fusion], siehe <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] nach [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-ID]</td> 
   <td>Geben Sie die ID des Assets ein, das Sie herunterladen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-Version]</td> 
   <td> <p>Geben Sie die Version des Assets ein oder ordnen Sie sie zu, das Sie herunterladen möchten. Lassen Sie das Feld leer, um die neueste Version des Assets herunterzuladen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Hochladen des Assets]

Dieses Aktionsmodul lädt ein einzelnes Asset hoch.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Bynder] Konto [!DNL Workfront Fusion], siehe <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] nach [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Speichern unter]</td> 
   <td> <p>Wählen Sie aus, wie Sie die hochgeladene Datei speichern möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Neues Asset]</strong> </p> <p>Wählen Sie die Felder und Metaeigenschaften aus, für die Sie Informationen eingeben möchten, und geben Sie dann die Informationen in diese Felder ein.</p> <p>Geben Sie die Kennung der Marke ein, die Sie für das hochgeladene Asset verwenden möchten, oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Neue Asset-Version]</strong> </p> <p>Geben Sie die ID des Assets ein, für das Sie eine neue Version hochladen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</td> 
  </tr> 
 </tbody> 
</table>

### Suchvorgänge

* [[!UICONTROL Listeneintrag]](#list-record)
* [[!UICONTROL Suchen nach Assets]](#search-for-assets)

#### [!UICONTROL Listeneintrag]

Dieses Suchmodul ruft alle Elemente eines bestimmten Typs ab.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Bynder] Konto [!DNL Workfront Fusion], siehe <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] nach [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den aufzulistenden Datensatztyp aus.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Alle Sammlungen lesen]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Informationen über alle Tags]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL Alle Assets einer Sammlung lesen]</strong> </p> <p>Geben Sie die ID der Sammlung ein oder ordnen Sie sie zu, deren Assets Sie auflisten möchten.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Felder aus, die Sie in die Ausgabe des Moduls aufnehmen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Assets ein oder ordnen Sie sie zu, die das Modul während des Ausführungsprozesses jedes Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suchen nach Assets]

Dieses Suchmodul sucht nach Assets basierend auf von Ihnen angegebenen Kriterien.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Bynder] Konto [!DNL Workfront Fusion], siehe <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] nach [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kriterien]</td> 
   <td> <p>Geben Sie die Suchkriterien ein. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Field]</strong> </p> <p>Wählen Sie das Feld aus, das Sie für die Suche verwenden möchten</p> </li> 
     <li> <p><strong>[!UICONTROL Logischer Operator]</strong> </p> <p>Wählen Sie den Operator aus, den Sie für die Suche verwenden möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL Wert]</strong> </p> <p>Geben Sie den zu suchenden Wert in das ausgewählte Feld ein oder ordnen Sie ihn zu. Der Werttyp sollte mit dem Datentyp des ausgewählten Felds übereinstimmen. </p> <p>Weitere Informationen zu Datentypen finden Sie unter <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Elementdatentypen in [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Result set]</td> 
   <td>Wählen Sie aus, ob Sie das erste übereinstimmende Asset oder alle übereinstimmenden Assets zurückgeben möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sortieren nach]</td> 
   <td> <p>Wählen Sie das Feld aus, nach dem Sie sortieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sortierrichtung]</td> 
   <td> <p>Wählen Sie aus, ob Sie eine aufsteigende oder absteigende Sortierung vornehmen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Felder aus, die Sie in die Ausgabe des Moduls aufnehmen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Assets ein oder ordnen Sie sie zu, die das Modul während des Ausführungsprozesses jedes Szenarios zurückgeben soll.</p> </td> 
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
    <td role="rowheader"> <p>[!UICONTROL Verbindung]</p> </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Bynder] Konto [!DNL Workfront Fusion], siehe <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Bynder] nach [!DNL Workfront Fusion] </a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Event type</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select whether you want to start the scenario when a new asset is created or when an existing asset is updated.</td>
   --> 
  </tr> 
  <tr>
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Sammlungen]</td>
   <td> <p>Wählen Sie die Sammlung aus, die Sie für neue Assets überwachen möchten. Lassen Sie dieses Feld leer, wenn Sie alle Sammlungen überwachen möchten.</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Outputs</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the fields that you want to include in the output.</td>
   --> 
  </tr> 
  <tr> 
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL Limit]</td>

<td> <p>Geben Sie die maximale Anzahl von Datensätzen an, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>
