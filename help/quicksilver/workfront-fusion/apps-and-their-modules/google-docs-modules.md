---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connector
navigation-topic: apps-and-their-modules
title: Google Docs-Module
description: Die Adobe Workfront-Fusion [!DNL Google Docs] -Module ermöglichen es Ihnen, Dokumente in Ihrer [!DNL Google Docs] und [!DNL Google Docs] (für [!DNL G Suite]-Benutzer).
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: fbe7d628-d833-43ce-83b8-8e4e6a812fd1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '4090'
ht-degree: 0%

---

# [!DNL Google Docs]-Module

Die [!DNL Adobe Workfront Fusion] [!DNL Google Docs] -Module ermöglichen es Ihnen, Dokumente in Ihrer [!DNL Google Docs] und [!DNL Google Docs] (für [!DNL G Suite] Benutzer).

Zur Verwendung [!DNL Google Docs] mit [!DNL Adobe Workfront Fusion], muss ein [!DNL Google] -Konto. Wenn Sie keine [!DNL Google] -Konto erstellen können, können Sie eines im [!DNL Google] Hilfeseite für Konten.

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
   <td>
   <p>Aktuelle Lizenzanforderungen: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Ältere Lizenzanforderungen: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderungen: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Ältere Produktanforderungen: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Verwendung [!DNL Google Docs] -Module verwenden, müssen Sie über ein Google-Konto verfügen.

## [!DNL Google Docs] Module und ihre Felder

Bei der Konfiguration [!DNL Google Docs] Module, [!UICONTROL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Google Docs] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Dokument

* [[!UICONTROL Dokumente ansehen]](#watch-documents)
* [[!UICONTROL Auflisten von Dokumenten]](#list-documents)
* [[!UICONTROL Inhalt eines Dokuments abrufen]](#get-content-of-a-document)
* [[!UICONTROL Dokument erstellen]](#create-a-document)
* [[!UICONTROL Erstellen eines Dokuments aus einer Vorlage]](#create-a-document-from-a-template)
* [[!UICONTROL Einfügen eines Absatzes in ein Dokument]](#insert-a-paragraph-to-a-document)
* [[!UICONTROL Einfügen eines Bildes in ein Dokument]](#insert-an-image-to-a-document)
* [[!UICONTROL Ersetzen eines Bildes durch ein neues Bild]](#replace-an-image-with-a-new-image)
* [[!UICONTROL Text in einem Dokument ersetzen]](#replace-text-in-a-document)
* [[!UICONTROL Dokument herunterladen]](#download-a-document)
* [[!UICONTROL Löschen eines Dokuments]](#delete-a-document)

#### [!UICONTROL Dokumente ansehen]

Dieses Trigger-Modul gibt Dokumentdetails zurück, wenn ein neues Dokument im ausgewählten Ordner erstellt oder geändert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dokumente ansehen]</td> 
   <td> <p style="color: #000000;">Wählen Sie aus, ob die erstellten ([!UICONTROL By Created Date]) oder geänderten ([!UICONTROL By Modified Date]) Dokumente angezeigt werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den zu überwachenden Laufwerkstyp aus.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mein Laufwerk]</strong> </p> <p>Wählen Sie den Ordner aus, den Sie für erstellte oder geänderte Dokumente überwachen möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL Für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, den Sie für erstellte oder geänderte Dokumente überwachen möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Freigegebenes Laufwerk]</strong> (verfügbar für [!DNL G Suite] nur Benutzer)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain Admin Access] verwenden möchten. Wenn Sie [!UICONTROL Ja] auswählen, wird die Anfrage als Domain-Administrator ausgegeben und alle freigegebenen Laufwerke, bei denen der Anforderer ein Administrator ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, das Sie sehen möchten.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Shared Drive] in diesem Feld ein und Sie sind keine [!DNL G Suite] Benutzer, der Fehler <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Legen Sie die maximale Anzahl der von Workfront Fusion zurückgegebenen Dokumente in einem Ausführungszyklus fest.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Auflisten von Dokumenten]

Dieses Aktionsmodul ruft eine Liste von Dokumenten aus dem ausgewählten Ordner ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, aus dem Sie Dokumente auflisten möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mein Laufwerk]</strong> </p> <p>Wählen Sie den Ordner aus, aus dem Sie Dokumente auflisten möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL Für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, aus dem Sie Dokumente auflisten möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Freigegebenes Laufwerk]</strong> (verfügbar für [!DNL G Suite] nur Benutzer)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain Admin Access] verwenden möchten. Wenn Sie [!UICONTROL Ja] auswählen, wird die Anfrage als Domain-Administrator ausgegeben und alle freigegebenen Laufwerke, bei denen der Anforderer ein Administrator ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, aus dem Dokumente aufgelistet werden sollen.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ein und Sie sind keine [!DNL G Suite] Benutzer, der Fehler <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Maximale Anzahl an Dokumenten festlegen [!DNL Workfront Fusion] in einem Ausführungszyklus zurückgibt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Inhalt eines Dokuments abrufen]

Dieses Aktionsmodul ruft ein angegebenes Dokument ab.

Möglicherweise müssen Sie Ihre Berechtigungen erweitern.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inhalt eines Dokuments abrufen]</td> 
   <td> <p>Wählen Sie aus, ob Sie die Dokument-ID des Dokuments zuordnen möchten, oder wählen Sie das Dokument manuell aus dem Dropdown-Menü aus.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, der das Dokument enthält, das Sie abrufen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mein Laufwerk]</strong> </p> <p>Wählen Sie den Ordner aus, der das Dokument enthält, das Sie abrufen möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL Für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, der das Dokument enthält, das Sie abrufen möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Freigegebenes Laufwerk]</strong> (verfügbar für [!DNL G Suite] nur Benutzer)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain Admin Access] verwenden möchten. Wenn Sie [!UICONTROL Ja] auswählen, wird die Anfrage als Domain-Administrator ausgegeben und alle freigegebenen Laufwerke, bei denen der Anforderer ein Administrator ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, das das Dokument enthält, das Sie abrufen möchten.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ein und Sie sind keine [!DNL G Suite] Benutzer, der Fehler <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>Wählen Sie das Objekt aus, das in der Ausgabe des Moduls zurückgegeben werden soll.</p> 
    <ul> 
     <li>[!UICONTROL Bild] (Standard)</li> 
     <li>[!UICONTROL Drawing]</li> 
     <li>[!UICONTROL Diagramm]</li> 
    </ul> <p>Notiz:  <p>Verwenden Sie für die weitere Zuordnung dieser Objekte den Wert [!UICONTROL Inline Objects Array] in der Ausgabe dieses Moduls (anstelle von [!UICONTROL inlineObjects]).</p> <p>Die [!UICONTROL Inline Objects Array]-Objekte werden in derselben Reihenfolge sortiert, in der sie im Dokument angezeigt werden. Dadurch wird jede weitere Verarbeitung erleichtert.</p> </p> </td> 
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
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Geben Sie den Namen des Dokuments ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content]</td> 
   <td> <p>Geben Sie den Inhalt des Dokuments ein. HTML wird unterstützt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, auf dem Sie ein Dokument erstellen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mein Laufwerk]</strong> </p> <p>Wählen Sie den Ordner aus, in dem Sie ein Dokument erstellen möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL Für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem Sie ein Dokument erstellen möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Freigegebenes Laufwerk]</strong> (verfügbar für [!DNL G Suite] nur Benutzer)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain Admin Access] verwenden möchten. Wenn Sie [!UICONTROL Ja] auswählen, wird die Anfrage als Domain-Administrator ausgegeben und alle freigegebenen Laufwerke, bei denen der Anforderer ein Administrator ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf dem Sie ein Dokument erstellen möchten.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ein und Sie sind keine [!DNL G Suite] Benutzer, der Fehler <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header einfügen]</td> 
   <td> <p> Aktivieren Sie diese Option, um die Kopfzeile in das Dokument einzufügen, und geben Sie dann den Text der Kopfzeile ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fußzeile einfügen] </td> 
   <td> <p>Aktivieren Sie diese Option, um die Fußzeile zum Dokument einzufügen, und geben Sie dann den Text der Kopfzeile ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen eines Dokuments aus einer Vorlage]

Dieses Aktionsmodul erstellt eine Kopie eines vorhandenen Vorlagendokuments und ersetzt alle Tags. Dieses Modul ermöglicht es Benutzern auch, Bilder durch neue Bilder nach URL zu ersetzen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Dokument aus einer Vorlage erstellen]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Nach Zuordnung]</strong> <br>Wählen Sie diese Option, um die Dokumentvorlage zuzuordnen.</li> 
     <li><strong>[!UICONTROL Nach Dropdown]</strong> <br>Wählen Sie diese Option aus, um die Dokumentvorlage aus dem Dropdown-Menü auszuwählen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, auf dem sich Ihre Vorlage befindet. Diese Option ist verfügbar, wenn Sie im vorherigen Feld [!UICONTROL Nach Dropdown] ausgewählt haben.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mein Laufwerk]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich Ihre Vorlage befindet.</p> </li> 
     <li> <p><strong>[!UICONTROL Für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich Ihre Vorlage befindet.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Freigegebenes Laufwerk]</strong> (verfügbar für [!DNL G Suite] nur Benutzer)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain Admin Access] verwenden möchten. Wenn Sie [!UICONTROL Ja] auswählen, wird die Anfrage als Domain-Administrator ausgegeben und alle freigegebenen Laufwerke, bei denen der Anforderer ein Administrator ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf dem sich Ihre Vorlage befindet.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ein und Sie sind keine [!DNL G Suite] Benutzer, der Fehler <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Werte]</p> </td> 
   <td> <p>Geben Sie die Werte ein, die anstelle der Variablen in das neue Dokument eingegeben werden sollen.</p> 
    <ul> 
     <li><strong>[!UICONTROL Tags]</strong> <br>Geben Sie die Tags ein, die in der Dokumentvorlage enthalten sind. Nicht anwenden <code>&#123;&#123;&#125;&#125;</code>. Beispiel: use <code>name</code> anstelle von <code>&#123;&#123;name&#125;&#125;</code>.</li> 
     <li><strong>[!UICONTROL Ersetzter Wert]</strong><br>Geben Sie den Wert des Tags ein.</li> 
    </ul> <p>Beispiel:<code> &#123;&#123;name&#125;&#125;</code> im Quelldokument wird hier als Namensfeld angezeigt, in das der Wert eingefügt werden kann, z. B. <code>John</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Implacement]</p> </td> 
   <td> <p>Geben Sie den Link zur [!UICONTROL Image Object ID] und [!UICONTROL Image URL] ein, die das aktuelle Bild ersetzen.</p> <p>Hinweis: Sie können die Bild-IDs mithilfe des Moduls [!UICONTROL Dokument abrufen] abrufen, in dem die IDs im Array [!UICONTROL Inline Object Array] enthalten sind.</p> <p>Es wird empfohlen, den Bildern in der [!DNL Google] Dokument. </p> <p>So fügen Sie ALT-Text zum [!DNL Google Docs] image:</p> 
    <ol> 
     <li value="1">Klicken Sie mit der rechten Maustaste auf das Bild.</li> 
     <li value="2">Wählen Sie die Option [!UICONTROL ALT Text] aus.</li> 
     <li value="3">Geben Sie den ALT-Text [!UICONTROL] in das Feld [!UICONTROL Titel] ein und klicken Sie auf [!UICONTROL OK].</li> 
    </ol> <p>Nachdem dem Bild der ALT-Text hinzugefügt wurde, wird der ALT-Text im Feldnamen in Klammern angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Titel] </td> 
   <td> <p>Geben Sie den Namen für das neue Dokument ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, auf dem sich Ihre Vorlage befindet. Diese Option ist verfügbar, wenn Sie im vorherigen Feld [!UICONTROL Nach Dropdown] ausgewählt haben.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mein Laufwerk]</strong> </p> <p>Wählen Sie den Ordner aus, in dem das Dokument erstellt werden soll.</p> </li> 
     <li> <p><strong>[!UICONTROL Für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem das Dokument erstellt werden soll.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Freigegebenes Laufwerk]</strong> (verfügbar für [!DNL G Suite] nur Benutzer)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain Admin Access] verwenden möchten. Wenn Sie [!UICONTROL Ja] auswählen, wird die Anfrage als Domain-Administrator ausgegeben und alle freigegebenen Laufwerke, bei denen der Anforderer ein Administrator ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf dem das Dokument erstellt werden soll.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ein und Sie sind keine [!DNL G Suite] Benutzer, der Fehler <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Einfügen eines Absatzes in ein Dokument]

Dieses Aktionsmodul hängt einen neuen Absatz an ein vorhandenes Dokument an oder fügt ihn ein.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Dokument auswählen]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Nach Zuordnung]</strong> <br>Wählen Sie diese Option, um das Dokument zuzuordnen.</li> 
     <li><strong>[!UICONTROL Nach Dropdown]</strong> <br> Wählen Sie diese Option aus, um das Dokument aus dem Dropdown-Menü auszuwählen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, unter dem sich das Dokument befindet, dem Sie einen Absatz hinzufügen möchten. Diese Option ist verfügbar, wenn Sie im vorherigen Feld [!UICONTROL Nach Dropdown] ausgewählt haben.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mein Laufwerk]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, dem Sie einen Absatz hinzufügen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL Für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, dem Sie einen Absatz hinzufügen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Freigegebenes Laufwerk]</strong> (verfügbar für [!DNL G Suite] nur Benutzer)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain Admin Access] verwenden möchten. Wenn Sie [!UICONTROL Ja] auswählen, wird die Anfrage als Domain-Administrator ausgegeben und alle freigegebenen Laufwerke, bei denen der Anforderer ein Administrator ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf dem sich das Dokument befindet, dem Sie einen Absatz hinzufügen möchten, und wählen Sie dann das Dokument aus.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ein und Sie sind keine [!DNL G Suite] Benutzer, der Fehler <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Absatz einfügen]</p> </td> 
   <td> <p>Wählen Sie aus, wie der neue Text in das Dokument eingefügt werden soll.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nach Ortsangabe]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Nach Index]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Index]</strong> </p> <p>Geben Sie die Indexnummer ein, unter der Sie Text einfügen möchten. Sie können das Modul [!UICONTROL Dokument abrufen] verwenden, um die Indexnummer abzurufen.</p> <p>Um alle Zeichen (einschließlich ausgeblendeter Zeichen) im Dokument anzuzeigen, können Sie das Add-on [!UICONTROL Anzeigen] verwenden. Sie finden das Add-on unter [!UICONTROL Add-ons] &gt; [!UICONTROL Add-ons abrufen]. Suchen Sie nach [!UICONTROL Show] und installieren Sie das Add-on [!UICONTROL Show].</p> </li> 
         <li> <p><strong>[!UICONTROL Eingefügter Text]</strong> </p> <p>Geben Sie den Text ein, den Sie in das Dokument einfügen möchten.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL Nach Segment-ID]</strong> </p> <p>Wählen Sie die Kopf- und Fußzeile aus, in die Sie den Textinhalt einfügen möchten, und geben Sie den einzufügenden Text in die entsprechenden Felder ein.</p> <p>Wenn die Kopf- oder Fußzeile bereits Text enthält, wird der neue Text vor dem vorhandenen Text hinzugefügt.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Durch Anhängen an den Text des Dokuments]</strong> </p> <p>Hängt den eingegebenen Text am Ende des Textinhalts des Dokuments an.</p> <p>Der Stil des neuen Absatzes wird am aktuellen Einfügeindex aus dem Absatz kopiert, einschließlich Listen und Aufzählungszeichen.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Durch Anhängen an das Ende des Segments (Kopf- und Fußzeile)]</strong> </p> <p>Wählen Sie die Kopf- und Fußzeile aus, in die Sie den Textinhalt einfügen möchten, und geben Sie den einzufügenden Text in die entsprechenden Felder ein.</p> <p>Wenn die Kopf- oder Fußzeile bereits Text enthält, wird der neue Text nach dem vorhandenen Text hinzugefügt.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Angehängter Text]</td> 
   <td>Geben Sie den Text ein oder ordnen Sie ihn dem Dokument zu.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Einfügen eines Bildes in ein Dokument]

Dieses Aktionsmodul fügt ein Bild aus der URL zum Dokument ein.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Dokument auswählen]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Nach Zuordnung]</strong> <br>Wählen Sie diese Option, um die Dokumentvorlage zuzuordnen.</li> 
     <li><strong>[!UICONTROL Nach Dropdown]</strong> <br> Wählen Sie diese Option aus, um das Dokument aus dem Dropdown-Menü auszuwählen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, auf dem sich das Dokument befindet, dem Sie ein Bild hinzufügen möchten. Diese Option ist verfügbar, wenn Sie im vorherigen Feld [!UICONTROL Nach Dropdown] ausgewählt haben.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mein Laufwerk]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, dem Sie ein Bild hinzufügen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL Für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, dem Sie ein Bild hinzufügen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Freigegebenes Laufwerk]</strong> (verfügbar für [!DNL G Suite] nur Benutzer)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain Admin Access] verwenden möchten. Wenn Sie [!UICONTROL Ja] auswählen, wird die Anfrage als Domain-Administrator ausgegeben und alle freigegebenen Laufwerke, bei denen der Anforderer ein Administrator ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf dem sich das Dokument befindet, dem Sie ein Bild hinzufügen möchten, und wählen Sie dann das Dokument aus.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ein und Sie sind keine [!DNL G Suite] Benutzer, der Fehler <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bild einfügen]</p> </td> 
   <td> <p>Wählen Sie aus, wie das neue Bild in das Dokument eingefügt werden soll.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nach Ortsangabe]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Nach Index]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Index]</strong> </p> <p>Geben Sie die Indexnummer an, unter der Sie Ihr Bild einfügen möchten. Sie können das Modul [!UICONTROL Dokument abrufen] verwenden, um die [!UICONTROL Indexnummer] abzurufen.</p> <p>Um alle Zeichen (einschließlich ausgeblendeter Zeichen) im Dokument anzuzeigen, können Sie das Add-on [!UICONTROL Anzeigen] verwenden. Sie finden das Add-on unter [!UICONTROL Add-ons] &gt; [!UICONTROL Add-ons abrufen]. Suchen Sie nach [!UICONTROL Show] und installieren Sie das Add-on [!UICONTROL Show].</p> </li> 
         <li> <p><strong>[!UICONTROL Bild-URL]</strong> </p> <p>Geben Sie die URL des Bildes ein, das Sie in das Dokument einfügen möchten.</p> <p>Die maximale Bildgröße beträgt 50 MB. Darf 25 Megapixel nicht überschreiten. Nur das Format PNG, JPEG oder GIF wird unterstützt.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL Nach Segment-ID]</strong> </p> <p>Wählen Sie die Kopf- und Fußzeile aus, in die das Bild eingefügt werden soll, und geben Sie die Bild-URL in die entsprechenden Felder ein.</p> <p>Die maximale Bildgröße beträgt 50 MB. Das Bild darf 25 Megapixel nicht überschreiten. Nur das Format PNG, JPEG oder GIF wird unterstützt.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Durch Anhängen an den Text des Dokuments]</strong> </p> <p>Hängt ein bestimmtes Bild am Ende des Textinhalts des Dokuments an.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Durch Anhängen an das Ende des Segments (Kopf- und Fußzeile)]</strong> </p> <p>Wählen Sie die Kopf- und Fußzeile aus, in die Sie ein Bild einfügen möchten, und geben Sie die Bild-URL ein, die Sie in die entsprechenden Felder einfügen möchten.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Höhenhöhe in Punkten/Breitenhöhe in Punkten]</p> </td> 
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
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Dokument auswählen]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Nach Zuordnung]</strong> <br>Wählen Sie diese Option, um die Dokumentvorlage zuzuordnen.</li> 
     <li><strong>[!UICONTROL Nach Dropdown]</strong> <br> Wählen Sie diese Option aus, um das Dokument aus dem Dropdown-Menü auszuwählen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, auf dem sich das Dokument befindet, das Sie ein Bild ersetzen möchten. Diese Option ist verfügbar, wenn Sie im vorherigen Feld [!UICONTROL Nach Dropdown] ausgewählt haben.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mein Laufwerk]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, das Sie ersetzen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL Für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, das Sie ersetzen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Freigegebenes Laufwerk]</strong> (verfügbar für [!DNL G Suite] nur Benutzer)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain Admin Access] verwenden möchten. Wenn Sie [!UICONTROL Ja] auswählen, wird die Anfrage als Domain-Administrator ausgegeben und alle freigegebenen Laufwerke, bei denen der Anforderer ein Administrator ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf dem sich das Dokument befindet, das Sie ein Bild ersetzen möchten, und wählen Sie dann das Dokument aus.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ein und Sie sind keine [!DNL G Suite] Benutzer, der Fehler <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bild-URL]</p> </td> 
   <td> <p>Geben Sie die URL des neuen Bildes ein, das das vorhandene Bild ersetzen soll, oder ordnen Sie es zu.</p> <p>Bilder werden in der Reihenfolge aufgelistet, in der sie im Dokument angezeigt werden. Beispiel: <code>Body: Image No. 1</code> ist das erste Bild im Dokument.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Text in einem Dokument ersetzen]

Dieses Aktionsmodul ersetzt Text in einem Dokument.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Dokument auswählen]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Nach Zuordnung]</strong> <br>Wählen Sie diese Option, um die Dokumentvorlage zuzuordnen.</li> 
     <li><strong>[!UICONTROL Nach Dropdown]</strong> <br> Wählen Sie diese Option aus, um das Dokument aus dem Dropdown-Menü auszuwählen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, auf dem sich das Dokument befindet, dem Sie Text hinzufügen möchten. Diese Option ist verfügbar, wenn Sie im vorherigen Feld [!UICONTROL Nach Dropdown] ausgewählt haben.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mein Laufwerk]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, dem Sie Text hinzufügen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL Für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, dem Sie Text hinzufügen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Freigegebenes Laufwerk]</strong> (verfügbar für [!DNL G Suite] nur Benutzer)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain Admin Access] verwenden möchten. Wenn Sie [!UICONTROL Ja] auswählen, wird die Anfrage als Domain-Administrator ausgegeben und alle freigegebenen Laufwerke, bei denen der Anforderer ein Administrator ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf dem sich das Dokument befindet, dem Sie Text hinzufügen möchten, und wählen Sie dann das Dokument aus.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ein und Sie sind keine [!DNL G Suite] Benutzer, der Fehler <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Text ersetzen]</p> </td> 
   <td> <p>Fügen Sie jeden Text hinzu, den Sie ersetzen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Alter Text, der ersetzt werden soll]</strong> </p> <p>Geben Sie den Text ein, den Sie ersetzen möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL Neuer Text wird eingefügt]</strong> </p> <p>Geben Sie den neuen Text ein.</p> </li> 
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
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, auf den sich das Dokument befindet, das Sie herunterladen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mein Laufwerk]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, das Sie herunterladen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL Für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, das Sie herunterladen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Freigegebenes Laufwerk]</strong> (verfügbar für [!DNL G Suite] nur Benutzer)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain Admin Access] verwenden möchten. Wenn Sie [!UICONTROL Ja] auswählen, wird die Anfrage als Domain-Administrator ausgegeben und alle freigegebenen Laufwerke, bei denen der Anforderer ein Administrator ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf das sich das Dokument befindet, das Sie herunterladen möchten, und wählen Sie dann das Dokument aus.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ein und Sie sind keine [!DNL G Suite] Benutzer, der Fehler <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Typ] </p> </td> 
   <td> <p>Wählen Sie das Zieldateiformat des heruntergeladenen Dokuments aus.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Löschen eines Dokuments]

Dieses Aktionsmodul löscht ein Dokument.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, unter dem sich das zu löschende Dokument befindet.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mein Laufwerk]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, das Sie löschen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL Für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, das Sie löschen möchten, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Freigegebenes Laufwerk]</strong> (verfügbar für [!DNL G Suite] nur Benutzer)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain Admin Access] verwenden möchten. Wenn Sie [!UICONTROL Ja] auswählen, wird die Anfrage als Domain-Administrator ausgegeben und alle freigegebenen Laufwerke, bei denen der Anforderer ein Administrator ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf dem sich das zu löschende Dokument befindet, und wählen Sie dann das Dokument aus.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ein und Sie sind keine [!DNL G Suite] Benutzer, der Fehler <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Freigegebenes Laufwerk]</td> 
   <td> <p>Wählen Sie das Laufwerk aus, das das Dokument enthält, das Sie herunterladen möchten, und wählen Sie dann ein Dokument aus. Diese Option ist verfügbar, wenn Sie [!DNL Google Docs] im Feld [!UICONTROL Laufwerk auswählen]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dokument-ID]</td> 
   <td> <p> Wählen Sie das Dokument aus oder ordnen Sie es zu, in dem Sie ein oder mehrere Bilder ersetzen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Sonstige

* [[!UICONTROL API-Aufruf durchführen]](#make-an-api-call)
* [[!UICONTROL Alle Links in einem Dokument anklickbar machen]](#make-all-links-in-a-document-clickable)

#### [!UICONTROL API-Aufruf durchführen]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten API-Aufruf ausführen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Geben Sie einen Pfad relativ zu ein <code>https://docs.googleapis.com/</code>. Beispiel: <code>/v1/documents/{presentationID}</code>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode]</td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anforderung in Form eines standardmäßigen JSON-Objekts hinzu. Beispiel: <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p> Geben Sie die Abfragezeichenfolge der Anfrage ein.</p> </td> 
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

**Beispiel:** Mit dem folgenden API-Aufruf werden die Details für das angegebene Dokument in Ihren Google-Dokumenten abgerufen:

**URL:**

/v1/documents/1ujkf-GDgB0TQSYPrxbCSK4Uso54tHVMqHZEVZZxB6aY

**Methode:**

[!UICONTROL GET]

![](assets/api-call-example.png)

Details zum abgerufenen Dokument finden Sie in der Ausgabe des Moduls unter [!UICONTROL Bundle] > [!UICONTROL body].

![](assets/api-output.png)

#### [!UICONTROL Alle Links in einem Dokument anklickbar machen]

Dieses Aktionsmodul sucht alle Links im Dokument und lässt sie anklickbar werden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Google] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]</a> im Artikel <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Alle Links in einem Dokument erstellen]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL Nach Zuordnung]</strong> <br>Wählen Sie diese Option, um die Dokumentvorlage zuzuordnen.</li> 
     <li><strong>[!UICONTROL Nach Dropdown]</strong> <br> Wählen Sie diese Option aus, um das Dokument aus dem Dropdown-Menü auszuwählen.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Laufwerk auswählen]</td> 
   <td> <p>Wählen Sie den Laufwerkstyp aus, in dem sich das Dokument befindet, in dem die Links anklickbar sein sollen. Diese Option ist verfügbar, wenn Sie im vorherigen Feld [!UICONTROL Nach Dropdown] ausgewählt haben.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Mein Laufwerk]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, in dem die Links angeklickt werden sollen, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL Für mich freigegeben]</strong> </p> <p>Wählen Sie den Ordner aus, in dem sich das Dokument befindet, in dem die Links angeklickt werden sollen, und wählen Sie dann das Dokument aus.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Freigegebenes Laufwerk]</strong> (verfügbar für [!DNL G Suite] nur Benutzer)</p> <p>Wählen Sie aus, ob Sie [!UICONTROL Domain Admin Access] verwenden möchten. Wenn Sie [!UICONTROL Ja] auswählen, wird die Anfrage als Domain-Administrator ausgegeben und alle freigegebenen Laufwerke, bei denen der Anforderer ein Administrator ist, werden zurückgegeben.</p> <p>Wählen Sie das freigegebene Laufwerk aus, auf dem sich das Dokument befindet, auf das Sie Links anklickbar machen möchten, und wählen Sie dann das Dokument aus.</p> <p>Hinweis: Wenn Sie die Option [!DNL Google Docs] in diesem Feld ein und Sie sind keine [!DNL G Suite] Benutzer, der Fehler <code>[400] Invalid Value</code> zurückgegeben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Freigegebenes Laufwerk]</td> 
   <td> <p>Wählen Sie das Laufwerk aus, das das Dokument enthält, in dem Sie Links aktualisieren möchten, und wählen Sie dann ein Dokument aus. Diese Option ist verfügbar, wenn Sie [!DNL Google Docs] im Feld [!UICONTROL Laufwerk auswählen].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dokument-ID]</td> 
   <td> <p> Wählen Sie das Dokument aus oder ordnen Sie es zu, in dem die Links aktualisiert werden sollen.</p> </td> 
  </tr> 
 </tbody> 
</table>
