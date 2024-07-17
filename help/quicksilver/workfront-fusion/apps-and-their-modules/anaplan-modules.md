---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Anaplan Module
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die Anaplan verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: 03bcd0a4-c8ec-4f44-b1e1-b57e79595309
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1844'
ht-degree: 0%

---

# [!DNL Anaplan] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Anaplan] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

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

Bevor Sie den Connector [!DNL Anaplan] verwenden können, müssen Sie sicherstellen, dass die folgenden Voraussetzungen erfüllt sind:

* Sie müssen über ein aktives [!UICONTROL Anaplan] -Konto verfügen.
* Sie müssen Arbeitsbereiche, Modelle und andere [!DNL Anaplan] -Objekte in Ihrem [!UICONTROL Anaplan] -Konto konfigurieren, bevor [!DNL Workfront Fusion] mit ihnen interagieren kann.

## [!DNL Anaplan] mit [!DNL Workfront Fusion] verbinden {#connect-anaplan-to-workfront-fusion}

So erstellen Sie eine Verbindung für Ihre [!DNL Anaplan] -Module:

1. Klicken Sie neben dem Feld [!UICONTROL Verbindung] auf **[!UICONTROL Hinzufügen]** .
1. Wählen Sie den Verbindungstyp aus.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL Basic]</td> 
      <td> <p>Eine Verbindung vom Typ [!DNL Anaplan] [!UICONTROL Basic] erfordert nur eine E-Mail-Adresse und ein Passwort, um die Verbindung herzustellen. </p> <p>Geben Sie einen Namen für die Verbindung ein und geben Sie dann Ihre E-Mail-Adresse und das Kennwort Ihres [!DNL Anaplan]-Kontos ein.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL CA-Zertifikat]</td> 
      <td> <p>Eine Verbindung mit dem [!UICONTROL CA-Zertifikat] erfordert einen [!UICONTROL-Zertifikatschlüssel], [!UICONTROL kodierte Daten] und [!UICONTROL kodierte signierte Daten]. [!DNL Anaplan] Sie können diese in Ihrem [!DNL Anaplan] -Konto generieren. Anweisungen finden Sie in der Dokumentation zu [!DNL Anaplan] .</p> <p>Geben Sie einen Namen für die Verbindung ein und geben Sie dann den [!UICONTROL Zertifikatschlüssel], die [!UICONTROL Kodierten Daten] und die [!UICONTROL Kodierten signierten Daten] ein, die Sie in Ihrem [!DNL Anaplan]-Konto generiert haben.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu speichern und zum Modul zurückzukehren.

## [!DNL Anaplan] Module und ihre Felder

Wenn Sie [!DNL Anaplan] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Anaplan] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Anaplan] finden Sie in diesem Artikel unter <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] mit [!DNL Workfront Fusion]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objekttyp, der überwacht werden soll</td> 
   <td>Wählen Sie den Elementtyp aus, den Sie sehen möchten. Das Szenario beginnt mit der Erstellung oder Aktualisierung dieses Datensatztyps.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">&lt;Object&gt; ID</td> 
   <td>Geben Sie die ID des Objekts in Anaplan ein, z. B. ein Modell oder ein Modul, das mit den Objekten verknüpft ist, die Sie sehen möchten</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie [Aktion] für das Modul während jedes Szenario-Ausführungszyklus zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL Erstellen eines Listenelements]](#create-a-list-item)
* [[!UICONTROL Erstellen eines benutzerdefinierten API-Aufrufs]](#make-a-custom-api-call)
* [[!UICONTROL Datensatz lesen]](#read-a-record)
* [[!UICONTROL Ausführen einer Aktion]](#run-an-action)
* [[!UICONTROL Datensatz aktualisieren]](#update-a-record)
* [[!UICONTROL  Datei hochladen]](#upload-a-file)

#### [!UICONTROL Erstellen eines Listenelements]

Dieses Aktionsmodul fügt ein neues Element zu einer Liste in Anaplan hinzu.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Verbindung]</td>
        <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Anaplan] finden Sie in diesem Artikel unter <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] mit [!DNL Workfront Fusion]</a> .</td>
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
        <td>Wenn die Liste, der Sie Elemente hinzufügen möchten, benutzerdefinierte Teilmengen enthält, wählen Sie die Teilmengen aus, denen das Element hinzugefügt werden soll, und wählen Sie dann <b>[!UICONTROL Ja]</b> aus, um das neue Element dieser Teilmenge hinzuzufügen.</td>
    </tr>
</table>

#### [!UICONTROL Erstellen eines benutzerdefinierten API-Aufrufs]

Mit diesem Modul können Sie einen benutzerdefinierten API-Aufruf an die [!DNL Anaplan] -API ausführen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Anaplan] finden Sie in diesem Artikel unter <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] mit [!DNL Workfront Fusion]</a> .</td> 
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
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
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
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Anaplan] finden Sie in diesem Artikel unter <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] mit [!DNL Workfront Fusion]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Wählen Sie die ID des Anaplan Workspace aus oder ordnen Sie sie zu, das das zu löschende Objekt enthält.</td> 
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
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Anaplan] finden Sie in diesem Artikel unter <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] mit [!DNL Workfront Fusion]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den zu lesenden Datensatztyp aus.</p> 
    <ul> 
     <li> <p><b>Modell</b> </p> <p>Auswählen oder Zuordnen der ID des Modells, das Sie lesen möchten</p> </li> 
     <li> <p><b>Modellliste</b> </p> <p>Wählen Sie die Kennungen der Workspace und des Modells aus oder ordnen Sie sie zu, die die zu lesende Liste enthalten, und wählen Sie dann die Liste aus. Wählen Sie im Feld [!UICONTROL Datentyp] aus, ob Sie Daten oder Metadaten lesen möchten.</p> </li> 
     <li> <p><b>Modellversion</b> </p> <p>Wählen Sie die ID des Modells aus, das Sie lesen möchten, oder ordnen Sie sie zu.</p> </li> 
     <li> <p><b>Benutzer</b> </p> <p>Wählen Sie aus, ob Sie Daten zum Eigentümer des verwendeten Kontos oder zu einem anderen Benutzer zurückgeben möchten. Wenn Sie einen anderen Benutzer auswählen, wählen Sie den Namen des Benutzers aus.</p> </li> 
     <li> <p><b>Workspace</b> </p> <p>Wählen Sie die ID der Workspace aus, die Sie lesen möchten, oder ordnen Sie sie zu.</p> </li> 
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
        <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Anaplan] finden Sie in diesem Artikel unter <a href="#Connect" class="MCXref xref" >[!UICONTROL Connect Anaplan zu Workfront Fusion]</a>.</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Workspace ID]</td>
        <td>Wählen Sie die ID des [!DNL Anaplan] Workspace aus oder ordnen Sie sie zu, in dem Sie die Aktion durchführen möchten</td>
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
                 <p><b>[!UICONTROL Prozess]</b>
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
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Anaplan] finden Sie in diesem Artikel unter <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] mit [!DNL Workfront Fusion]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ des Datensatzes aus, den Sie aktualisieren möchten.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Listenelement]</b> </p> <p>Informationen zu Feldern finden Sie unter <a href="#create-a-list-item" class="MCXref xref">Listenelement erstellen</a> in diesem Artikel.</p> </li> 
     <li> <p><b>[!UICONTROL Module cell data]</b> </p> <p>Wenn Sie Zelldaten aktualisieren, werden auch alle nachgelagerten Berechnungen, die diese Daten verwenden, aktualisiert.</p> <p>Füllen Sie die folgenden Felder aus:</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Modell-ID]</b> </p> <p>Wählen Sie das Modell aus oder ordnen Sie es zu, das die zu aktualisierende Zelle enthält.</p> </li> 
       <li> <p><b>[!UICONTROL Module ID]</b> </p> <p>Wählen Sie das Modul aus oder ordnen Sie es zu, das die Zelle enthält, die Sie aktualisieren möchten</p> </li> 
       <li> <p><b>[!UICONTROL Zeileneintrag]</b> </p> <p>Auswählen oder Zuordnen des Zeileneintrags der Zelle, die Sie aktualisieren möchten</p> </li> 
       <li> <p style="font-weight: bold;">[!UICONTROL Dimensionen-ID]</p> <p>Wählen Sie die Dimension im Zeilenelement aus oder ordnen Sie sie zu.</p> 
       <p><b>Hinweis: </b> 
       <ul>
       <li> Dimension key (value) muss entweder <code>dimensionName</code> (next) oder <code>dimensionId</code> (ID) sein.</li>
       <li>Der Elementschlüssel (Wert) muss <code>itemName</code> (Text), <code>itemCode</code> (Text) oder <code>itemId</code> (ID) sein.</li>
       <li>Dimension- und Elementschlüssel müssen denselben Typ aufweisen (Text oder ID).
       </ul>
        </p> 
        <p>Suchen Sie nach Dimensionen in der [!DNL Anaplan Anapedia], um Informationen zu Dimensionen zu erhalten.</p> </li> 
       <li> <p><b>[!UICONTROL Wert]</b> </p> <p>Geben Sie den neuen Wert für die Zelle ein oder ordnen Sie ihn zu.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Modell für das aktuelle Geschäftsjahr]</b> </p> <p>Geben Sie die Workspace ID und die Modell-ID des Modells ein, für das Sie das Geschäftsjahr aktualisieren möchten, und geben Sie dann das neue Jahr für das Modell ein oder ordnen Sie es zu.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL  Datei hochladen]

Dieses Aktionsmodul lädt eine Datei in Anaplan hoch. Die Datei muss bereits in Anaplan hochgeladen worden sein. Sie können dieses Modul verwenden, um es an zusätzliche Speicherorte in Anaplan hochzuladen.
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL Verbindung]</td>
<td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Anaplan] finden Sie in diesem Artikel unter <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] mit [!DNL Workfront Fusion]</a> .</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL Workspace ID]</td>
<td>Wählen Sie die Kennung des [!DNL Anaplan] Workspace aus oder ordnen Sie sie zu, in den Sie eine Datei hochladen möchten.</td>
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
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Anaplan] finden Sie in diesem Artikel unter <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Anaplan] mit [!DNL Workfront Fusion]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Types]</td> 
   <td> <p>Wählen Sie den Typ des Datensatzes aus, den Sie abrufen möchten.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Workspaces]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Modelle]</b> </p> </li> 
       <li> <p><b>[!UICONTROL Zeileneinträge]</b> </p> <p>Wählen Sie die ID des Modells aus oder ordnen Sie sie zu, das die [!DNL line] Elemente enthält, die Sie abrufen möchten.</p> </li> 
       <li> <p><b>[!UICONTROL Modelllisten]</b> </p> <p>Wählen Sie die ID der Workspace- und Modell-ID aus oder ordnen Sie sie zu, die die Modelllisten enthält, die Sie abrufen möchten.</p> </li> 
       <li> <p><b>[!UICONTROL Modellkalender]</b> </p> <p>Wählen Sie die ID der Workspace aus oder ordnen Sie sie zu, die den Modellkalender enthält, den Sie abrufen möchten.</p> </li> 
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
