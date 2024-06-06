---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 Email
description: In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die Microsoft Office 365 Email verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 29b69e8c-a889-441e-a052-287f1db2052d
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '1974'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Email]

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!UICONTROL Microsoft Office 365 Email], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.

Zur Verwendung [!UICONTROL Office 365 Email] mit [!DNL Adobe Workfront Fusion], muss ein [!UICONTROL Office 365-Konto]. Sie können eine unter www.office.com erstellen.

Anweisungen zum Verbinden der [!UICONTROL Office 365] -Konto [!DNL Workfront Fusion], siehe [Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

Nachdem Sie die Einwilligung erteilt haben, werden Sie zum [!UICONTROL Workfront Fusion] Administrationsseite, auf der Sie Ihr Szenario weiter erstellen können.

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
   <p>Aktuelle Lizenzanforderungen: nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Verwendung [!DNL Microsoft Office 365 Email] -Module, müssen Sie über eine [!DNL Microsoft Office 365 Email] -Konto.



## Verbinden des [!DNL Office 365 Email] Dienst an [!DNL Workfront Fusion]

Anweisungen zum Verbinden der [!DNL Office 365 Email] -Konto [!UICONTROL Workfront Fusion], siehe [Erstellen Sie eine Verbindung zu [!UICONTROL Adobe Workfront Fusion] - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Einige Microsoft-Apps verwenden dieselbe Verbindung, die an individuelle Benutzerberechtigungen gebunden ist. Daher werden beim Erstellen einer Verbindung im Bildschirm für die Genehmigung von Berechtigungen alle Berechtigungen angezeigt, die zuvor für die Verbindung dieses Benutzers gewährt wurden, zusätzlich zu den neuen Berechtigungen, die für die aktuelle Anwendung erforderlich sind.
>
>Wenn beispielsweise ein Benutzer über den Excel-Connector über die Berechtigung &quot;Tabelle lesen&quot;verfügt und dann im Outlook-Connector eine Verbindung zum Lesen von E-Mails erstellt, zeigt der Bildschirm für die Genehmigung der Berechtigungen sowohl die bereits erteilte Berechtigung &quot;Tabelle lesen&quot;als auch die neu erforderliche Berechtigung &quot;E-Mail schreiben&quot;an.

## [!DNL Microsoft Office 365 Email] Module und ihre Felder

Bei der Konfiguration [!DNL Microsoft Office 365 Email] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Microsoft Office 365 Email] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Nachricht](#message)
* [Entwurfsnachricht](#draft-message)
* [Anhang](#attachment)
* [Sonstige](#other)

### Nachricht

* [[!UICONTROL Nachrichten ansehen]](#watch-messages)
* [[!UICONTROL Suchmeldungen]](#search-messages)
* [[!UICONTROL Nachricht abrufen]](#get-a-message)
* [[!UICONTROL Erstellen und Senden einer Nachricht]](#create-and-send-a-message)
* [[!UICONTROL Nachricht verschieben]](#move-a-message)
* [[!UICONTROL Nachricht löschen]](#delete-a-message)

#### [!UICONTROL Nachrichten ansehen]

Trigger, in denen eine neue E-Mail-Nachricht gesendet oder empfangen wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] -Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nachrichten ansehen]</p> </td> 
   <td> <p>Wählen Sie die zu überwachenden Nachrichten aus:</p> 
    <ul> 
     <li>[!UICONTROL Only Unread]</li> 
     <li>[!UICONTROL Only read]</li> 
     <li>[!UICONTROL All]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail-Ordner]</td> 
   <td> <p>Wählen Sie den Ordner aus, der die zu überwachenden Nachrichten enthält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suche]</td> 
   <td>Geben Sie Ihre Suchabfrage ein. Informationen zum Schreiben einer Suchabfrage finden Sie unter [!DNL Microsoft] Support-Artikel <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Search Mail and People in [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Maximale Nachrichtenanzahl eingeben [!DNL Workfront Fusion] sollte während eines Szenario-Ausführungszyklus zurückgegeben werden.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suchmeldungen]

Sucht nach Nachrichten basierend auf bestimmten Kriterien.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] -Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail-Ordner]</td> 
   <td> <p>Wählen Sie den Ordner aus, der die zu suchenden Nachrichten enthält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Suche]</td> 
   <td>Geben Sie Ihre Suchabfrage ein. Informationen zum Schreiben einer Suchabfrage finden Sie unter [!DNL Microsoft] Support-Artikel <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">Search Mail and People in [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reihenfolge nach]</td> 
   <td> <p>Wählen Sie aus, wie die Ergebnisse sortiert werden sollen:</p> 
    <ul> 
     <li>[!UICONTROL Subject (aufsteigend oder absteigend)]</li> 
     <li>[!UICONTROL Erstellungszeitpunkt (aufsteigend oder absteigend)]</li> 
     <li>[!UICONTROL Last Modified Date Time (aufsteigend oder absteigend)]</li> 
     <li>[!UICONTROL Empfangsdatumszeit (aufsteigend oder absteigend)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Maximale Nachrichtenanzahl eingeben [!DNL Workfront Fusion] sollte während eines Szenario-Ausführungszyklus zurückgegeben werden.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Nachricht abrufen]

Ruft die Metadaten einer bestimmten Nachricht ab

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] -Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nachrichten-ID]</td> 
   <td> <p> Wählen Sie die ID der Nachricht aus, für die Sie Metadaten abrufen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL MIME-Inhalte abrufen]</td> 
   <td>Aktivieren Sie diese Option, um Daten zum MIME-Inhalt der Nachricht abzurufen. [!UICONTROL MIME]-Inhalte können Bilder, Audio, Video oder andere Dateitypen umfassen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen und Senden einer Nachricht]

Erstellt und sendet eine E-Mail-Nachricht.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] -Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Betreff]</td> 
   <td> <p>Geben Sie die Betreffzeile der Nachricht ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Textinhalt]</td> 
   <td>Wählen Sie aus, ob der Hauptteilinhalt der Nachricht HTML oder Text ist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Textkörper]</td> 
   <td> <p>Geben Sie den Nachrichtentext der E-Mail ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Wichtigkeit]</td> 
   <td> <p>E-Mail-Wichtigkeit auswählen</p> 
    <ul> 
     <li>[!UICONTROL Niedrig]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Hoch]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Für Empfänger]</p> </td> 
   <td> <p>Fügen Sie die E-Mail-Adresse hinzu, an die Sie die Nachrichten senden möchten:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Geben Sie den Namen des Kontakts ein</p> </li> 
     <li> <p><strong>[!UICONTROL E-Mail-Adresse]</strong> </p> <p>Geben Sie die E-Mail-Adresse des Kontakts ein.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Empfänger]</p> </td> 
   <td> <p>Fügen Sie die Empfänger hinzu, die eine Kopie der Nachricht erhalten sollen:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Geben Sie den Namen des Kontakts ein</p> </li> 
     <li> <p><strong>[!UICONTROL E-Mail-Adresse]</strong> </p> <p>Geben Sie die E-Mail-Adresse des Kontakts ein.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bcc Empfänger]</p> </td> 
   <td> <p>Fügen Sie die Empfänger hinzu, die Sie in die Nachricht kopieren möchten, ohne dass andere Empfänger ihre Namen oder E-Mail-Adressen sehen können:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Geben Sie den Namen des Kontakts ein</p> </li> 
     <li> <p><strong>[!UICONTROL E-Mail-Adresse]</strong> </p> <p>Geben Sie die E-Mail-Adresse des Kontakts ein.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Fügen Sie die Anlagen zur E-Mail hinzu:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Dateiname]</strong> </p> <p>Geben Sie den Dateinamen ein. Beispiel: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Daten]</strong> </p> <p>Geben Sie die Dateidaten in das Feld ein oder ordnen Sie die Quelle der Datei zu.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Internet Message Headers]</td> 
   <td> <p>Fügen Sie die Kopfzeilen für die E-Mail hinzu.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Geben Sie den Namen der Kopfzeile ein.</p> </li> 
     <li> <p><strong>[!UICONTROL E-Mail-Adresse]</strong> </p> <p>Geben Sie einen Wert für die Kopfzeile ein.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Nachricht verschieben]

Verschiebt eine E-Mail-Nachricht in einen ausgewählten Ordner im Postfach.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] -Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nachrichten-ID]</td> 
   <td> <p> Wählen Sie die Kennung der Nachricht aus, die Sie in einen anderen Ordner verschieben möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail-Ordner] </td> 
   <td> <p>Wählen Sie die Kennung des Ordners aus, in den Sie die Nachricht verschieben möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Nachricht löschen]

Löscht eine vorhandene E-Mail-Nachricht.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] -Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nachrichten-ID]</td> 
   <td> <p> Wählen Sie die Kennung der Nachricht aus, die Sie löschen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Entwurfsnachricht

* [Nachrichtenentwurf erstellen](#create-a-draft-message)
* [Nachrichtenentwurf senden](#send-a-draft-message)
* [Nachricht aktualisieren](#update-a-message)

#### [!UICONTROL Nachrichtenentwurf erstellen]

Erstellt eine neue E-Mail-Nachricht.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] -Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Betreff]</td> 
   <td> <p>Geben Sie die Betreffzeile der Nachricht ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Textinhalt]</td> 
   <td>Wählen Sie aus, ob der Hauptteilinhalt der Nachricht HTML oder Text ist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Textkörper]</td> 
   <td> <p>Geben Sie den Nachrichtentext der E-Mail ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Wichtigkeit]</td> 
   <td> <p>E-Mail-Wichtigkeit auswählen</p> 
    <ul> 
     <li>[!UICONTROL Niedrig]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Hoch]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Für Empfänger]</p> </td> 
   <td> <p>Fügen Sie die Empfänger hinzu, an die Sie die Nachrichten senden möchten:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Geben Sie den Namen des Kontakts ein</p> </li> 
     <li> <p><strong>[!UICONTROL E-Mail-Adresse]</strong> </p> <p>Geben Sie die E-Mail-Adresse des Kontakts ein.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Empfänger]</p> </td> 
   <td> <p>Empfänger hinzufügen Der Empfänger, der eine Kopie der Nachricht erhalten soll:</p> 
    <ul> 
     <li> <p><strong>Name</strong> </p> <p>Geben Sie den Namen des Kontakts ein</p> </li> 
     <li> <p><strong>Email-Adresse</strong> </p> <p>Geben Sie die E-Mail-Adresse des Kontakts ein.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>BCC-Empfänger</p> </td> 
   <td> <p>Fügen Sie die Empfänger hinzu, die Sie in die Nachricht kopieren möchten, ohne dass andere Empfänger ihre Namen oder E-Mail-Adressen sehen können:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Geben Sie den Namen des Kontakts ein</p> </li> 
     <li> <p><strong>[!UICONTROL E-Mail-Adresse]</strong> </p> <p>Geben Sie die E-Mail-Adresse des Kontakts ein.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Fügen Sie die Anlagen zur E-Mail hinzu:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Dateiname]</strong> </p> <p>Geben Sie den Dateinamen ein. Beispiel: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Daten]</strong> </p> <p>Geben Sie die Dateidaten in das Feld ein oder ordnen Sie die Quelle der Datei zu.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Nachrichtenentwurf senden]

Sendet eine E-Mail-Nachricht, die sich derzeit im Entwurf befindet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] -Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entwurfs-Nachrichten-ID]</td> 
   <td> <p> Wählen Sie die Nachrichten-ID des Entwurfs aus oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Nachricht aktualisieren]

Aktualisiert eine vorhandene Nachricht.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] -Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nachrichten-ID eingeben]</td> 
   <td> <p>Wählen Sie aus, wie Sie die zu aktualisierende Nachricht identifizieren möchten:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Manuell eingeben]</strong> </p> <p>Geben Sie die Nachrichten-ID ein oder ordnen Sie sie zu.</p> </li> 
     <li> <p><strong>[!UICONTROL Aus Liste auswählen]</strong> </p> <p>Wählen Sie den Ordner aus, der die zu aktualisierende Nachricht enthält, und wählen Sie dann die Nachricht aus</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Betreff]</td> 
   <td> <p>Geben Sie die Betreffzeile der Nachricht ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Textkörper]</td> 
   <td> <p>Geben Sie den Nachrichtentext der E-Mail ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Wichtigkeit]</td> 
   <td> <p>E-Mail-Wichtigkeit auswählen</p> 
    <ul> 
     <li>[!UICONTROL Niedrig]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Hoch]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Für Empfänger]</p> </td> 
   <td> <p>Fügen Sie die E-Mail-Adresse hinzu, an die Sie die Nachrichten senden möchten:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Geben Sie den Namen des Kontakts ein</p> </li> 
     <li> <p><strong>[!UICONTROL E-Mail-Adresse]</strong> </p> <p>Geben Sie die E-Mail-Adresse des Kontakts ein.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Empfänger]</p> </td> 
   <td> <p>Empfänger hinzufügen Der Empfänger, der eine Kopie der Nachricht erhalten soll:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Geben Sie den Namen des Kontakts ein</p> </li> 
     <li> <p><strong>[!UICONTROL E-Mail-Adresse]</strong> </p> <p>Geben Sie die E-Mail-Adresse des Kontakts ein.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bcc Empfänger]</p> </td> 
   <td> <p>Fügen Sie die Empfänger hinzu, die Sie in die Nachricht kopieren möchten, ohne dass andere Empfänger ihre Namen oder E-Mail-Adressen sehen können:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Geben Sie den Namen des Kontakts ein</p> </li> 
     <li> <p><strong>[!UICONTROL E-Mail-Adresse]</strong> </p> <p>Geben Sie die E-Mail-Adresse des Kontakts ein.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Fügen Sie die Anlagen zur E-Mail hinzu:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Dateiname]</strong> </p> <p>Geben Sie den Dateinamen ein. Beispiel: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Daten]</strong> </p> <p>Geben Sie die Dateidaten in das Feld ein oder ordnen Sie die Quelle der Datei zu.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Markieren Sie es als gelesen .</td> 
   <td>Aktivieren Sie diese Option, um die aktualisierte Nachricht als gelesen zu markieren.</td> 
  </tr> 
 </tbody> 
</table>

### Anhang

* [[!UICONTROL Listen-Anhänge]](#list-attachments)
* [[!UICONTROL Herunterladen eines Anhangs]](#download-an-attachment)

#### [!UICONTROL Listen-Anhänge]

Dieses Modul ruft eine Liste von Anlagen ab, die zur angegebenen Nachricht gehören.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] -Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nachrichten-ID]</td> 
   <td> <p> Wählen Sie die ID der Nachricht aus, aus der Sie Anlagen abrufen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Anlagen ein oder ordnen Sie sie zu, die das Modul während jedes Szenario-Ausführungszyklus zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Herunterladen eines Anhangs]

Dieses Modul lädt den angegebenen Anhang herunter.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] -Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nachrichten-ID]</td> 
   <td> <p> Wählen Sie die Kennung der Nachricht aus, die den herunterzuladenden Anhang enthält, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Attachment ID]</td> 
   <td> <p>Geben Sie die Kennung des Anhangs ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Sonstige

* [[!UICONTROL API-Aufruf durchführen]](#make-an-api-call)
* [[!UICONTROL Anlage hinzufügen]](#add-an-attachment)

#### [!UICONTROL API-Aufruf durchführen]

Mit diesem Modul können Sie einen benutzerdefinierten API-Aufruf ausführen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] -Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Geben Sie einen Pfad relativ zu ein <code>https://graph.microsoft.com</code>. Beispiel:<code> /v1.0/me/messages</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Methode]</p> </td> 
   td&gt; <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anforderung in Form eines standardmäßigen JSON-Objekts hinzu. Beispiel: <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p> Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Anlage hinzufügen]

Dieses Modul fügt einer Nachricht eine große Anlage hinzu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Office 365] -Konto [!DNL Workfront Fusion], siehe <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nachrichten-ID]</td> 
   <td> <p> Wählen Sie die Kennung der Nachricht aus, der Sie einen Anhang hinzufügen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quelldatei]</td> 
   <td> <p>Wählen Sie eine Datei aus einem vorherigen Modul aus oder ordnen Sie den Namen und die Daten der Quelldatei zu.</p> </td> 
  </tr> 
 </tbody> 
</table>
