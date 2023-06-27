---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Anaplan-Module
description: In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die Anaplan verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: 03bcd0a4-c8ec-4f44-b1e1-b57e79595309
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1844'
ht-degree: 1%

---

# [!DNL Anaplan] Module

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Anaplan], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.

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

Bevor Sie die [!DNL Anaplan] müssen Sie sicherstellen, dass die folgenden Voraussetzungen erfüllt sind:

* Sie müssen über eine aktive [!UICONTROL Anaplan] -Konto.
* Sie müssen Arbeitsbereiche, Modelle und andere [!DNL Anaplan] Objekte in [!UICONTROL Anaplan] account before [!DNL Workfront Fusion] kann mit ihnen interagieren.

## Verbinden [!DNL Anaplan] nach [!DNL Workfront Fusion] {#connect-anaplan-to-workfront-fusion}

So erstellen Sie eine Verbindung für Ihre [!DNL Anaplan] -Module:

1. Klicken **[!UICONTROL Hinzufügen]** neben dem [!UICONTROL Verbindung] ankreuzen.
1. Wählen Sie den Verbindungstyp aus.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL Basic]</td> 
      <td> <p>Ein [!DNL Anaplan] Die Verbindung [!UICONTROL Basic] erfordert nur eine E-Mail-Adresse und ein Passwort, um die Verbindung herzustellen. </p> <p>Geben Sie einen Namen für die Verbindung ein und geben Sie dann Ihre E-Mail-Adresse und das Passwort Ihrer [!DNL Anaplan] -Konto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL CA-Zertifikat]</td> 
      <td> <p>Ein [!DNL Anaplan] Für die Verbindung zum CA-Zertifikat ist ein [!UICONTROL-Zertifikatschlüssel], [!UICONTROL-kodierte Daten] und [!UICONTROL kodierte signierte Daten] erforderlich. Sie können diese in der [!DNL Anaplan] -Konto. Anweisungen finden Sie in der [!DNL Anaplan] Dokumentation.</p> <p>Geben Sie einen Namen für die Verbindung ein und geben Sie dann den [!UICONTROL Zertifikatschlüssel], die kodierten [!UICONTROL Daten] und die in Ihrer [!DNL Anaplan] -Konto.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **[!UICONTROL Weiter]** , um die Verbindung zu speichern und zum Modul zurückzukehren.

## [!DNL Anaplan] Module und ihre Felder

Bei der Konfiguration [!DNL Anaplan] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Anaplan] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Trigger

#### [!DNL Watch records]

Dieses Trigger-Modul startet ein Szenario, wenn ein Datensatz des ausgewählten Typs erstellt oder aktualisiert wird.

>[!NOTE]
>
>Dieses Modul gibt die Daten neuer Datensätze zurück. Es werden keine Daten geänderter vorhandener Datensätze zurückgegeben.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Anaplan], siehe <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objekttyp, der überwacht werden soll</td> 
   <td>Wählen Sie den Elementtyp aus, den Sie sehen möchten. Das Szenario beginnt mit der Erstellung oder Aktualisierung dieses Datensatztyps.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">&lt;object&gt; ID</td> 
   <td>Geben Sie die ID des Objekts in Anaplan ein, z. B. ein Modell oder ein Modul, das mit den Objekten verknüpft ist, die Sie sehen möchten</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie [Aktion] für das Modul während jedes Szenario-Ausführungszyklus zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL Listenelement erstellen]](#create-a-list-item)
* [[!UICONTROL Benutzerdefinierte API-Aufrufe durchführen]](#make-a-custom-api-call)
* [[!UICONTROL Datensatz lesen]](#read-a-record)
* [[!UICONTROL Ausführen einer Aktion]](#run-an-action)
* [[!UICONTROL Datensatz aktualisieren]](#update-a-record)
* [[!UICONTROL Datei hochladen]](#upload-a-file)

#### [!UICONTROL Listenelement erstellen]

Dieses Aktionsmodul fügt ein neues Element zu einer Liste in Anaplan hinzu.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Verbindung]</td>
        <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Anaplan], siehe <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Workspace ID]</td>
        <td>Wählen Sie die ID des Anaplan Workspace aus oder ordnen Sie sie zu, der die Liste enthält, in der Sie ein Element hinzufügen möchten.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Modell-ID]</td>
        <td>Wählen Sie die ID des Modells aus oder ordnen Sie sie zu, das die Liste enthält, in der Sie ein Element hinzufügen möchten.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Listen-ID]</td>
        <td>Wählen Sie die ID der Liste aus oder ordnen Sie sie zu, in der Sie ein Element erstellen möchten.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Name]</td>
        <td>Geben Sie einen Namen für das neue Element ein.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Code]</td>
        <td>Geben Sie den Code für das neue Element ein. Codes sind benutzergenerierte Codes, mit denen Sie zwischen Zeileneinträgen mit demselben Namen unterscheiden können.</td>
    </tr>
    <tr>
        <td>Übergeordnetes Element von [!UICONTROL]</td>
        <td>Geben Sie den Namen des übergeordneten Elements ein, unter dem Sie das neue Element erstellen möchten.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Eigenschaften]</td>
        <td>Wenn die Liste, der Sie ein Element hinzufügen möchten, benutzerdefinierte Eigenschaften aufweist, wählen Sie die Eigenschaften aus, für die Sie Werte hinzufügen möchten, und fügen Sie dann die Werte hinzu.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Teilmengen]</td>
        <td>Wenn die Liste, der Sie Elemente hinzufügen möchten, benutzerdefinierte Teilmengen enthält, wählen Sie die Teilmengen aus, denen Sie das Element hinzufügen möchten, und wählen Sie dann <b>[!UICONTROL Ja]</b> , um das neue Element zu dieser Teilmenge hinzuzufügen.</td>
    </tr>
</table>

#### [!UICONTROL Benutzerdefinierte API-Aufrufe durchführen]

Mit diesem Modul können Sie einen benutzerdefinierten API-Aufruf an die [!DNL Anaplan] API.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Anaplan], siehe <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Geben Sie einen Pfad relativ zu ein <code>https://api.anaplan.com/2/0/</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Methode]</p> </td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] fügt automatisch Autorisierungskopfzeilen hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge] </td> 
   <td> <p>Geben Sie die Abfragezeichenfolge der Anfrage ein.</p> </td> 
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

#### [!UICONTROL Datensatz löschen]

Dieses Aktionsmodul löscht einen vorhandenen Datensatz.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Anaplan], siehe <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Wählen Sie die ID des Anaplan Workspace aus oder ordnen Sie sie zu, der das zu löschende Objekt enthält.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Modell-ID]</td> 
   <td>Geben Sie die ID des Modells ein oder ordnen Sie sie zu, das das zu löschende Objekt enthält.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Löschen</td> 
   <td> <p>Wählen Sie den Typ des zu löschenden Objekts aus.</p> 
    <ul> 
     <li> <p><b>Aktion</b> </p> <p>Wählen Sie die zu löschende Aktion aus oder ordnen Sie sie zu.</p> </li> 
     <li> <p><b>Listenelement</b> </p> <p>Wählen Sie die Liste aus, aus der Sie ein Element löschen möchten, und geben Sie dann die ID oder den Code des Elements ein, das Sie löschen möchten.</p>  </li> 
     <li> <p><b>[!UICONTROL Datei]</b> </p> <p>Wählen Sie die zu löschende Datei aus oder ordnen Sie sie zu.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datensatz lesen]

Dieses Aktionsmodul liest einen einzelnen Datensatz.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Anaplan], siehe <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ des zu lesenden Datensatzes aus.</p> 
    <ul> 
     <li> <p><b>Modell</b> </p> <p>Auswählen oder Zuordnen der ID des Modells, das Sie lesen möchten</p> </li> 
     <li> <p><b>Modellliste</b> </p> <p>Wählen Sie die IDs von Workspace und Modell aus, die die zu lesende Liste enthalten, oder ordnen Sie sie zu und wählen Sie dann die Liste aus. Wählen Sie im Feld [!UICONTROL Datentyp] aus, ob Sie Daten oder Metadaten lesen möchten.</p> </li> 
     <li> <p><b>Modellversion</b> </p> <p>Wählen Sie die ID des Modells aus, das Sie lesen möchten, oder ordnen Sie sie zu.</p> </li> 
     <li> <p><b>Benutzerin oder Benutzer</b> </p> <p>Wählen Sie aus, ob Sie Daten zum Eigentümer des verwendeten Kontos oder zu einem anderen Benutzer zurückgeben möchten. Wenn Sie einen anderen Benutzer auswählen, wählen Sie den Namen des Benutzers aus.</p> </li> 
     <li> <p><b>Arbeitsbereich</b> </p> <p>Wählen Sie die ID des Workspace aus, den Sie lesen möchten, oder ordnen Sie sie zu.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ausführen einer Aktion]

Dieses Aktionsmodul importiert, exportiert, löscht oder verarbeitet eine Aktion.

<table style="table-layout:auto"> 
     <col/>
     <col/>
     <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Verbindung]</td>
        <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Anaplan], siehe <a href="#Connect" class="MCXref xref" >[!UICONTROL Anaplan mit Workfront Fusion verbinden]</a> in diesem Artikel.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Workspace ID]</td>
        <td>Auswählen oder Zuordnen der ID des [!DNL Anaplan] Arbeitsbereich, in dem Sie die Aktion durchführen möchten</td>
      </tr>
      <tr >
        <td role="rowheader">[!UICONTROL Modell-ID]</td>
        <td>Wählen Sie die ID des Modells aus oder ordnen Sie sie zu, in dem Sie die Aktion durchführen möchten.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Aktionstyp]</td>
        <td>
          <p>Wählen Sie die Aktion aus, die Sie ausführen möchten</p>
            <ul>
              <li>
                <p><b>[!UICONTROL Löschen]</b>
                </p>
                <p>Geben Sie die ID der Aktion ein, die Sie löschen möchten, oder ordnen Sie sie zu.</p>
              </li>
              <li>
                <p><b>[!UICONTROL Export]</b>
                </p>
                <p>Geben Sie die Kennung der Exportdefinition ein oder ordnen Sie sie zu. Sie können in die folgenden Dateiformate exportieren:</p>
                  <ul>
                    <li>
                      <p>XLS</p>
                    </li>
                    <li>
                      <p>XLSX</p>
                    </li>
                    <li>
                      <p>CSV</p>
                    </li>
                  </ul>
                </li>
                <li>
                  <p><b>[!UICONTROL Import] </b>
                  </p>
                  <p style="font-weight: normal;">Geben Sie die Kennung der Importdefinition ein oder ordnen Sie sie zu.</p>
                </li>
                <li>
                 <p><b>[!UICONTROL-Prozess]</b>
                 </p>
                  <p>Geben Sie die Kennung des Prozesses ein, den Sie verwenden möchten, oder ordnen Sie sie zu. </p>
                </li>
              </ul>
            </td>
          </tr>
        </tbody>
      </table>


#### [!UICONTROL Datensatz aktualisieren]

Dieses Aktionsmodul aktualisiert einen einzelnen Datensatz in [!UICONTROL Anaplan].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Anaplan], siehe <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den zu aktualisierenden Datensatztyp aus.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Listenelement]</b> </p> <p>Informationen zu Feldern finden Sie unter <a href="#create-a-list-item" class="MCXref xref">Listenelement erstellen</a> in diesem Artikel.</p> </li> 
     <li> <p><b>[!UICONTROL Module cell data]</b> </p> <p>Wenn Sie Zelldaten aktualisieren, werden auch alle nachgelagerten Berechnungen, die diese Daten verwenden, aktualisiert.</p> <p>Füllen Sie die folgenden Felder aus:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Modell-ID]</b> </p> <p>Wählen Sie das Modell aus oder ordnen Sie es zu, das die zu aktualisierende Zelle enthält.</p> </li> 
       <li> <p><b>[!UICONTROL Modul-ID]</b> </p> <p>Wählen Sie das Modul aus oder ordnen Sie es zu, das die Zelle enthält, die Sie aktualisieren möchten</p> </li> 
       <li> <p><b>[!UICONTROL Zeileneintrag]</b> </p> <p>Auswählen oder Zuordnen des Zeileneintrags der Zelle, die Sie aktualisieren möchten</p> </li> 
       <li> <p style="font-weight: bold;">[!UICONTROL Dimension ID]</p> <p>Wählen Sie die Dimension im Zeilenelement aus oder ordnen Sie sie zu.</p> 
       <p><b>Notiz: </b> 
       <ul>
       <li> Dimension key (value) muss entweder <code>dimensionName</code> (next) oder <code>dimensionId</code> (ID).</li>
       <li>Elementschlüssel (Wert) muss <code>itemName</code> (Text), <code>itemCode</code> (Text) oder <code>itemId</code> (ID).</li>
       <li>Dimension- und Elementschlüssel müssen denselben Typ aufweisen (Text oder ID).
       </ul>
        </p> 
        <p>Informationen zu Dimensionen finden Sie bei der Suche nach Dimensionen in der [!DNL Anaplan Anapedia].</p> </li> 
       <li> <p><b>[!UICONTROL Wert]</b> </p> <p>Geben Sie den neuen Wert für die Zelle ein oder ordnen Sie ihn zu.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Modell für das aktuelle Geschäftsjahr]</b> </p> <p>Geben Sie die Workspace-ID und die Modell-ID des Modells ein, für das Sie das Geschäftsjahr aktualisieren möchten, und geben Sie dann das neue Jahr für das Modell ein oder ordnen Sie es zu.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei hochladen]

Dieses Aktionsmodul lädt eine Datei in Anaplan hoch. Die Datei muss bereits in Anaplan hochgeladen worden sein. Sie können dieses Modul verwenden, um es an zusätzliche Speicherorte in Anaplan hochzuladen.
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL Verbindung]</td>
<td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Anaplan], siehe <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL Workspace ID]</td>
<td>Auswählen oder Zuordnen der ID des [!DNL Anaplan] Arbeitsbereich, in den Sie eine Datei hochladen möchten.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL Modell-ID]</td>
<td>Wählen Sie die ID des Modells aus oder ordnen Sie sie zu, in das Sie eine Datei hochladen möchten.</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL Datei-ID]</td>
<td>Wählen Sie die ID der Datei aus, die Sie hochladen möchten, oder ordnen Sie sie zu.</td>
</tr>
</tbody>
</table>
</div>

### Suchvorgänge

#### [!UICONTROL Datensatz abrufen]

Dieses Suchmodul gibt alle verfügbaren Datensätze des ausgewählten Typs zurück.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Anaplan], siehe <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Types]</td> 
   <td> <p>Wählen Sie den Typ des Datensatzes aus, den Sie abrufen möchten.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Arbeitsbereiche]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Modelle]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Zeileneinträge]</b> </p> <p>Wählen Sie die ID des Modells aus, das die [!DNL line] -Elemente, die Sie abrufen möchten.</p> </li> 
       <li> <p><b>[!UICONTROL Modelllisten]</b> </p> <p>Wählen Sie die ID des Arbeitsbereichs und die Modell-ID aus oder ordnen Sie sie zu, die die Modelllisten enthalten, die Sie abrufen möchten.</p> </li> 
       <li> <p><b>[!UICONTROL Modellkalender]</b> </p> <p>Wählen Sie die ID des Workspace aus oder ordnen Sie sie zu, der den Modellkalender enthält, den Sie abrufen möchten.</p> </li> 
       <li> <p><b>Modellversionen</b> </p> </li> 
       <li> <p>Wählen oder ordnen Sie [!UICONTROL ] die Kennung des Modells zu, das die Modellversionen enthält, die Sie abrufen möchten.</p> </li> 
       <li> <p><b>[!UICONTROL Benutzer]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Ansichten]</b> </p> <p>Wählen Sie aus, ob Sie die Ansicht nach Modul oder Modell auswählen möchten, und wählen Sie dann die ID des Moduls oder Modells aus, das die Ansicht enthält, die Sie abrufen möchten, oder ordnen Sie sie zu.</p> </li> 
      </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Größe des Arbeitsbereichs für die Rückkehr]</td> 
   <td>Aktivieren Sie diese Option, um eine Schätzung der aktuellen Größe des Arbeitsbereichs zurückzugeben. Diese Schätzung basiert auf den Größen aller im Arbeitsbereich enthaltenen Module.</td> 
  </tr> 
 </tbody> 
</table>
