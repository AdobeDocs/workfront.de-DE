---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Salesforce-Module
description: In einem Adobe Workfront Fusion-Szenario können Sie Workflows automatisieren, die Salesforce verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 3c8adcd9-fb5f-400d-9edd-6d9fc30cc728
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2768'
ht-degree: 0%

---

# [!DNL Salesforce]-Module

In einem Adobe Workfront Fusion-Szenario können Sie Workflows automatisieren, die [!DNL Salesforce], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.

Informationen zum Erstellen eines Szenarios finden Sie unter [Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!NOTE]
>
>* Nicht alle Ausgaben von [!DNL Salesforce] haben API-Zugriff. Weitere Informationen finden Sie in den Informationen zu [!DNL Salesforce] Editionen mit API-Zugriff auf die [!DNL Salesforce] Community-Site.
>* Informationen zu spezifischen Fehlern, die von der [!DNL Salesforce] API, siehe [!DNL Salesforce] API-Dokumente. Sie können auch den Status der [!DNL Salesforce] API für alle möglichen Dienstausfälle.
>

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

Verwendung [!DNL Salesforce] -Module, müssen Sie über eine [!DNL Salesforce] -Konto.

## Über die Suche nach [!DNL Salesforce] Objekte

Bei der Suche nach Objekten können Sie entweder einzelne Suchbegriffe eingeben oder mithilfe von Platzhaltern und Operatoren eine komplexere Abfrage erstellen:

* Verwenden Sie die Platzhalterkarte (\*) als Ersatz für null oder mehr Zeichen. Wenn Sie beispielsweise nach Ca\* suchen, werden Elemente gefunden, die mit Ca beginnen
* Verwenden Sie eine Fragezeichen-Platzhalterkarte (?) als Ersatz für ein einzelnes Zeichen. Beispielsweise findet eine Suche nach Jo?n Elemente mit dem Begriff John oder Joan, aber nicht Jon
* Verwenden Sie den Anführungszeichen-Operator (&quot;&quot;&quot;), um eine exakte Wortübereinstimmung zu finden. Beispiel: &quot;Montag&quot;

Weitere Informationen zu Suchmöglichkeiten finden Sie unter [!DNL Salesforce] Entwicklerdokumentation zu SOQL und SOSL.

## [!DNL Salesforce] Module und ihre Felder

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Trigger

* [[!UICONTROL Auf Aufzeichnungen achten]](#watch-for-records)
* [[!UICONTROL Ausgehende Nachrichten ansehen]](#watch-outbound-messages)
* [[!UICONTROL Anzeigen eines Felds]](#watch-a-field)

#### [!UICONTROL Auf Aufzeichnungen achten]

Dieses Trigger-Modul führt ein Szenario aus, wenn ein Datensatz in einem Objekt erstellt oder aktualisiert wird. Das Modul gibt alle mit dem Datensatz oder den Datensätzen verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Salesforce] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Typ] </td> 
   <td> <p>Wählen Sie den Typ [!DNL Salesforce] notieren, dass das Modul überwacht werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datensatzfelder]</td> 
   <td>Wählen Sie die Felder aus, die das Modul überwachen soll. Die verfügbaren Felder hängen vom Datensatztyp ab.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl der Datensätze]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch]</td> 
   <td> <p>Bestimmen Sie, ob im Szenario nur neue Datensätze des ausgewählten Typs oder neue Datensätze des ausgewählten Typs sowie alle anderen Änderungen an Datensätzen dieses Typs berücksichtigt werden sollen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ausgehende Nachrichten ansehen]

Dieses Trigger-Modul führt ein Szenario aus, wenn jemand eine Nachricht sendet. Das Modul gibt alle mit dem Datensatz oder den Datensätzen verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Dieses Modul erfordert einige zusätzliche Einstellungen:

1. Navigieren Sie zu [!DNL Salesforce] Setup-Seite.

   Um auf die Einrichtungsseite zuzugreifen, suchen Sie die Schaltfläche mit der Bezeichnung &quot;[!UICONTROL Einrichtung]&quot; in der oberen rechten Ecke der [!DNL Salesforce] -Konto. Aus dem [!DNL Salesforce] Setup-Seite, suchen Sie nach &quot;[!UICONTROL Schnellsuche/Suche]&quot; Balken auf der linken Seite. Suchen Sie nach &quot;[!UICONTROL Workflow-Regeln].&quot;

1. Klicken **[!UICONTROL Workflow-Regeln]**.
1. Im Bereich [!UICONTROL Workflow-Regeln] Seite, die angezeigt wird, klicken Sie auf **[!UICONTROL Neue Regel]** und wählen Sie den Objekttyp aus, auf den die Regel angewendet werden soll (z. B.[!UICONTROL Chancen]&quot;, wenn Sie Aktualisierungen von Opportunity-Datensätzen überwachen).
1. Klicken **[!UICONTROL Nächste]**.
1. Legen Sie einen Regelnamen, Bewertungskriterien und Regelkriterien fest und klicken Sie dann auf **[!UICONTROL Speichern]** und **[!UICONTROL Nächste]**.

1. Klicken **[!UICONTROL Fertig]**.
1. Klicken Sie in der neu erstellten Workflow-Regel auf **[!UICONTROL Bearbeiten]**.
1. Aus dem **[!UICONTROL Workflow-Aktion hinzufügen]** Dropdown-Liste auswählen **[!UICONTROL Neue ausgehende Nachricht]**.

1. Geben Sie Namen, Beschreibung, Endpunkt-URL und Felder an, die Sie in die neue ausgehende Nachricht aufnehmen möchten, und klicken Sie dann auf **[!UICONTROL Speichern]**.

   Die **[!UICONTROL Endpunkt-URL]** enthält die URL, die im Feld [!DNL Salesforce] [!UICONTROL Ausgehende Nachricht] in [!DNL Workfront Fusion].

1. Konfigurieren Sie ein Szenario, das mit dem [!UICONTROL Ausgehende Nachricht] -Ereignis.

1. Klicken Sie auf **&lt;/>** rechts unten und kopieren Sie die angegebene URL.
1. Kehren Sie zu **[!UICONTROL Workflow-Regeln]** Seite, suchen Sie die neu erstellte Regel und klicken Sie auf **[!UICONTROL Aktivieren]**.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td> <p>Wählen Sie den Webhook aus, den Sie zum Anzeigen ausgehender Nachrichten verwenden möchten. Um einen Webhook hinzuzufügen, klicken Sie auf <strong>[!UICONTROL Hinzufügen]</strong> und geben Sie den Namen und die Verbindung des Webhooks ein.</p> <p>Anweisungen zum Verbinden der [!DNL Salesforce] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbindung zu [!UICONTROL Adobe Workfront Fusion] erstellen - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Wählen Sie den Typ [!DNL Salesforce] notieren, dass das Modul auf ausgehende Nachrichten überwachen soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Felder]</td> 
   <td> <p>Wählen Sie die Felder aus, die das Modul auf ausgehende Nachrichten überwachen soll. Die verfügbaren Felder hängen vom Datensatztyp ab.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### *[!UICONTROL Anzeigen eines Felds]*

Dieses Trigger-Modul startet ein Szenario, wenn ein Feld in aktualisiert wird. [!DNL Salesforce].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Salesforce] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Wählen Sie den Datensatztyp aus, der das Feld enthält, das das Modul überwachen soll. Sie müssen einen Datensatztyp auswählen, für den [!UICONTROL Feldverlauf] aktiviert ist. [!DNL Salesforce] einrichten. Weitere Informationen finden Sie unter <a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">Feldverlauf-Tracking</a> im [!DNL Salesforce] Dokumentation. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Field]</td> 
   <td> <p>Wählen Sie die Felder aus, die das Modul auf Änderungen überwachen soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Feldern ein oder ordnen Sie sie zu, die das Modul während der Ausführung jedes Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL Datensatz erstellen]](#create-a-record)
* [[!UICONTROL Datensatz lesen]](#read-a-record)
* [[!UICONTROL Datensatz löschen]](#delete-a-record)
* [[!UICONTROL Benutzerspezifischer API-Aufruf]](#custom-api-call)
* [[!UICONTROL Anhang/Dokument hochladen]](#upload-attachmentdocument)
* [[!UICONTROL Anhang/Dokument herunterladen]](#download-attachmentdocument)

#### [!UICONTROL Datensatz erstellen]

Dieses Aktionsmodul erstellt einen neuen Datensatz in einem Objekt.

Mit dem -Modul können Sie auswählen, welche der Objektfelder im -Modul verfügbar sind. Dadurch wird die Anzahl der Felder reduziert, die beim Einrichten des Moduls durchsucht werden müssen.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Salesforce] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Record Type] </p> </td> 
   <td> <p>Wählen Sie den Typ [!DNL Salesforce] notieren, dass das Modul erstellt werden soll. Felder werden je nach dem im Feld [!UICONTROL Record Type] ausgewählten Datensatztyp verfügbar. Diese Felder basieren auf dem [!DNL Salesforce] API.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Felder zur Zuordnung auswählen]</td> 
   <td> <p>Wählen Sie die Felder aus, die das Modul beim Erstellen des neuen Datensatzes konfigurieren soll. Die erforderlichen Felder befinden sich oben in der Liste. </p> <p>Die ausgewählten Felder werden unter diesem Feld geöffnet. Sie können jetzt Werte in diese Felder eingeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datensatz lesen]

Dieses Aktionsmodul liest Daten aus einem einzelnen Objekt in [!DNL Salesforce].

Sie geben die Kennung des Datensatzes an.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden der [!DNL Salesforce] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Record Type]</td>
    <td>Wählen Sie den Typ [!DNL Salesforce] notieren, dass das Modul [action].read lauten soll.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Datensatzfelder]</td>
    <td>Wählen Sie die Felder aus, die das Modul lesen soll. Sie müssen mindestens ein Feld auswählen.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL ID]</td>
    <td> <p>Eindeutige Eingabe oder Zuordnung [!DNL Salesforce] Kennung des Datensatzes, den das Modul lesen soll.</p> <p>Um die ID abzurufen, öffnen Sie die [!DNL Salesforce] -Objekt in Ihrem Browser ein und kopieren Sie den Text am Ende der URL nach dem letzten Schrägstrich (/). Beispiel: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datensatz löschen]

Dieses Aktionsmodul löscht einen vorhandenen Datensatz in einem Objekt.

Sie geben die Kennung des Datensatzes an.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Salesforce] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Wählen Sie den Typ [!DNL Salesforce] notieren, dass das Modul gelöscht werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Eindeutige Eingabe oder Zuordnung [!DNL Salesforce] Kennung des Datensatzes, den das Modul löschen soll.</p> <p>Um die ID abzurufen, öffnen Sie die [!DNL Salesforce] -Objekt in Ihrem Browser ein und kopieren Sie den Text am Ende der URL nach dem letzten Schrägstrich (/). Beispiel: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Benutzerspezifischer API-Aufruf]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Salesforce] API. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von der anderen nicht durchgeführt werden kann [!DNL Salesforce] Module.

Das Modul gibt Folgendes zurück:

* **[!UICONTROL Status-Code]** (Zahl): Dies zeigt an, ob Ihre HTTP-Anforderung erfolgreich oder fehlgeschlagen ist. Dies sind Standardcodes, die Sie im Internet nachschlagen können.
* **[!UICONTROL Kopfzeilen]** (Objekt): Ein detaillierterer Kontext für den Antwort-/Status-Code, der sich nicht auf den Ausgabetext bezieht. Nicht alle Header, die in einem Antwortheader angezeigt werden, sind Antwortheader, sodass einige möglicherweise nicht nützlich für Sie sind.

  Die Antwortheader hängen von der HTTP-Anforderung ab, die Sie beim Konfigurieren des Moduls ausgewählt haben.

* **[!UICONTROL body]** (Objekt): Je nach der HTTP-Anforderung, die Sie beim Konfigurieren des Moduls ausgewählt haben, erhalten Sie möglicherweise einige Daten zurück. Diese Daten, z. B. die Daten aus einem [!UICONTROL GET] -Anfrage ist in diesem Objekt enthalten.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Salesforce] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Geben Sie einen Pfad relativ zu ein<code> &lt;Instance URL&gt;/services/data/v46.0/</code>.</p> <p>Die Liste der verfügbaren Endpunkte finden Sie im Abschnitt <a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Salesforce REST API-Entwicklerhandbuch</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Methode]</p> </td> 
   td&gt; <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anforderung in Form eines standardmäßigen JSON-Objekts hinzu. Beispiel: <code>{"Content-type":"application/json"}</code>. Workfront Fusion fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu. Beispiel: <code>{"name":"something-urgent"}</code></p> </td> 
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

>[!INFO]
>
>**Beispiel:** Der folgende API-Aufruf gibt die Liste aller Benutzer in Ihrer [!DNL Salesforce] Konto:
>
>* **URL**: `query`
>
>* **Methode**: [!UICONTROL GET]
>
>* **Abfragezeichenfolge**:
>
>* **Schlüssel**: `q`
>
>* **Wert**: `SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`
>
>Treffer der Suche finden Sie in der Ausgabe des Moduls unter **[!UICONTROL Bundle] > [!UICONTROL body] > [!UICONTROL records]**.
>
>In unserem Beispiel wurden 6 Benutzer zurückgegeben:
>
>![](assets/matches-of-the-search-350x573.png)


#### [!UICONTROL Anhang/Dokument hochladen]

Dieses Aktionsmodul lädt eine Datei hoch und hängt sie an einen von Ihnen angegebenen Datensatz an oder lädt ein Dokument hoch.

Das Modul gibt die ID des Anhangs oder Dokuments sowie alle zugehörigen Felder zusammen mit benutzerdefinierten Feldern und Werten zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Salesforce] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Typ des Uploads]</td> 
   <td>Wählen Sie aus, ob das Modul eine Anlage oder ein Dokument hochladen soll.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Geben Sie die ID des Objekts ein, in das Sie eine Anlage hochladen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner]</td> 
   <td>Wählen Sie den Ordner aus, der die Datei enthält, die das Modul hochladen soll. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Quelldatei]</td> 
   <td>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Anhang/Dokument herunterladen]

Dieses Aktionsmodul lädt ein Dokument oder eine Anlage aus einem Datensatz herunter.

Sie geben die Kennung des Datensatzes und den gewünschten Download-Typ an.

Das Modul gibt die ID des Anhangs oder Dokuments sowie alle zugehörigen Felder zusammen mit benutzerdefinierten Feldern und Werten zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden der [!DNL Salesforce] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Download-Typ]</td>
    <td> <p>Geben Sie den Dateityp an, den Sie aus Salesforce herunterladen möchten.</p> 
     <ul> 
      <li>[!UICONTROL Anhang]</li> 
      <li>[!UICONTROL Document]</li> 
      <li>[!UICONTROL ContentDocument] (Dies ist ein Dokument, das in eine Bibliothek in [!DNL Saleforce CRM Content] oder [!DNL Salesforce Files].</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[!UICONTROL ID] / </p> <p>[!UICONTROL Attachment ID] / </p> <p>[!UICONTROL ContentDocument ID]</p> </td>
    <td> <p>Eindeutige Eingabe oder Zuordnung [!DNL Salesforce] Kennung des Datensatzes, den das Modul herunterladen soll.</p> <p>Um die ID abzurufen, öffnen Sie die [!DNL Salesforce] -Objekt in Ihrem Browser ein und kopieren Sie den Text am Ende der URL nach dem letzten Schrägstrich (/). Beispiel: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Datensatz aktualisieren]

Dieses Aktionsmodul bearbeitet einen Datensatz in einem Objekt.

Mit dem -Modul können Sie auswählen, welche der Objektfelder im -Modul verfügbar sind. Dadurch wird die Anzahl der Felder reduziert, die beim Einrichten des Moduls durchsucht werden müssen.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Salesforce] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Geben Sie die Kennung des Datensatzes ein, den Sie aktualisieren möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Record Type] </p> </td> 
   <td> <p>Wählen Sie den Typ [!DNL Salesforce] notieren, dass das Modul aktualisiert werden soll. Felder werden je nach dem im Feld Datensatztyp ausgewählten Datensatztyp verfügbar. Diese Felder basieren auf dem [!DNL Salesforce] API.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Felder zur Zuordnung auswählen]</td> 
   <td> <p>Wählen Sie die Felder aus, die das Modul beim Erstellen des neuen Datensatzes konfigurieren soll. Die erforderlichen Felder befinden sich oben in der Liste. </p> <p>Die ausgewählten Felder werden unter diesem Feld geöffnet. Sie können jetzt Werte in diese Felder eingeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Suchvorgänge

#### [!UICONTROL Suche mit Abfrage]

Dieses Suchmodul sucht nach Datensätzen in einem Objekt in [!DNL Salesforce] die mit der angegebenen Suchabfrage übereinstimmen. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Salesforce] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Suchtyp]</td> 
   <td> <p>Wählen Sie den Suchtyp aus, den das Modul ausführen soll:</p> 
    <ul> 
     <li> <p>[!UICONTROL Simple]</p> </li> 
     <li> <p>[!UICONTROL Verwenden von SOSL (Salesforce Object Search Language)]</p> </li> 
     <li> <p>[!UICONTROL Using SOQL (Salesforce Object Query Language)]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Typ] </p> </td> 
   <td> <p>Wenn Sie den Typ Einfache Suche ausgewählt haben, wählen Sie den Typ [!DNL Salesforce] -Datensatz, nach dem das -Modul suchen soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abfrage] / [!UICONTROL SOSL-Abfrage] / [!UICONTROL SOQL-Abfrage]</td> 
   <td> <p>Geben Sie die Abfrage ein, nach der Sie suchen möchten.</p> <p>Weitere Informationen zu SOSL finden Sie unter <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">Salesforce Object Search Language (SOSL)</a> im [!DNL Salesforce] Dokumentation.</p> <p>Weitere Informationen zu SOQL finden Sie unter <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">Salesforce Object Query Language (SOQL)</a> im [!DNL Salesforce] Dokumentation.</p> <p>Hinweis: Beachten Sie, dass der Wert des Parameters <code>RETURNING </code>beeinflusst die Ausgabe des Moduls. Wenn Sie <code>LIMIT</code>, [!DNL Fusion] ignoriert die Einstellungen im Feld [!UICONTROL Maximale Anzahl an Datensätzen] . Wenn Sie keine Begrenzung festlegen, fügt Fusion den Wert [!UICONTROL LIMIT = Maximale Anzahl an Datensätzen] ein.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl der Datensätze]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suche]

Dieses Aktionsmodul ruft alle Datensätze ab, die bestimmte Kriterien erfüllen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td>Anweisungen zum Verbinden der [!DNL Salesforce] Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu[!DNL  Adobe Workfront Fusion] - Grundlegende Anweisungen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Typ]</td> 
   <td> <p>Wählen Sie den Objekttyp aus, nach dem Sie suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suchkriterien]</td> 
   <td>Wählen Sie das Feld aus, nach dem Sie suchen möchten, den Operator, den Sie in Ihrer Abfrage verwenden möchten, und den Wert, nach dem Sie im Feld suchen. Sie können Abfragen mit UND oder ODER verbinden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td>Wählen Sie die Felder aus, die Sie in die Ausgabe des Moduls aufnehmen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Result set]</td> 
   <td>Wählen Sie aus, ob das Modul alle übereinstimmenden Datensätze zurückgeben soll oder nur den ersten übereinstimmenden Datensatz.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximal]</td> 
   <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen des Szenarios abrufen soll.</td> 
  </tr> 
 </tbody> 
</table>
