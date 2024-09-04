---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Connector
navigation-topic: apps-and-their-modules
title: Workfront Proof-Module
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die [!DNL Workfront Proof] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion, Workfront Proof, Digital Content and Documents
exl-id: f5c6fb08-880d-4432-aef1-57db13b3ecdb
source-git-commit: 558ca6a1935d33e2c3c7ea3f4c1bd90a493ef8ff
workflow-type: tm+mt
source-wordcount: '3099'
ht-degree: 0%

---

# [!DNL Workfront Proof] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Workfront Proof] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

Dies ist nützlich, wenn Sie Aufgaben ausführen müssen, die derzeit beim Testen innerhalb von [!DNL Workfront] oder in [!DNL Workfront Proof] nicht unterstützt werden, z. B. Testsendungen basierend auf bestimmten Ereignissen aktualisieren und nach Empfängern eines Testversands suchen.

Der Connector [!DNL Workfront Proof] zählt nicht mit der Anzahl der aktiven Apps, die für Ihr Unternehmen verfügbar sind. Alle Szenarien, auch wenn sie nur die [!DNL Workfront Proof] -App verwenden, werden mit der Gesamtanzahl der Szenarien Ihrer Organisation angerechnet.

Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
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

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL Workfront Proof] mit [!DNL Workfront Fusion] verbinden

Sie können eine Verbindung zu Ihrem [!DNL Workfront Proof]-Konto direkt aus einem [!DNL Workfront Fusion]-Modul erstellen.

1. Klicken Sie in einem beliebigen [!DNL Workfront Fusion]-Modul neben dem Feld [!UICONTROL Verbindung] auf [!UICONTROL **Hinzufügen**] .

2. Füllen Sie die folgenden Felder aus:

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Verbindungsname]</p>
                </td>
                <td>Geben Sie einen Namen für die Verbindung ein</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL connections.environmentType]</td>
                <td>Wählen Sie aus, ob es sich um eine Produktionsumgebung oder eine Nicht-Produktionsumgebung wie Vorschau oder Sandbox handelt.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL connections.authenticationType]</td>
                <td>Wählen Sie aus, ob es sich um ein Dienstkonto oder ein persönliches Konto handelt.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL E-Mail/Benutzername]</td>
                <td>Geben Sie den Benutzernamen für Ihr [!DNL Workfront Proof] -Konto ein.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Kennwort]</td>
                <td>Geben Sie das Kennwort für Ihr [!DNL Workfront Proof] -Konto ein.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Mandantenkennung]</td>
                <td><strong>Hinweis</strong>: Kunden, die BYOK nicht verwenden, müssen dieses Feld leer lassen. <p>Geben Sie die Mandantenkennung für dieses Konto ein. Wenn Sie Hilfe bei der Suche nach Ihrer Mandantenkennung benötigen, wenden Sie sich an den Workfront-Support.</p></td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Domain-Erweiterung]</td>
                <td>Geben Sie die Erweiterung für die URL ein, mit der Sie auf Ihr Konto zugreifen. <p>Beispiel: <code>com</code> oder <code>eu</code></p></td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Produktion, Vorschau oder benutzerdefinierte Umgebung]</td>
                <td>Wählen Sie eine Verbindung zu einer Produktions-, Vorschau- oder einer benutzerdefinierten Umgebung aus.</td>
            </tr>
        </tbody>
    </table>


3. Klicken Sie auf [!UICONTROL **Weiter**] , um die Verbindung zu speichern und zum Modul zurückzukehren.

## [!DNL Workfront Proof] Module und ihre Felder

Wenn Sie [!DNL Workfront Proof] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Workfront Proof] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Trigger

* [Testsendungen ansehen](#watch-proofs)
* [PDF-Zusammenfassung ansehen](#watch-for-pdf-summary)
* [[!UICONTROL Aktivität &quot;Testversand ansehen&quot;]](#watch-proof-activity)

#### [!UICONTROL Testsendungen ansehen]

Dieses geplante Trigger-Modul führt ein Szenario aus, wenn ein Benutzer einen Testversand erstellt oder eine Entscheidung darüber trifft.

Das Modul gibt eine Liste aller Datensätze zurück, die es während des angegebenen Zeitraums findet, zusammen mit den Typen. Außerdem werden die Werte der von Ihnen angegebenen Felder zurückgegeben. Wenn das Modul Entscheidungen über den Testversand gefunden hat, enthält es sowohl die vorherigen als auch die aktuellen Werte in separaten Feldern. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Dies geschieht in einem regelmäßig von Ihnen festgelegten Intervall.

Sie müssen über ausreichende Berechtigungen verfügen, um auf den Testversand oder die Testsendungen in [!DNL Workfront Proof] zugreifen zu können, um diese Informationen abrufen zu können.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Datensatztyp</td> 
   <td>Wählen Sie den Typ von [!DNL Workfront Proof] Datensatz aus, den das Modul überwachen soll.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Ausgaben</td> 
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabebundle für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Limit</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Achten Sie auf die PDF-Zusammenfassung]

Dieses Instant Trigger-Modul führt ein Szenario aus, wenn jemand eine PDF-Zusammenfassung für einen Testversand erstellt.

In diesem Modul ist ein Webhook erforderlich.

Das Modul gibt alle mit dem Testversand verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Außerdem wird ein neues Ereignisabonnement für PDF-Zusammenfassungen erstellt und der Inhalt aus dem in der Payload gesendeten Attribut &quot;pdf_url&quot;ausgegeben. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td>Sie können einen vorhandenen Webhook auswählen oder einen neuen erstellen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Instant Trigger (Webhooks) in [!DNL Adobe Workfront Fusion]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aktivität &quot;Testversand ansehen&quot;]

Dieses Trigger-Modul führt ein Szenario aus, wenn eine bestimmte Aktivität auf einem Testversand erfolgt.

Das Modul gibt alle mit dem Testversand verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Außerdem wird ein neues Ereignisabonnement für PDF-Zusammenfassungen erstellt und der Inhalt aus dem in der Payload gesendeten `pdf_url` -Attribut ausgegeben. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aktivitätstyp]</td> 
   <td>Wählen Sie aus, ob Sie eine neue Entscheidung (einschließlich der Statusänderungen des [!UICONTROL Testversands]) oder nur allgemeine Statusänderungen des Testversands sehen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl von Datensätzen ein oder ordnen Sie sie zu, die das Modul während der verschiedenen Ausführungszyklen eines Szenarios zurückgeben soll.</td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL Testversand erstellen]](#create-proof)
* [[!UICONTROL Benutzerspezifischer API-Aufruf]](#custom-api-call)
* [[!UICONTROL Testversand herunterladen]](#download-proof)
* [[!UICONTROL Datensatz lesen]](#read-a-record)
* [[!UICONTROL PDF-Zusammenfassung anfordern]](#request-pdf-summary)
* [[!UICONTROL Testversand aktualisieren]](#update-proof)
* [[!UICONTROL Datei hochladen]](#upload-file)

#### [!UICONTROL Testversand erstellen]

Dieses Aktionsmodul erstellt einen neuen Testversand oder eine neue Version eines Testversands in [!DNL Workfront Proof].

Wenn Sie eine neue Version erstellen, geben Sie die Parameter für den neuen Testversand und den Quell-Testversand an.

Das Modul gibt die Kennung der neuen Testversand- oder Testversion zurück. Sie können diese Informationen in nachfolgenden Modulen des Szenarios zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testtyp]</td> 
   <td> <p>Geben Sie an, ob der erstellte Testversand einen einfachen Workflow oder einen automatisierten [!UICONTROL Workflow] enthalten soll.</p> <p>Füllen Sie dann die Felder aus, die für den gewählten Testversand-Typ angezeigt werden. Wenn Sie beispielsweise [!UICONTROL Automatisierter Workflow] auswählen, füllen Sie das Feld <strong>[!UICONTROL Workflow-Phasen]</strong> aus, um die Bühnen zu konfigurieren.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Herunterladen der Originaldatei zulassen]</td> 
   <td>Wählen Sie aus, ob Sie den Download der Originaldatei, aus der der Testversand erstellt wurde, zulassen möchten.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Classic Proof Viewer]</td> 
   <td>Wählen Sie aus, ob Sie den klassischen Proof-Viewer verwenden.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Alle Dateien in einem Testversand zusammenführen]</td> 
   <td>Aktivieren Sie diese Option, um alle Dateien zu einem mehrseitigen Testversand zusammenzufassen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Neue Testversion erstellen]</td> 
   <td>Wählen Sie diese Option aus, wenn das Modul eine neue Version eines vorhandenen Testversands erstellen soll. Geben Sie dann im angezeigten Feld <strong>[!UICONTROL Existing Proof ID]</strong> die eindeutige Kennung des Testversands ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Custom Link Label]</td> 
   <td>Geben Sie einen Titel für den benutzerspezifischen Testversand-Link ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benutzerspezifische Link-URL]</td> 
   <td>Geben Sie die URL für den benutzerspezifischen Link ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Standard-E-Mail-Benachrichtigungen für Abonnenten]</td> 
   <td>Geben Sie eine der folgenden Zahlen ein, um anzugeben, welche der folgenden standardmäßigen E-Mail-Benachrichtigungseinstellungen Sie für den erstellten Testversand verwenden möchten.
    <ul>
     <li><strong>1</strong> - Alle neuen Kommentare und Antworten</li>
     <li><strong>2</strong> - Antworten auf meine Kommentare</li>
     <li><strong>3</strong> - Tägliche Zusammenfassung</li>
     <li><strong>4</strong> - Stündliche Zusammenfassung</li>
     <li><strong>5</strong> - Nur Entscheidungen</li>
     <li><strong>9</strong> - Deaktiviert</li>
    </ul></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Excel-Zusammenfassung deaktivieren]</td> 
   <td>Wählen Sie aus, ob Sie die Möglichkeit zum Herunterladen von Testversand-Kommentaren in eine Excel-Datei deaktivieren möchten.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL PDF-Zusammenfassung deaktivieren]</td> 
   <td>Wählen Sie aus, ob Sie die Möglichkeit zum Herunterladen von Testversand-Kommentaren in eine PDF-Datei deaktivieren möchten.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Abonnement-E-Mail deaktivieren]</td> 
   <td>Wählen Sie aus, ob Sie die Abonnement-E-Mail für diesen Testversand deaktivieren möchten.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Einbettungs-Player aktivieren]</td> 
   <td>Wählen Sie aus, ob Sie den eingebetteten Player für diesen Testversand aktivieren möchten.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Abonnements aktivieren]</td> 
   <td>Wählen Sie aus, ob Personen, die nicht Teilnehmer sind, den Testversand abonnieren dürfen.<br>Wenn Sie diese Option auswählen, können Sie auch die Standardrolle für Abonnenten auswählen, wie in dieser Tabelle beschrieben.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Validierung von Abonnements aktivieren]</td> 
   <td>Wählen Sie aus, ob Sie die E-Mail-Validierung des Abonnements aktivieren möchten. Ist diese Option aktiviert, muss der Abonnent auf einen Link in einer E-Mail klicken, um auf einen Testversand zugreifen zu können.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Team-URL aktivieren]</td> 
   <td>Wählen Sie aus, ob der erstellte Testversand die Team-URL ausblenden oder anzeigen soll.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Datei-Hash] <span style="font-weight: normal;">oder </span> [!UICONTROL Datei-Hashes]</td> 
   <td>Fügen Sie die Kennung der Datei(en) hinzu, aus der/denen Sie einen Testversand oder Testsendungen erstellen möchten.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Dateinamen]</td> 
   <td>Fügen Sie den Dateinamen oder die Namen für den erstellten Testversand hinzu. Dies ist ein erforderliches Feld.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Testversand sperren, wenn alle erforderlichen Entscheidungen getroffen werden]</td> 
   <td>Geben Sie an, ob der erstellte Testversand gesperrt werden soll, nachdem alle erforderlichen Entscheidungen getroffen wurden.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Empfänger über diesen Testversand informieren]</td> 
   <td>Wählen Sie eine Option aus, um anzugeben, ob Empfänger beim Erstellen des Testversands benachrichtigt werden sollen.&gt;</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testname]</td> 
   <td>Geben Sie einen Namen für den erstellten Testversand ein. Dies ist ein erforderliches Feld. Verwenden Sie ein senkrechte Strich (|), um Namen für mehrere Testsendungen zu trennen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kennung des Testinhabers]</td> 
   <td>Geben Sie die Kennung des Testversand-Eigentümers ein oder ordnen Sie sie zu. Wenn dieses Feld leer gelassen wird, wird der Testversand-Inhaber auf den aktuellen Benutzer gesetzt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Referenz-ID]</td> 
   <td>Geben Sie die Referenz-ID für den Testversand ein.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Elektronische Signatur erforderlich]</td> 
   <td>Wählen Sie aus, ob Sie die Übermittlung einer elektronischen Signatur durch einen Benutzer, der über einen Testversand entscheidet, vorschreiben möchten.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Anmeldung erforderlich]</td> 
   <td> <p>Geben Sie an, ob für den erstellten Testversand eine Anmeldung erforderlich ist. </p> <p>Dies entspricht der Einstellung [!UICONTROL Anmeldung erforderlich] , die unter <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Testeinstellungen konfigurieren] in [!DNL Workfront Proof]</a> erläutert wird.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Auflösung-ID]</td> 
   <td>Geben Sie die Kennung der Auflösung ein, die Sie für Ihren Testversand verwenden möchten. Eine Liste der Auflösungs-IDs finden Sie in der [!DNL Workfront Proof] <a href="https://api.proofhq.com/home/objects/soapworkflowproofobject.html">API-Dokumentation</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL SWF]</td> 
   <td>Geben Sie den Typ des SWF-Testversands an.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Show] [item]</td> 
   <td>Wählen Sie für jedes Element aus, ob es im Testversand angezeigt werden soll.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Workspace ID]</td> 
   <td>Geben Sie die Kennung des Arbeitsbereichs ein, in dem Sie den Testversand erstellen möchten. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Empfänger]</td> 
   <td>Fügen Sie die E-Mail-Adressen der Empfänger hinzu, die für den erstellten Testversand verwendet werden sollen .</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Deadline]</td> 
   <td> <p>Geben Sie den Termin für den erstellten Testversand an. Verwenden Sie das folgende Datumsformat:</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Benutzerspezifischer API-Aufruf]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Workfront Proof] -API durchführen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von anderen [!DNL Workfront Proof] -Modulen nicht ausgeführt werden kann.

Das Modul gibt den Statuscode, die Kopfzeilen und den Hauptteil zurück. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Methode]</td> 
   <td>Legen Sie die Aktion für den API-Aufruf fest. Informationen zu verfügbaren Aktionen finden Sie in der <a href="https://api.proofhq.com/">Dokumentation zur Proof API</a> .</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Body (XML)]</td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Beispiel:**
>
>![](assets/wfp-api-module-example-350x586.png)

#### [!UICONTROL Testversand herunterladen]

Dieses Aktionsmodul lädt die Quelldatei eines bestimmten Testversands herunter, den Sie anhand der zugehörigen ID identifizieren.

Sie geben die Kennung des Testversands an.

Das Modul gibt den Inhalt der Quelldatei zurück, die zum Erstellen des Testversands verwendet wird. Sie können diese Informationen in nachfolgenden Modulen des Szenarios zuordnen.

Sie müssen über ausreichende Berechtigungen zum Zugriff auf den Datensatz in [!DNL Workfront Proof] verfügen, um diese Informationen abrufen zu können.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testversand-ID]</td> 
   <td> <p>Geben Sie die eindeutige Kennung des Testversands ein, die Sie auf der Seite [!UICONTROL Testversanddetails] finden. Weitere Informationen finden Sie unter <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Testversand-Details verwalten in [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datensatz lesen]

Dieses Aktionsmodul liest Daten aus einem einzelnen Testversand in [!DNL Workfront Proof].

Geben Sie die Kennung des Testversands und die gewünschten Informationen aus dem Testversand an.

Das Modul gibt die Werte der für den Testversand ausgewählten Felder sowie deren Typen zurück. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Sie müssen über ausreichende Berechtigungen zum Zugriff auf den Datensatz in [!DNL Workfront Proof] verfügen, um diese Informationen abrufen zu können.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record Type]</td> 
   <td>Wählen Sie aus, ob Sie einen Testversand, Testversand-Kommentare oder Testversand-Reviewer lesen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabebundle für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Geben Sie die eindeutige [!DNL Workfront Proof]-ID des Datensatzes ein oder ordnen Sie sie zu, den das Modul lesen soll.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL PDF-Zusammenfassung anfordern]

Dieses Aktionsmodul fordert die PDF-Zusammenfassung für einen bestimmten Testversand in [!DNL Workfront Proof] an.

Sie geben die Kennung des Testversands an.

Das Modul gibt PDF-Zusammenfassungsinformationen zurück. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Sie müssen über ausreichende Berechtigungen zum Zugriff auf den Datensatz in [!DNL Workfront Proof] verfügen, um diese Informationen abrufen zu können.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testversand-ID]</td> 
   <td> <p>Geben Sie die eindeutige [!DNL Workfront Proof]-ID des Testversands ein, für den Sie eine PDF-Zusammenfassung anfordern möchten.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Callback-URL]</td> 
   <td>Geben Sie die URL ein oder ordnen Sie sie zu, an die die PDF-Zusammenfassung gesendet werden soll.</td> 
  </tr> 
 </tbody> 
</table>

##### Mögliche Fehler

* **Fehler**: &quot;[!UICONTROL Sie haben keine Berechtigung, diese Anforderung auszuführen. Die Bühne muss mindestens einen Empfänger enthalten.]&quot;
* **Lösung**: Stellen Sie sicher, dass Sie nicht die einzige Lösung sind, die den Phasen des Workflows zugewiesen ist. Den Phasen des Workflows muss ein anderer Benutzer zugewiesen sein.

#### [!UICONTROL Testversand aktualisieren]

Dieses Aktionsmodul aktualisiert einen vorhandenen Testversand in [!DNL Workfront Proof].

Geben Sie die Kennung des Testversands und den Datensatztyp sowie die Felder an, die in die Ausgabe aufgenommen werden sollen.

Das Modul gibt alle mit dem Datensatz verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Sie müssen über ausreichende Berechtigungen zum Zugriff auf den Datensatz in [!DNL Workfront Proof] verfügen, um diese Informationen abrufen zu können.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testversand-ID]</td> 
   <td> <p>Geben Sie die eindeutige Kennung des Testversands ein, die Sie auf der Seite [!UICONTROL Testversanddetails] finden. Weitere Informationen finden Sie unter <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Testversand-Details verwalten in [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Deadline]</td> 
   <td> <p>Geben Sie den Termin für den erstellten Testversand an. Verwenden Sie das folgende Datumsformat:</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Standard-E-Mail-Benachrichtigungen für Abonnenten]</td> 
   <td>Wählen Sie aus, welche der folgenden Standard-E-Mail-Benachrichtigungseinstellungen Sie für den erstellten Testversand verwenden möchten.
    <ul>
     <li> [!UICONTROL Alle neuen Kommentare und Antworten</li>
     <li>[!UICONTROL Antworten auf meine Kommentare]</li>
     <li>[!UICONTROL Tägliche Zusammenfassung]</li>
     <li> [!UICONTROL Stündliche Zusammenfassung]</li>
     <li> [!UICONTROL Entscheidungen]</li>
     <li> [!UICONTROL Deaktiviert]</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Standardrolle]</td> 
   <td>Wählen Sie die Standardrolle für den Testversand aus.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abonnement-E-Mail deaktivieren]</td> 
   <td>Wählen Sie aus, ob Sie die Abonnement-E-Mail für diesen Testversand deaktivieren möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abonnements aktivieren]</td> 
   <td>Wählen Sie aus, ob Personen, die nicht Teilnehmer sind, den Testversand abonnieren dürfen.<br>Wenn Sie diese Option auswählen, können Sie auch die [!UICONTROL Standardrolle] für Abonnenten auswählen, wie in dieser Tabelle beschrieben.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Validierung von Abonnements aktivieren]</td> 
   <td>Wählen Sie aus, ob Sie die E-Mail-Validierung des Abonnements aktivieren möchten. Ist diese Option aktiviert, muss der Abonnent auf einen Link in einer E-Mail klicken, um auf einen Testversand zugreifen zu können.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team-URL aktivieren]</td> 
   <td>Wählen Sie aus, ob der erstellte Testversand die Team-URL ausblenden oder anzeigen soll.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testversand sperren, wenn alle erforderlichen Entscheidungen getroffen werden]</td> 
   <td>Geben Sie an, ob der erstellte Testversand gesperrt werden soll, nachdem alle erforderlichen Entscheidungen getroffen wurden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nachricht]</td> 
   <td>Geben Sie eine Nachricht ein oder ordnen Sie sie zu, die Sie dem Testversand hinzufügen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testversand-ID] </td> 
   <td>Geben Sie die Kennung des Testversands ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testname]</td> 
   <td>Geben Sie den Namen des Testversands ein, den Sie aktualisieren möchten, oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anmeldung erforderlich]</td> 
   <td> <p>Geben Sie an, ob für den erstellten Testversand eine Anmeldung erforderlich ist. </p> <p>Dies entspricht der Einstellung [!UICONTROL Anmeldung erforderlich] , die unter <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Testeinstellungen konfigurieren] in [!DNL Workfront Proof]</a> erläutert wird.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Versionen anzeigen wie]</td> 
   <td>Wählen Sie aus, ob Sie einen Link zu anderen Versionen dieses Testversands anzeigen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Betreff]</td> 
   <td>Betreff des Testversands eingeben oder zuordnen</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei hochladen]

Dieses Aktionsmodul lädt eine Datei zur Verwendung mit dem Modul [!UICONTROL Testversand erstellen] in [!DNL Workfront Proof] hoch.

Das Modul gibt eine Hash-ID für die hochgeladene Datei zurück. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source-Datei]</td> 
   <td> <p>Wählen Sie eine Quelldatei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Suchvorgänge

* [[!UICONTROL Workflow-Vorlagen auflisten]](#list-workflow-templates)
* [[!UICONTROL Suche]](#search)

#### [!UICONTROL Workflow-Vorlagen auflisten]

Dieses Suchmodul listet alle verfügbaren Workflow-Vorlagen auf.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabebundle für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Vorlagen ein oder ordnen Sie sie zu, die das Modul während der Ausführung jedes Szenarios zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suche]

Dieses Suchmodul sucht nach Datensätzen in einem Objekt in [!DNL Workfront Proof], die mit der von Ihnen angegebenen Suchabfrage übereinstimmen.

Das Modul gibt die Kennung des Testversands zurück, wenn es nach einem Testversand sucht. Oder sie gibt die Benutzer-IDs, E-Mails, Namen, Positionen und E-Mail-Aliase der Empfänger zurück, wenn sie nach Empfängern sucht. Sie können diese Informationen in nachfolgenden Modulen des Szenarios zuordnen.

Sie müssen über ausreichende Berechtigungen zum Zugriff auf den Datensatz in [!DNL Workfront Proof] verfügen, um diese Informationen abrufen zu können.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Suchen nach</td> 
   <td> <p>Wählen Sie unter [!UICONTROL] den Datensatztyp aus, nach dem das Modul suchen soll.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Testversand]</strong> </p> <p>Geben Sie den Testversand-Namen des Testversands ein, nach dem Sie suchen möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL Empfänger]</strong> </p> <p>Geben Sie die E-Mail-Adresse des Empfängers ein, nach dem Sie suchen möchten.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ergebnissatz]</td> 
   <td>Geben Sie an, ob das Modul nach <strong>[!UICONTROL Alle übereinstimmenden Datensätze]</strong> oder nur dem <strong>[!UICONTROL ersten übereinstimmenden Datensatz]</strong> sucht.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Sortieren nach:</td> 
   <td>Wählen Sie das Feld aus, nach dem die Ergebnisse sortiert werden sollen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Sortierrichtung]</td> 
   <td> <p>Wählen Sie aus, ob die Ergebnisse auf- oder absteigend sortiert werden sollen.</p> </td> 
  </tr> 
 </tbody> 
</table>
