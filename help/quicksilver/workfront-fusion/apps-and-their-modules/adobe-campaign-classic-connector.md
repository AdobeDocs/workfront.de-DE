---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Adobe Campaign Classic-Module
description: Mit dem [!DNL Adobe Campaign Classic] -Module, können Sie eine [!DNL Adobe Workfront Fusion] Szenario basierend auf Ereignissen in Ihrer [!DNL Adobe Campaign Classic] Konten, erstellen, lesen oder aktualisieren Sie Vereinbarungen und andere Datensätze, suchen Sie nach Datensätzen anhand von von Ihnen festgelegten Kriterien und laden Sie Dokumente hoch.
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 482725764ede6b2700985fa67dc2cb9f92d3bb12
workflow-type: tm+mt
source-wordcount: '1146'
ht-degree: 1%

---

# [!DNL Adobe Campaign Classic]-Module

Mit dem [!DNL Adobe Campaign Classic] -Module, können Sie eine [!DNL Adobe Workfront Fusion] Szenario basierend auf Ereignissen in Ihrer [!DNL Adobe Campaign Classic] -Konto, erstellen, lesen oder aktualisieren Sie Datensätze, suchen Sie mithilfe der von Ihnen festgelegten Kriterien nach Datensätzen und führen Sie benutzerdefinierte API-Aufrufe durch.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Verbinden [!DNL Adobe Campaign Classic] nach [!DNL Adobe Workfront Fusion]

1. In jeder [!DNL Adobe Campaign Classic] Modul, klicken Sie auf **[!UICONTROL Hinzufügen]** neben dem [!UICONTROL Verbindung] -Feld.
1. Geben Sie die Basis-URL ein, über die Sie eine Verbindung zu Ihrer [!DNL Adobe Campaign Classic] -Instanz.
1. Geben Sie Ihren Benutzernamen und Ihr Passwort ein.
1. Klicken **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

## [!DNL Adobe Campaign Classic] Module und ihre Felder

Bei der Konfiguration [!DNL Adobe Campaign Classic] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Adobe Campaign Classic] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Trigger

#### [!UICONTROL Aufnahmen ansehen]

Dieses geplante Trigger-Modul startet ein Szenario, wenn sich ein Datensatz ändert.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign Classic], siehe <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Campaign Classic]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Wählen Sie aus, ob Sie nach neuen, aktualisierten oder beidem suchen möchten.</td> 
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
   <td>Klicken Sie für jedes benutzerdefinierte Feld, das Sie in die Ausgabe einbeziehen möchten, auf <b>[!UICONTROL Hinzufügen]</b> und geben Sie den Namen des benutzerdefinierten Felds ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl an zurückgegebenen Ergebnissen]</td> 
   <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td> 
  </tr> 
 </tbody> 
</table>


### Aktionen

* [[!UICONTROL Datensatz erstellen]](#create-a-record)
* [[!UICONTROL Benutzerdefinierte API-Aufrufe durchführen]](#make-a-custom-api-call)
* [[!UICONTROL Datensatz löschen]](#delete-record)
* [[!UICONTROL Durchführen einer Aktion]](#perform-an-action)
* [[!UICONTROL Datensatz lesen]](#-read-a-record)
* [[!UICONTROL Abonnieren oder Abmelden]](#subscribe-or-unsubscribe)
* [[!UICONTROL Datensatz aktualisieren]](#update-record)

#### [!UICONTROL Datensatz erstellen]

Dieses Aktionsmodul erstellt einen neuen Datensatz in [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign Classic], siehe <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Campaign Classic]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Wählen Sie den Typ [!DNL Adobe Campaign Classic] -Datensatz, den Sie erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Felder] </td> 
   <td>Wählen Sie die Felder aus, für die Sie bei der Erstellung des Datensatzes Werte festlegen möchten, und geben Sie dann die Werte für diese Felder ein. Die Felder variieren je nach ausgewähltem Datensatztyp.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Benutzerdefinierte Felder]</td> 
   <td> Klicken Sie für jedes benutzerdefinierte Feld, das Sie zum neuen Datensatz hinzufügen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie den Namen und Wert des Felds ein oder ordnen Sie ihn zu. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Benutzerdefinierte API-Aufrufe durchführen]

Dieses Modul führt einen benutzerdefinierten API-Aufruf an die [!DNL Adobe Campaign Classic] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign Classic], siehe <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Campaign Classic]</a> in diesem Artikel.</td> 
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

Dieses Aktionsmodul löscht einen einzelnen Datensatz aus [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign Classic], siehe <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Campaign Classic]</a> in diesem Artikel.</td> 
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

Dieses Aktionsmodul führt eine ausgewählte Aktion für ein Objekt im [!DNL Adobe Campaign Classic] API.

Informationen zu bestimmten Aktionen und Feldern finden Sie unter [[!DNL Adobe Campaign] - API-Dokumentation](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign Classic], siehe <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Campaign Classic]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aktion]</td> 
   <td><p>Wählen Sie die Aktion aus, die für das Objekt ausgeführt werden soll.</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> Verfügbare Felder finden Sie unter <a href="#search" class="MCXref xref" >[!UICONTROL Suche]</a> in diesem Artikel. </p></li>
     <li><p><b>[!UICONTROL Get]</b></p><p> Verfügbare Felder finden Sie unter <a href="#search" class="MCXref xref" >[!UICONTROL Suche]</a> in diesem Artikel. </p></li> 
   <li><p><b>[!UICONTROL Erstellen]</b></p><p> Verfügbare Felder finden Sie unter <a href="#create-a-record" class="MCXref xref" >[!UICONTROL Datensatz erstellen]</a> in diesem Artikel. </p></li>
   <li><p><b>[!UICONTROL Update]</b></p><p> Verfügbare Felder finden Sie unter <a href="#update-record" class="MCXref xref" >[!UICONTROL Datensatz aktualisieren]</a> in diesem Artikel. </p></li>
   <li><p><b>[!UICONTROL Löschen]</b></p><p> Verfügbare Felder finden Sie unter <a href="#delete-record" class="MCXref xref" >[!UICONTROL Datensatz löschen]</a> in diesem Artikel. </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL Datensatz lesen]

Dieses Aktionsmodul liest einen Datensatz aus [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign Classic], siehe <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Campaign Classic]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Wählen Sie den Typ [!DNL Adobe Campaign Classic] -Eintrag, den Sie lesen möchten.</td> 
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
   <td>Klicken Sie für jedes benutzerdefinierte Feld, das Sie in die Ausgabe einbeziehen möchten, auf <b>[!UICONTROL Hinzufügen]</b> und geben Sie den Namen des benutzerdefinierten Felds ein.</td> 
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
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign Classic], siehe <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Campaign Classic]</a> in diesem Artikel.</td> 
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

Dieses Aktionsmodul aktualisiert einen einzelnen Datensatz in [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td>
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign Classic], siehe <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Campaign Classic]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Wählen Sie den Typ [!DNL Adobe Campaign Classic] -Datensatz, den Sie erstellen möchten.</td> 
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
   <td> Klicken Sie für jedes benutzerdefinierte Feld, das Sie aktualisieren möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie den Namen und Wert des Felds ein oder ordnen Sie ihn zu. </td> 
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
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe Campaign Classic], siehe <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Erstellen Sie eine Verbindung zu [!DNL Adobe Campaign Classic]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Wählen Sie den Typ [!DNL Adobe Campaign Classic] -Datensatz, den Sie erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td> 
  </tr> 
 </tbody> 
</table>
