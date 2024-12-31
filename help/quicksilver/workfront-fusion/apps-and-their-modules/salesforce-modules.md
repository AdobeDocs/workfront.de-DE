---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: Salesforce-Module
description: In einem Adobe Workfront Fusion-Szenario können Sie Workflows automatisieren, die Salesforce verwenden, und sie mit mehreren Anwendungen und Services von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 3c8adcd9-fb5f-400d-9edd-6d9fc30cc728
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '2758'
ht-degree: 0%

---

# [!DNL Salesforce]

In einem Adobe Workfront Fusion-Szenario können Sie Workflows automatisieren, die [!DNL Salesforce] verwenden, und sie mit mehreren Anwendungen und Services von Drittanbietern verbinden.

Eine Videoeinführung zum Salesforce-Connector finden Sie unter:

* [Salesforce](https://video.tv.adobe.com/v/3427027/){target=_blank}

Anweisungen zum Erstellen eines Szenarios finden Sie unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!NOTE]
>
>* Nicht alle Editionen von [!DNL Salesforce] verfügen über API-Zugriff. Weitere Informationen finden Sie in den Informationen zu [!DNL Salesforce] Editionen mit API-Zugriff auf der [!DNL Salesforce] Community-Site.
>* Informationen zu bestimmten Fehlern, die von der [!DNL Salesforce]-API zurückgegeben werden, finden Sie in den Dokumenten zur [!DNL Salesforce]-API. Sie können auch den Status der [!DNL Salesforce]-API auf mögliche Service-Ausfälle überprüfen.
>

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

Um [!DNL Salesforce]-Module verwenden zu können, müssen Sie über ein [!DNL Salesforce]-Konto verfügen.

## Salesforce-API-Informationen

Der Salesforce-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td> {connection.instanceUrl}</td>
  </tr> 
  <tr> 
   <td role="rowheader">API-Version</td> 
   <td> v46.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.15.14</td> 
  </tr>
 </tbody> 
 </table>

## Über die Suche nach [!DNL Salesforce] Objekten

Bei der Suche nach Objekten können Sie entweder einzelne Suchbegriffe eingeben oder eine komplexere Abfrage mit Platzhaltern und Operatoren erstellen:

* Verwenden Sie den Sternchen-Platzhalter (\*) als Ersatz für null oder mehr Zeichen. Bei einer Suche nach Ca\* werden beispielsweise Elemente gefunden, die mit Ca beginnen
* Mit einem Fragezeichen (?) als Ersatz für ein einzelnes Zeichen. Bei einer Suche nach Jon?n werden beispielsweise Elemente mit dem Begriff John oder Joan, aber nicht Jon gefunden
* Verwenden Sie den Anführungszeichen-Operator (“ „), um eine exakte Übereinstimmung der Phrasen zu finden. Beispiel: „Montagstreffen“

Weitere Informationen zu Suchmöglichkeiten finden Sie in der [!DNL Salesforce] Entwicklerdokumentation zu SOQL und SOSL.

## [!DNL Salesforce] Module und ihre Felder

* [Trigger ](#triggers)
* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Trigger

* [[!UICONTROL Auf Datensätze achten]](#watch-for-records)
* [[!UICONTROL Ausgehende Nachrichten ansehen]](#watch-outbound-messages)
* [[!UICONTROL Feld ansehen]](#watch-a-field)

#### [!UICONTROL Auf Datensätze achten]

Dieses Trigger-Modul führt ein Szenario aus, wenn ein Datensatz in einem Objekt erstellt oder aktualisiert wird. Das Modul gibt alle Standardfelder zurück, die mit dem Datensatz oder den Datensätzen verknüpft sind, sowie alle benutzerdefinierten Felder und Werte, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Typ] </td> 
   <td> <p>Wählen Sie den Typ [!DNL Salesforce] Datensatzes aus, den das Modul überwachen soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datensatzfelder]</td> 
   <td>Wählen Sie die Felder aus, die das Modul überwachen soll. Die verfügbaren Felder hängen vom Typ des Datensatzes ab.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl von Datensätzen]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Uhr]</td> 
   <td> <p>Legen Sie fest, ob das Szenario nur neue Datensätze des ausgewählten Typs oder neue Datensätze des ausgewählten Typs und alle anderen Änderungen an Datensätzen dieses Typs sehen soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ausgehende Nachrichten ansehen]

Dieses Trigger-Modul führt ein Szenario aus, wenn jemand eine Nachricht sendet. Das Modul gibt alle Standardfelder zurück, die mit dem Datensatz oder den Datensätzen verknüpft sind, sowie alle benutzerdefinierten Felder und Werte, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Dieses Modul erfordert einige zusätzliche Einstellungen:

1. Navigieren Sie zur Seite [!DNL Salesforce].

   Um auf die Setup-Seite zuzugreifen, suchen Sie die Schaltfläche mit der Bezeichnung [!UICONTROL Setup] in der oberen rechten Ecke des [!DNL Salesforce] Kontos. Suchen Sie auf der Seite &quot;[!DNL Salesforce]&quot; die Leiste [!UICONTROL Schnellsuche/Suche] auf der linken Seite. Suchen Sie nach [!UICONTROL Workflow-Regeln].

1. Klicken Sie **[!UICONTROL Workflow-Regeln]**.
1. Klicken Sie auf der [!UICONTROL Workflow-]) auf **[!UICONTROL Neue Regel]** und wählen Sie den Objekttyp aus, auf den die Regel angewendet werden soll (z. B. [!UICONTROL Opportunity], wenn Sie Aktualisierungen von Opportunity-Datensätzen überwachen).
1. Klicken Sie **[!UICONTROL Weiter]**.
1. Legen Sie einen Regelnamen, Bewertungskriterien und Regelkriterien fest und klicken Sie dann auf **[!UICONTROL Speichern]** und **[!UICONTROL Weiter]**.

1. Klicken Sie **[!UICONTROL Fertig]**.
1. Klicken Sie in der neu erstellten Workflow-Regel auf **[!UICONTROL Bearbeiten]**.
1. Wählen Sie in **[!UICONTROL Dropdown-Liste]** Workflow-Aktion hinzufügen“ **[!UICONTROL Neue ausgehende Nachricht]** aus.

1. Geben Sie Namen, Beschreibung, Endpunkt-URL und Felder an, die in die neue ausgehende Nachricht aufgenommen werden sollen. Klicken Sie dann auf **[!UICONTROL Speichern]**.

   Das **[!UICONTROL Endpunkt-URL]**-Feld enthält die URL, die in der [!DNL Workfront Fusion] [!DNL Salesforce]Ausgehende [!UICONTROL Nachricht] angegeben ist.

1. Konfigurieren Sie ein Szenario, das mit dem Ereignis [!UICONTROL Ausgehende Nachricht] beginnt.

1. Klicken Sie auf das Symbol **&lt;/>** unten rechts und kopieren Sie die bereitgestellte URL.
1. Kehren Sie zur Seite **[!UICONTROL Workflow-Regeln]** zurück, suchen Sie die neu erstellte Regel und klicken Sie dann auf **[!UICONTROL Aktivieren]**.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td> <p>Wählen Sie den Webhook aus, mit dem Sie ausgehende Nachrichten beobachten möchten. Um einen Webhook hinzuzufügen, klicken Sie auf <strong>[!UICONTROL Hinzufügen]</strong> und geben Sie den Namen und die Verbindung des Webhooks ein.</p> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!UICONTROL Adobe Workfront Fusion] - Grundanweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datensatztyp] </td> 
   <td> <p>Wählen Sie den Typ [!DNL Salesforce] Datensatzes aus, den das Modul auf ausgehende Nachrichten überwachen soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Felder]</td> 
   <td> <p>Wählen Sie die Felder aus, die das Modul auf ausgehende Nachrichten überwachen soll. Die verfügbaren Felder hängen vom Typ des Datensatzes ab.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### *[!UICONTROL Feld ansehen]*

Dieses Feldmodul startet ein Trigger, wenn ein Feld in [!DNL Salesforce] aktualisiert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datensatztyp] </td> 
   <td> <p>Wählen Sie den Typ des Datensatzes aus, der das Feld enthält, das vom Modul überwacht werden soll. Sie müssen einen Datensatztyp auswählen, für den [!UICONTROL Field History] in [!DNL Salesforce] Setup aktiviert ist. Weitere Informationen finden Sie unter <a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">Feldverlaufsverfolgung</a> in der [!DNL Salesforce]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Feld]</td> 
   <td> <p>Wählen Sie die Felder aus, die das Modul auf Änderungen überwachen soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Feldern ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL Datensatz erstellen]](#create-a-record)
* [[!UICONTROL Datensatz lesen]](#read-a-record)
* [[!UICONTROL Löschen eines Datensatzes]](#delete-a-record)
* [[!UICONTROL Benutzerdefinierter API-Aufruf]](#custom-api-call)
* [[!UICONTROL Anlage/Dokument hochladen]](#upload-attachmentdocument)
* [[!UICONTROL Anlage/Dokument herunterladen]](#download-attachmentdocument)

#### [!UICONTROL Datensatz erstellen]

Dieses Aktionsmodul erstellt einen neuen Datensatz in einem -Objekt.

Mit dem Modul können Sie auswählen, welche der Objektfelder im Modul verfügbar sind. Dadurch wird die Anzahl der Felder reduziert, die beim Einrichten des Moduls durchgescrollt werden müssen.

Das Modul gibt die ID des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Datensatztyp] </p> </td> 
   <td> <p>Wählen Sie den Typ [!DNL Salesforce] Datensatzes aus, den das Modul erstellen soll. Die Felder werden je nach dem im Feld [!UICONTROL Record Type] ausgewählten Datensatztyp verfügbar. Diese Felder basieren auf der [!DNL Salesforce]-API.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Felder zum Zuordnen auswählen]</td> 
   <td> <p>Wählen Sie die Felder aus, die das Modul beim Erstellen des neuen Datensatzes konfigurieren soll. Erforderliche Felder befinden sich oben in der Liste. </p> <p>Die Felder, die Sie auswählen, werden unter diesem Feld geöffnet. Sie können jetzt Werte in diese Felder eingeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datensatz lesen]

Dieses Aktionsmodul liest Daten aus einem einzelnen -Objekt in [!DNL Salesforce].

Sie geben die ID des Datensatzes an.

Das Modul gibt die ID des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL-Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Datensatztyp]</td>
    <td>Wählen Sie den Typ [!DNL Salesforce] Datensatzes aus, den das Modul [action].read.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Datensatzfelder]</td>
    <td>Wählen Sie die Felder aus, die das Modul lesen soll. Sie müssen mindestens ein Feld auswählen.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL ID]</td>
    <td> <p>Geben Sie die eindeutige [!DNL Salesforce]-ID des Datensatzes ein, den das Modul lesen soll, oder mappen Sie sie.</p> <p>Um die ID abzurufen, öffnen Sie das [!DNL Salesforce] in Ihrem Browser und kopieren Sie den Text am Ende der URL nach dem letzten Schrägstrich (/). Beispiel: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Löschen eines Datensatzes]

Dieses Aktionsmodul löscht einen vorhandenen Datensatz in einem Objekt.

Sie geben die ID des Datensatzes an.

Das Modul gibt die ID des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datensatztyp] </td> 
   <td> <p>Wählen Sie den Typ [!DNL Salesforce] Datensatzes aus, den das Modul löschen soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Geben Sie die eindeutige [!DNL Salesforce]-ID des Datensatzes ein, den Sie löschen möchten, oder mappen Sie sie.</p> <p>Um die ID abzurufen, öffnen Sie das [!DNL Salesforce] in Ihrem Browser und kopieren Sie den Text am Ende der URL nach dem letzten Schrägstrich (/). Beispiel: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Benutzerdefinierter API-Aufruf]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Salesforce]-API durchführen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von den anderen [!DNL Salesforce] nicht durchgeführt werden kann.

Das -Modul gibt Folgendes zurück:

* **[!UICONTROL Status-Code]** (Zahl): Dies zeigt den Erfolg oder Misserfolg Ihrer HTTP-Anfrage an. Dies sind Standardcodes, die Sie im Internet nachschlagen können.
* **[!UICONTROL Headers]** (Objekt): Ein detaillierterer Kontext für die Antwort/den Status-Code, der sich nicht auf den Ausgabetext bezieht. Nicht alle Kopfzeilen, die in einer Antwort-Kopfzeile angezeigt werden, sind Antwort-Kopfzeilen, sodass einige möglicherweise nicht für Sie nützlich sind.

  Die Antwort-Header hängen von der HTTP-Anfrage ab, die Sie beim Konfigurieren des Moduls ausgewählt haben.

* **[!UICONTROL body]** (Objekt): Je nach der HTTP-Anfrage, die Sie beim Konfigurieren des Moduls ausgewählt haben, erhalten Sie möglicherweise einige Daten zurück. Diese Daten, z. B. die Daten aus einer [!UICONTROL GET]-Anfrage, sind in diesem Objekt enthalten.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Geben Sie einen Pfad relativ zu ein<code> &lt;Instance URL&gt;/services/data/v46.0/</code>.</p> <p>Eine Liste der verfügbaren Endpunkte finden Sie im <a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Salesforce REST API-Entwicklerhandbuch</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Methode]</p> </td> 
   td&gt; <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anfragemethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Kopfzeilen]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu, z. B. <code>{"Content-type":"application/json"}</code>. Workfront Fusion fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu. Beispiel: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL body]</td> 
   <td> <p>Fügen Sie den Hauptteil des Inhalts für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Wenn Sie bedingte Anweisungen wie <code>if</code> in Ihrer JSON-Datei verwenden, setzen Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Beispiel:** Der folgende API-Aufruf gibt die Liste aller Benutzer in Ihrem [!DNL Salesforce]-Konto zurück:
>
>* **URL**: `query`
>
>* **Methode**: [!UICONTROL GET]
>
>* **Abfragezeichenfolge**:
>
>* **key**: `q`
>
>* **Wert**: `SELECT Id, Name, CreatedDate, LastModifiedDate FROM User LIMIT 10`
>
>Treffer der Suche finden Sie in der Modulausgabe unter **[!UICONTROL Bundle] > [!UICONTROL Body] > [!UICONTROL records]**.
>
>In unserem Beispiel wurden 6 Benutzer zurückgegeben:
>
>![](assets/matches-of-the-search-350x573.png)


#### [!UICONTROL Anlage/Dokument hochladen]

Dieses Aktionsmodul lädt eine Datei hoch und hängt sie an einen von Ihnen angegebenen Datensatz an oder lädt ein Dokument hoch.

Das Modul gibt die ID des Anhangs oder Dokuments und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Typ des Uploads]</td> 
   <td>Wählen Sie aus, ob das Modul eine Anlage oder ein Dokument hochladen soll.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Geben Sie die ID des Objekts ein, zu dem Sie eine Anlage hochladen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Ordner]</td> 
   <td>Wählen Sie den Ordner aus, der die Datei enthält, die das Modul hochladen soll. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source-Datei]</td> 
   <td>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Anlage/Dokument herunterladen]

Dieses Aktionsmodul lädt ein Dokument oder eine Anlage aus einem Datensatz herunter.

Sie geben die ID des Datensatzes und den gewünschten Download-Typ an.

Das Modul gibt die ID des Anhangs oder Dokuments und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr>
    <td>[!UICONTROL-Verbindung]</td>
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Downloadtyp]</td>
    <td> <p>Geben Sie den Dateityp an, den Sie von Salesforce herunterladen möchten.</p> 
     <ul> 
      <li>[!UICONTROL-Anhang]</li> 
      <li>[!UICONTROL-Dokument]</li> 
      <li>[!UICONTROL ContentDocument] (Dies ist ein Dokument, das in [!DNL Saleforce CRM Content] oder [!DNL Salesforce Files] in eine Bibliothek hochgeladen wurde.)</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[!UICONTROL ID] / </p> <p>[!UICONTROL Attachment ID] / </p> <p>[!UICONTROL ContentDocument-ID]</p> </td>
    <td> <p>Geben Sie die eindeutige [!DNL Salesforce]-ID des Datensatzes ein, den das Modul herunterladen soll, oder ordnen Sie sie zu.</p> <p>Um die ID abzurufen, öffnen Sie das [!DNL Salesforce] in Ihrem Browser und kopieren Sie den Text am Ende der URL nach dem letzten Schrägstrich (/). Beispiel: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Aktualisieren eines Datensatzes]

Dieses Aktionsmodul bearbeitet einen Datensatz in einem -Objekt.

Mit dem Modul können Sie auswählen, welche der Objektfelder im Modul verfügbar sind. Dadurch wird die Anzahl der Felder reduziert, die beim Einrichten des Moduls durchgescrollt werden müssen.

Das Modul gibt die ID des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Geben Sie die ID des Datensatzes ein, den Sie aktualisieren möchten, oder mappen Sie sie.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Datensatztyp] </p> </td> 
   <td> <p>Wählen Sie den Typ [!DNL Salesforce] Datensatzes aus, den das Modul aktualisieren soll. Die Felder werden je nach dem im Feld Datensatztyp ausgewählten Datensatztyp verfügbar. Diese Felder basieren auf der [!DNL Salesforce]-API.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Felder zum Zuordnen auswählen]</td> 
   <td> <p>Wählen Sie die Felder aus, die das Modul beim Erstellen des neuen Datensatzes konfigurieren soll. Erforderliche Felder befinden sich oben in der Liste. </p> <p>Die Felder, die Sie auswählen, werden unter diesem Feld geöffnet. Sie können jetzt Werte in diese Felder eingeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Suchvorgänge

#### [!UICONTROL Suche mit Abfrage]

Dieses Suchmodul sucht in einem -Objekt nach Datensätzen, [!DNL Salesforce] mit der angegebenen Suchanfrage übereinstimmen. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Suchtyp]</td> 
   <td> <p>Wählen Sie die Art der Suche aus, die das Modul durchführen soll:</p> 
    <ul> 
     <li> <p>[!UICONTROL Einfach]</p> </li> 
     <li> <p>[!UICONTROL mit SOSL (Salesforce Object Search Language)]</p> </li> 
     <li> <p>[!UICONTROL mit SOQL (Salesforce Object Query Language)]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Typ] </p> </td> 
   <td> <p>Wenn Sie den Typ Einfache Suche ausgewählt haben, wählen Sie den Typ [!DNL Salesforce] Datensatzes aus, nach dem das Modul suchen soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Abfrage] / [!UICONTROL SOL-Abfrage] / [!UICONTROL SOQL-Abfrage]</td> 
   <td> <p>Geben Sie die Abfrage ein, nach der Sie suchen möchten.</p> <p>Weitere Informationen zu SOSL finden Sie unter <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">Salesforce Object Search Language (SOSL)</a> in der [!DNL Salesforce].</p> <p>Weitere Informationen zu SOQL finden Sie unter <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">Salesforce Object Query Language (SOQL)</a> in der [!DNL Salesforce].</p> <p>Hinweis: Beachten Sie, dass der Wert des Parameters <code>RETURNING </code>die Ausgabe des Moduls beeinflusst. Wenn Sie <code>LIMIT</code> verwenden, ignorieren [!DNL Fusion] die Einstellungen im Feld [!UICONTROL Maximale Anzahl von Datensätzen]. Wenn Sie kein Limit festlegen, fügt Fusion den Wert [!UICONTROL LIMIT = Maximale Anzahl von Datensätzen] ein.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Anzahl von Datensätzen]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suche]

Dieses Aktionsmodul ruft alle Datensätze ab, die ein bestimmtes Kriterium erfüllen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu[!DNL  Adobe Workfront Fusion] - Grundlegende Anweisungen</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Typ]</td> 
   <td> <p>Wählen Sie den Typ des Objekts aus, nach dem Sie suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suchkriterien]</td> 
   <td>Wählen Sie das Feld aus, nach dem Sie suchen möchten, den Operator, den Sie in Ihrer Abfrage verwenden möchten, und den Wert, nach dem Sie im Feld suchen. Sie können Abfragen mithilfe von AND oder OR verbinden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgaben]</td> 
   <td>Wählen Sie die Felder aus, die Sie in die Ausgabe des Moduls aufnehmen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ergebnissatz]</td> 
   <td>Wählen Sie aus, ob das Modul alle übereinstimmenden Datensätze oder nur den ersten übereinstimmenden Datensatz zurückgeben soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum]</td> 
   <td>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus abrufen soll, oder mappen Sie sie.</td> 
  </tr> 
 </tbody> 
</table>
