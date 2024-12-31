---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: Google Docs-Module
description: Mit den Adobe Workfront Fusion [!DNL Google Docs] Modulen können Sie Dokumente in Ihren und/oder  [!DNL Google Docs]  [!DNL Google Docs]  (für  [!DNL Google Workspace] ) überwachen, erstellen bearbeiten und abrufen.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: fbe7d628-d833-43ce-83b8-8e4e6a812fd1
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '4105'
ht-degree: 0%

---

# [!DNL Google Docs]

Mit den [!DNL Adobe Workfront Fusion] [!DNL Google Docs] können Sie Dokumente in Ihren [!DNL Google Docs] und [!DNL Google Docs] (für [!DNL Google Workspace] Benutzer) überwachen, erstellen, bearbeiten und abrufen.

Um [!DNL Google Docs] mit [!DNL Adobe Workfront Fusion] verwenden zu können, muss ein [!DNL Google] Konto vorhanden sein. Wenn Sie noch kein [!DNL Google] Konto haben, können Sie eines auf der Hilfeseite zum [!DNL Google] Konto erstellen.

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

Um [!DNL Google Docs] Module verwenden zu können, müssen Sie über ein Google-Konto verfügen.

## Google Docs-API-Informationen

Der Google Docs-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td> https://docs.googleapis.com/v1</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Version</td> 
   <td> v1 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.4.13</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Google Docs] Module und ihre Felder

Beim Konfigurieren von [!DNL Google Docs]-Modulen zeigt [!UICONTROL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service weitere [!DNL Google Docs] angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Dokument

* [[!UICONTROL Dokumente ansehen]](#watch-documents)
* [[!UICONTROL Dokumente auflisten]](#list-documents)
* [[!UICONTROL Abrufen des Inhalts eines Dokuments]](#get-content-of-a-document)
* [[!UICONTROL Dokument erstellen]](#create-a-document)
* [[!UICONTROL Erstellen eines Dokuments aus einer Vorlage]](#create-a-document-from-a-template)
* [[!UICONTROL Einfügen eines Absatzes in ein Dokument]](#insert-a-paragraph-to-a-document)
* [[!UICONTROL Einfügen eines Bildes in ein Dokument]](#insert-an-image-to-a-document)
* [[!UICONTROL Ersetzen eines Bildes durch ein neues Bild]](#replace-an-image-with-a-new-image)
* [[!UICONTROL Ersetzen von Text in einem Dokument]](#replace-text-in-a-document)
* [[!UICONTROL Dokument herunterladen]](#download-a-document)
* [[!UICONTROL Dokument löschen]](#delete-a-document)

#### [!UICONTROL Dokumente ansehen]

Dieses Ordnermodul gibt Dokumentdetails zurück, wenn ein neues Trigger erstellt oder geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dokumente ansehen]</td> 
   <td> <p style="color: #000000;">Wählen Sie aus, ob die Dokumente Erstellt ([!UICONTROL By Created Date]) oder Geändert ([!UICONTROL By Modified Date]) angezeigt werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, den Sie überwachen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Wählen Sie den Ordner aus, der auf erstellte oder geänderte Dokumente überwacht werden soll.</p> </li> 
     <li> <p><strong>[!UICONTROL für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, der auf erstellte oder geänderte Dokumente überwacht werden soll.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (nur für [!DNL Google Workspace] Benutzer verfügbar)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain-Administratorzugriff verwenden] möchten. Bei Auswahl von [!UICONTROL Yes] wird die Anfrage als Domain-Administrator ausgegeben, und alle freigegebenen Laufwerke, deren Administrator der Anforderer ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, das Sie überwachen möchten.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Shared Drive] in diesem Feld ausgewählt haben und kein [!DNL Google Workspace] Benutzer sind, wird der <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Legen Sie die maximale Anzahl von Dokumenten fest, die Workfront Fusion in einem Ausführungszyklus zurückgibt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Dokumente auflisten]

Dieses Aktionsmodul ruft eine Liste der Dokumente aus dem ausgewählten Ordner ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, von dem Dokumente aufgelistet werden sollen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Wählen Sie den Ordner aus, aus dem Dokumente aufgelistet werden sollen.</p> </li> 
     <li> <p><strong>[!UICONTROL für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, aus dem Dokumente aufgelistet werden sollen.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (nur für [!DNL Google Workspace] Benutzer verfügbar)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain-Administratorzugriff verwenden] möchten. Bei Auswahl von [!UICONTROL Yes] wird die Anfrage als Domain-Administrator ausgegeben, und alle freigegebenen Laufwerke, deren Administrator der Anforderer ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, dessen Dokumente Sie auflisten möchten.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ausgewählt haben und kein [!DNL Google Workspace] Benutzer sind, wird der <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Legen Sie die maximale Anzahl von Dokumenten fest, [!DNL Workfront Fusion] in einem Ausführungszyklus zurückgegeben werden.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Abrufen des Inhalts eines Dokuments]

Dieses Aktionsmodul ruft ein angegebenes Dokument ab.

Möglicherweise müssen Sie Ihre Berechtigungen erweitern.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inhalt eines Dokuments abrufen]</td> 
   <td> <p>Wählen Sie aus, ob Sie die Dokument-ID des Dokuments zuordnen möchten, oder wählen Sie das Dokument aus dem Dropdown-Menü manuell aus.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, der das Dokument enthält, das Sie abrufen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Wählen Sie den Ordner aus, der das Dokument enthält, das Sie abrufen möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, der das Dokument enthält, das Sie abrufen möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (nur für [!DNL Google Workspace] Benutzer verfügbar)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain-Administratorzugriff verwenden] möchten. Bei Auswahl von [!UICONTROL Yes] wird die Anfrage als Domain-Administrator ausgegeben, und alle freigegebenen Laufwerke, deren Administrator der Anforderer ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, das das Dokument enthält, das Sie abrufen möchten.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ausgewählt haben und kein [!DNL Google Workspace] Benutzer sind, wird der <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL filter]</p> </td> 
   <td> <p>Wählen Sie das -Objekt aus, das in der Ausgabe des Moduls zurückgegeben werden soll.</p> 
    <ul> 
     <li>[!UICONTROL Image] (Standard)</li> 
     <li>[!UICONTROL Zeichnung]</li> 
     <li>[!UICONTROL-Diagramm]</li> 
    </ul> <p>Hinweis:  <p>Für weitere Zuordnungen dieser Objekte verwenden Sie bitte den Wert [!UICONTROL Inline Objects Array] in der Ausgabe dieses Moduls (anstelle von [!UICONTROL inlineObjects]).</p> <p>Die [!UICONTROL Inline Objects Array]-Objekte werden in der gleichen Reihenfolge sortiert, in der sie im Dokument erscheinen. Dies erleichtert die weitere Verarbeitung.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Dokument erstellen]

Mit diesem Aktionsmodul können Sie ein neues Dokument im ausgewählten Ordner erstellen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Geben Sie den Namen des Dokuments ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Inhalt]</td> 
   <td> <p>Geben Sie den Inhalt des Dokuments ein. HTML wird unterstützt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, auf dem Sie ein Dokument erstellen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Wählen Sie den Ordner aus, in dem Sie ein Dokument erstellen möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem Sie ein Dokument erstellen möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (nur für [!DNL Google Workspace] Benutzer verfügbar)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain-Administratorzugriff verwenden] möchten. Bei Auswahl von [!UICONTROL Yes] wird die Anfrage als Domain-Administrator ausgegeben, und alle freigegebenen Laufwerke, deren Administrator der Anforderer ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf dem Sie ein Dokument erstellen möchten.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ausgewählt haben und kein [!DNL Google Workspace] Benutzer sind, wird der <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kopfzeile einfügen]</td> 
   <td> <p> Aktivieren Sie diese Option, um die Kopfzeile in das Dokument einzufügen und den Text der Kopfzeile einzugeben oder zuzuordnen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fußzeile einfügen] </td> 
   <td> <p>Aktivieren Sie diese Option, um die Fußzeile in das Dokument einzufügen und dann den Text der Kopfzeile einzugeben oder zuzuordnen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen eines Dokuments aus einer Vorlage]

Dieses Aktionsmodul erstellt eine Kopie eines vorhandenen Vorlagendokuments und ersetzt alle Tags. Dieses Modul ermöglicht es den Benutzern auch, Bilder durch neue Bilder anhand der URL zu ersetzen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Dokument aus Vorlage erstellen]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Wählen Sie diese Option, um die Dokumentvorlage zuzuordnen.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br>Wählen Sie diese Option, um die Dokumentvorlage aus dem Dropdown-Menü auszuwählen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, auf dem sich Ihre Vorlage befindet. Diese Option ist verfügbar, wenn Sie im vorherigen Feld [!UICONTROL By Dropdown] ausgewählt haben.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich Ihre Vorlage befindet.</p> </li> 
     <li> <p><strong>[!UICONTROL für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich Ihre Vorlage befindet.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (nur für [!DNL Google Workspace] Benutzer verfügbar)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain-Administratorzugriff verwenden] möchten. Bei Auswahl von [!UICONTROL Yes] wird die Anfrage als Domain-Administrator ausgegeben, und alle freigegebenen Laufwerke, deren Administrator der Anforderer ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf dem sich Ihre Vorlage befindet.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ausgewählt haben und kein [!DNL Google Workspace] Benutzer sind, wird der <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Werte]</p> </td> 
   <td> <p>Geben Sie die Werte ein, die anstelle der Variablen in das neue Dokument eingegeben werden sollen.</p> 
    <ul> 
     <li><strong>[!UICONTROL Tags]</strong><br>Geben Sie die Tags ein, die in der Dokumentvorlage enthalten sind. Verwenden Sie <code>&#123;&#123;&#125;&#125;</code> nicht. Beispiel: Verwenden Sie <code>name</code> anstelle von <code>&#123;&#123;name&#125;&#125;</code>.</li> 
     <li><strong>[!UICONTROL Replace Value]</strong><br>Geben Sie den Wert des Tags ein.</li> 
    </ul> <p>Beispielsweise wird die Variable <code> &#123;&#123;name&#125;&#125;</code> Quelldokument hier als Namensfeld angezeigt, in das der Wert eingefügt werden kann, z. B. <code>John</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Images Replacement]</p> </td> 
   <td> <p>Geben Sie den Link zur [!UICONTROL Bildobjekt-ID] und [!UICONTROL Bildobjekt-URL] ein, die das aktuelle Bild ersetzen sollen.</p> <p>Hinweis: Sie können die Bild-IDs mit dem Modul [!UICONTROL Dokument abrufen] abrufen, wobei die IDs im Array [!UICONTROL Inline Object Array] enthalten sind.</p> <p>Es wird empfohlen, Bildern in Ihrem [!DNL Google]-Dokument ALT-Text hinzuzufügen. </p> <p>So fügen Sie dem [!DNL Google Docs] einen ALT-Text hinzu:</p> 
    <ol> 
     <li value="1">Rechtsklick auf das Bild.</li> 
     <li value="2">Wählen Sie die Option [!UICONTROL ALT text].</li> 
     <li value="3">Geben Sie den [!UICONTROL ALT-Text] in das Feld [!UICONTROL Title] ein und klicken Sie auf [!UICONTROL OK].</li> 
    </ol> <p>Nachdem der ALT-Text zum Bild hinzugefügt wurde, wird der ALT-Text im Feldnamen in Klammern angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Titel] </td> 
   <td> <p>Geben Sie den Namen für das neue Dokument ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, auf dem sich Ihre Vorlage befindet. Diese Option ist verfügbar, wenn Sie im vorherigen Feld [!UICONTROL By Dropdown] ausgewählt haben.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Wählen Sie den Ordner aus, in dem das Dokument erstellt werden soll.</p> </li> 
     <li> <p><strong>[!UICONTROL für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem das Dokument erstellt werden soll.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (nur für [!DNL Google Workspace] Benutzer verfügbar)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain-Administratorzugriff verwenden] möchten. Bei Auswahl von [!UICONTROL Yes] wird die Anfrage als Domain-Administrator ausgegeben, und alle freigegebenen Laufwerke, deren Administrator der Anforderer ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf dem das Dokument erstellt werden soll.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ausgewählt haben und kein [!DNL Google Workspace] Benutzer sind, wird der <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Einfügen eines Absatzes in ein Dokument]

Dieses Aktionsmodul fügt einen neuen Absatz an ein vorhandenes Dokument an oder fügt ihn ein.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Dokument auswählen]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Wählen Sie diese Option, um das Dokument zuzuordnen.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> Wählen <br> diese Option, um das Dokument aus dem Dropdown-Menü auszuwählen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, auf dem sich das Dokument befindet, dem Sie einen Absatz hinzufügen möchten. Diese Option ist verfügbar, wenn Sie im vorherigen Feld [!UICONTROL By Dropdown] ausgewählt haben.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, dem Sie einen Absatz hinzufügen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, dem Sie einen Absatz hinzufügen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (nur für [!DNL Google Workspace] Benutzer verfügbar)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain-Administratorzugriff verwenden] möchten. Bei Auswahl von [!UICONTROL Yes] wird die Anfrage als Domain-Administrator ausgegeben, und alle freigegebenen Laufwerke, deren Administrator der Anforderer ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf dem sich das Dokument befindet, dem Sie einen Absatz hinzufügen möchten, und wählen Sie dann das Dokument aus.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ausgewählt haben und kein [!DNL Google Workspace] Benutzer sind, wird der <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Absatz einfügen]</p> </td> 
   <td> <p>Wählen Sie aus, wie der neue Text in das Dokument eingefügt werden soll.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nach Angabe des Ortes]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL nach Index]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Index]</strong> </p> <p>Geben Sie die Indexnummer ein, unter der Sie Ihren Text einfügen möchten. Sie können das Modul [!UICONTROL Dokument abrufen] zum Abrufen der Indexnummer verwenden.</p> <p>Um alle Zeichen (einschließlich ausgeblendeter) im Dokument anzuzeigen, können Sie das Add-on [!UICONTROL Anzeigen] verwenden. Das Add-on finden Sie unter [!UICONTROL Add-ons] &gt; [!UICONTROL Get Add-ons]. Suchen Sie nach [!UICONTROL Show] und installieren Sie das Add-on [!UICONTROL Show].</p> </li> 
         <li> <p><strong>[!UICONTROL eingefügter Text]</strong> </p> <p>Geben Sie den Text ein, den Sie in das Dokument einfügen möchten.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL nach Segment-ID]</strong> </p> <p>Wählen Sie die Kopf- und Fußzeile aus, in die Sie den Textinhalt einfügen möchten, und geben Sie den einzufügenden Text in die entsprechenden Felder ein.</p> <p>Wenn die Kopf- oder Fußzeile bereits Text enthält, wird der neue Text vor dem vorhandenen Text hinzugefügt.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Durch Anhängen von an den Hauptteil des Dokuments]</strong> </p> <p>Hängt den eingegebenen Text am Ende des Textinhalts des Dokuments an.</p> <p>Der Stil des neuen Absatzes wird am aktuellen Einfügeindex aus dem Absatz kopiert, einschließlich Listen und Aufzählungszeichen.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Durch Anhängen von an das Ende des Segments (Kopf- und Fußzeile)]</strong> </p> <p>Wählen Sie die Kopf- und Fußzeile aus, in die Sie den Textinhalt einfügen möchten, und geben Sie den einzufügenden Text in die entsprechenden Felder ein.</p> <p>Wenn die Kopf- oder Fußzeile bereits Text enthält, wird der neue Text nach dem vorhandenen Text hinzugefügt.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL angehängter Text]</td> 
   <td>Text eingeben oder zuordnen, der an das Dokument angehängt werden soll</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Einfügen eines Bildes in ein Dokument]

Dieses Aktionsmodul fügt ein Bild aus der URL in das Dokument ein.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Dokument auswählen]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Wählen Sie diese Option, um die Dokumentvorlage zuzuordnen.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> Wählen <br> diese Option, um das Dokument aus dem Dropdown-Menü auszuwählen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, auf dem sich das Dokument befindet, dem Sie ein Bild hinzufügen möchten. Diese Option ist verfügbar, wenn Sie im vorherigen Feld [!UICONTROL By Dropdown] ausgewählt haben.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, dem Sie ein Bild hinzufügen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, dem Sie ein Bild hinzufügen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (nur für [!DNL Google Workspace] Benutzer verfügbar)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain-Administratorzugriff verwenden] möchten. Bei Auswahl von [!UICONTROL Yes] wird die Anfrage als Domain-Administrator ausgegeben, und alle freigegebenen Laufwerke, deren Administrator der Anforderer ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf dem sich das Dokument befindet, dem Sie ein Bild hinzufügen möchten, und wählen Sie dann das Dokument aus.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ausgewählt haben und kein [!DNL Google Workspace] Benutzer sind, wird der <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bild einfügen]</p> </td> 
   <td> <p>Auswählen, wie das neue Bild in das Dokument eingefügt werden soll.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nach Angabe des Ortes]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL nach Index]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Index]</strong> </p> <p>Geben Sie die Indexnummer ein, unter der Sie Ihr Bild einfügen möchten. Sie können das Modul [!UICONTROL Dokument abrufen] verwenden, um [!UICONTROL Indexnummer] abzurufen.</p> <p>Um alle Zeichen (einschließlich ausgeblendeter) im Dokument anzuzeigen, können Sie das Add-on [!UICONTROL Anzeigen] verwenden. Das Add-on finden Sie unter [!UICONTROL Add-ons] &gt; [!UICONTROL Get Add-ons]. Suchen Sie nach [!UICONTROL Show] und installieren Sie das Add-on [!UICONTROL Show].</p> </li> 
         <li> <p><strong>[!UICONTROL Bild URL]</strong> </p> <p>Geben Sie die URL des Bildes ein, das Sie in das Dokument einfügen möchten.</p> <p>Die maximale Bildgröße beträgt 50 MB. Darf 25 Megapixel nicht überschreiten. Es wird nur das PNG-, JPEG- oder GIF-Format unterstützt.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL nach Segment-ID]</strong> </p> <p>Wählen Sie die Kopf- und Fußzeile aus, in die Sie das Bild einfügen möchten, und geben Sie die Bild-URL in die entsprechenden Felder ein.</p> <p>Die maximale Bildgröße beträgt 50 MB. Das Bild darf 25 Megapixel nicht überschreiten. Es wird nur das PNG-, JPEG- oder GIF-Format unterstützt.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Durch Anhängen von an den Hauptteil des Dokuments]</strong> </p> <p>Hängt ein bestimmtes Bild an das Ende des Textinhalts des Dokuments an.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Durch Anhängen von an das Ende des Segments (Kopf- und Fußzeile)]</strong> </p> <p>Wählen Sie die Kopf- und Fußzeile aus, in die Sie ein Bild einfügen möchten, und geben Sie die Bild-URL ein, die Sie in die entsprechenden Felder einfügen möchten.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Höhe Betrag in Punkt/Breite Betrag in Punkt]</p> </td> 
   <td> <p>Definieren Sie die Größe des eingefügten Bildes. Das Seitenverhältnis wird beibehalten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ersetzen eines Bildes durch ein neues Bild]

Dieses Aktionsmodul ersetzt ein vorhandenes Bild. Das Seitenverhältnis des Originalbilds wird beibehalten.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Dokument auswählen]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Wählen Sie diese Option, um die Dokumentvorlage zuzuordnen.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> Wählen <br> diese Option, um das Dokument aus dem Dropdown-Menü auszuwählen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, auf dem sich das Dokument befindet, das Sie durch ein Bild ersetzen möchten. Diese Option ist verfügbar, wenn Sie im vorherigen Feld [!UICONTROL By Dropdown] ausgewählt haben.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, das Sie durch ein Bild ersetzen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, das Sie durch ein Bild ersetzen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (nur für [!DNL Google Workspace] Benutzer verfügbar)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain-Administratorzugriff verwenden] möchten. Bei Auswahl von [!UICONTROL Yes] wird die Anfrage als Domain-Administrator ausgegeben, und alle freigegebenen Laufwerke, deren Administrator der Anforderer ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf dem sich das Dokument befindet, das Sie durch ein Bild ersetzen möchten, und wählen Sie dann das Dokument aus.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ausgewählt haben und kein [!DNL Google Workspace] Benutzer sind, wird der <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bild-URL]</p> </td> 
   <td> <p>Geben Sie die URL des neuen Bildes, das das vorhandene Bild ersetzen soll, ein oder mappen Sie sie.</p> <p>Bilder werden in der Reihenfolge aufgelistet, in der sie im Dokument angezeigt werden. Beispielsweise ist <code>Body: Image No. 1</code> das erste Bild im Dokument.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ersetzen von Text in einem Dokument]

Dieses Aktionsmodul ersetzt Text in einem Dokument.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Dokument auswählen]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Wählen Sie diese Option, um die Dokumentvorlage zuzuordnen.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> Wählen <br> diese Option, um das Dokument aus dem Dropdown-Menü auszuwählen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, auf dem sich das Dokument befindet, dem Sie Text hinzufügen möchten. Diese Option ist verfügbar, wenn Sie im vorherigen Feld [!UICONTROL By Dropdown] ausgewählt haben.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, dem Sie Text hinzufügen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, dem Sie Text hinzufügen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (nur für [!DNL Google Workspace] Benutzer verfügbar)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain-Administratorzugriff verwenden] möchten. Bei Auswahl von [!UICONTROL Yes] wird die Anfrage als Domain-Administrator ausgegeben, und alle freigegebenen Laufwerke, deren Administrator der Anforderer ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf dem sich das Dokument befindet, dem Sie Text hinzufügen möchten, und wählen Sie dann das Dokument aus.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ausgewählt haben und kein [!DNL Google Workspace] Benutzer sind, wird der <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Text ersetzen]</p> </td> 
   <td> <p>Fügen Sie jeden Text hinzu, den Sie ersetzen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Alter Text, der ersetzt werden soll]</strong> </p> <p>Geben Sie den Text ein, den Sie ersetzen möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL Neuer einzufügender Text]</strong> </p> <p>Geben Sie den neuen Text ein.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Dokument herunterladen]

Dieses Aktionsmodul konvertiert das ausgewählte Dokument und lädt es herunter.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, auf dem sich das Dokument befindet, das Sie herunterladen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das herunterzuladende Dokument befindet, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das herunterzuladende Dokument befindet, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (nur für [!DNL Google Workspace] Benutzer verfügbar)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain-Administratorzugriff verwenden] möchten. Bei Auswahl von [!UICONTROL Yes] wird die Anfrage als Domain-Administrator ausgegeben, und alle freigegebenen Laufwerke, deren Administrator der Anforderer ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf das sich das Dokument befindet, das Sie herunterladen möchten, und wählen Sie dann das Dokument aus.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ausgewählt haben und kein [!DNL Google Workspace] Benutzer sind, wird der <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Typ] </p> </td> 
   <td> <p>Zieldateiformat des heruntergeladenen Dokuments auswählen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Dokument löschen]

Dieses Aktionsmodul löscht ein Dokument.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, auf dem sich das zu löschende Dokument befindet.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das zu löschende Dokument befindet, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das zu löschende Dokument befindet, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (nur für [!DNL Google Workspace] Benutzer verfügbar)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain-Administratorzugriff verwenden] möchten. Bei Auswahl von [!UICONTROL Yes] wird die Anfrage als Domain-Administrator ausgegeben, und alle freigegebenen Laufwerke, deren Administrator der Anforderer ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf dem sich das zu löschende Dokument befindet, und wählen Sie dann das Dokument aus.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ausgewählt haben und kein [!DNL Google Workspace] Benutzer sind, wird der <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Shared Drive]</td> 
   <td> <p>Wählen Sie das Laufwerk aus, das das Dokument enthält, das Sie herunterladen möchten, und wählen Sie dann ein Dokument aus. Diese Option ist verfügbar, wenn Sie [!DNL Google Docs] im Feld [!UICONTROL Laufwerk auswählen] ausgewählt haben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dokument-ID]</td> 
   <td> <p> Wählen Sie das Dokument aus, in dem Sie ein oder mehrere Bilder ersetzen möchten, oder ordnen Sie es zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Sonstige

* [[!UICONTROL Erstellen eines API-Aufrufs]](#make-an-api-call)
* [[!UICONTROL Alle Links in einem Dokument können angeklickt werden]](#make-all-links-in-a-document-clickable)

#### [!UICONTROL Erstellen eines API-Aufrufs]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten API-Aufruf durchführen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Geben Sie einen Pfad relativ zu <code>https://docs.googleapis.com/</code> ein. Beispiel: <code>/v1/documents/{presentationID}</code>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Methode]</td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-Anfragemethoden in [!DNL Adobe Workfront Fusion]</a>.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Kopfzeilen]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu, z. B. <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p> Geben Sie die Abfragezeichenfolge der Anfrage ein.</p> </td> 
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

**Beispiel:** Der folgende API-Aufruf ruft die Details für das angegebene Dokument in Ihren Google-Dokumenten ab:

**URL:**

/v1/documents/1ujkf-GDgB0TQSYPrxbCSK4Uso54tHVMqHZEVZZxB6aY

**Methode:**

[!UICONTROL GET]

![](assets/api-call-example.png)

Details zum abgerufenen Dokument finden Sie in der Ausgabe des Moduls unter [!UICONTROL Bundle] > [!UICONTROL Body].

![](assets/api-output.png)

#### [!UICONTROL Alle Links in einem Dokument können angeklickt werden]

Dieses Aktionsmodul findet alle Links im Dokument und macht sie anklickbar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden der Mobile App oder des Webservices des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Alle Links in einem Dokument erstellen]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Wählen Sie diese Option, um die Dokumentvorlage zuzuordnen.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> Wählen <br> diese Option, um das Dokument aus dem Dropdown-Menü auszuwählen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, auf dem sich das Dokument befindet, auf das Links geklickt werden sollen. Diese Option ist verfügbar, wenn Sie im vorherigen Feld [!UICONTROL By Dropdown] ausgewählt haben.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, auf das Sie auf Links klicken möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, auf das Sie auf Links klicken möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (nur für [!DNL Google Workspace] Benutzer verfügbar)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain-Administratorzugriff verwenden] möchten. Bei Auswahl von [!UICONTROL Yes] wird die Anfrage als Domain-Administrator ausgegeben, und alle freigegebenen Laufwerke, deren Administrator der Anforderer ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf dem sich das Dokument befindet, auf das Sie Links klicken möchten, und wählen Sie dann das Dokument aus.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ausgewählt haben und kein [!DNL Google Workspace] Benutzer sind, wird der <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Shared Drive]</td> 
   <td> <p>Wählen Sie das Laufwerk aus, das das Dokument enthält, in dem Links aktualisiert werden sollen, und wählen Sie dann ein Dokument aus. Diese Option ist verfügbar, wenn Sie [!DNL Google Docs] im Feld [!UICONTROL Laufwerk auswählen] ausgewählt haben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dokument-ID]</td> 
   <td> <p> Wählen Sie das Dokument aus, in dem Sie die Links aktualisieren möchten, oder ordnen Sie es zu.</p> </td> 
  </tr> 
 </tbody> 
</table>
