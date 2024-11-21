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
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '2758'
ht-degree: 0%

---

# [!DNL Salesforce] Module

In einem Adobe Workfront Fusion-Szenario können Sie Workflows automatisieren, die [!DNL Salesforce] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

Eine Videoeinführung zum Salesforce-Connector finden Sie unter:

* [Salesforce](https://video.tv.adobe.com/v/3427027/){target=_blank}

Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

>[!NOTE]
>
>* Nicht alle Editionen von [!DNL Salesforce] haben API-Zugriff. Weitere Informationen finden Sie in den Informationen zu [!DNL Salesforce] Editionen mit API-Zugriff auf die [!DNL Salesforce] Community-Site.
>* Informationen zu spezifischen Fehlern, die von der [!DNL Salesforce] -API zurückgegeben werden, finden Sie in den API-Dokumenten von [!DNL Salesforce] . Sie können auch den Status der [!DNL Salesforce]-API auf mögliche Dienstausfälle überprüfen.
>

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

Um [!DNL Salesforce] -Module zu verwenden, müssen Sie über ein [!DNL Salesforce] -Konto verfügen.

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

## Über die Suche nach [!DNL Salesforce] -Objekten

Bei der Suche nach Objekten können Sie entweder einzelne Suchbegriffe eingeben oder mithilfe von Platzhaltern und Operatoren eine komplexere Abfrage erstellen:

* Verwenden Sie die Platzhalterkarte (\*) als Ersatz für null oder mehr Zeichen. Beispielsweise findet eine Suche nach Ca\* Elemente, die mit Ca beginnen
* Verwenden Sie eine Fragezeichen-Platzhalter (?) als Ersatz für ein einzelnes Zeichen. Beispielsweise findet eine Suche nach Jo?n Elemente mit dem Begriff John oder Joan, aber nicht Jon
* Verwenden Sie den Anführungszeichen-Operator (&quot;&quot;&quot;), um eine exakte Wortübereinstimmung zu finden. Beispiel: &quot;Montag-Sitzung&quot;

Weitere Informationen zu Suchmöglichkeiten finden Sie in der [!DNL Salesforce] Entwicklerdokumentation zu SOQL und SOSL.

## [!DNL Salesforce] Module und ihre Felder

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Trigger

* [[!UICONTROL Auf Aufzeichnungen achten]](#watch-for-records)
* [[!UICONTROL Ausgehende Nachrichten ansehen]](#watch-outbound-messages)
* [[!UICONTROL Ein Feld ansehen]](#watch-a-field)

#### [!UICONTROL Auf Aufzeichnungen achten]

Dieses Trigger-Modul führt ein Szenario aus, wenn ein Datensatz in einem Objekt erstellt oder aktualisiert wird. Das Modul gibt alle mit dem Datensatz oder den Datensätzen verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Typ] </td> 
   <td> <p>Wählen Sie den Typ von [!DNL Salesforce] Datensatz aus, den das Modul überwachen soll.</p> </td> 
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

1. Gehen Sie zur Setup-Seite [!DNL Salesforce] .

   Um auf die Einrichtungsseite zuzugreifen, suchen Sie die Schaltfläche mit der Bezeichnung &quot;[!UICONTROL Setup]&quot; in der oberen rechten Ecke des [!DNL Salesforce]-Kontos und klicken Sie darauf. Suchen Sie auf der Setup-Seite [!DNL Salesforce] die Leiste &quot;[!UICONTROL Schnellsuche/Suche]&quot; auf der linken Seite. Suchen Sie nach &quot;[!UICONTROL Workflow-Regeln]&quot;.

1. Klicken Sie auf **[!UICONTROL Workflow-Regeln]**.
1. Klicken Sie auf der angezeigten Seite [!UICONTROL Workflow-Regeln] auf **[!UICONTROL Neue Regel]** und wählen Sie den Objekttyp aus, auf den die Regel angewendet werden soll (z. B. &quot;[!UICONTROL Chancen]&quot;, wenn Sie Aktualisierungen von Opportunity-Datensätzen überwachen).
1. Klicken Sie auf **[!UICONTROL Weiter]**.
1. Legen Sie einen Regelnamen, Bewertungskriterien und Regelkriterien fest und klicken Sie dann auf **[!UICONTROL Speichern]** und **[!UICONTROL Weiter]**.

1. Klicken Sie auf **[!UICONTROL Fertig]**.
1. Klicken Sie in der neu erstellten Workflow-Regel auf **[!UICONTROL Bearbeiten]**.
1. Wählen Sie aus der Dropdownliste **[!UICONTROL Workflow-Aktion hinzufügen]** die Option **[!UICONTROL Neue ausgehende Nachricht hinzufügen]** aus.

1. Geben Sie den Namen, die Beschreibung, die Endpunkt-URL und die Felder an, die Sie in die neue ausgehende Nachricht aufnehmen möchten, und klicken Sie dann auf **[!UICONTROL Speichern]**.

   Das Feld **[!UICONTROL Endpunkt-URL]** enthält die URL, die auf der [!DNL Salesforce] [!UICONTROL Ausgehende Nachricht ] in [!DNL Workfront Fusion] angegeben ist.

1. Konfigurieren Sie ein Szenario, das mit dem Ereignis [!UICONTROL Ausgehende Nachricht ] beginnt.

1. Klicken Sie unten rechts auf das Symbol **&lt;/>** und kopieren Sie die angegebene URL.
1. Kehren Sie zur Seite **[!UICONTROL Workflow-Regeln]** zurück, suchen Sie die neu erstellte Regel und klicken Sie dann auf **[!UICONTROL Aktivieren]**.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td> <p>Wählen Sie den Webhook aus, den Sie zum Anzeigen ausgehender Nachrichten verwenden möchten. Um einen Webhook hinzuzufügen, klicken Sie auf <strong>[!UICONTROL Add]</strong> und geben Sie den Namen und die Verbindung des Webhooks ein.</p> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit [!UICONTROL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Wählen Sie den Typ von [!DNL Salesforce] Datensatz aus, den das Modul auf ausgehende Nachrichten überwachen soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Felder]</td> 
   <td> <p>Wählen Sie die Felder aus, die das Modul auf ausgehende Nachrichten überwachen soll. Die verfügbaren Felder hängen vom Datensatztyp ab.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### *[!UICONTROL Ein Feld ansehen]*

Dieses Trigger-Modul startet ein Szenario, wenn ein Feld in [!DNL Salesforce] aktualisiert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Wählen Sie den Datensatztyp aus, der das Feld enthält, das das Modul überwachen soll. Sie müssen einen Datensatztyp auswählen, für den [!UICONTROL Feldverlauf] bei der Einrichtung von [!DNL Salesforce] aktiviert ist. Weitere Informationen finden Sie unter <a href="https://help.salesforce.com/articleView?id=tracking_field_history.htm&amp;type=5">Feldverlauf-Tracking</a> in der Dokumentation zu [!DNL Salesforce]. </p> </td> 
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

* [[!UICONTROL Erstellen eines Datensatzes]](#create-a-record)
* [[!UICONTROL Datensatz lesen]](#read-a-record)
* [[!UICONTROL Einen Datensatz löschen]](#delete-a-record)
* [[!UICONTROL Benutzerspezifischer API-Aufruf]](#custom-api-call)
* [[!UICONTROL Anhang/Dokument hochladen]](#upload-attachmentdocument)
* [[!UICONTROL Anhang/Dokument herunterladen]](#download-attachmentdocument)

#### [!UICONTROL Erstellen eines Datensatzes]

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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Record Type] </p> </td> 
   <td> <p>Wählen Sie den Typ von [!DNL Salesforce] Datensatz aus, den das Modul erstellen soll. Felder werden je nach dem im Feld [!UICONTROL Record Type] ausgewählten Datensatztyp verfügbar. Diese Felder basieren auf der [!DNL Salesforce] -API.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Record Type]</td>
    <td>Wählen Sie den Typ von [!DNL Salesforce] Datensatz aus, den das Modul [action].read lauten soll.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL Datensatzfelder]</td>
    <td>Wählen Sie die Felder aus, die das Modul lesen soll. Sie müssen mindestens ein Feld auswählen.</td>
  </tr> 
  <tr>
    <td>[!UICONTROL ID]</td>
    <td> <p>Geben Sie die eindeutige [!DNL Salesforce]-ID des Datensatzes ein oder ordnen Sie sie zu, den das Modul lesen soll.</p> <p>Um die ID abzurufen, öffnen Sie das Objekt [!DNL Salesforce] in Ihrem Browser und kopieren Sie den Text am Ende der URL nach dem letzten Schrägstrich (/). Beispiel: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Einen Datensatz löschen]

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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type] </td> 
   <td> <p>Wählen Sie den Typ von [!DNL Salesforce] Datensatz aus, den das Modul löschen soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td> <p>Geben Sie die eindeutige [!DNL Salesforce]-ID des Datensatzes ein oder ordnen Sie sie zu, den das Modul löschen soll.</p> <p>Um die ID abzurufen, öffnen Sie das Objekt [!DNL Salesforce] in Ihrem Browser und kopieren Sie den Text am Ende der URL nach dem letzten Schrägstrich (/). Beispiel: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Benutzerspezifischer API-Aufruf]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Salesforce] -API durchführen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von anderen [!DNL Salesforce] -Modulen nicht ausgeführt werden kann.

Das Modul gibt Folgendes zurück:

* **[!UICONTROL Status-Code]** (Zahl): Zeigt an, ob Ihre HTTP-Anforderung erfolgreich oder fehlgeschlagen ist. Dies sind Standardcodes, die Sie im Internet nachschlagen können.
* **[!UICONTROL Kopfzeilen]** (Objekt): Ein detaillierterer Kontext für den Antwort-/Statuscode, der sich nicht auf den Ausgabetext bezieht. Nicht alle Header, die in einem Antwortheader angezeigt werden, sind Antwortheader, sodass einige möglicherweise nicht nützlich für Sie sind.

  Die Antwortheader hängen von der HTTP-Anforderung ab, die Sie beim Konfigurieren des Moduls ausgewählt haben.

* **[!UICONTROL Hauptteil]** (Objekt): Je nach der HTTP-Anforderung, die Sie beim Konfigurieren des Moduls ausgewählt haben, erhalten Sie möglicherweise einige Daten zurück. Diese Daten, z. B. die Daten einer [!UICONTROL GET] -Anfrage, sind in diesem Objekt enthalten.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Geben Sie einen Pfad relativ zu <code> &lt;Instance URL&gt;/services/data/v46.0/</code> ein.</p> <p>Die Liste der verfügbaren Endpunkte finden Sie im <a href="https://developer.salesforce.com/docs/atlas.en-us.api_rest.meta/api_rest/intro_what_is_rest_api.htm">Salesforce REST API Developer Guide</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Methode]</p> </td> 
   td&gt; <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu, z. B. <code>{"Content-type":"application/json"}</code>. Workfront Fusion fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p>Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu. Beispiel: <code>{"name":"something-urgent"}</code></p> </td> 
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

>[!INFO]
>
>**Beispiel:** Der folgende API-Aufruf gibt die Liste aller Benutzer in Ihrem [!DNL Salesforce] -Konto zurück:
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
>Übereinstimmungen der Suche finden Sie in der Ausgabe des Moduls unter **[!UICONTROL Bundle] > [!UICONTROL Hauptteil] > [!UICONTROL Datensätze]**.
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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
   <td>[!UICONTROL Source-Datei]</td> 
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr>
    <td>[!UICONTROL Download-Typ]</td>
    <td> <p>Geben Sie den Dateityp an, den Sie von Salesforce herunterladen möchten.</p> 
     <ul> 
      <li>[!UICONTROL Anhang]</li> 
      <li>[!UICONTROL Document]</li> 
      <li>[!UICONTROL ContentDocument] (Dies ist ein Dokument, das in [!DNL Saleforce CRM Content] oder [!DNL Salesforce Files] in eine Bibliothek hochgeladen wurde.)</li> 
     </ul> </td>
  </tr> 
  <tr>
    <td> <p>[!UICONTROL ID] / </p> <p>[!UICONTROL Attachment ID] / </p> <p>[!UICONTROL ContentDocument ID]</p> </td>
    <td> <p>Geben Sie die eindeutige [!DNL Salesforce]-ID des Datensatzes ein oder ordnen Sie sie zu, den das Modul herunterladen soll.</p> <p>Um die ID abzurufen, öffnen Sie das Objekt [!DNL Salesforce] in Ihrem Browser und kopieren Sie den Text am Ende der URL nach dem letzten Schrägstrich (/). Beispiel: <code>https://eu5.salesforce.com/&lt;object ID&gt;</code></p> </td>
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
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Geben Sie die Kennung des Datensatzes ein, den Sie aktualisieren möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Record Type] </p> </td> 
   <td> <p>Wählen Sie den Typ von [!DNL Salesforce] Datensatz aus, den das Modul aktualisieren soll. Felder werden je nach dem im Feld Datensatztyp ausgewählten Datensatztyp verfügbar. Diese Felder basieren auf der [!DNL Salesforce] -API.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Felder zur Zuordnung auswählen]</td> 
   <td> <p>Wählen Sie die Felder aus, die das Modul beim Erstellen des neuen Datensatzes konfigurieren soll. Die erforderlichen Felder befinden sich oben in der Liste. </p> <p>Die ausgewählten Felder werden unter diesem Feld geöffnet. Sie können jetzt Werte in diese Felder eingeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Suchvorgänge

#### [!UICONTROL Suche mit Abfrage]

Dieses Suchmodul sucht nach Datensätzen in einem Objekt in [!DNL Salesforce], die mit der von Ihnen angegebenen Suchabfrage übereinstimmen. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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
   <td> <p>Wenn Sie den Typ Einfache Suche ausgewählt haben, wählen Sie den Typ von [!DNL Salesforce] Datensatz aus, nach dem das Modul suchen soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abfrage] / [!UICONTROL SOSL-Abfrage] / [!UICONTROL SOQL-Abfrage]</td> 
   <td> <p>Geben Sie die Abfrage ein, nach der Sie suchen möchten.</p> <p>Weitere Informationen zu SOSL finden Sie unter <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_sosl.htm">Salesforce Object Search Language (SOSL)</a> in der Dokumentation zu [!DNL Salesforce].</p> <p>Weitere Informationen zu SOQL finden Sie unter <a href="https://developer.salesforce.com/docs/atlas.en-us.soql_sosl.meta/soql_sosl/sforce_api_calls_soql.htm">Salesforce Object Query Language (SOQL)</a> in der Dokumentation zu [!DNL Salesforce].</p> <p>Hinweis: Beachten Sie, dass der Wert des Parameters <code>RETURNING </code>die Ausgabe des Moduls beeinflusst. Wenn Sie <code>LIMIT</code> verwenden, ignoriert [!DNL Fusion] die Einstellungen im Feld [!UICONTROL Maximale Anzahl von Datensätzen]. Wenn Sie keine Begrenzung festlegen, fügt Fusion den Wert [!UICONTROL LIMIT = Maximale Anzahl an Datensätzen] ein.</p> </td> 
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
   <td>Anweisungen zum Verbinden Ihres [!DNL Salesforce]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL  Adobe Workfront Fusion] - Grundlegende Anweisungen</a></td> 
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
