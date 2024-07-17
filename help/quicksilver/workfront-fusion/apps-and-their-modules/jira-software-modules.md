---
title: Jira-Softwaremodule
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die [!DNL Jira] Software verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2072'
ht-degree: 1%

---

# [!DNL Jira Software] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Jira Software] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

<!-- Bob Fix this compared to original -->

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

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Voraussetzungen

Um [!DNL Jira] -Module zu verwenden, müssen Sie über ein [!DNL Jira] -Konto verfügen.

## [!DNL Jira Software] mit [!DNL Workfront Fusion] verbinden

Ihre Verbindungsmethode basiert darauf, ob Sie [!DNL Jira Cloud] oder [!DNL Jira Server] verwenden.

* [Verbinden von [!DNL Jira Cloud] mit Workfront Fusion](#connect-jira-cloud-to-workfront-fusion)
* [ [!DNL Jira Server] an [!DNL Workfront Fusion] verbinden](#connect-jira-server-to-workfront-fusion)

### [!DNL Jira Cloud] mit [!DNL Workfront Fusion] verbinden

[!DNL Jira Cloud] mit [!DNL Workfront Fusion] verbinden

Um [!DNL Jira Software] mit [!DNL Workfront Fusion] zu verbinden, müssen Sie ein API-Token erstellen und es zusammen mit Ihrer Dienst-URL und Ihrem Benutzernamen in das Feld [!UICONTROL Verbindung erstellen] in [!DNL Workfront Fusion] einfügen.

#### API-Token in [!DNL Jira] erstellen

1. Gehen Sie zu [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) und melden Sie sich an.
1. Klicken Sie auf **[!UICONTROL API-Token erstellen]**.
1. Geben Sie einen Namen für das Token ein, z. B. *Workfront Fusion*.
1. Kopieren Sie das Token mithilfe der Schaltfläche **[!UICONTROL In die Zwischenablage kopieren]** .

   >[!IMPORTANT]
   >
   >Sie können das Token nach dem Schließen dieses Dialogfelds nicht erneut anzeigen.
1. Speichern Sie das generierte Token an einem sicheren Ort.
1. Fahren Sie mit [Konfigurieren des  [!DNL Jira] API-Tokens in [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion) fort.

#### Konfigurieren des [!DNL Jira]-API-Tokens in [!DNL Workfront Fusion]

1. Fügen Sie in [!DNL Workfront Fusion] ein [!DNL Jira] -Modul zu einem Szenario hinzu, um das Feld **[!UICONTROL Verbindung erstellen]** zu öffnen.
1. Geben Sie die folgenden Informationen an:

   * **[!UICONTROL Dienst-URL]**
   * **[!UICONTROL Benutzername]**
   * **[!UICONTROL API-Token]:** Dies ist das API-Token, das Sie im Abschnitt [API-Token in  [!DNL Jira]](#create-an-api-token-in-jira) dieses Artikels erstellen.

1. Klicken Sie auf [!UICONTROL Weiter] , um die Verbindung zu erstellen und zum Modul zurückzukehren.

### [!DNL Jira Server] mit [!DNL Workfront Fusion] verbinden

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

Um eine Verbindung zwischen [!DNL Workfront Fusion] und [!DNL Jira Server] zu autorisieren, benötigen Sie Ihren Kundenschlüssel, Ihren privaten Schlüssel und Ihre Dienst-URL. Möglicherweise müssen Sie sich für diese Informationen an Ihren [!DNL Jira] -Administrator wenden.

* [Öffentliche und private Schlüssel für Ihre [!DNL Jira] Verbindung generieren](#generate-public-and-private-keys-for-your-jira-connection)
* [Konfigurieren der Client-App als Verbraucher in  [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)
* [Erstellen einer Verbindung zum [!DNL Jira] Server- oder Jira-Rechenzentrum in [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### Öffentlichen und privaten Schlüssel für Ihre [!DNL Jira]-Verbindung generieren

Um einen privaten Schlüssel für Ihre [!DNL Workfront Fusion Jira]-Verbindung zu erhalten, müssen Sie öffentliche und private Schlüssel generieren.

1. Führen Sie in Ihrem Terminal die folgenden `openssl`-Befehle aus.

   * `openssl genrsa -out jira_privatekey.pem 1024`

     Dieser Befehl generiert einen privaten 1024-Bit-Schlüssel.

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

     Mit diesem Befehl wird ein X509-Zertifikat erstellt.

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

     Dieser Befehl extrahiert den privaten Schlüssel (PKCS8-Format) in den `jira_privatekey.pcks8`
-Datei.

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

     Mit diesem Befehl wird der öffentliche Schlüssel aus dem Zertifikat in die Datei `jira_publickey.pem` extrahiert.

     >[!NOTE]
     >
     >Wenn Sie Windows verwenden, müssen Sie den öffentlichen Schlüssel möglicherweise manuell in der Datei `jira_publickey.pem` speichern:
     >
     >1. Führen Sie in Ihrem Terminal den folgenden Befehl aus:
     >   
     >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
     >   
     >1. Kopieren Sie die Terminal-Ausgabe (einschließlich `-------BEGIN PUBLIC KEY--------` und `-------END PUBLIC KEY--------`)
     >   
     >1. Fügen Sie die Terminal-Ausgabe in eine Datei namens `jira_publickey.pem` ein.


1. Fahren Sie mit [Konfigurieren der Client-App als Verbraucher in [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira) fort.

#### Konfigurieren der Client-App als Verbraucher in [!DNL Jira]

1. Melden Sie sich bei Ihrer [!DNL Jira] -Instanz an.
1. Klicken Sie im linken Navigationsfenster auf **[!UICONTROL [!DNL Jira]Einstellungen]** ![](assets/jira-settings-icon.png) > **[!UICONTROL Anwendungen]**> **[!UICONTROL Anwendungslinks]**.
1. Geben Sie im Feld **[!UICONTROL die URL der Anwendung ein, die Sie verknüpfen möchten]** .

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. Klicken Sie auf **[!UICONTROL Neuen Link erstellen]**. Ignorieren Sie die Fehlermeldung &quot;Von der eingegebenen URL wurde keine Antwort empfangen&quot;.
1. Geben Sie im Fenster **[!UICONTROL Anwendungen verknüpfen]** Werte in die Felder **[!UICONTROL Consumer key]** und **[!UICONTROL Shared secret]** ein.

   Sie können die Werte für diese Felder auswählen.

1. Kopieren Sie die Werte der Felder **[!UICONTROL Consumer key]** und **[!UICONTROL Shared secret]** an einen sicheren Speicherort.

   Sie benötigen diese Werte später im Konfigurationsprozess.

1. Füllen Sie die URL-Felder wie folgt aus:

   | Feld | Beschreibung |
   |---|---|
   | [!UICONTROL Anfrage-Token-URL] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL Autorisierungs-URL] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL Zugriffstoken-URL] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. Aktivieren Sie das Kontrollkästchen **[!UICONTROL Eingehenden Link erstellen]** .
1. Klicken Sie auf **[!UICONTROL Weiter]**.
1. Füllen Sie im Fenster **[!UICONTROL Anwendungen verknüpfen]** die folgenden Felder aus:

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
      <td>Fügen Sie den öffentlichen Schlüssel aus Ihrer <code>[!DNL jira_publickey.pem]</code> -Datei ein.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Weiter]**.
1. Fahren Sie mit [Erstellen einer Verbindung zu [!DNL Jira Server] oder [!DNL Jira Data Center] in [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion) fort.

#### Erstellen einer Verbindung zu [!DNL Jira Server] oder [!DNL Jira Data Center] in [!DNL Workfront Fusion]

>[!NOTE]
>
>Verwenden Sie die [!DNL Jira Server]-App, um eine Verbindung zu [!DNL Jira Server] oder [!DNL Jira Data Center] herzustellen.
1. Klicken Sie in einem beliebigen [!DNL Jira Server]-Modul in [!DNL Workfront Fusion] auf **[!UICONTROL Hinzufügen]** neben dem Feld [!UICONTROL Verbindung] .
1. Füllen Sie im Bereich [!UICONTROL Verbindung erstellen] die folgenden Felder aus:

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
      <td>Fügen Sie den Consumer-Schlüssel ein, den Sie in <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">Client-App als Verbraucher konfigurieren in [!DNL Jira]</a> an einen sicheren Speicherort kopiert haben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>Fügen Sie den privaten Schlüssel aus der Datei <code>[!DNL jira_privatekey.pcks8]</code> ein, die Sie unter <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">Öffentliche und private Schlüssel für Ihre [!DNL Jira] Verbindung generieren</a> erstellt haben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>Geben Sie Ihre [!DNL Jira] Instanz-URL ein. </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

## [!DNL Jira Software] Module und ihre Felder

Wenn Sie [!DNL Jira Software] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Jira Software] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
     <li value="1">Klicken Sie auf <strong>[!UICONTROL Add]</strong></li> 
     <li value="2">Geben Sie einen Namen für den Webhook ein.</li> 
     <li value="3"> <p>Wählen Sie die Verbindung aus, die Sie für Ihren Webhook verwenden möchten. </p> <p>Anweisungen zum Verbinden Ihres [!DNL Jira Software]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL Jira Software] mit [!DNL Workfront Fusion]</a> .</p> </li> 
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
* [[!UICONTROL Erstellen eines Datensatzes]](#create-a-record)
* [[!UICONTROL Datensatz löschen]](#delete-a-record)
* [[!UICONTROL Herunterladen eines Anhangs]](#download-an-attachment)
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Jira Software]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL Jira Software] mit [!DNL Workfront Fusion]</a> .</p> </td> 
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

#### [!UICONTROL Erstellen eines Datensatzes]

Dieses Aktionsmodul erstellt einen neuen Datensatz in Jira.

Das Modul gibt alle mit dem Datensatz verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Jira Software]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL Jira Software] mit [!DNL Workfront Fusion]</a> .</p> </td> 
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

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Jira Software] -API durchführen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von anderen [!DNL Jira Software] -Modulen nicht ausgeführt werden kann.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Jira Software]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL Jira Software] mit [!DNL Workfront Fusion]</a> .</p> </td> 
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
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Jira Software]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL Jira Software] mit [!DNL Workfront Fusion]</a> .</p> </td> 
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

#### [!UICONTROL Herunterladen eines Anhangs]

Dieses Aktionsmodul lädt eine bestimmte Anlage herunter.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Jira Software]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL Jira Software] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Geben Sie die Kennung des Anhangs ein oder ordnen Sie sie zu.</td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Jira Software]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL Jira Software] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Typ von [!DNL Jira] Datensatz aus, den das Modul lesen soll.</p> 
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
   <td> <p>Geben Sie die eindeutige [!DNL Jira Software]-ID des Datensatzes ein oder ordnen Sie sie zu, den das Modul lesen soll.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Jira Software]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL Jira Software] mit [!DNL Workfront Fusion]</a> .</p> </td> 
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
   <td>Geben Sie die Kennung oder den Schlüssel des Datensatzes ein, den Sie aktualisieren möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

### Suchvorgänge

* [[!UICONTROL Listeneinträge]](#list-records)
* [[!UICONTROL Suche nach Datensätzen]](#search-for-records)

#### [!UICONTROL Listeneinträge]

Dieses Suchmodul ruft alle Elemente eines bestimmten Typs ab, die Ihrer Suchabfrage entsprechen

Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Jira Software]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL Jira Software] mit [!DNL Workfront Fusion]</a> .</p> </td> 
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

#### [!UICONTROL Suche nach Datensätzen]

Dieses Suchmodul sucht nach Datensätzen in einem Objekt in [!DNL Jira Software], die mit der von Ihnen angegebenen Suchabfrage übereinstimmen.

Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Jira Software]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">Verbinden von [!DNL Jira Software] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>Wählen Sie den Datensatztyp aus, nach dem das Modul suchen soll. Wenn Sie einen Datensatztyp auswählen, werden andere für diesen Datensatztyp spezifische Felder im Modul angezeigt.</p> 
    <ul> 
     <li>[!UICONTROL Probleme]</li> 
     <li> <p>[!UICONTROL Probleme durch JQL (Jira Query Language)] </p> <p>Weitere Informationen zu JQL finden Sie unter <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> auf der Atlassian-Hilfeseite. </p> </li> 
     <li>[!UICONTROL Projekt]</li> 
     <li>Projekt nach Ausgabe</li> 
     <li>[!UICONTROL Benutzer]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
