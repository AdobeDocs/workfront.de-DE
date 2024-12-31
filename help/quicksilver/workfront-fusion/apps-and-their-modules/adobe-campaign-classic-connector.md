---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: Adobe Campaign v7/v8-Module
description: Mit den  [!DNL Adobe Campaign] -Modulen können Sie ein auf  [!DNL Adobe Workfront Fusion]  Ereignissen in Ihrem  [!DNL Adobe Campaign] -Konto basierendes Szenario starten, Vereinbarungen und andere Datensätze erstellen, lesen oder aktualisieren, mit von Ihnen festgelegten Kriterien nach Datensätzen suchen und Dokumente hochladen.
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1448'
ht-degree: 1%

---

# [!DNL Adobe Campaign]

Mit den [!DNL Adobe Campaign]-Modulen können Sie ein [!DNL Adobe Workfront Fusion] Szenario auf der Grundlage von Ereignissen in Ihrem [!DNL Adobe Campaign v7/v8]-Konto starten, Datensätze erstellen, lesen oder aktualisieren, mit von Ihnen festgelegten Kriterien nach Datensätzen suchen und benutzerdefinierte API-Aufrufe durchführen.

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

Fügen Sie die Fusion-IP-Adressen zu [!DNL Adobe Campaign] hinzu.

* Anweisungen zum Hinzufügen von IP-Adressen zu Ihrer Campaign-Zulassungsliste auf die Zulassungsliste setzte finden Sie unter [Hinzufügen von IP-Adressen ](https://experienceleague.adobe.com/en/docs/control-panel/using/sftp-management/ip-range-allow-listing#adding-ip-addresses-allow-list) der Adobe Campaign-Dokumentation.
* Eine Liste der IP-Adressen, die der Zulassungsliste hinzugefügt werden können, finden Sie unter [IP-Adressen für den Zugriff auf Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/get-started/ip-addresses-for-fusion.md).

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
>Es wird dringend empfohlen, eine Server-zu-Server-Verbindung zu erstellen. Adobe Campaign hat seine API so aktualisiert, dass nur Server-zu-Server-Verbindungen akzeptiert werden. Wenn Sie eine Verbindung zu Campaign Version 8 oder höher herstellen, **müssen** eine Server-zu-Server-Verbindung erstellen.
>
>Weitere Informationen zu den neuen Verbindungsanforderungen von Campaign finden Sie unter [Migration technischer Campaign-Benutzerinnen und -Benutzer zu Adobe Developer Console](https://experienceleague.adobe.com/docs/campaign/technotes-ac/tn-new/ims-migration.html) in der Campaign-Dokumentation.

1. Klicken Sie in einem [!DNL Adobe Campaign] Modul **[!UICONTROL Hinzufügen]** neben dem Feld [!UICONTROL Verbindung].
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
            <p>Wählen Sie aus, ob Sie eine Basisverbindung oder eine Server-zu-Server-Verbindung erstellen.</p>
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
          <td>Wenn Sie eine Server-zu-Server-Verbindung erstellen, geben Sie Ihre [!DNL Adobe] [!UICONTROL Client ID] ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client-Geheimnis]</td>
          <td>Wenn Sie eine Server-zu-Server-Verbindung erstellen, geben Sie Ihren [!DNL Adobe] [!UICONTROL Client Secret] ein. Dies finden Sie im Abschnitt [!UICONTROL Anmeldeinformationen] des [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Umgebung]</td>
          <td>Wählen Sie aus, ob Sie eine Verbindung zu einer Produktions- oder Nicht-Produktionsumgebung herstellen.
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Typ]</td>
          <td>Wählen Sie aus, ob Sie eine Verbindung zu einem Service-Konto oder einem persönlichen Konto herstellen möchten.
        </tr>
   </tbody>
    </table>
1. Klicken Sie **[!UICONTROL Fortfahren]**, um die Verbindung zu erstellen, und kehren Sie zum Modul zurück.

## [!DNL Adobe Campaign] Module und ihre Felder

Beim Konfigurieren [!DNL Adobe Campaign] Module zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service weitere [!DNL Adobe Campaign] angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Trigger

#### [!UICONTROL Einträge beobachten]

Dieses Modul für geplante Trigger startet ein Szenario, wenn sich ein Datensatz ändert.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie unter <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Campaign]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL filter]</td> 
   <td>Wählen Sie aus, ob auf neue, aktualisierte oder beides Datensätze geachtet werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Ressource]</td> 
   <td>Wählen Sie die Ressource aus, auf die Sie achten möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Felder, die in die Ausgabe aufgenommen werden sollen]</td> 
   <td>Wählen Sie die Felder aus, die Sie in die Ausgabe des Moduls aufnehmen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!Benutzerdefinierte UICONTROL-Felder, die in die Ausgabe aufgenommen werden sollen]</td> 
   <td>Klicken Sie für jedes benutzerdefinierte Feld, das Sie in die Ausgabe aufnehmen möchten, auf <b>[!UICONTROL Hinzufügen]</b> und geben Sie den Namen des benutzerdefinierten Felds ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl der zurückgegebenen Ergebnisse]</td> 
   <td>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</td> 
  </tr> 
 </tbody> 
</table>


### Aktionen

* [[!UICONTROL Datensatz erstellen]](#create-a-record)
* [[!UICONTROL Erstellen eines benutzerdefinierten API-Aufrufs]](#make-a-custom-api-call)
* [[!UICONTROL Löschen eines Datensatzes]](#delete-record)
* [[!UICONTROL Durchführen einer Aktion]](#perform-an-action)
* [[!UICONTROL Datensatz lesen]](#-read-a-record)
* [[!UICONTROL An- oder Abmelden]](#subscribe-or-unsubscribe)
* [[!UICONTROL Aktualisieren eines Datensatzes]](#update-record)

#### [!UICONTROL Datensatz erstellen]

Dieses Aktionsmodul erstellt einen neuen Datensatz in [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie unter <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Campaign]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Ressource]</td> 
   <td>Wählen Sie den Typ [!DNL Adobe Campaign] Datensatzes aus, den Sie erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Felder] </td> 
   <td>Wählen Sie die Felder aus, für die Sie Werte festlegen möchten, wenn der Datensatz erstellt wird, und füllen Sie dann die Werte für diese Felder aus. Felder variieren je nach ausgewähltem Datensatztyp.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Benutzerdefinierte Felder]</td> 
   <td> Klicken Sie für jedes benutzerdefinierte Feld, das Sie dem neuen Datensatz hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie den Namen und Wert des Feldes ein oder mappen Sie ihn. </td> 
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
      <td role="rowheader">[!UICONTROL-Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie unter <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Campaign]</a> in diesem Artikel.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL-Aktion]</td>
      <td><p>Wählen Sie die Aktion aus, die der API-Aufruf ausführen soll.</p>
      <p>[!UICONTROL Abfrage ausführen]</p>
      <p>[!UICONTROL schreiben]</p>
      <p>[!UICONTROL Entität aus neuerer Zeit abrufen]</p>
      <p>[!UICONTROL Alle auswählen]</p>
      <p>[!UICONTROL Push-Ereignis]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL-Kopfzeilen]</td>
      <td>
        <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p>
        <p>Beispiel: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] fügt automatisch die Kopfzeile des [!UICONTROL x-security]-Tokens hinzu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL XML-Hauptteil]</td>
   <td> <p>Fügen Sie den Hauptteil des API-Aufrufs in XML hinzu, ohne das Sitzungselement zu verwenden. </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Datensatz löschen]

Dieses Aktionsmodul löscht einen einzelnen Datensatz aus [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie unter <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Campaign]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Ressource]</td> 
   <td>Wählen Sie den Ressourcentyp aus, den Sie löschen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die ID der Ressource ein, die Sie löschen möchten, oder mappen Sie sie.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Durchführen einer Aktion]

Dieses Aktionsmodul führt eine ausgewählte Aktion für ein Objekt in der [!DNL Adobe Campaign]-API aus.

Informationen zu bestimmten Aktionen und Feldern finden Sie unter [[!DNL Adobe Campaign]  - API-Dokumentation](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie unter <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Campaign]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Aktion]</td> 
   <td><p>Wählen Sie die Aktion aus, die mit dem Objekt durchgeführt werden soll.</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> Verfügbare Felder finden Sie unter <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> in diesem Artikel. </p></li>
     <li><p><b>[!UICONTROL GET]</b></p><p> Verfügbare Felder finden Sie unter <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> in diesem Artikel. </p></li> 
   <li><p><b>[!UICONTROL Erstellen]</b></p><p> Verfügbare Felder finden Sie unter <a href="#create-a-record" class="MCXref xref" >[!UICONTROL, Datensatz erstellen]</a> in diesem Artikel. </p></li>
   <li><p><b>[!UICONTROL aktualisieren]</b></p><p> Informationen zu verfügbaren Feldern finden Sie unter <a href="#update-record" class="MCXref xref" >[!UICONTROL Aktualisieren eines Datensatzes]</a> in diesem Artikel. </p></li>
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
   <td role="rowheader">[!UICONTROL-Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie unter <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Campaign]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Ressource]</td> 
   <td>Wählen Sie den Typ [!DNL Adobe Campaign] Datensatzes aus, den Sie lesen möchten.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Geben Sie die Zuordnungs-ID des Datensatzes ein, den Sie lesen möchten.</td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL-Felder, die in die Ausgabe aufgenommen werden sollen] </td> 
   <td>Wählen Sie die Felder aus, die Sie in die Ausgabe des Moduls aufnehmen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!Benutzerdefinierte UICONTROL-Felder, die in die Ausgabe aufgenommen werden sollen]</td> 
   <td>Klicken Sie für jedes benutzerdefinierte Feld, das Sie in die Ausgabe aufnehmen möchten, auf <b>[!UICONTROL Hinzufügen]</b> und geben Sie den Namen des benutzerdefinierten Felds ein.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL An- oder Abmelden]

Dieses Aktionsmodul meldet eine Benutzerin bzw. einen Benutzer an oder ab für einen Informations-Service.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie unter <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Campaign]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL An- oder Abmelden]</td> 
   <td>Wählen Sie aus, ob Sie den Informations-Service abonnieren oder abmelden möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Dienstname]</td> 
   <td>Wählen Sie den Service aus, den Sie abonnieren oder abbestellen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Empfänger-E-Mail-Adresse] </td> 
   <td>Geben Sie die E-Mail-Adresse des Benutzers ein, den Sie für den Informations-Service abonnieren oder abmelden möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eintrag aktualisieren]

Dieses Aktionsmodul aktualisiert einen einzelnen Datensatz in [!DNL Adobe Campaign].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie unter <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Campaign]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Ressource]</td> 
   <td>Wählen Sie den Typ [!DNL Adobe Campaign] Datensatzes aus, den Sie erstellen möchten.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Geben Sie die Zuordnungs-ID des Datensatzes ein, den Sie aktualisieren möchten.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL-Felder] </td> 
   <td>Wählen Sie die Felder aus, für die Sie Werte aktualisieren möchten, und füllen Sie dann die Werte für diese Felder aus. Felder variieren je nach ausgewähltem Datensatztyp.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Benutzerdefinierte Felder]</td> 
   <td> Klicken Sie für jedes benutzerdefinierte Feld, das Sie aktualisieren möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie den Namen und den Wert des Felds ein oder ordnen Sie ihn zu. </td> 
  </tr> 
 </tbody> 
</table>

### Suchvorgänge

#### [!UICONTROL Suche]

Dieses Suchmodul gibt Datensätze basierend auf den angegebenen Kriterien zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign] finden Sie unter <a href="#connect-adobe-campaign-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe Campaign]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Ressource]</td> 
   <td>Wählen Sie den Typ [!DNL Adobe Campaign] Datensatzes aus, den Sie erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</td> 
  </tr> 
 </tbody> 
</table>
