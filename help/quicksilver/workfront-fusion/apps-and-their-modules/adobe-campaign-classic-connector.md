---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Adobe Campaign v7/v8-Module
description: Mit den [!DNL Adobe Campaign] Modulen können Sie ein [!DNL Adobe Workfront Fusion] Szenario starten, das auf Ereignissen in Ihrem [!DNL Adobe Campaign] Konto basiert, Vereinbarungen und andere Datensätze erstellen, lesen oder aktualisieren, nach Datensätzen anhand von von Ihnen festgelegten Kriterien suchen und Dokumente hochladen.
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1448'
ht-degree: 1%

---

# [!DNL Adobe Campaign] Module

Mit den [!DNL Adobe Campaign] -Modulen können Sie ein [!DNL Adobe Workfront Fusion] -Szenario starten, das auf Ereignissen in Ihrem [!DNL Adobe Campaign v7/v8] -Konto basiert, Datensätze erstellen, lesen oder aktualisieren, nach Datensätzen suchen, indem Sie von Ihnen festgelegte Kriterien verwenden, und benutzerdefinierte API-Aufrufe durchführen.

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
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebene Funktionalität nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Sie müssen die Fusion-IP-Adressen zu [!DNL Adobe Campaign] hinzufügen.

* Anweisungen zum Hinzufügen von IP-Adressen zu Ihrer Campaign-Zulassungsliste finden Sie unter [Hinzufügen von IP-Adressen zur Zulassungsliste von Campaign ](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/ip-range-allow-listing#adding-ip-addresses-allow-list) in der Adobe Campaign-Dokumentation.
* Eine Liste der IP-Adressen, die der Zulassungsliste hinzugefügt werden sollen, finden Sie unter [IP-Adressen für den Zugriff auf Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/get-started/ip-addresses-for-fusion.md).

## Adobe Campaign-API-Informationen

Der Adobe Campaign-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.7.22</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Adobe Campaign] mit [!DNL Adobe Workfront Fusion] verbinden

>[!IMPORTANT]
>
>Es wird dringend empfohlen, eine Server-zu-Server-Verbindung zu erstellen. Adobe Campaign hat seine API aktualisiert, um nur Server-zu-Server-Verbindungen zu akzeptieren. Wenn Sie eine Verbindung zu Campaign Version 8 oder höher herstellen, müssen Sie **1} eine Server-zu-Server-Verbindung erstellen.**
>
>Weitere Informationen zu den neuen Verbindungsanforderungen von Campaign finden Sie unter [Migration der technischen Campaign-Benutzer zu Adobe Developer Console](https://experienceleague.adobe.com/docs/campaign/technotes-ac/tn-new/ims-migration.html) in der Campaign-Dokumentation.

1. Klicken Sie in einem beliebigen [!DNL Adobe Campaign]-Modul neben dem Feld [!UICONTROL Verbindung] auf **[!UICONTROL Hinzufügen]** .
1. Füllen Sie die folgenden Felder aus:
   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Verbindungstyp]</td>
          <td>
            <p>Wählen Sie aus, ob Sie eine einfache Verbindung oder eine Server-zu-Server-Verbindung erstellen.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Verbindungsname]</td>
          <td>
            <p>Geben Sie einen Namen für diese Verbindung ein.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Basis-URL]</td>
          <td>Geben Sie die Basis-URL ein, mit der Sie eine Verbindung zu Ihrer [!DNL Adobe Campaign]-Instanz herstellen.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Benutzername]</td>
          <td>Wenn Sie eine Basisverbindung erstellen, geben Sie Ihren Adobe Campaign-Benutzernamen ein.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Kennwort]</td>
          <td>Wenn Sie eine Basisverbindung erstellen, geben Sie Ihr Adobe Campaign-Kennwort ein.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client-ID]</td>
          <td>Wenn Sie eine Server-zu-Server-Verbindung erstellen, geben Sie Ihre [!DNL Adobe] [!UICONTROL Client-ID] ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des Abschnitts [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]</td>
          <td>Wenn Sie eine Server-zu-Server-Verbindung erstellen, geben Sie Ihren [!DNL Adobe] [!UICONTROL Client Secret] ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des Abschnitts [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Umgebung]</td>
          <td>Wählen Sie aus, ob Sie eine Verbindung zu einer Produktions- oder Nicht-Produktionsumgebung herstellen.
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Typ]</td>
          <td>Wählen Sie aus, ob Sie eine Verbindung zu einem Dienstkonto oder einem persönlichen Konto herstellen möchten.
        </tr>
   </tbody>
    </table>
1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

## [!DNL Adobe Campaign] Module und ihre Felder

Wenn Sie [!DNL Adobe Campaign] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Adobe Campaign] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Trigger

#### [!UICONTROL Datensätze ansehen]

Dieses geplante Trigger-Modul startet ein Szenario, wenn sich ein Datensatz ändert.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie in diesem Artikel unter <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Campaign]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Wählen Sie aus, ob Sie nach neuen, aktualisierten Datensätzen oder beidem suchen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Wählen Sie die Ressource aus, die Sie überwachen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Felder für die Ausgabe]</td> 
   <td>Wählen Sie die Felder aus, die Sie in die Ausgabe des Moduls aufnehmen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Benutzerdefinierte Felder für die Ausgabe]</td> 
   <td>Klicken Sie für jedes benutzerdefinierte Feld, das Sie in die Ausgabe aufnehmen möchten, auf "<b>[!UICONTROL Hinzufügen]</b>"und geben Sie den Namen des benutzerdefinierten Felds ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen]</td> 
   <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td> 
  </tr> 
 </tbody> 
</table>


### Aktionen

* [[!UICONTROL Erstellen eines Datensatzes]](#create-a-record)
* [[!UICONTROL Erstellen eines benutzerdefinierten API-Aufrufs]](#make-a-custom-api-call)
* [[!UICONTROL Datensatz löschen]](#delete-record)
* [[!UICONTROL Durchführen einer Aktion]](#perform-an-action)
* [[!UICONTROL Datensatz lesen]](#-read-a-record)
* [[!UICONTROL Abonnieren oder Abmelden]](#subscribe-or-unsubscribe)
* [[!UICONTROL Datensatz aktualisieren]](#update-record)

#### [!UICONTROL Erstellen eines Datensatzes]

Dieses Aktionsmodul erstellt einen neuen Datensatz in [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie in diesem Artikel unter <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Campaign]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Wählen Sie den Typ des zu erstellenden [!DNL Adobe Campaign] Datensatzes aus.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Felder] </td> 
   <td>Wählen Sie die Felder aus, für die Sie bei der Erstellung des Datensatzes Werte festlegen möchten, und geben Sie dann die Werte für diese Felder ein. Die Felder variieren je nach ausgewähltem Datensatztyp.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Benutzerdefinierte Felder]</td> 
   <td> Klicken Sie für jedes benutzerdefinierte Feld, das Sie dem neuen Datensatz hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie den Namen und Wert des Felds ein oder ordnen Sie ihn zu. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen eines benutzerdefinierten API-Aufrufs]

Dieses Modul führt einen benutzerdefinierten API-Aufruf an die [!DNL Adobe Campaign]-API durch

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie in diesem Artikel unter <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Campaign]</a> .</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Aktion]</td>
      <td><p>Wählen Sie die Aktion aus, die der API-Aufruf ausführen soll.</p>
      <p>[!UICONTROL Abfrage ausführen]</p>
      <p>[!UICONTROL Schreiben]</p>
      <p>[!UICONTROL Entität abrufen, falls aktueller)</p>
      <p>[!UICONTROL Alle auswählen]</p>
      <p>[!UICONTROL Push-Ereignis]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Header]</td>
      <td>
        <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p>
        <p>Beispiel: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] fügt die [!UICONTROL x-security]-Token-Kopfzeile automatisch hinzu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL XML Body]</td>
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in XML ohne das Sitzungselement hinzu. </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Datensatz löschen]

Dieses Aktionsmodul löscht einen einzelnen Datensatz aus [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie in diesem Artikel unter <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Campaign]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Wählen Sie den Ressourcentyp aus, den Sie löschen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die Kennung der Ressource ein, die Sie löschen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Durchführen einer Aktion]

Dieses Aktionsmodul führt eine ausgewählte Aktion für ein Objekt in der [!DNL Adobe Campaign]-API aus.

Informationen zu bestimmten Aktionen und Feldern finden Sie in der [[!DNL Adobe Campaign]  - API-Dokumentation](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie in diesem Artikel unter <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Campaign]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aktion]</td> 
   <td><p>Wählen Sie die Aktion aus, die für das Objekt ausgeführt werden soll.</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> Verfügbare Felder finden Sie unter <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> in diesem Artikel. </p></li>
     <li><p><b>[!UICONTROL Get]</b></p><p> Verfügbare Felder finden Sie unter <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> in diesem Artikel. </p></li> 
   <li><p><b>[!UICONTROL Erstellen]</b></p><p> Verfügbare Felder finden Sie unter <a href="#create-a-record" class="MCXref xref" >[!UICONTROL Datensatz erstellen]</a> in diesem Artikel. </p></li>
   <li><p><b>[!UICONTROL Update]</b></p><p> Verfügbare Felder finden Sie unter <a href="#update-record" class="MCXref xref" >[!UICONTROL Datensatz aktualisieren]</a> in diesem Artikel. </p></li>
   <li><p><b>[!UICONTROL Löschen]</b></p><p> Verfügbare Felder finden Sie unter <a href="#delete-record" class="MCXref xref" >[!UICONTROL Datensatz löschen]</a> in diesem Artikel. </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL Datensatz lesen]

Dieses Aktionsmodul liest einen Datensatz aus [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie in diesem Artikel unter <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Campaign]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Wählen Sie den Typ von [!DNL Adobe Campaign] Datensatz aus, den Sie lesen möchten.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Geben Sie die Kennung des Datensatzes, den Sie lesen möchten, ein.</td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL Felder für die Ausgabe] </td> 
   <td>Wählen Sie die Felder aus, die Sie in die Ausgabe des Moduls aufnehmen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Benutzerdefinierte Felder für die Ausgabe]</td> 
   <td>Klicken Sie für jedes benutzerdefinierte Feld, das Sie in die Ausgabe aufnehmen möchten, auf "<b>[!UICONTROL Hinzufügen]</b>"und geben Sie den Namen des benutzerdefinierten Felds ein.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Abonnieren oder Abmelden]

Dieses Aktionsmodul meldet einen Benutzer an oder meldet ihn von einem Informationsdienst ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie in diesem Artikel unter <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Campaign]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abonnieren oder Abmelden]</td> 
   <td>Wählen Sie aus, ob Sie den Informationsdienst abonnieren oder abmelden möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dienstname]</td> 
   <td>Wählen Sie den Dienst aus, den Sie abonnieren oder abmelden möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Empfänger-E-Mail-Adresse] </td> 
   <td>Geben Sie die E-Mail-Adresse des Benutzers ein, den Sie für den Informationsdienst anmelden oder abmelden möchten, oder ordnen Sie diese zu.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datensatz aktualisieren]

Dieses Aktionsmodul aktualisiert einen einzelnen Datensatz in [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie in diesem Artikel unter <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Campaign]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Wählen Sie den Typ des zu erstellenden [!DNL Adobe Campaign] Datensatzes aus.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Geben Sie die Kennung des Datensatzes ein, den Sie aktualisieren möchten.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Felder] </td> 
   <td>Wählen Sie die Felder aus, für die Sie Werte aktualisieren möchten, und geben Sie dann die Werte für diese Felder ein. Die Felder variieren je nach ausgewähltem Datensatztyp.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Benutzerdefinierte Felder]</td> 
   <td> Klicken Sie für jedes benutzerdefinierte Feld, das Sie aktualisieren möchten, auf "<b>[!UICONTROL Element hinzufügen]</b>"und geben Sie den Namen und Wert des Felds ein oder ordnen Sie ihn zu. </td> 
  </tr> 
 </tbody> 
</table>

### Suchvorgänge

#### [!UICONTROL Suche]

Dieses Suchmodul gibt Datensätze zurück, die auf den angegebenen Kriterien basieren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie in diesem Artikel unter <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Campaign]</a> .</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Wählen Sie den Typ des zu erstellenden [!DNL Adobe Campaign] Datensatzes aus.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td> 
  </tr> 
 </tbody> 
</table>
