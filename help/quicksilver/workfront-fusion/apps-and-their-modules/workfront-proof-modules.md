---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: Workfront Proof-Module
description: In  [!DNL Adobe Workfront Fusion]  Szenario können Sie Workflows automatisieren, die  [!DNL Workfront Proof] verwenden, und sie mit mehreren Anwendungen und Services von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion, Workfront Proof, Digital Content and Documents
exl-id: f5c6fb08-880d-4432-aef1-57db13b3ecdb
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '3176'
ht-degree: 0%

---

# [!DNL Workfront Proof]

In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die [!DNL Workfront Proof] verwenden, und sie mit mehreren Anwendungen und Services von Drittanbietern verbinden.

Dies ist nützlich, wenn Sie Aufgaben ausführen müssen, die derzeit beim Proofing in [!DNL Workfront] oder in [!DNL Workfront Proof] nicht unterstützt werden, z. B. das Aktualisieren von Korrekturabzügen auf der Grundlage bestimmter Ereignisse und die Suche nach den Empfängern eines Korrekturabzugs.

Der [!DNL Workfront Proof]-Connector wird nicht auf die Anzahl der aktiven Apps angerechnet, die für Ihre Organisation verfügbar sind. Alle Szenarien werden mit der Gesamtanzahl der Szenarien Ihres Unternehmens verrechnet, auch wenn sie nur die [!DNL Workfront Proof]-App verwenden.

Anweisungen zum Erstellen eines Szenarios finden Sie unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## Workfront Proof-Informationen

Der Workfront Proof-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API-Version</td> 
   <td> v21.3.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.8.92</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Workfront Proof] mit [!DNL Workfront Fusion] verbinden

Sie können direkt aus einem [!DNL Workfront Fusion]-Modul heraus eine Verbindung zu Ihrem [!DNL Workfront Proof]-Konto herstellen.

1. Klicken Sie in einem [!DNL Workfront Fusion] Modul [!UICONTROL **Hinzufügen**] neben dem Feld [!UICONTROL Verbindung]

2. Füllen Sie die folgenden Felder aus:

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Verbindungsname]</p>
                </td>
                <td>Einen Namen für die Verbindung eingeben</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL connections.environmentType]</td>
                <td>Wählen Sie aus, ob es sich um eine Produktionsumgebung oder eine Nicht-Produktionsumgebung wie Vorschau oder Sandbox handelt.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL connections.authenticationType]</td>
                <td>Wählen Sie aus, ob dies ein Service-Konto oder ein persönliches Konto ist.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL E-Mail/Benutzername]</td>
                <td>Geben Sie den Benutzernamen für Ihr [!DNL Workfront Proof] ein.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Kennwort]</td>
                <td>Geben Sie das Passwort für Ihr [!DNL Workfront Proof] Konto ein.</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Mandanten-ID]</td>
                <td><strong>Hinweis</strong>: Kunden, die BYOK nicht verwenden, müssen dieses Feld leer lassen. <p>Mandanten-ID für dieses Konto eingeben. Wenn Sie Hilfe bei der Suche nach Ihrer Mandanten-ID benötigen, wenden Sie sich an den Kunden-Support von Workfront.</p></td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Domain-Erweiterung]</td>
                <td>Geben Sie die Erweiterung für die URL ein, über die Sie auf Ihr Konto zugreifen möchten. <p>Beispiel: <code>com</code> oder <code>eu</code></p></td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Produktions-, Vorschau- oder benutzerdefinierte Umgebung]</td>
                <td>Wählen Sie eine Verbindung zu einer Produktions-, Vorschau- oder benutzerdefinierten Umgebung aus.</td>
            </tr>
        </tbody>
    </table>


3. Klicken Sie [!UICONTROL **Fortfahren**], um die Verbindung zu speichern und zum Modul zurückzukehren

## [!DNL Workfront Proof] Module und ihre Felder

Beim Konfigurieren [!DNL Workfront Proof] Module zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service weitere [!DNL Workfront Proof] angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Suchvorgänge](#searches)

### Trigger

* [Korrekturabzüge ansehen](#watch-proofs)
* [Auf PDF-Zusammenfassung achten](#watch-for-pdf-summary)
* [[!UICONTROL Aktivität „Korrekturabzug ansehen]](#watch-proof-activity)

#### [!UICONTROL Testsendungen ansehen]

Dieses Modul für geplante Trigger führt ein Szenario aus, wenn jemand einen Korrekturabzug erstellt oder eine Entscheidung darüber trifft.

Das Modul gibt eine Liste aller Datensätze zusammen mit ihren Typen zurück, die es während des von Ihnen angegebenen Zeitraums findet. Außerdem werden die Werte der angegebenen Felder zurückgegeben. Wenn das Modul Entscheidungen gefunden hat, die für den Korrekturabzug getroffen wurden, enthält es sowohl den vorherigen als auch den aktuellen Wert in separaten Feldern. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Dies geschieht in einem regelmäßig geplanten Intervall, das Sie angeben.

Sie müssen über ausreichende Berechtigungen für den Zugriff auf den/die Korrekturabzug(e) in [!DNL Workfront Proof] verfügen, um diese Informationen abrufen zu können.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Datensatztyp</td> 
   <td>Wählen Sie den Typ [!DNL Workfront Proof] Datensatzes aus, den das Modul überwachen soll.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Ausgaben</td> 
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabepaket für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Grenze</td> 
   <td> <p>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Nach PDF-Zusammenfassung ansehen]

Dieses Instant Trigger-Modul führt ein Szenario aus, wenn jemand eine PDF-Zusammenfassung für einen Korrekturabzug erstellt.

In diesem Modul ist ein Webhook erforderlich.

Das Modul gibt alle Standardfelder zurück, die mit dem Korrekturabzug verknüpft sind, sowie alle benutzerdefinierten Felder und Werte, auf die die Verbindung zugreift. Außerdem wird ein neues Ereignisabonnement für PDF-Zusammenfassungen erstellt und der Inhalt des in der Payload gesendeten Attributs „pdf_url“ ausgegeben. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Webhook]</td> 
   <td>Sie können einen vorhandenen Webhook auswählen oder einen neuen erstellen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Instant Trigger (Webhooks) in [!DNL Adobe Workfront Fusion]</a>. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aktivität „Korrekturabzug ansehen]

Dieses Trigger-Modul führt ein Szenario aus, wenn eine bestimmte Aktivität in einem Korrekturabzug stattfindet.

Das Modul gibt alle Standardfelder zurück, die mit dem Korrekturabzug verknüpft sind, sowie alle benutzerdefinierten Felder und Werte, auf die die Verbindung zugreift. Außerdem wird ein neues Ereignisabonnement für PDF-Zusammenfassungen erstellt und der Inhalt des `pdf_url`-Attributs ausgegeben, das in der Payload gesendet wird. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aktivitätstyp]</td> 
   <td>Wählen Sie aus, ob Sie eine neue Entscheidung (einschließlich [!UICONTROL PROOF]-Statusänderungen) oder nur die Änderungen des Gesamtstatus des Korrekturabzugs ansehen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl von Datensätzen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL Korrekturabzug erstellen]](#create-proof)
* [[!UICONTROL Benutzerdefinierter API-Aufruf]](#custom-api-call)
* [[!UICONTROL Testversand herunterladen]](#download-proof)
* [[!UICONTROL Datensatz lesen]](#read-a-record)
* [[!UICONTROL PDF-Zusammenfassung anfordern]](#request-pdf-summary)
* [[!UICONTROL Korrekturabzug aktualisieren]](#update-proof)
* [[!UICONTROL Datei hochladen]](#upload-file)

#### [!UICONTROL Korrekturabzug erstellen]

Dieses Aktionsmodul erstellt einen neuen Korrekturabzug oder eine neue Version eines Korrekturabzugs in [!DNL Workfront Proof].

Sie geben die Parameter für den neuen Korrekturabzug und den Quellkorrektur an, wenn Sie eine neue Version erstellen.

Das Modul gibt die ID der neuen Korrekturabzugs- oder Korrekturabzugsversion zurück. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testversand-Typ]</td> 
   <td> <p>Geben Sie an, ob für den erstellten Korrekturabzug ein einfacher Workflow oder ein automatisierter [!UICONTROL Workflow] verwendet werden soll.</p> <p>Füllen Sie dann die Felder aus, die für den von Ihnen ausgewählten Testversand-Typ angezeigt werden. Wenn Sie beispielsweise [!UICONTROL Automated Workflow] ausgewählt haben, füllen Sie das Feld <strong>[!UICONTROL Workflow-Phasen]</strong> aus, um die Phasen zu konfigurieren.</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ursprüngliche Datei herunterladen zulassen]</td> 
   <td>Wählen Sie aus, ob der Download der Originaldatei, aus der der Korrekturabzug erstellt wurde, zugelassen werden soll.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Classic Proof Viewer]</td> 
   <td>Wählen Sie aus, ob Sie die klassische Korrekturabzugsansicht verwenden.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Alle Dateien in einem Korrekturabzug kombinieren]</td> 
   <td>Aktivieren Sie diese Option, um alle Dateien in einem mehrseitigen Korrekturabzug zu kombinieren.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Neue Korrekturabzugsversion erstellen]</td> 
   <td>Wählen Sie diese Option aus, wenn das Modul eine neue Version eines vorhandenen Korrekturabzugs erstellen soll. Ordnen Sie dann im Feld <strong>[!UICONTROL Existing Proof ID]</strong>, das angezeigt wird, die eindeutige ID des Korrekturabzugs zu oder geben Sie sie ein.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kennzeichnung benutzerdefinierter Links]</td> 
   <td>Geben Sie einen Titel für den benutzerdefinierten Korrekturabzugs-Link ein oder ordnen Sie ihn zu.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL URL für benutzerdefinierten Link]</td> 
   <td>Geben Sie die URL für den benutzerdefinierten Link ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Standard-E-Mail-Benachrichtigungen für Abonnenten]</td> 
   <td>Geben Sie eine der folgenden Zahlen ein, um anzugeben, welche der folgenden standardmäßigen E-Mail-Benachrichtigungseinstellungen Sie für den erstellten Korrekturabzug verwenden möchten.
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
   <td>Wählen Sie aus, ob Sie die Möglichkeit deaktivieren möchten, Korrekturabzugskommentare in eine Excel-Datei herunterzuladen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL PDF deaktivieren]</td> 
   <td>Wählen Sie aus, ob Sie die Möglichkeit deaktivieren möchten, Korrekturabzugskommentare auf eine PDF-Datei herunterzuladen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Abonnement-E-Mail deaktivieren]</td> 
   <td>Wählen Sie aus, ob Sie die Abonnement-E-Mail für diesen Korrekturabzug deaktivieren möchten.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Einbettungs-Player aktivieren]</td> 
   <td>Wählen Sie aus, ob Sie den eingebetteten Player für diesen Korrekturabzug aktivieren möchten.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Abonnements aktivieren]</td> 
   <td>Wählen Sie aus, ob Personen, die nicht Teilnehmer sind, den Testversand abonnieren dürfen.<br>Wenn Sie diese Option auswählen, können Sie auch die Standardrolle für Abonnenten auswählen, wie in dieser Tabelle beschrieben.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Abonnementvalidierung aktivieren]</td> 
   <td>Wählen Sie aus, ob Sie die Validierung von Abonnement-E-Mails aktivieren möchten. Wenn diese Option aktiviert ist, muss der Abonnent auf einen Link in einer E-Mail klicken, um auf einen Korrekturabzug zuzugreifen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Team-URL aktivieren]</td> 
   <td>Wählen Sie aus, ob der erstellte Korrekturabzug die Team-URL ausblenden oder anzeigen soll.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Datei Hash] <span style="font-weight: normal;">oder</span> [!UICONTROL Datei Hashes]</td> 
   <td>Fügen Sie die ID der Datei(en) hinzu, aus der/denen Sie einen Korrekturabzug oder Korrekturabzüge erstellen möchten.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Dateinamen]</td> 
   <td>Dateinamen für den erstellten Korrekturabzug hinzufügen. Dies ist ein Pflichtfeld.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Sperren Sie den Korrekturabzug, wenn alle erforderlichen Entscheidungen getroffen werden]</td> 
   <td>Geben Sie an, ob der Korrekturabzug, der erstellt wird, nach allen erforderlichen Entscheidungen gesperrt werden soll.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Empfänger über diesen Korrekturabzug informieren]</td> 
   <td>Wählen Sie eine Option aus, um anzugeben, ob die Empfänger bei der Erstellung des Korrekturabzugs benachrichtigt werden sollen.&gt;</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Name des Korrekturabzugs]</td> 
   <td>Geben Sie einen Namen für den Korrekturabzug ein, der erstellt wird. Dies ist ein Pflichtfeld. Verwenden Sie ein senkrechtes Strichsymbol (|), um Namen für mehrere Korrekturabzüge zu trennen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Testversand-Besitzer-ID]</td> 
   <td>Geben Sie die ID des Testversand-Inhabers ein oder mappen Sie sie. Wenn dieses Feld leer gelassen wird, wird der/die Verantwortliche für den Korrekturabzug auf den aktuellen Benutzer bzw. die aktuelle Benutzerin festgelegt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Referenz-ID]</td> 
   <td>Geben Sie die Referenz-ID für den Testversand ein.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Elektronische Signatur erforderlich]</td> 
   <td>Wählen Sie aus, ob eine Person, die über einen Korrekturabzug entscheidet, eine elektronische Signatur senden soll.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Anmeldung erforderlich]</td> 
   <td> <p>Geben Sie an, ob für den erstellten Korrekturabzug eine Anmeldung erforderlich sein soll. </p> <p>Dies entspricht der Einstellung von [!UICONTROL Login Required], die unter <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Konfigurieren der Korrekturabzugseinstellungen] in [!DNL Workfront Proof]</a> erläutert wird.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Auflösungs-ID]</td> 
   <td>Geben Sie die ID der Auflösung ein, die Sie für Ihren Korrekturabzug verwenden möchten. Eine Liste der Auflösungs-IDs finden Sie in der [!DNL Workfront Proof] <a href="https://api.proofhq.com/home/objects/soapworkflowproofobject.html">API-Dokumentation</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL SWF]</td> 
   <td>Geben Sie den Typ des SWF-Korrekturabzugs ein.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Anzeigen] [Element]</td> 
   <td>Wählen Sie für jedes Element aus, ob es im Korrekturabzug angezeigt werden soll.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Workspace ID]</td> 
   <td>Geben Sie die ID des Arbeitsbereichs ein, in dem Sie den Korrekturabzug erstellen möchten. </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Empfänger]</td> 
   <td>Fügen Sie die E-Mail-Adressen der Empfänger hinzu, die für den erstellten Korrekturabzug verwendet werden sollen.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Frist]</td> 
   <td> <p>Geben Sie die Frist an, bis zu der der Korrekturabzug erstellt werden soll. Verwenden Sie das folgende Datumsformat:</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Benutzerdefinierter API-Aufruf]

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Workfront Proof]-API durchführen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von den anderen [!DNL Workfront Proof] nicht durchgeführt werden kann.

Das Modul gibt den Status-Code, die Kopfzeilen und den Hauptteil zurück. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL-Methode]</td> 
   <td>Festlegen der Aktion für den API-Aufruf. Informationen zu verfügbaren Aktionen finden Sie in der <a href="https://api.proofhq.com/">Dokumentation zur Korrekturabzugs-API</a>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Hauptteil (XML)]</td> 
   <td> <p>Fügen Sie den Hauptteil des Inhalts für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Wenn Sie bedingte Anweisungen wie <code>if</code> in Ihrer JSON-Datei verwenden, setzen Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
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

Dieses Aktionsmodul lädt die Quelldatei eines bestimmten Korrekturabzugs herunter, den Sie mithilfe seiner ID identifizieren.

Sie geben die ID des Korrekturabzugs an.

Das -Modul gibt den Inhalt der Quelldatei zurück, die zum Erstellen des Korrekturabzugs verwendet wird. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Sie müssen über ausreichende Berechtigungen für den Zugriff auf den Datensatz in [!DNL Workfront Proof] verfügen, um diese Informationen abrufen zu können.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Korrekturabzugs-ID]</td> 
   <td> <p>Geben Sie die eindeutige ID des Korrekturabzugs ein, die auf der Seite [!UICONTROL Korrekturabzugsdetails] zu finden ist. Weitere Informationen finden Sie unter <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Verwalten von Korrekturabzugsdetails in [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datensatz lesen]

Dieses Aktionsmodul liest Daten aus einem einzelnen Korrekturabzug in [!DNL Workfront Proof].

Geben Sie die ID des Korrekturabzugs und die Informationen an, die Sie vom Korrekturabzug erhalten möchten.

Das Modul gibt die Werte der Felder zurück, die Sie für den Testversand auswählen, zusammen mit ihren Typen. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Sie müssen über ausreichende Berechtigungen für den Zugriff auf den Datensatz in [!DNL Workfront Proof] verfügen, um diese Informationen abrufen zu können.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Datensatztyp]</td> 
   <td>Wählen Sie aus, ob Sie einen Korrekturabzug, Kommentare zu Korrekturabzügen oder Prüfer für Korrekturabzüge lesen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabepaket für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ID]</td> 
   <td>Geben Sie die eindeutige [!DNL Workfront Proof]-ID des Datensatzes ein, den das Modul lesen soll, oder mappen Sie sie.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL PDF-Zusammenfassung anfordern]

Dieses Aktionsmodul fordert die PDF-Zusammenfassung für einen bestimmten Korrekturabzug in [!DNL Workfront Proof] an.

Sie geben die ID des Korrekturabzugs an.

Das Modul gibt zusammenfassende PDF-Informationen zurück. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Sie müssen über ausreichende Berechtigungen für den Zugriff auf den Datensatz in [!DNL Workfront Proof] verfügen, um diese Informationen abrufen zu können.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Korrekturabzugs-ID]</td> 
   <td> <p>Geben Sie die eindeutige [!DNL Workfront Proof]-ID des Korrekturabzugs ein, für den Sie eine PDF-Zusammenfassung anfordern möchten.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Callback-URL]</td> 
   <td>Geben Sie die URL ein, an die die PDF-Zusammenfassung gesendet werden soll, oder mappen Sie sie.</td> 
  </tr> 
 </tbody> 
</table>

##### Möglicher Fehler

* **Error**: &quot;[!UICONTROL Sie sind nicht berechtigt, diese Anfrage auszuführen. Die Phase muss mindestens einen Empfänger enthalten.]&quot;
* **Lösung**: Stellen Sie sicher, dass Sie nicht die einzige Person sind, die den Phasen des Workflows zugewiesen ist. Den Phasen des Workflows muss ein anderer Benutzer zugewiesen sein.

#### [!UICONTROL Korrekturabzug aktualisieren]

Dieses Aktionsmodul aktualisiert einen vorhandenen Korrekturabzug in [!DNL Workfront Proof].

Sie geben die ID und den Datensatztyp des Korrekturabzugs an und legen fest, welche Felder in die Ausgabe aufgenommen werden sollen.

Das Modul gibt alle Standardfelder zurück, die mit dem Datensatz verknüpft sind, sowie alle benutzerdefinierten Felder und Werte, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Sie müssen über ausreichende Berechtigungen für den Zugriff auf den Datensatz in [!DNL Workfront Proof] verfügen, um diese Informationen abrufen zu können.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Korrekturabzugs-ID]</td> 
   <td> <p>Geben Sie die eindeutige ID des Korrekturabzugs ein, die auf der Seite [!UICONTROL Korrekturabzugsdetails] zu finden ist. Weitere Informationen finden Sie unter <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md" class="MCXref xref" data-mc-variable-override="">Verwalten von Korrekturabzugsdetails in [!DNL Workfront Proof]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Frist]</td> 
   <td> <p>Geben Sie die Frist an, bis zu der der Korrekturabzug erstellt werden soll. Verwenden Sie das folgende Datumsformat:</p> <p><code>YYYY-MM-DD hh:mm</code></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Standard-E-Mail-Benachrichtigungen für Abonnenten]</td> 
   <td>Wählen Sie aus, welche der folgenden standardmäßigen E-Mail-Benachrichtigungseinstellungen Sie für den erstellten Korrekturabzug verwenden möchten.
    <ul>
     <li> [!UICONTROL Alle neuen Kommentare und Antworten]</li>
     <li>[!UICONTROL antwortet auf meine Kommentare]</li>
     <li>[!UICONTROL Tägliche Zusammenfassung]</li>
     <li> [!UICONTROL Stündliche Zusammenfassung]</li>
     <li> [!Nur UICONTROL-Entscheidungen]</li>
     <li> [!UICONTROL deaktiviert]</li>
    </ul></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Standardrolle]</td> 
   <td>Wählen Sie die Standardrolle für den Korrekturabzug aus.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abonnement-E-Mail deaktivieren]</td> 
   <td>Wählen Sie aus, ob Sie die Abonnement-E-Mail für diesen Korrekturabzug deaktivieren möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abonnements aktivieren]</td> 
   <td>Wählen Sie aus, ob Personen, die nicht Teilnehmer sind, den Testversand abonnieren dürfen.<br>Wenn Sie diese Option auswählen, können Sie auch die [!UICONTROL Standardrolle] für Abonnenten auswählen, wie in dieser Tabelle beschrieben.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abonnementvalidierung aktivieren]</td> 
   <td>Wählen Sie aus, ob Sie die Validierung von Abonnement-E-Mails aktivieren möchten. Wenn diese Option aktiviert ist, muss der Abonnent auf einen Link in einer E-Mail klicken, um auf einen Korrekturabzug zuzugreifen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Team-URL aktivieren]</td> 
   <td>Wählen Sie aus, ob der erstellte Korrekturabzug die Team-URL ausblenden oder anzeigen soll.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sperren Sie den Korrekturabzug, wenn alle erforderlichen Entscheidungen getroffen werden]</td> 
   <td>Geben Sie an, ob der Korrekturabzug, der erstellt wird, nach allen erforderlichen Entscheidungen gesperrt werden soll.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nachricht]</td> 
   <td>Geben Sie eine Nachricht ein, die Sie dem Testversand beifügen möchten, oder mappen Sie sie.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Korrekturabzugs-ID] </td> 
   <td>Geben Sie die ID des Korrekturabzugs ein, den Sie aktualisieren möchten, oder mappen Sie sie.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Korrekturabzug-Name]</td> 
   <td>Geben Sie den Namen des Korrekturabzugs ein, den Sie aktualisieren möchten, oder mappen Sie ihn.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anmeldung erforderlich]</td> 
   <td> <p>Geben Sie an, ob für den erstellten Korrekturabzug eine Anmeldung erforderlich sein soll. </p> <p>Dies entspricht der Einstellung von [!UICONTROL Login Required], die unter <a href="../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">[!UICONTROL Konfigurieren der Korrekturabzugseinstellungen] in [!DNL Workfront Proof]</a> erläutert wird.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Versionen anzeigen wie]</td> 
   <td>Wählen Sie aus, ob ein Link zu anderen Versionen dieses Korrekturabzugs angezeigt werden soll.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Betreff]</td> 
   <td>Betreff des Testversands eingeben oder zuordnen</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Datei hochladen]

Dieses Aktionsmodul lädt eine Datei zur Verwendung mit dem Modul [!UICONTROL Korrekturabzug erstellen] in [!DNL Workfront Proof] hoch.

Das Modul gibt eine Hash-ID für die hochgeladene Datei zurück. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
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
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabepaket für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Vorlagen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suche]

Dieses Suchmodul sucht in einem -Objekt nach Datensätzen, [!DNL Workfront Proof] mit der angegebenen Suchanfrage übereinstimmen.

Das Modul gibt die ID des Korrekturabzugs zurück, wenn es nach einem Korrekturabzug sucht. Oder es gibt die Benutzer-IDs, E-Mails, Namen, Positionen und E-Mail-Aliase der Empfänger zurück, wenn es nach Empfängern sucht. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Sie müssen über ausreichende Berechtigungen für den Zugriff auf den Datensatz in [!DNL Workfront Proof] verfügen, um diese Informationen abrufen zu können.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Suchen nach</td> 
   <td> <p>Legen Sie[!UICONTROL ]fest, wählen Sie den Typ des Datensatzes aus, nach dem das Modul suchen soll.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Korrekturabzug]</strong> </p> <p>Geben Sie den Namen des Korrekturabzugs ein, nach dem Sie suchen möchten.</p> </li> 
     <li> <p><strong>[!UICONTROL recipient]</strong> </p> <p>Geben Sie die E-Mail-Adresse des Empfängers ein, nach dem Sie suchen möchten.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Ergebnissatz]</td> 
   <td>Geben Sie an, ob das Modul nach <strong>[!UICONTROL All Matching Records]</strong> oder nur nach dem <strong>[!UICONTROL First Matching Record]</strong> sucht.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL sortieren nach]</td> 
   <td>Wählen Sie das Feld aus, nach dem Sie die Ergebnisse sortieren möchten.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Sortierrichtung]</td> 
   <td> <p>Wählen Sie aus, ob die Ergebnisse auf- oder absteigend sortiert werden sollen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Workflow-Vorlagen auflisten]

Dieses Suchmodul listet alle verfügbaren Workflow-Vorlagen auf.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Connection]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Workfront Proof]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ausgaben]</td> 
   <td> <p>Wählen Sie die Informationen aus, die im Ausgabepaket für dieses Modul enthalten sein sollen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Vorlagen ein, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll, oder mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>
