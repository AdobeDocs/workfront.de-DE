---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Adobe Experience Manager Assets-Module
description: Mit dem [!DNL Adobe Experience Manager Assets] Connector für das [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Assets] -Konto können Sie Assets erstellen, hochladen und aktualisieren sowie Ordner und Assets kopieren oder verschieben.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 0749f230-8cab-464f-863c-9cb4870125d1
source-git-commit: 993d10a93eca28573aaa38e4ce76e5a1b30ec42e
workflow-type: tm+mt
source-wordcount: '1706'
ht-degree: 0%

---

# [!DNL Adobe Experience Manager Assets] Module

Mit dem [!DNL Adobe Experience Manager Assets] -Connector für [!DNL Adobe Workfront Fusion] können Sie ein Szenario starten, das auf Ereignissen in Ihrem [!DNL Adobe Experience Manager Assets]-Konto basiert, Assets erstellen, hochladen und aktualisieren sowie Ordner und Assets kopieren oder verschieben.

Eine Einführung in den Adobe Experience Manager Assets-Connector finden Sie unter:

* [Adobe Experience Manager Assets](https://video.tv.adobe.com/v/3427034/){target=_blank}

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

* Sie müssen über ein [!DNL Adobe Experience Manager Assets] -Konto verfügen, um diese Module verwenden zu können.
* Sie müssen den Fluss &quot;[!UICONTROL Server-zu-Server]&quot;im Ordner &quot;[!DNL Adobe Developer console]&quot;einrichten.

  Anweisungen zum Einrichten des Flusses &quot;[!UICONTROL Server-zu-Server]&quot;im Ordner &quot;[!DNL Adobe Developer console]&quot;finden Sie unter [Generieren von Zugriffstoken für Server-seitige APIs](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).
* Ihr technisches Adobe Experience Manager-Konto muss über Schreibberechtigungen verfügen.

  Anweisungen zum Hinzufügen von Schreibberechtigungen zu Ihrem technischen Adobe Experience Manager-Konto finden Sie unter [Dienstberechtigungen](https://experienceleague.adobe.com/en/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials) in der Adobe Experience Manager-Dokumentation.

## [!DNL Adobe Experience Manager Assets] mit [!DNL Workfront Fusion] verbinden {#connect-adobe-experience-manager-assets-to-workfront-fusion}

So erstellen Sie eine Verbindung für Ihre [!DNL Adobe Experience Manager Assets] -Module:

1. Klicken Sie neben dem Feld [!UICONTROL Verbindung] auf [!UICONTROL Hinzufügen] .

2. Wählen Sie den Verbindungstyp aus, den Sie erstellen:

   * **[!DNL AEM Assets as a Cloud Service]**

     Für diese Konfiguration sind Informationen von [!DNL Adobe Admin Console] erforderlich.

   * **[!DNL AEM Assets Basic]([!DNL Adobe Managed Services])**

     Diese Konfiguration erfordert einen Benutzernamen und ein Kennwort.

3. Füllen Sie die Felder für den Verbindungstyp aus, den Sie erstellen.

   Informationen zu [!DNL AEM Assets as a Cloud Service] finden Sie unter [Konfigurieren der Verbindung für  [!DNL AEM Assets as a Cloud Service]](#configure-the-connection-for-aem-assets-as-a-cloud-service).

   Informationen zu [!UICONTROL AEM Assets Basic] ([!DNL Adobe Managed Services]) finden Sie unter [Konfigurieren der Verbindung für [!UICONTROL AEM Assets Basic]](#configure-the-connection-for-aem-assets-basic).

4. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu speichern und zum Modul zurückzukehren.


### Konfigurieren der Verbindung für [!DNL AEM Assets as a Cloud Service]

>[!NOTE]
>
>* Die Informationen für diese Felder werden im Rahmen der Einrichtung des Flusses &quot;[!UICONTROL Server-zu-Server]&quot;auf dem [!DNL Adobe Developer Console] generiert. Sie finden diese Werte in der JSON-Datei mit den Dienstanmeldeinformationen, die im Rahmen dieser Einrichtung generiert wurde.
>
>   Anweisungen zum Einrichten des Flusses &quot;[!UICONTROL Server-zu-Server]&quot;auf dem [!UICONTROL Adobe Developer Console] finden Sie unter [Generieren von Zugriffstoken für serverseitige APIs](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).
>
>* Ihr technisches Adobe Experience Manager-Konto muss über Schreibberechtigungen verfügen.
>
>   Anweisungen zum Hinzufügen von Schreibberechtigungen zu Ihrem technischen Adobe Experience Manager-Konto finden Sie unter [Dienstberechtigungen](https://experienceleague.adobe.com/en/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials) in der Adobe Experience Manager-Dokumentation.


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
                  <td>Geben Sie die URL für Ihre [!DNL Adobe Experience Manager] -Instanz ein. Fügen Sie am Ende der URL keinen Schrägstrich <code>/</code> ein.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Optionen zum Ausfüllen der Kontodetails]</td>
                  <td>Wählen Sie aus, ob Sie JSON bereitstellen möchten, das Ihre Kontodetails beschreibt, oder ob Sie Details manuell eingeben möchten.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Technische Kontodetails im JSON-Format]</td>
                  <td>Wenn Sie JSON bereitstellen, geben Sie die JSON-Datei ein oder fügen Sie sie ein, die Ihre Kontodetails beschreibt.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Client-ID]</td>
                  <td>Geben Sie bei der manuellen Eingabe der Details die Client-ID ein, die beim [!UICONTROL Server-to-Server]-Setup generiert wurde.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Client Secret]</td>
                  <td>Geben Sie bei der manuellen Eingabe der Details das im [!UICONTROL Server-to-Server]-Setup generierte Client-Geheimnis ein.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL ID des technischen Kontos]</td>
                  <td>Geben Sie bei der manuellen Eingabe der Details die Kennung des technischen Kontos ein. Dies ist das Feld "[!UICONTROL id]"in der JSON-Datei mit den Client-Anmeldeinformationen.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Organisations-ID]</td>
                  <td class="">Geben Sie bei der manuellen Eingabe der Details die Kennung Ihres Unternehmens ein. Dies ist das Feld "[!UICONTROL org]" in der JSON-Datei mit den Client-Anmeldeinformationen.</td>
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


### Konfigurieren der Verbindung für [!DNL AEM Assets Basic] ([!DNL Adobe Managed Services])

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
                <td>Geben Sie die URL für Ihre [!DNL Adobe Experience Manager] -Instanz ein. Fügen Sie am Ende der URL keinen Schrägstrich <code>/</code> ein.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Benutzername]</td>
                <td>Geben Sie den Benutzernamen für das von dieser Verbindung verwendete [!DNL AEM Assets] -Konto ein.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Kennwort]</td>
                <td>Geben Sie das Kennwort für das von dieser Verbindung verwendete [!DNL AEM Assets]-Konto ein.</td>
            </tr>
        </tbody>
    </table>


## [!DNL Adobe Experience Manager Assets] Module und ihre Felder

Wenn Sie [!DNL Adobe Experience Manager Essentials] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Adobe Experience Manager Essentials] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Kopieren von Ordnern oder Assets](#copy-a-folder-or-asset)
* [Datensatz erstellen](#create-a-record)
* [Löschen von Ordnern, Assets oder Ausgabedarstellungen](#delete-a-folder-asset-or-rendition)
* [Abrufen einer Ordnerliste](#get-a-folder-listing)
* [Benutzerdefinierte API-Aufrufe durchführen](#make-a-custom-api-call)
* [Verschieben von Ordnern oder Assets](#move-a-folder-or-asset)
* [Datensatz aktualisieren](#update-a-record)
* [Hochladen eines Assets](#upload-an-asset)

### [!UICONTROL Kopieren eines Ordners oder Assets]

Dieses Aktionsmodul kopiert einen Ordner oder ein Asset an einen anderen Speicherort in Ihrem Adobe Experience Manager Assets-Konto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Experience Manager Assets]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Adobe Experience Manager Assets] mit [!DNL Workfront Fusion]</a> .</p> </td> 
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
   <td>Geben Sie einen Namen für den neuen Ordner oder das neue Asset ein. Der in [!DNL Adobe Experience Manager Assets] angezeigte Ordnername ist mit dem ursprünglichen Namen identisch. Der hier eingegebene Name wird in der URL des neuen Ordners oder Assets angezeigt.</td> 
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

### [!UICONTROL Erstellen eines Datensatzes]

Dieses Aktionsmodul erstellt einen Ordner oder einen Asset-Kommentar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Experience Manager Assets]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Adobe Experience Manager Assets] mit [!DNL Workfront Fusion]</a> .</p> </td> 
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

### [!UICONTROL Löschen eines Ordners, Assets oder Ausgabeformats]

Dieses Aktionsmodul löscht einen Ordner, ein Asset oder eine Ausgabedarstellung.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Experience Manager Assets]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Adobe Experience Manager Assets] mit [!DNL Workfront Fusion]</a> .</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Experience Manager Assets]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Adobe Experience Manager Assets] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner]</td> 
   <td>Wählen Sie den Ordner aus oder ordnen Sie ihn zu, den Sie abrufen möchten. Um dem Pfad Unterordner hinzuzufügen, klicken Sie auf das Pluszeichen und wählen Sie den Unterordner aus.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Erstellen eines benutzerdefinierten API-Aufrufs]

Dieses Aktionsmodul führt einen benutzerdefinierten API-Aufruf an die [!DNL Adobe Experience Manager Assets] -API durch.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Experience Manager Assets]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Adobe Experience Manager Assets] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Geben Sie einen Pfad relativ zu Ihrer Basis-URL für [!DNL Adobe Experience Manager] ein.</p> </td> 
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
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Verschieben eines Ordners oder Assets]

Dieses Aktionsmodul verschiebt das Asset oder den Ordner an den angegebenen Pfad an einen neuen Speicherort.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Experience Manager Assets]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Adobe Experience Manager Assets] mit [!DNL Workfront Fusion]</a> .</p> </td> 
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
   <td>Geben Sie einen neuen Namen für den verschobenen Ordner oder das verschobene Asset ein. Der in [!DNL Adobe Experience Manager Assets] angezeigte Ordnername ist mit dem ursprünglichen Namen identisch. Der hier eingegebene Name wird in der URL des verschobenen Ordners oder Assets angezeigt.</td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Experience Manager Assets]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Adobe Experience Manager Assets] mit [!DNL Workfront Fusion]</a> .</p> </td> 
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

### [!UICONTROL  Hochladen eines Assets ]

Dieses Aktionsmodul lädt ein Asset in Ihr [!DNL Adobe Experience Manager Assets]-Konto hoch.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Adobe Experience Manager Assets]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Adobe Experience Manager Assets] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ziel]</td> 
   <td> <p>Wählen Sie den Ordner aus, in den Sie ein Asset hochladen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Datei]</td> 
   <td>Geben Sie den Namen und die Daten der Quelldatei ein oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>
