---
title: Breitenmodule
description: In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!UICONTROL Erweitert] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: d46935bc-4f6c-4502-bd2f-3927f33241e1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1582'
ht-degree: 1%

---

# [!DNL Widen] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!UICONTROL Erweitert] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

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

Um die Module [!UICONTROL WAN] zu verwenden, müssen Sie über ein [!UICONTROL WAN] -Konto verfügen.

## [!DNL Widen] mit [!DNL Workfront Fusion] verbinden {#connect-widen-to-workfront-fusion}

Sie können eine Verbindung zu Ihrem [!DNL Widen]-Konto direkt aus einem [!DNL Widen]-Modul erstellen.

1. Klicken Sie in einem beliebigen [!DNL Widen]-Modul neben dem Feld [!UICONTROL Verbindung] auf **[!UICONTROL Hinzufügen]** .
1. Wählen Sie die Domäne [!DNL Widen] aus, mit der Sie eine Verbindung herstellen möchten.
1. Geben Sie das Token für Ihr [!DNL Widen] -Konto ein. Anweisungen zum Auffinden dieses Tokens finden Sie in den [[!DNL Widen] API-FAQs](https://community.widen.com/collective/s/article/API-FAQs).
1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

## [!DNL Widen] Module und ihre Felder

Wenn Sie [!DNL Widen] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Widen] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger-Module](#trigger-modules)
* [Aktionsmodule](#action-modules)
* [Suchmodule](#search-modules)

### Trigger-Module

#### [!UICONTROL Assets ansehen]

Dieses Trigger-Modul startet ein Szenario, wenn ein Asset erstellt oder aktualisiert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Widen]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Widen] mit [!DNL Workfront Fusion] </a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ereignistyp]</td> 
   <td> <p>Wählen Sie aus, ob Sie neue Assets oder aktualisierte Assets anzeigen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>Wählen Sie zusätzlich zu den Asset-Feldern die Eigenschaften aus, die Sie in die Modulausgabe einbeziehen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td>Wählen Sie die Felder aus, die Sie in die Modulausgabe einbeziehen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Assets ein oder ordnen Sie sie zu, mit denen das Modul während jedes Szenario-Ausführungszyklus arbeiten soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionsmodule

* [[!UICONTROL Benutzerspezifischer API-Aufruf]](#custom-api-call)
* [[!UICONTROL Asset-Informationen lesen]](#read-asset-info)
* [[!UICONTROL Hinzufügen von Assets zu Sammlungen]](#add-assets-to-collections)
* [[!UICONTROL Entfernen von Assets aus der Sammlung]](#remove-assets-from-collection)
* [[!UICONTROL Aktualisieren von Asset-Metadaten]](#update-asset-metadata)
* [[!UICONTROL Datei herunterladen]](#download-file)
* [[!UICONTROL  Hochladen] einer Datei](#upload-a-file)

#### [!UICONTROL Benutzerspezifischer API-Aufruf]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Widen] -API durchführen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von anderen [!DNL Widen] -Modulen nicht ausgeführt werden kann.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Widen]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Widen] mit [!DNL Workfront Fusion] </a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API-Version]</td> 
   <td>Wählen Sie aus, ob Sie die neueste Version der [!DNL Widen] -API oder Version 1.0 verwenden möchten</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Geben Sie die URL für Ihren API-Aufruf ein oder ordnen Sie sie zu.</td> 
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

#### [!UICONTROL Asset-Informationen lesen]

Dieses Aktionsmodul ruft ein einzelnes Asset anhand seiner eindeutigen ID ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Widen]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Widen] mit [!DNL Workfront Fusion] </a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-ID]</td> 
   <td> <p>Geben Sie die ID des Assets ein, für das Sie Informationen lesen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>Wählen Sie zusätzlich zu den Asset-Feldern die Eigenschaften aus, die Sie in die Modulausgabe einbeziehen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td>Wählen Sie die Felder aus, die Sie in die Modulausgabe einbeziehen möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Hinzufügen von Assets zu Sammlungen]

Dieses Aktionsmodul fügt Sammlungen ein oder mehrere Assets hinzu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Widen]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Widen] mit [!DNL Workfront Fusion] </a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sammlungs-ID]</td> 
   <td> <p>Für jede Sammlung, zu der Sie die Assets hinzufügen möchten:</p> 
    <ol> 
     <li value="1"> <p> Klicken Sie auf <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Geben Sie die [!UICONTROL Collection ID] ein oder ordnen Sie sie zu.</p> </li> 
     <li value="3"> <p>Klicken Sie auf <strong>[!UICONTROL Element hinzufügen]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assets ID]</td> 
   <td> <p>Für jedes Asset, das Sie einer Sammlung hinzufügen möchten:</p> 
    <ol> 
     <li value="1"> <p> Klicken Sie auf <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Geben Sie die Asset-ID ein oder ordnen Sie sie zu.</p> </li> 
     <li value="3"> <p>Klicken Sie auf <strong>[!UICONTROL Element hinzufügen]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Assets ein oder ordnen Sie sie zu, mit denen das Modul während jedes Szenario-Ausführungszyklus arbeiten soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Entfernen von Assets aus der Sammlung]

Dieses Aktionsmodul entfernt mindestens ein Asset aus Sammlungen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Widen]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Widen] mit [!DNL Workfront Fusion] </a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sammlungs-ID]</td> 
   <td> <p>Für jede Sammlung, aus der Sie die Assets entfernen möchten:</p> 
    <ol> 
     <li value="1"> <p> Klicken Sie auf <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Geben Sie die Sammlungs-ID ein oder ordnen Sie sie zu.</p> </li> 
     <li value="3"> <p>Klicken Sie auf <strong>[!UICONTROL Element hinzufügen]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ASSETS ID</td> 
   <td> <p>Für jedes Asset, das Sie aus einer Sammlung entfernen möchten:</p> 
    <ol> 
     <li value="1"> <p> Klicken Sie auf <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Geben Sie die Asset-ID ein oder ordnen Sie sie zu.</p> </li> 
     <li value="3"> <p>Klicken Sie auf <strong>[!UICONTROL Element hinzufügen]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Assets ein oder ordnen Sie sie zu, mit denen das Modul während jedes Szenario-Ausführungszyklus arbeiten soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aktualisieren von Asset-Metadaten]

Dieses Aktionsmodul aktualisiert die Metadatenfelder eines Assets.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Widen]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Widen] mit [!DNL Workfront Fusion] </a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-ID]</td> 
   <td> <p>Geben Sie die ID des Assets ein oder ordnen Sie sie zu, in dem Sie Metadaten aktualisieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadatentyp]</td> 
   <td> <p>Wählen Sie den Metadatentyp für die Metadaten aus, die Sie aktualisieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadaten]</td> 
   <td>Wählen Sie die Metadatenfelder aus, die Sie aktualisieren möchten. Geben Sie für jedes Feld den neuen Wert für das Feld ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Assets ein oder ordnen Sie sie zu, mit denen das Modul während jedes Szenario-Ausführungszyklus arbeiten soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei herunterladen]

Dieses Aktionsmodul lädt ein Asset aus Ihrem [!DNL Widen]-Konto herunter.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Widen]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Widen] mit [!DNL Workfront Fusion] </a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-ID]</td> 
   <td> <p>Geben Sie die ID des Assets ein, das Sie herunterladen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL  Datei hochladen]

Dieses Aktionsmodul lädt eine Datei in Ihr [!DNL Widen] -Konto hoch.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Widen]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Widen] mit [!DNL Workfront Fusion] </a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Profil hochladen:</td> 
   <td> <p>Wählen Sie das Upload-Profil aus, das das Modul verwenden soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Upload-Methode]</td> 
   <td> <p>Wählen Sie aus, wie die Datei hochgeladen werden soll.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL from File]</strong> </p> <p>Wählen Sie die Quelldatei aus einem vorherigen Modul aus oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Nach URL]</strong> </p> <p>Geben Sie die URL der Datei ein oder ordnen Sie sie zu.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dateiname]</td> 
   <td>Geben Sie einen Namen für die hochgeladene Datei ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadatentyp]</td> 
   <td>Wählen Sie den Metadatentyp für die Datei aus, die Sie hochladen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadaten]</td> 
   <td>Wählen Sie die Metadatenfelder aus, die Sie in den Datei-Upload einbeziehen möchten. Geben Sie für jedes Feld den [!UICONTROL Wert] für das Feld ein.</td> 
  </tr> 
 </tbody> 
</table>

### Suchmodule

* [[!UICONTROL Lesen von Sammlungs-Assets]](#read-collection-assets)
* [[!UICONTROL Assets durchsuchen]](#search-assets)

#### [!UICONTROL Lesen von Sammlungs-Assets]

Dieses Aktionsmodul ruft eine Liste von Assets innerhalb einer Sammlung ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Widen]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Widen] mit [!DNL Workfront Fusion] </a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collection ID]</td> 
   <td> <p>Geben Sie die ID der Sammlung ein, die die Assets enthält, die Sie lesen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start]</td> 
   <td>Geben Sie die Nummer des ersten Elements ein, das Sie auflisten möchten, oder ordnen Sie sie zu. Auf diese Weise können Sie die Datensätze paginieren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sortieren nach:</td> 
   <td> <p>Wählen Sie die Eigenschaft aus, nach der Sie die Assets sortieren möchten. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order]</td> 
   <td>Wählen Sie aus, ob Sie Assets auf- oder absteigend sortieren möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td>Wählen Sie die Felder aus, die Sie in die Modulausgabe einbeziehen möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Assets durchsuchen]

Dieses Suchmodul ruft eine Liste von Assets ab, die den jeweiligen Suchkriterien entsprechen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
  <td> <p>Anweisungen zum Verbinden Ihres [!DNL Widen]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Widen] mit [!DNL Workfront Fusion] </a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suchabfrage]</td> 
   <td> <p>Geben Sie die Kriterien ein, nach denen Sie nach Assets suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sortieren nach:</td> 
   <td> <p>Wählen Sie aus, wie Sie die Assets sortieren möchten. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order]</td> 
   <td>Wählen Sie aus, ob Sie Assets auf- oder absteigend sortieren möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Einschließen gelöscht]</td> 
   <td>Aktivieren Sie diese Option, um gelöschte Assets in die Suche einzuschließen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Include archived]</p> </td> 
   <td> <p>Aktivieren Sie diese Option, um archivierte Assets in die Suche einzuschließen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suchdokumenttext]</td> 
   <td>Aktivieren Sie diese Option, um Dokumenttext in die Suche einzuschließen, oder false , um nur Assets einzuschließen, für die der Titel den Suchkriterien entspricht.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Offset]</td> 
   <td>Geben Sie die Nummer des ersten Elements ein, für das Sie Details abrufen möchten, oder ordnen Sie sie zu. Auf diese Weise können Sie die Datensätze paginieren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scroll]</td> 
   <td>Aktivieren Sie diese Option, um das Scrollen zu ermöglichen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>Wählen Sie zusätzlich zu den Asset-Feldern die Eigenschaften aus, die Sie in die Modulausgabe einbeziehen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td>Wählen Sie die Felder aus, die Sie in die Modulausgabe einbeziehen möchten.</td> 
  </tr> 
 </tbody> 
</table>
