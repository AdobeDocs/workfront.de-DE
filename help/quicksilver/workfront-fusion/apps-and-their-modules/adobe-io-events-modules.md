---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Adobe I/O-Ereignismodule
description: Mit den Adobe I/O-Ereignismodulen können Sie ein Adobe Workfront Fusion-Szenario starten, das auf Ereignissen in Ihren Adobe-Anwendungen basiert.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 18ad8098-9742-44d2-97cd-b0c2b5591538
source-git-commit: db322faeb53a0ae4a061076d457f3c10c31ec33c
workflow-type: tm+mt
source-wordcount: '912'
ht-degree: 1%

---

# Adobe I/O-Ereignismodule

Mit den Adobe I/O-Ereignismodulen können Sie ein Adobe Workfront Fusion-Szenario starten, das auf Ereignissen in Adobe-Konten und -Diensten basiert, die über keinen dedizierten Workfront Fusion-Connector verfügen.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Pro oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan, Arbeit</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion-Lizenz**</td> 
   <td> <p>Workfront Fusion für Arbeitsautomatisierung und -integration </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss Adobe Workfront Fusion sowie Adobe Workfront erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

&#42;&#42;Informationen zu Adobe Workfront Fusion-Lizenzen finden Sie unter [Adobe Workfront Fusion-Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Voraussetzungen

Bevor Sie den Adobe I/O Events Connector verwenden können, müssen Sie sicherstellen, dass die folgenden Voraussetzungen erfüllt sind:

* Sie müssen über ein aktives Adobe-Konto verfügen.

## Herstellen einer Verbindung zu Adobe I/O-Ereignissen

So erstellen Sie eine Verbindung für Ihre Adobe I/O-Ereignismodule:

1. Klicken Sie neben dem Feld Verbindung auf Hinzufügen .

1. Füllen Sie die folgenden Felder aus:

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">Verbindungsname</td>
        <td>
          <p>Geben Sie einen Namen für diese Verbindung ein.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Typ</td>
        <td>
          <p>Wählen Sie aus, ob Sie eine Verbindung zu einem Dienstkonto oder einem persönlichen Konto herstellen möchten.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Zusätzliche Bereiche</td>
        <td>Um weitere Bereiche hinzuzufügen, klicken Sie auf <b>Element hinzufügen</b> und geben Sie den Bereich ein.</td>
      </tr>
      <tr>
        <td role="rowheader">Client-ID</td>
        <td>Geben Sie Ihre Adobe Client-ID ein. Dies finden Sie im Abschnitt mit Anmeldeinformationen des Adobe Developer Console</td>
      </tr>
      <tr>
        <td role="rowheader">Geheimer Client-Schlüssel</td>
        <td>Geben Sie Ihren Adobe Client Secret ein. Dies finden Sie im Abschnitt mit Anmeldeinformationen des Adobe Developer Console</td>
      </tr>
      </tr>
        <tr>
        <td role="rowheader">Kundenorg-ID</td>
        <td>Geben Sie Ihre Kundenorg-ID ein. Dies finden Sie in der Berechtigungs-URL des Projekts: <code>https://developer.adobe.com/console/projects/{consumer org ID}/ {project ID}/credentials/{credential ID}/details</code></td>
      </tr>
      <tr>
        <td role="rowheader">Credential ID</td>
        <td>Geben Sie Ihre Berechtigungs-ID ein. Dies finden Sie in der Berechtigungs-URL des Projekts: <code>https://developer.adobe.com/console/projects/{consumer org ID}/ {project ID}/credentials/{credential ID}/details</code></td>
      </tr>
      <tr>
        <td role="rowheader">Kennung der IMS-Organisation</td>
        <td>Geben Sie Ihre Adobe-Organisations-ID ein. Dies finden Sie im Abschnitt mit Anmeldeinformationen des Adobe Developer Console</td>
      </tr>
        <tr>
        <td role="rowheader">Projekt-ID</td>
        <td>Geben Sie Ihre Projekt-ID ein. Dies finden Sie in der Berechtigungs-URL des Projekts: <code>https://developer.adobe.com/console/projects/{consumer org ID}/ {project ID}/credentials/{credential ID}/details</code></td>
      </tr>
      <tr>
        <td role="rowheader">WORKSPACE ID</td>
        <td>Laden Sie Ihre Projektdetails von der Projektübersichtsseite in Adobe Developer Console herunter, um die Workspace ID Ihres Projekts anzuzeigen. </td>
      </tr>
    </tbody>
    </table>

1. Klicken Sie auf **Weiter** , um die Verbindung zu speichern und zum Modul zurückzukehren.

## Adobe I/O-Ereignismodule und ihre Felder

Wenn Sie [!DNL Adobe I/O Events] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Adobe I/O Events] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Trigger

#### Ereignisregistrierung erstellen

Dieses Aktionsmodul verwendet einen Webhook, um eine Ereignisbeschreibung zu erstellen. Hier können Sie einen Webhook konfigurieren. Wenn Sie einen vorhandenen Webhook verwenden, sind die Felder in diesem Modul schreibgeschützt.

So erstellen Sie einen Webhook:

1. Klicken Sie neben dem Webhook-Feld auf **Hinzufügen** .
1. Füllen Sie die folgenden Felder aus:

   <table>
     <col/>
     <col/>
     <tbody>
       <tr>
         <td role="rowheader">[!UICONTROL Webhook name]</td>
        <td>Geben Sie einen Namen für diesen Webhook ein.</td>
       </tr>
       <tr>
         <td role="rowheader">[!UICONTROL Verbindung]</td>
        <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe I/O Events] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe I/O Events]</a> .</td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Webhook description]
         </td>
         <td>
           Geben Sie eine Beschreibung für diesen Webhook ein.
        </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Ereignisanbieter]
         </td>
         <td>
           Wählen Sie das Produkt oder Konto aus, aus dem Sie Ereignisse erstellen möchten.
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Ereignistyp]
         </td>
         <td>
           Wählen Sie die Ereignisse aus, die der Webhook überwachen soll. Das Szenario wird Trigger, wenn diese Ereignisse auftreten.
         </td>
       </tr>
     </tbody>
   </table>

1. Klicken Sie auf Speichern , um den Webhook zu speichern und zum Modul zurückzukehren.

### Aktionen

#### Abrufen aller Ereignisse aus einem Protokoll

Dieses Suchmodul ruft alle Ereignisse für eine Registrierung aus einem Protokoll ab.

<table>
     <col/>
     <col/>
     <tbody>
       <tr>
         <td role="rowheader">[!UICONTROL Verbindung]</td>
        <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe I/O Events] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe I/O Events]</a> .</td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Registrierungs-ID]
         </td>
         <td>
           Wählen Sie die Registrierung aus, für die Sie Ereignisse abrufen möchten.
        </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Maximale Anzahl an zurückgegebenen Datensätzen]
         </td>
         <td>
              Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll. 
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Rückkehrereignisse, die nach auftreten]
         </td>
         <td>
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Seek]
         </td>
         <td>
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Neueste Version]
         </td>
         <td>
         Aktivieren Sie diese Option, um das neueste Ereignis zurückzugeben.
         </td>
       </tr>
     </tbody>
   </table>

#### Benutzerdefinierte API-Aufrufe durchführen

Dieses Aktionsmodul führt einen benutzerdefinierten API-Aufruf an die [!DNL Adobe I/O Events]-API durch

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Verbindung]</td>
        <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe I/O Events] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe I/O Events]</a> .</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Geben Sie einen Pfad relativ zu ein <code>https://api.adobe.io/events</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Methode]</p>
      </td>
      <td>
  <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p>  
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Header]</td>
      <td>
        <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p>
        <p>Beispiel: <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion fügt Autorisierungs-Header und x-api-Schlüssel-Header automatisch hinzu.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Abfragezeichenfolge]  </td>
      <td>
        <p>Geben Sie die Abfragezeichenfolge der Anfrage ein.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### Suchvorgänge

#### Abrufen von Anbieter- und Ereignis-IDs

Dieses Suchmodul ruft die Adobe I/O Events-IDs für den angegebenen Anbieter und die angegebenen Ereignisse ab.

<table>
     <col/>
     <col/>
     <tbody>
       <tr>
         <td role="rowheader">[!UICONTROL Verbindung]</td>
        <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Adobe I/O Events] finden Sie in diesem Artikel unter <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >Erstellen einer Verbindung zu [!DNL Adobe I/O Events]</a> .</td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Ereignisanbieter]
         </td>
         <td>
           Wählen Sie den Provider aus, für den Sie die ID abrufen möchten.
        </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Ereignistyp]
         </td>
         <td>
              Wählen Sie die Ereignisse aus, für die Sie IDs bereitstellen möchten. Ereignisse sind je nach Ereignisanbieter verfügbar. 
         </td>
       </tr>
     </tbody>
   </table>

<!--

Watch Events

This trigger module starts a scenario when an event occurs in the chosen Adobe product or service.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Webhook</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>Add</b> next to the webhook field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The source of the events you want to watch</li></ul></li><li>Click <b>Save</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

-->
