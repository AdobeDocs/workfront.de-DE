---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Adobe Experience Manager Assets-Module
description: Mit dem [!DNL Adobe Experience Manager Assets] Connector für [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Assets] -Konto erstellen, Assets hochladen und aktualisieren sowie Ordner und Assets kopieren oder verschieben.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 0749f230-8cab-464f-863c-9cb4870125d1
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 0%

---

# [!DNL Adobe Experience Manager Assets]-Module

Mit dem [!DNL Adobe Experience Manager Assets] Connector für [!DNL Adobe Workfront Fusion]können Sie ein Szenario starten, das auf Ereignissen in Ihrer [!DNL Adobe Experience Manager Assets] -Konto erstellen, Assets hochladen und aktualisieren sowie Ordner und Assets kopieren oder verschieben.

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

* Sie müssen über eine [!DNL Adobe Experience Manager Assets] , um diese Module zu verwenden.
* Sie müssen [!UICONTROL Server-zu-Server] im [!DNL Adobe Developer console].

   Anweisungen zum Einrichten von [!UICONTROL Server-zu-Server] im [!DNL Adobe Developer console], siehe [Generieren von Zugriffstoken für serverseitige APIs](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).

## Verbinden [!DNL Adobe Experience Manager Assets] nach [!DNL Workfront Fusion] {#connect-adobe-experience-manager-assets-to-workfront-fusion}

So erstellen Sie eine Verbindung für Ihre [!DNL Adobe Experience Manager Assets] -Module:

1. Klicken [!UICONTROL Hinzufügen] neben dem [!UICONTROL Verbindung] ankreuzen.

2. Wählen Sie den Verbindungstyp aus, den Sie erstellen:

   * **[!DNL AEM Assets as a Cloud Service]**

      Diese Konfiguration erfordert Informationen aus dem [!DNL Adobe Admin Console].

   * **[!DNL AEM Assets Basic]**

      Diese Konfiguration erfordert einen Benutzernamen und ein Kennwort.

3. Füllen Sie die Felder für den Verbindungstyp aus, den Sie erstellen.

   Für [!DNL AEM Assets as a Cloud Service], siehe [Konfigurieren Sie die Verbindung für [!DNL AEM Assets as a Cloud Service]](#configure-the-connection-for-aem-assets-as-a-cloud-service).

   Für [!UICONTROL AEM Assets Basic], siehe [Konfigurieren Sie die Verbindung für [!UICONTROL AEM Assets Basic]](#configure-the-connection-for-aem-assets-basic).

4. Klicken **[!UICONTROL Weiter]** , um die Verbindung zu speichern und zum Modul zurückzukehren.


### Konfigurieren Sie die Verbindung für [!DNL AEM Assets as a Cloud Service]

>[!NOTE]
>
>Die Informationen für diese Felder werden im Rahmen der Einrichtung von [!UICONTROL Server-zu-Server] Fluss auf [!DNL Adobe Developer Console]. Sie finden diese Werte in der JSON-Datei mit den Dienstanmeldeinformationen, die im Rahmen dieser Einrichtung generiert wurde.
>
>Anweisungen zum Einrichten von [!UICONTROL Server-zu-Server] Fluss auf [!UICONTROL Adobe Developer-Konsole], siehe [Generieren von Zugriffstoken für serverseitige APIs](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).


<table style="table-layout:auto"> 
          <col/>
          <col/>
          <tbody>
              <tr>
                  <td role="rowheader">[!UICONTROL Verbindungsname]</td>
                  <td>
                      <p>Geben Sie einen Namen für diese Verbindung ein</p>
                  </td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Instanz-URL ohne Schrägstrich]</td>
                  <td>Geben Sie die URL für Ihre [!DNL Adobe Experience Manager] -Instanz. Schrägstrich nicht einschließen <code>/</code> am Ende der URL.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Client-ID]</td>
                  <td>Geben Sie die im [!UICONTROL Server-to-Server]-Setup generierte Client-ID ein.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Client Secret]</td>
                  <td>Geben Sie den Client-Geheimnisschlüssel ein, der im [!UICONTROL Server-to-Server]-Setup generiert wurde.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL ID des technischen Kontos]</td>
                  <td>Geben Sie die Kennung des technischen Kontos ein. Dies ist das Feld "[!UICONTROL id]"in der JSON-Datei mit den Client-Anmeldeinformationen.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Organisations-ID]</td>
                  <td class="">Geben Sie die Kennung Ihrer Organisation ein. Dies ist das Feld "[!UICONTROL org]" in der JSON-Datei mit den Client-Anmeldedaten.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Meta Scopes]</td>
                  <td>Geben Sie die im [!UICONTROL Server-to-Server]-Setup generierten Meta-Perimeter ein.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Privater Schlüssel]</td>
                  <td>Geben Sie den generierten privaten Schlüssel ein, der bei der [!UICONTROL Server-to-Server]-Einrichtung gewonnen wird. Um den privaten Schlüssel zu extrahieren, klicken Sie auf [!UICONTROL Extract], geben Sie dann die zu extrahierende Datei und das Kennwort für die Datei ein.</td>
              </tr>
          </tbody>
      </table>


### Konfigurieren Sie die Verbindung für [!DNL AEM Assets Basic]

<table style="table-layout:auto"> 
        <col/>
        <col />
        <tbody>
            <tr>
                <td role="rowheader">[!UICONTROL Verbindungsname]</td>
                <td>
                    <p>Geben Sie einen Namen für diese Verbindung ein</p>
                </td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Instanz-URL ohne Schrägstrich]</td>
                <td>Geben Sie die URL für Ihre [!DNL Adobe Experience Manager] -Instanz. Schrägstrich nicht einschließen <code>/</code> am Ende der URL.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Benutzername]</td>
                <td>Geben Sie den Benutzernamen für die [!DNL AEM Assets] -Konto, das diese Verbindung verwendet.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Kennwort]</td>
                <td>Geben Sie das Kennwort für die [!DNL AEM Assets] -Konto, das diese Verbindung verwendet.</td>
            </tr>
        </tbody>
    </table>


## [!DNL Adobe Experience Manager Assets] Module und ihre Felder

Bei der Konfiguration [!DNL Adobe Experience Manager Essentials] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Adobe Experience Manager Essentials] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### [!UICONTROL Kopieren von Ordnern oder Assets]

Dieses Aktionsmodul kopiert einen Ordner oder ein Asset an einen anderen Speicherort in Ihrem Adobe Experience Manager Assets-Konto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Adobe Experience Manager Assets] Konto [!DNL Workfront Fusion], siehe <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Adobe Experience Manager Assets] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie aus, ob Sie einen Ordner oder ein Asset kopieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner] / [!UICONTROL Asset-Auswahl]</td> 
   <td>Wählen Sie den Ordner oder das Asset aus oder ordnen Sie ihn bzw. das Asset zu, das Sie kopieren möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zielpfad]</td> 
   <td>Wählen Sie den Pfad zum Speicherort für den neuen Ordner oder das neue Asset aus oder ordnen Sie ihn ihm zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name des kopierten Ordners] / [!UICONTROL Asset]</td> 
   <td>Geben Sie einen Namen für den neuen Ordner oder das neue Asset ein. Der Ordnername, der in [!DNL Adobe Experience Manager Assets] entspricht dem ursprünglichen Namen. Der hier eingegebene Name wird in der URL des neuen Ordners oder Assets angezeigt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Untergeordnete Elemente kopieren]</td> 
   <td>Aktivieren Sie diese Option, um alle Unterordner oder Assets im Ordner zu kopieren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Overwrite]</td> 
   <td>Aktivieren Sie diese Option, um alle Ordner oder Assets im Zielspeicherort zu überschreiben, die denselben Namen wie der kopierte Ordner oder das kopierte Asset haben.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensatz erstellen]

Dieses Aktionsmodul erstellt einen Ordner oder einen Asset-Kommentar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Adobe Experience Manager Assets] Konto [!DNL Workfront Fusion], siehe <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Adobe Experience Manager Assets] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Objekttyp]</td> 
   <td> <p>Wählen Sie aus, ob Sie einen Ordner oder einen Kommentar für ein Asset erstellen möchten.</p> 
    <ul> 
     <li> <p>[!UICONTROL Ordner]</p> <p>Füllen Sie die folgenden Felder aus:</p> 
      <ul> 
       <li> <p>[!UICONTROL Name]</p> <p>Geben Sie einen Namen für den Ordner ein. Dieser Name erscheint im Dateipfad, darf also keine Leerzeichen oder anderen Zeichen enthalten. </p> </li> 
       <li> <p>[!UICONTROL Titel]</p> <p>Geben Sie einen Titel für den Ordner ein, der anstelle des Namens angezeigt werden kann.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Asset-Kommentar]</p> <p>Füllen Sie die folgenden Felder aus:</p> 
      <ul> 
       <li> <p>[!UICONTROL Asset-Auswahl]</p> <p>Wählen Sie die ID des Assets aus oder ordnen Sie sie zu, dem Sie einen Kommentar hinzufügen möchten.</p> </li> 
       <li> <p>[!UICONTROL Kommentar]</p> <p>Geben Sie den Text des Kommentars ein.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensatz löschen]

Dieses Aktionsmodul löscht einen Ordner, ein Asset oder eine Ausgabedarstellung.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Adobe Experience Manager Assets] Konto [!DNL Workfront Fusion], siehe <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Adobe Experience Manager Assets] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie aus, ob Sie einen Ordner, ein Asset oder eine Ausgabedarstellung löschen möchten.</p> 
    <ul> 
     <li> <p>[!UICONTROL Ordner]</p> <p>Wählen Sie den zu löschenden Ordner aus, indem Sie die Ordner im Pfad auswählen.</p> </li> 
     <li> <p>[!UICONTROL Asset] </p> <p>Wählen Sie das Asset aus, indem Sie die Ordner im Pfad und dann das Asset auswählen, das Sie löschen möchten.</p> </li> 
     <li> <p>[!UICONTROL Rendition]</p> <p>Wählen Sie die Ausgabedarstellung aus, indem Sie die Ordner im Pfad auswählen.</p> <p>Geben Sie den Namen der Ausgabedarstellung ein oder ordnen Sie ihn zu.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Abrufen einer Ordnerliste]

Dieses Aktionsmodul ruft eine Darstellung eines vorhandenen Ordners und seiner untergeordneten Entitäten (Ordner oder Assets) ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Adobe Experience Manager Assets] Konto [!DNL Workfront Fusion], siehe <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Adobe Experience Manager Assets] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner]</td> 
   <td>Wählen Sie den Ordner aus oder ordnen Sie ihn zu, den Sie abrufen möchten. Um dem Pfad Unterordner hinzuzufügen, klicken Sie auf das Pluszeichen und wählen Sie den Unterordner aus.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Benutzerdefinierte API-Aufrufe durchführen]

Dieses Aktionsmodul führt einen benutzerdefinierten API-Aufruf an die [!DNL Adobe Experience Manager Assets] API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Adobe Experience Manager Assets] Konto [!DNL Workfront Fusion], siehe <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Adobe Experience Manager Assets] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Geben Sie einen Pfad relativ zu Ihrer [!DNL Adobe Experience Manager] Basis-URL.</p> </td> 
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
   <td> <p>Geben Sie die Abfragezeichenfolge der Anfrage ein. Klicken Sie für jedes Schlüssel/Wert-Paar auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie den [!UICONTROL Schlüssel] und den [!UICONTROL Wert] ein.</p> </td> 
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

### [!UICONTROL Verschieben von Ordnern oder Assets]

Dieses Aktionsmodul verschiebt das Asset oder den Ordner an den angegebenen Pfad an einen neuen Speicherort.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Adobe Experience Manager Assets] Konto [!DNL Workfront Fusion], siehe <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Adobe Experience Manager Assets] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie aus, ob Sie einen Ordner oder ein Asset verschieben möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner] / [!UICONTROL Asset]</td> 
   <td>Wählen Sie den Ordner oder das Asset aus oder ordnen Sie ihn bzw. das Asset zu, das Sie verschieben möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zielpfad]</td> 
   <td>Wählen Sie den Pfad zu dem Speicherort aus, an den Sie den Ordner oder das Asset verschieben möchten, oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name des verschobenen Ordners] / [!UICONTROL Asset]</td> 
   <td>Geben Sie einen neuen Namen für den verschobenen Ordner oder das verschobene Asset ein. Der Ordnername, der in [!DNL Adobe Experience Manager Assets] entspricht dem ursprünglichen Namen. Der hier eingegebene Name wird in der URL des verschobenen Ordners oder Assets angezeigt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Overwrite]</td> 
   <td>Aktivieren Sie diese Option, um alle Ordner oder Assets im Zielspeicherort zu überschreiben, die denselben Namen wie der kopierte Ordner oder das kopierte Asset haben.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Datensatz aktualisieren]

Dieses Aktionsmodul aktualisiert einen vorhandenen Datensatz.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Adobe Experience Manager Assets] Konto [!DNL Workfront Fusion], siehe <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Adobe Experience Manager Assets] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie aus, ob Sie Asset-Metadaten oder eine Asset-Ausgabedarstellung löschen möchten.</p> 
    <ul> 
     <li> <p>[!UICONTROL Asset-Metadaten]</p> 
      <ul> 
       <li> <p>Wählen Sie das Asset aus, für das Sie Metadaten aktualisieren möchten.</p> </li> 
       <li> <p>Geben Sie den neuen Titel des Assets ein.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Asset-Ausgabedarstellung]</p> 
      <ul> 
       <li> <p>Wählen Sie das Asset aus, für das Sie die Ausgabedarstellung aktualisieren möchten.</p> </li> 
       <li> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Hochladen eines Assets]

Dieses Aktionsmodul lädt ein Asset in Ihre [!DNL Adobe Experience Manager Assets] -Konto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Adobe Experience Manager Assets] Konto [!DNL Workfront Fusion], siehe <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Adobe Experience Manager Assets] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ziel]</td> 
   <td> <p>Wählen Sie den Ordner aus, in den Sie ein Asset hochladen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td>Geben Sie den Namen und die Daten der Quelldatei ein oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>
