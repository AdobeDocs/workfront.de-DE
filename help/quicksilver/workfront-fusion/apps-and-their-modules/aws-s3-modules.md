---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: AWS S3-Module
description: Die [!DNL Adobe Workfront Fusion AWS] Mit S3-Modulen können Sie Vorgänge an Ihren S3-Buckets durchführen.
author: Becky
feature: Workfront Fusion
exl-id: 33623b5d-d9ff-4d41-b938-33378f50539e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1429'
ht-degree: 1%

---

# AWS S3-Module

Die [!DNL Adobe Workfront Fusion AWS] Mit S3-Modulen können Sie Vorgänge an Ihren S3-Buckets durchführen.

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

Verwendung [!UICONTROL AWS S3] -Module, müssen Sie über eine [!DNL Amazon Web Service] -Konto.

## Verbinden [!DNL AWS] nach [!DNL Workfront Fusion] {#connect-aws-to-workfront-fusion}

Verbindung herstellen [!DNL AWS S3] nach [!DNL Workfront Fusion] Sie müssen Ihre [!DNL AWS] Konto [!DNL Workfront Fusion]. Dazu müssen Sie zunächst einen API-Benutzer in [!DNL AWS] [!UICONTROL IAM].

1. Melden Sie sich bei Ihrer [!DNL AWS] [!UICONTROL IAM] -Konto.
1. Navigieren Sie zu **[!UICONTROL Identitäts- und Zugriffsverwaltung]** > **[!UICONTROL Zugriffsverwaltung]** > **[!UICONTROL Benutzer]**.

1. Klicken **[!UICONTROL Benutzer hinzufügen]**.
1. Geben Sie den Namen des neuen Benutzers ein und wählen Sie die **[!UICONTROL Programmierter Zugriff]** in der [!UICONTROL Zugriffstyp] Abschnitt.
1. Klicken **[!UICONTROL Vorhandene Richtlinien direkt anhängen]**, suchen Sie dann nach **[!UICONTROL AmazonS3FullAccess]** in der Suchleiste. Klicken Sie darauf, wenn es angezeigt wird, und klicken Sie dann auf **[!UICONTROL Nächste]**.

1. Fahren Sie durch die anderen Dialogfeldbildschirme und klicken Sie auf **[!UICONTROL Benutzer erstellen]**.
1. Kopieren Sie die bereitgestellte **[!UICONTROL Zugriffsschlüssel-ID]** und **[!UICONTROL Geheimer Zugriffsschlüssel]**.

1. Navigieren Sie zu [!DNL Workfront Fusion] und öffnen Sie die [!DNL AWS S3] -Modul **[!UICONTROL Verbindung erstellen]** angezeigt.
1. Geben Sie die [!UICONTROL Zugriffsschlüssel-ID] und [!UICONTROL Geheimer Zugriffsschlüssel] von Schritt 7 in die entsprechenden Felder und klicken Sie auf **[!UICONTROL Weiter]** um die Verbindung herzustellen.

Die Verbindung wurde hergestellt. Sie können mit der Einrichtung des Moduls fortfahren.

## [!DNL AWS S3] Module und ihre Felder

Bei der Konfiguration [!DNL AWS S3] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL AWS S3] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Aktionen

* [[!UICONTROL Bucket erstellen]](#create-bucket)
* [[!UICONTROL Datei abrufen]](#get-file)
* [[!UICONTROL Datei hochladen]](#upload-file)
* [[!UICONTROL API-Aufruf durchführen]](#make-an-api-call)

#### [!UICONTROL Bucket erstellen]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL AWS] Konto [!DNL Workfront Fusion], siehe <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL AWS] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Geben Sie den Namen des neuen Buckets ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Wählen Sie Ihren regionalen Endpunkt aus. Weitere Informationen finden Sie in der Diskussion unter <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regionale Endpunkte</a> in der AWS-Dokumentation.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei abrufen]

Lädt eine Datei aus einem Behälter herunter.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL AWS] Konto [!DNL Workfront Fusion], siehe <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL AWS] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Wählen Sie Ihren regionalen Endpunkt aus. Weitere Informationen finden Sie in der Diskussion unter <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regionale Endpunkte</a> im [!DNL AWS] Dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Wählen Sie den Behälter aus, aus dem Sie die Datei herunterladen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Path]</p> </td> 
   <td> <p>Geben Sie den Pfad zur Datei ein. Beispiel: <code>/photos/2019/February/image023.jpg</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei hochladen]

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL AWS] Konto [!DNL Workfront Fusion], siehe <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL AWS] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Wählen Sie Ihren regionalen Endpunkt aus. Weitere Informationen finden Sie in der Diskussion unter <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regionale Endpunkte</a> im [!DNL AWS] Dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Ordner] (optional) </p> </td> 
   <td> <p>Geben Sie den Zielordner an, in den Sie eine Datei hochladen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Header] (optional)</p> </td> 
   <td> <p> Fügen Sie Anforderungsheader ein. Die verfügbaren Kopfzeilen finden Sie im <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/API_PutObject.html">[!DNL AWS S3] Dokumentation - [!UICONTROL PUT]-Objekt</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL API-Aufruf durchführen]

Zur ausführlichen Erörterung der [!DNL Amazon S3] API, siehe [[!DNL Amazon S3] [!UICONTROL REST] API-Einführung](https://docs.aws.amazon.com/AmazonS3/latest/API/Welcome.html).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL AWS] Konto [!DNL Workfront Fusion], siehe <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL AWS] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Region] </td> 
   <td> <p>Wählen Sie Ihren regionalen Endpunkt aus. Weitere Informationen finden Sie in der Diskussion unter <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regionale Endpunkte</a> im [!DNL AWS] Dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL]</td> 
   <td> <p>URL Geben Sie eine Host-URL ein. Der Pfad muss relativ zu<code> https://s3.&lt;selected-region>.amazonaws.com/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Methode]</td> 
   <td> <p>Wählen Sie die [!UICONTROL HTTP]-Anforderungsmethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">[!UICONTROL HTTP]-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie eine Anfrage-Kopfzeile hinzu. Sie können die folgenden allgemeinen Anforderungsheader verwenden. Weitere Anfragekopfzeilen finden Sie unter <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html">[!DNL AWS S3] API-Dokumentation</a>.</p> <p>[!DNL Workfront Fusion] fügt automatisch Autorisierungskopfzeilen hinzu.</p> 
    <table style="table-layout:auto">
     <col> 
     <col> 
     <thead> 
      <tr> 
       <th>Header Name</th> 
       <th> <p> Beschreibung</p> </th> 
      </tr> 
     </thead> 
     <tbody> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Length]</p> </td> 
       <td> <p>Länge der Nachricht (ohne die Kopfzeilen) gemäß RFC 2616. Dieser Header ist für [!UICONTROL PUT]s und Vorgänge erforderlich, die XML laden, z. B. Protokollierung und ACLs.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-Type]</p> </td> 
       <td> <p>Der Inhaltstyp der Ressource, falls sich der Anfrageinhalt im Hauptteil befindet. Beispiel: <code>text/plain</code>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Content-MD5]</p> </td> 
       <td> <p>Der base64-kodierte 128-Bit-MD5-Digest der Nachricht (ohne Kopfzeilen) gemäß RFC 1864. Dieser Header kann als Integritätsprüfung für die Nachricht verwendet werden, um zu überprüfen, ob es sich bei den Daten um dieselben Daten handelt, die ursprünglich gesendet wurden. Obwohl dies optional ist, empfehlen wir die Verwendung des [!UICONTROL Content-MD5]-Mechanismus als End-to-End-Integritätsprüfung. Weitere Informationen zur [!UICONTROL REST]-Anforderungsauthentifizierung finden Sie unter <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/RESTAuthentication.html?r=1821">[!UICONTROL REST] Authentifizierung</a> im <i>[!DNL Amazon] Entwicklerhandbuch für einfachen Speicherdienst</i>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Datum]</p> </td> 
       <td> <p>Das aktuelle Datum und die aktuelle Uhrzeit entsprechend dem Anfragenden. Beispiel: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. Wenn Sie die <code>Authorization </code>-Kopfzeile angeben, müssen Sie entweder <code>x-amz-date</code> oder <code>Date </code>-Kopfzeile.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Expect]</p> </td> 
       <td> <p>Wenn Ihre Anwendung [!UICONTROL 100-continue] verwendet, sendet sie den Anfragetext erst, wenn sie eine Bestätigung erhält. Wenn die Nachricht aufgrund der Header abgelehnt wird, wird der Hauptteil der Nachricht nicht gesendet. Diese Kopfzeile kann nur verwendet werden, wenn Sie einen Hauptteil senden.</p> <p>Gültige Werte: [!UICONTROL 100-continue]</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL Host]</p> </td> 
       <td> <p>Bei Pfadanforderungen lautet der Wert <code>s3.amazonaws.com</code>. Bei Anforderungen im virtuellen Stil lautet der Wert <code>BucketName.s3.amazonaws.com</code>. Weitere Informationen finden Sie unter <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/VirtualHosting.html">Virtuelles Hosting</a> im <i>[!DNL Amazon] Entwicklerhandbuch für einfachen Speicherdienst</i>.</p> <p>Dieser Header ist für HTTP 1.1 erforderlich (die meisten Toolkits fügen diesen Header automatisch hinzu). optional für HTTP/1.0-Anforderungen.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-content-sha256]</p> </td> 
       <td> <p>Wenn Sie die Signaturversion 4 zum Authentifizieren der Anfrage verwenden, stellt dieser Header einen Hash der Anfrage-Payload bereit. Setzen Sie beim Hochladen eines Objekts in Teilen den Wert auf <code>STREAMING-AWS4-HMAC-SHA256-PAYLOAD</code> , um anzugeben, dass die Signatur nur Kopfzeilen abdeckt und dass keine Payload vorhanden ist. Weitere Informationen finden Sie unter <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/sigv4-streaming.html">Signaturberechnungen für die Autorisierungskopfzeile: Übertragen der Payload in mehrere Blöcke (Chunked Upload) ([!DNL AWS] Signature Version 4)</a>.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-date]</p> </td> 
       <td> <p>Das aktuelle Datum und die aktuelle Uhrzeit entsprechend dem Anfragenden. Beispiel: <code>Wed, 01 Mar 2006 12:00:00 GMT</code>. Wenn Sie die <code>Authorization </code>-Kopfzeile angeben, müssen Sie entweder <code>x-amz-date</code> oder <code>Date </code>-Kopfzeile. Wenn Sie beides angeben, wird der Wert für <code>x-amz-date</code> -Kopfzeile hat Vorrang.</p> </td> 
      </tr> 
      <tr> 
       <td role="rowheader"> <p>[!UICONTROL x-amz-security-token]</p> </td> 
       <td> <p>Diese Kopfzeile kann in den folgenden Szenarien verwendet werden:</p> 
        <ul> 
         <li>Stellen Sie Sicherheitstoken für bereit. [!DNL Amazon DevPay] Vorgänge. Jede Anfrage, die [!DNL Amazon DevPay] erfordert zwei <code>x-amz-security-token</code> Kopfzeilen: einen für das Produkt-Token und einen für das Benutzer-Token. Wann [!DNL Amazon S3] eine authentifizierte Anfrage erhält, vergleicht sie die berechnete Signatur mit der bereitgestellten Signatur. Fehlerhaft formatierte Header mit mehreren Werten, die zur Berechnung einer Signatur verwendet werden, können Authentifizierungsprobleme verursachen.</li> 
         <li>Stellen Sie bei Verwendung temporärer Sicherheitsberechtigungen ein Sicherheits-Token bereit. Bei Anfragen mit temporären Sicherheitsberechtigungen, die Sie von IAM erhalten haben, müssen Sie mithilfe dieses Headers ein Sicherheits-Token bereitstellen. Weitere Informationen zu temporären Sicherheitsberechtigungen finden Sie unter Anforderungen erstellen .</li> 
        </ul> <p>Diese Kopfzeile ist für Anfragen erforderlich, die [!DNL Amazon DevPay] und Anfragen, die mit temporären Sicherheitsberechtigungen signiert werden.</p> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p>Fügen Sie die gewünschten Abfragezeichenfolgen wie Parameter oder Formularfelder hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body]</td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Notiz:   <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Suchvorgänge

* [[!UICONTROL Listendateien]](#list-files)
* [[!UICONTROL Listenordner]](#list-folders)

#### [!UICONTROL Listendateien]

Gibt eine Liste von Dateien von einem angegebenen Speicherort zurück.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL AWS] Konto [!DNL Workfront Fusion], siehe <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL AWS] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Wählen Sie Ihren regionalen Endpunkt aus. Weitere Informationen finden Sie in der Diskussion unter <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regionale Endpunkte</a> im [!DNL AWS] Dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Wählen Sie die [!DNL Amazon S3] -Bucket, den Sie nach Dateien suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Präfix] (optional)</p> </td> 
   <td> <p> Pfad zu einem Ordner, in dem Dateien nachgeschlagen werden sollen, z. B. <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Listenordner]

Gibt eine Liste von Ordnern von einem angegebenen Speicherort zurück.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL AWS] Konto [!DNL Workfront Fusion], siehe <a href="#connect-aws-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL AWS] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Region] </td> 
   <td> <p>Wählen Sie Ihren regionalen Endpunkt aus. Weitere Informationen finden Sie in der Diskussion unter <a href="https://docs.aws.amazon.com/general/latest/gr/rande.html">regionale Endpunkte</a> in der AWS-Dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Bucket] </td> 
   <td> <p>Wählen Sie die [!DNL Amazon S3] -Behälter, den Sie nach Ordnern suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Präfix] (optional)</p> </td> 
   <td> <p> Pfad zu einem Ordner, in dem Ordner nachgeschlagen werden sollen, z. B. <code>workfrontfusion/work.</code></p> </td> 
  </tr> 
 </tbody> 
</table>
