---
title: Jira-Softwaremodule
description: In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Jira] Software, sowie die Verbindung mit mehreren Anwendungen und Services von Drittanbietern.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2085'
ht-degree: 1%

---

# [!DNL Jira Software]-Module

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Jira Software], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.

Informationen zum Erstellen eines Szenarios finden Sie unter [Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

<!-- Bob Fix this compared to original -->

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

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Voraussetzungen

Verwendung [!DNL Jira] -Module müssen Sie über eine [!DNL Jira] -Konto.

## Verbinden [!DNL Jira Software] nach [!DNL Workfront Fusion]

Ihre Verbindungsmethode basiert auf der Verwendung von [!DNL Jira Cloud] oder [!DNL Jira Server].

* [Verbinden [!DNL Jira Cloud] zu Workfront Fusion](#connect-jira-cloud-to-workfront-fusion)
* [Verbinden [!DNL Jira Server] nach [!DNL Workfront Fusion]](#connect-jira-server-to-workfront-fusion)

### Verbinden [!DNL Jira Cloud] nach [!DNL Workfront Fusion]

Verbinden [!DNL Jira Cloud] nach [!DNL Workfront Fusion]

Verbindung herstellen [!DNL Jira Software] nach [!DNL Workfront Fusion]müssen Sie ein API-Token erstellen und es zusammen mit Ihrer Dienst-URL und Ihrem Benutzernamen in die [!UICONTROL Verbindung erstellen] -Feld in [!DNL Workfront Fusion].

#### API-Token erstellen in [!DNL Jira]

1. Navigieren Sie zu [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) und melden Sie sich an.
1. Klicken **[!UICONTROL API-Token erstellen]**.
1. Geben Sie einen Namen für das Token ein, z. B. *Workfront Fusion*.
1. Kopieren Sie das Token mithilfe der **[!UICONTROL In Zwischenablage kopieren]** Schaltfläche.

   >[!IMPORTANT]
   >
   >Sie können das Token nach dem Schließen dieses Dialogfelds nicht erneut anzeigen.
1. Speichern Sie das generierte Token an einem sicheren Ort.
1. Fahren Sie mit [Konfigurieren Sie die [!DNL Jira] API-Token in [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion).

#### Konfigurieren Sie die [!DNL Jira] API-Token in [!DNL Workfront Fusion]

1. In [!DNL Workfront Fusion], fügen Sie eine [!DNL Jira] -Modul in ein Szenario klicken, um **[!UICONTROL Verbindung erstellen]** ankreuzen.
1. Geben Sie die folgenden Informationen an:

   * **[!UICONTROL Dienst-URL]**
   * **[!UICONTROL Benutzername]**
   * **[!UICONTROL API-Token]:** Dies ist das API-Token, das Sie im [API-Token erstellen in [!DNL Jira]](#create-an-api-token-in-jira) Abschnitt dieses Artikels.

1. Klicken [!UICONTROL Weiter] , um die Verbindung zu erstellen und zum Modul zurückzukehren.

### Verbinden [!DNL Jira Server] nach [!DNL Workfront Fusion]

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

So autorisieren Sie eine Verbindung zwischen [!DNL Workfront Fusion] und [!DNL Jira Server], benötigen Sie Ihren Kundenschlüssel, Ihren privaten Schlüssel und Ihre Dienst-URL. Möglicherweise müssen Sie Ihre [!DNL Jira] Administrator für diese Informationen.

* [Generieren Sie öffentliche und private Schlüssel für Ihre [!DNL Jira] connection](#generate-public-and-private-keys-for-your-jira-connection)
* [Konfigurieren Sie die Client-App als Verbraucher in [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)
* [Erstellen Sie eine Verbindung zu [!DNL Jira] Server- oder Jira-Rechenzentrum in [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Generieren Sie öffentliche und private Schlüssel für Ihre [!DNL Jira] connection

So erwerben Sie einen privaten Schlüssel für Ihre [!DNL Workfront Fusion Jira] -Verbindung, müssen Sie öffentliche und private Schlüssel generieren.

1. Führen Sie in Ihrem Terminal Folgendes aus: `openssl` Befehle.

   * `openssl genrsa -out jira_privatekey.pem 1024`

     Dieser Befehl generiert einen privaten 1024-Bit-Schlüssel.

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

     Dieser Befehl erstellt ein X509-Zertifikat.

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

     Dieser Befehl extrahiert den privaten Schlüssel (PKCS8-Format) in den `jira_privatekey.pcks8`
-Datei.

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

     Dieser Befehl extrahiert den öffentlichen Schlüssel aus dem Zertifikat in den `jira_publickey.pem` -Datei.

     >[!NOTE]
     >
     >Wenn Sie Windows verwenden, müssen Sie möglicherweise den öffentlichen Schlüssel im `jira_publickey.pem` Datei manuell:
     >
     >1. Führen Sie in Ihrem Terminal den folgenden Befehl aus:
     >   
     >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
     >   
     >1. Kopieren Sie die Terminal-Ausgabe (einschließlich `-------BEGIN PUBLIC KEY--------` und `-------END PUBLIC KEY--------`
     >   
     >1. Fügen Sie die Terminal-Ausgabe in eine Datei mit dem Namen `jira_publickey.pem`.


1. Weiter zu [Konfigurieren Sie die Client-App als Verbraucher in [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)

#### Konfigurieren Sie die Client-App als Verbraucher in [!DNL Jira]

1. Melden Sie sich bei Ihrer [!DNL Jira] -Instanz.
1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL [!DNL Jira]Einstellungen]** ![](assets/jira-settings-icon.png) > **[!UICONTROL Anwendungen]**> **[!UICONTROL Anwendungslinks]**.
1. Im **[!UICONTROL Geben Sie die URL der Anwendung ein, die Sie verknüpfen möchten]** Feld, eingeben

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. Klicken **[!UICONTROL Neuen Link erstellen]**. Ignorieren Sie die Fehlermeldung &quot;Von der eingegebenen URL wurde keine Antwort empfangen&quot;.
1. Im **[!UICONTROL Verknüpfen von Anwendungen]** -Fenster, geben Sie Werte in **[!UICONTROL Consumer key]** und **[!UICONTROL Gemeinsamer geheimer Schlüssel]** -Felder.

   Sie können die Werte für diese Felder auswählen.

1. Kopieren Sie die Werte der **[!UICONTROL Consumer key]** und **[!UICONTROL Gemeinsamer geheimer Schlüssel]** an einen sicheren Speicherort.

   Sie benötigen diese Werte später im Konfigurationsprozess.

1. Füllen Sie die URL-Felder wie folgt aus:

   | Feld | Beschreibung |
   |---|---|
   | [!UICONTROL Anfrage-Token-URL] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL Autorisierungs-URL] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL Zugriffstoken-URL] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. Wählen Sie die **[!UICONTROL Eingehende Links erstellen]** aktivieren.
1. Klicken **[!UICONTROL Weiter]**.
1. Im **[!UICONTROL Verknüpfen von Anwendungen]** die folgenden Felder ausfüllen:

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Consumer Key]</p> </td> 
      <td> Fügen Sie den Consumer-Schlüssel ein, den Sie an einen sicheren Speicherort kopiert haben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Kundenname]</td> 
      <td>Geben Sie einen Namen Ihrer Wahl ein. Dieser Name dient Ihrer eigenen Referenz.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Public key]</td> 
      <td>Fügen Sie den öffentlichen Schlüssel aus Ihrem <code>[!DNL jira_publickey.pem]</code> -Datei.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **[!UICONTROL Weiter]**.
1. Weiter zu [Erstellen Sie eine Verbindung zu [!DNL Jira Server] oder [!DNL Jira Data Center] in [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Erstellen Sie eine Verbindung zu [!DNL Jira Server] oder [!DNL Jira Data Center] in [!DNL Workfront Fusion]

>[!NOTE]
>
>Verwenden Sie die [!DNL Jira Server] App, mit der eine Verbindung hergestellt wird [!DNL Jira Server] oder [!DNL Jira Data Center].
1. In jeder [!DNL Jira Server] -Modul in [!DNL Workfront Fusion]klicken **[!UICONTROL Hinzufügen]** neben dem [!UICONTROL connection] -Feld.
1. Im [!UICONTROL Verbindung erstellen] die folgenden Felder aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Verbindungsname]</p> </td> 
      <td> <p>Geben Sie einen Namen für die Verbindung ein</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Consumer Key]</td> 
      <td>Fügen Sie den Consumer-Schlüssel ein, den Sie an einen sicheren Speicherort in kopiert haben. <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">Konfigurieren Sie die Client-App als Verbraucher in [!DNL Jira]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>Fügen Sie den privaten Schlüssel aus dem <code>[!DNL jira_privatekey.pcks8]</code> Datei, die Sie in <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">Generieren Sie öffentliche und private Schlüssel für Ihre [!DNL Jira] connection</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>Geben Sie Ihre [!DNL Jira] Instanz-URL. </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

## [!DNL Jira Software] Module und ihre Felder

Bei der Konfiguration [!DNL Jira Software] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Jira Software] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Trigger

#### [!UICONTROL Auf Datensätze achten]

Dieses Trigger-Modul startet ein Szenario, wenn ein Datensatz hinzugefügt, aktualisiert oder gelöscht wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Wählen Sie den Webhook aus, den Sie verwenden möchten, um nach Datensätzen zu suchen. </p> <p>So fügen Sie einen neuen Webhook hinzu:</p> 
    <ol> 
     <li value="1">Klicken <strong>[!UICONTROL Hinzufügen]</strong></li> 
     <li value="2">Geben Sie einen Namen für den Webhook ein.</li> 
     <li value="3"> <p>Wählen Sie die Verbindung aus, die Sie für Ihren Webhook verwenden möchten. </p> <p>Anweisungen zum Verbinden der [!DNL Jira Software] Konto [!DNL Workfront Fusion], siehe <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </li> 
     <li value="4"> <p>Wählen Sie den Datensatztyp aus, den die Software überwachen soll:</p> 
      <ul> 
       <li>[!UICONTROL Kommentar] </li> 
       <li>[!UICONTROL Problem]</li> 
       <li>[!UICONTROL Projekt] </li> 
       <li>[!UICONTROL Sprint]</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL Problem zum Sprint hinzufügen]](#add-issue-to-sprint)
* [[!UICONTROL Benutzerspezifischer API-Aufruf]](#custom-api-call)
* [[!UICONTROL Datensatz erstellen]](#create-a-record)
* [[!UICONTROL Datensatz löschen]](#delete-a-record)
* [[!UICONTROL Anlage herunterladen]](#download-an-attachment)
* [[!UICONTROL Datensatz lesen]](#read-a-record)
* [[!UICONTROL Datensatz aktualisieren]](#update-a-record)

#### [!UICONTROL Problem zum Sprint hinzufügen]

Dieses Aktionsmodul fügt einem Sprint ein oder mehrere Probleme hinzu.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Jira Software] Konto [!DNL Workfront Fusion], siehe <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sprint ID]</td> 
   <td>Geben Sie die Sprint-ID des Sprints ein oder ordnen Sie sie zu, dem Sie ein Problem hinzufügen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Problem-ID oder Schlüssel]</td> 
   <td>Fügen Sie für jedes Problem, das Sie zum Sprint hinzufügen möchten, eine Problem-ID oder einen Schlüssel hinzu.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datensatz erstellen]

Dieses Aktionsmodul erstellt einen neuen Datensatz in Jira.

Das Modul gibt alle mit dem Datensatz verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Jira Software] Konto [!DNL Workfront Fusion], siehe <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Datensatztyp aus, den das Modul erstellen soll. Wenn Sie einen Datensatztyp auswählen, werden andere für diesen Datensatztyp spezifische Felder im Modul angezeigt.</p> 
    <ul> 
     <li>[!UICONTROL Anhang]</li> 
     <li>[!UICONTROL Kommentar]</li> 
     <li>[!UICONTROL Problem]</li> 
     <li>[!UICONTROL Projekt]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Benutzerspezifischer API-Aufruf]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Jira Software] API. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von der anderen nicht durchgeführt werden kann [!DNL Jira Software] Module.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Jira Software] Konto [!DNL Workfront Fusion], siehe <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Geben Sie einen Pfad relativ zu ein<code>&lt;Instance URL>/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode]</td> 
   td&gt; <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"name":"something-urgent"}</code></p> </td> 
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

Dieses Aktionsmodul löscht einen bestimmten Datensatz.

Sie geben die Kennung des Datensatzes an.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Jira Software] Konto [!DNL Workfront Fusion], siehe <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Datensatztyp aus, den das Modul löschen soll. </p> 
    <ul> 
     <li>[!UICONTROL Anhang]</li> 
     <li>[!UICONTROL Kommentar]</li> 
     <li>[!UICONTROL Problem]</li> 
     <li>[!UICONTROL Projekt]</li> 
     <li>[!UICONTROL Sprint] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID oder Schlüssel]</td> 
   <td>Geben Sie die Kennung oder den Schlüssel des Datensatzes ein, den Sie löschen möchten, oder ordnen Sie ihn zu.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Anlage herunterladen]

Dieses Aktionsmodul lädt eine bestimmte Anlage herunter.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Jira Software] Konto [!DNL Workfront Fusion], siehe <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die Kennung des Anhangs ein, den Sie herunterladen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datensatz lesen]

Dieses Aktionsmodul liest Daten aus einem einzelnen Datensatz in [!DNL Jira Software].

Sie geben die Kennung des Datensatzes an.

Das Modul gibt alle mit dem Datensatz verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Jira Software] Konto [!DNL Workfront Fusion], siehe <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ [!DNL Jira] -Datensatz, den das -Modul lesen soll.</p> 
    <ul> 
     <li>[!UICONTROL Anhang]</li> 
     <li>[!UICONTROL Problem]</li> 
     <li>[!UICONTROL Projekt]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Benutzer]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td>Wählen Sie die Ausgaben aus, die Sie empfangen möchten. Die Ausgabeoptionen sind je nach dem im Feld "[!UICONTROL Record Type]" ausgewählten Datensatztyp verfügbar.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Eindeutige Eingabe oder Zuordnung [!DNL Jira Software] Kennung des Datensatzes, den das Modul lesen soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datensatz aktualisieren]

Dieses Aktionsmodul aktualisiert einen vorhandenen Datensatz, z. B. ein Problem oder ein Projekt.

Sie geben die Kennung des Datensatzes an.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Jira Software] Konto [!DNL Workfront Fusion], siehe <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Datensatztyp aus, den das Modul aktualisieren soll. Wenn Sie einen Datensatztyp auswählen, werden andere für diesen Datensatztyp spezifische Felder im Modul angezeigt.</p> 
    <ul> 
     <li>[!UICONTROL Kommentar]</li> 
     <li>[!UICONTROL Problem]</li> 
     <li>[!UICONTROL Projekt]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Übergangsproblem]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID oder Schlüssel]</td> 
   <td>Geben Sie die Kennung oder den Schlüssel des Datensatzes ein oder ordnen Sie ihn zu.</td> 
  </tr> 
 </tbody> 
</table>

### Suchvorgänge

* [[!UICONTROL Auflisten von Datensätzen]](#list-records)
* [[!UICONTROL Datensätze suchen]](#search-for-records)

#### [!UICONTROL Auflisten von Datensätzen]

Dieses Suchmodul ruft alle Elemente eines bestimmten Typs ab, die mit Ihrer Suchabfrage übereinstimmen

Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Jira Software] Konto [!DNL Workfront Fusion], siehe <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Datensatztyp aus, den das Modul auflisten soll. Wenn Sie einen Datensatztyp auswählen, werden andere für diesen Datensatztyp spezifische Felder im Modul angezeigt.</p> 
    <ul> 
     <li>[!UICONTROL Kommentar]</li> 
     <li>[!UICONTROL Problem]</li> 
     <li>[!UICONTROL Projekt]</li> 
     <li>[!UICONTROL Sprint issue]</li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Max Results]</p> </td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen des Szenarios abrufen soll.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Offset</td> 
    <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL Datensätze suchen]

Dieses Suchmodul sucht nach Datensätzen in einem Objekt in [!DNL Jira Software] die mit der angegebenen Suchabfrage übereinstimmen.

Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Jira Software] Konto [!DNL Workfront Fusion], siehe <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden [!DNL Jira Software] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Datensatztyp aus, nach dem das Modul suchen soll. Wenn Sie einen Datensatztyp auswählen, werden andere für diesen Datensatztyp spezifische Felder im Modul angezeigt.</p> 
    <ul> 
     <li>[!UICONTROL Probleme]</li> 
     <li> <p>[!UICONTROL Probleme durch JQL (Jira Query Language)] </p> <p>Weitere Informationen zu JQL finden Sie unter <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> auf der Hilfeseite von Atlassian. </p> </li> 
     <li>[!UICONTROL Projekt]</li> 
     <li>[!UICONTROL Projekt nach Ausgabe]</li> 
     <li>[!UICONTROL Benutzer]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
