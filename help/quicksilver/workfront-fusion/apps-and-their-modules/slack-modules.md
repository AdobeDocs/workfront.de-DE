---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Slack-Module
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die Slack verwenden, und sie mit mehreren Drittanbieteranwendungen und -diensten verbinden.
author: Becky
feature: Workfront Fusion
exl-id: ba5bad6a-3cb3-4024-82f7-d38ee9a8e0b5
source-git-commit: 27fb07b7b19bab25bb7ee925e722ccace3bea628
workflow-type: tm+mt
source-wordcount: '1761'
ht-degree: 1%

---

# [!DNL Slack] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Slack] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

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

Um [!DNL Slack] -Module zu verwenden, müssen Sie über ein [!DNL Slack] -Konto verfügen.

## Slack-API-Informationen

Der Slack-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td>{{ifempty(parameters.domain, 'https://slack.com/api/'}}</td> 
  </tr>
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v4.0.15</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Slack] Module und ihre Felder

Wenn Sie [!DNL Slack] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Slack] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Nachrichten](#messages)
* [Dateien](#files)
* [Kanäle](#channels)
* [Reaktionen](#reactions)
* [Sterne](#stars)
* [Gespeicherte Elemente](#saved-items)
* [Nadeln](#pins)
* [Benutzende](#users)
* [Erinnerungen](#reminders)
* [Veranstaltungen](#events)
* [Profil](#profile)
* [Sonstige](#other)

### Nachrichten

+++**[!UICONTROL Anzeigen öffentlicher Kanalmeldungen]**

Dieses Trigger-Modul startet das Szenario, wenn einem öffentlichen Kanal eine neue Nachricht hinzugefügt wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Slack]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kanal] </td> 
   <td> <p>Wählen Sie den öffentlichen Kanal aus, den Sie für neue Nachrichten überwachen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Legen Sie die maximale Anzahl von Nachrichten fest, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgibt.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL Private Kanal-Nachrichten ansehen]**

Dieses Trigger-Modul startet das Szenario, wenn einem privaten Kanal (Gruppe) eine neue Nachricht hinzugefügt wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Slack]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kanal] </td> 
   <td> <p>Wählen Sie den privaten Kanal aus, den Sie auf neue Nachrichten überwachen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Legen Sie die maximale Anzahl von Nachrichten fest, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgibt.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

<!--

+++ **[!UICONTROL Watch Direct Messages]**

This trigger module starts the scenario when a new message is added to a direct message.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel] </td> 
   <td> <p>Select the direct message conversation you want to watch for new messages.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Set the maximum number of messages [!DNL Workfront Fusion] will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Watch Multiparty Direct Messages]**

This trigger module starts the scenario when a new message is added to a multiparty direct message channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel] </td> 
   <td> <p>Select the direct message conversation you want to watch for new messages.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Set the maximum number of messages [!DNL Workfront Fusion] will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Search for Message]**

This search module returns messages matching a search query.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td> <p>Enter the query that you want to search by. </p> <p>For information on creating formulas from the mapping panel, see <a href="../../workfront-fusion/functions/map-using-functions.md" class="MCXref xref">Map items using functions in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Set the maximum number of messages [!DNL Workfront Fusion] will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

-->

+++ **[!UICONTROL Abrufen einer privaten Kanalmeldung]**

Dieses Aktionsmodul ruft die Details einer Nachricht von einem ausgewählten Kanal ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Slack]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Kanal-ID]</p> </td> 
   <td> <p>Geben Sie die Kanal-ID ein (zuordnen).</p> <p>Hinweis: Die Kanal-ID kann mithilfe des Moduls [!UICONTROL List Channels] abgerufen werden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nachrichten-ID (Zeitstempel)]</p> </td> 
   <td> <p> Geben Sie den Zeitstempel der Nachricht ein oder ordnen Sie ihn zu, über die Informationen abgerufen werden sollen.</p> <p>Hinweis: Der Zeitstempel kann mithilfe eines anderen Moduls wie dem Modul [!UICONTROL Public Channel] abgerufen werden.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Öffentlichen Kanal abrufen]**

Dieses Aktionsmodul gibt eine Nachricht mit einer angegebenen ID aus einem angegebenen öffentlichen Kanal zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Slack]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Kanal-ID]</p> </td> 
   <td> <p>Geben Sie die Kanal-ID ein oder ordnen Sie sie zu.</p> <p>Hinweis: Die Kanal-ID kann mithilfe des Moduls [!UICONTROL List Channels] abgerufen werden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nachrichten-ID (Zeitstempel)]</td> 
   <td> <p> Geben Sie den Zeitstempel der Nachricht ein oder ordnen Sie ihn zu, über die Informationen abgerufen werden sollen.</p> <p>Hinweis: Der Zeitstempel kann mithilfe eines anderen Moduls wie dem Modul [!UICONTROL Public Channel] abgerufen werden.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

<!--

+++ **[!UICONTROL List replies]**

This action module retrieves a thread of messages posted to a conversation.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that contains the message that you want to retrieve replies for, then select the channel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parent message ID (Time stamp)]</td> 
   <td> <p> Enter or map the message time stamp of the message you want to retrieve replies for.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Public Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of replies you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

-->

+++ **[!UICONTROL Erstellen einer Nachricht]**

Dieses Aktionsmodul erstellt eine neue Nachricht.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Slack]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Kanalkennung oder Namen eingeben]</p> </td> 
   <td> <p>Wählen Sie aus, wie Sie den Kanal auswählen möchten, in dem Sie eine Nachricht erstellen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie im Feld <strong>[!UICONTROL Channel ID or name]</strong> die Kanal-ID oder den Namen des Kanals ein, in dem die Nachricht gepostet werden soll, oder ordnen Sie sie zu.</p> <p>Hinweis: Die Kanal-ID kann mithilfe des Moduls [!UICONTROL List Channels] abgerufen werden.</p> </li> 
     <li> <p><strong>[!UICONTROL Auswahl aus der Liste]</strong> </p> <p>Wählen Sie den Typ des Kanals und dann den Kanal aus.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Text]</p> </td> 
   <td> <p>Geben Sie den Textinhalt der Nachricht ein, die Sie erstellen möchten.</p> <p>Hinweis: Detaillierte Informationen zur Textformatierung finden Sie unter <a href="https://api.slack.com/reference/surfaces/formatting">Formatieren von Text für App-Oberflächen</a> in der Dokumentation zu [!DNL Slack].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Blöcke]</td> 
   <td>Blöcke sind wiederverwendbare Komponenten, mit denen Sie Ihre Nachrichten anpassen und organisieren können. Weitere Informationen zu Bausteinen finden Sie unter <a href="https://api.slack.com/block-kit">Block Kit</a> in der Dokumentation zu [!DNL Slack].</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Thread message ID (Zeitstempel)]</td> 
   <td>Wenn es sich bei der neuen Nachricht um eine Antwort handelt, geben Sie den Zeitstempel der Nachricht ein, auf die Sie antworten möchten. Geben Sie nicht den Zeitstempel einer Nachricht ein, bei der es sich bereits um eine Antwort handelt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reply Broadcast]</td> 
   <td> <p>Wählen Sie <strong>[!UICONTROL Yes]</strong> aus, wenn beide der folgenden Bedingungen zutreffen:</p> 
    <ul> 
     <li> <p>Die neue Nachricht ist eine Antwort auf eine andere Nachricht.</p> </li> 
     <li> <p>Sie möchten, dass die neue Nachricht für alle Benutzer im Kanal sichtbar ist.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Linknamen]</p> </td> 
   <td> <p>Aktivieren Sie diese Option, damit Namen und Kanäle das Format <code>@username</code> oder <code>#channel</code> verwenden können. </p> <p>Weitere Informationen finden Sie unter <a href="https://api.slack.com/docs/formatting">Text für Anwendungsoberflächen formatieren</a> in der Dokumentation zu [!DNL Slack].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Parse message text]</p> </td> 
   <td> <p>Aktivieren Sie diese Option, um das automatische Parsen zu ermöglichen. </p> <p>Weitere Informationen finden Sie unter <a href="https://api.slack.com/docs/formatting">Text für Anwendungsoberflächen formatieren</a> in der Dokumentation zu [!DNL Slack].</p> <p>Hinweis: Wenn Sie die Optionen [!UICONTROL Linknamen] oder [!UICONTROL Nachrichtentext analysieren] in der ursprünglichen Nachricht verwendet haben, sollten Sie diese auch bei der Ausführung des Moduls [!UICONTROL Nachricht aktualisieren] angeben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Markdown verwenden]</p> </td> 
   <td> <p>Aktivieren Sie diese Option, damit [!DNL Slack] Markdown im Text verwenden kann.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Vorwiegend textbasierter Inhalt]</p> </td> 
   <td> <p>Aktivieren Sie diese Option, um das Entsperren primär textbasierter Inhalte zu ermöglichen. </p> <p>Weitere Informationen zum Entschärfen in [!DNL Slack] finden Sie unter <a href="https://api.slack.com/reference/messaging/link-unfurling">Entschärfen von Links in Nachrichten</a> in der Dokumentation zu [!DNL Slack].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Unfurl media content]</p> </td> 
   <td> <p>Aktivieren Sie diese Option, um das Entsperren von Medieninhalten zu ermöglichen. </p> <p>Weitere Informationen zum Entschärfen in [!DNL Slack] finden Sie unter <a href="https://api.slack.com/reference/messaging/link-unfurling">Entschärfen von Links in Nachrichten</a> in der Dokumentation zu [!DNL Slack].</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Aktualisieren einer Nachricht]**

Mit diesem Aktionsmodul können Sie eine vorhandene Nachricht bearbeiten.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Slack]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Kanalkennung oder Namen eingeben]</p> </td> 
   <td> <p>Wählen Sie aus, wie Sie die Nachricht auswählen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL manuell eingeben]</strong> </p> <p>Geben Sie im Feld <strong>[!UICONTROL Channel ID or name]</strong> die Kanal-ID oder den Kanal, der die Nachricht enthält, ein oder ordnen Sie sie zu und geben Sie dann den <strong>[!UICONTROL Zeitstempel (Nachrichten-ID)]</strong> der Nachricht ein. .</p> <p>Hinweis: Die Kanal-ID kann mithilfe des Moduls [!UICONTROL List Channels] abgerufen werden.</p> </li> 
     <li> <p><strong>[!UICONTROL Auswahl aus der Liste]</strong> </p> <p>Wählen Sie den Typ des Kanals aus, wählen Sie dann den Kanal aus und wählen Sie dann die Nachricht aus.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Text]</p> </td> 
   <td> <p>Geben Sie den neuen Textinhalt der Nachricht ein, die Sie aktualisieren möchten.</p> <p>Weitere Informationen finden Sie unter <a href="https://api.slack.com/docs/formatting">Text für Anwendungsoberflächen formatieren</a> in der Dokumentation zu [!DNL Slack].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Blöcke]</td> 
   <td>Blöcke sind wiederverwendbare Komponenten, mit denen Sie Ihre Nachrichten anpassen und organisieren können. Weitere Informationen zu Bausteinen finden Sie unter <a href="https://api.slack.com/block-kit">Block Kit</a> in der Dokumentation zu [!DNL Slack].</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Linknamen]</p> </td> 
   <td> <p>Aktivieren Sie diese Option, damit Namen und Kanäle das Format <code>@username</code> oder <code>#channel</code> verwenden können. </p> <p>Weitere Informationen finden Sie unter <a href="https://api.slack.com/docs/formatting">Text für Anwendungsoberflächen formatieren</a> in der Dokumentation zu [!DNL Slack].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Parse message text]</p> </td> 
   <td> <p>Aktivieren Sie diese Option, um das automatische Parsen zu ermöglichen. </p> <p> Weitere Informationen finden Sie unter <a href="https://api.slack.com/docs/formatting">Text für Anwendungsoberflächen formatieren</a> in der Dokumentation zu [!DNL Slack].</p> <p>Hinweis: Wenn Sie die Optionen [!UICONTROL Linknamen] oder [!UICONTROL Nachrichtentext analysieren] in der ursprünglichen Nachricht verwendet haben, sollten Sie sie auch bei der Ausführung des Moduls Nachricht aktualisieren angeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Eine Nachricht löschen]**

Dieses Aktionsmodul löscht eine bestimmte Nachricht.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Slack]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Kanal-ID]</p> </td> 
   <td> <p>Geben Sie die Kanal-ID ein oder ordnen Sie sie zu.</p> <p>Hinweis: Die Kanal-ID kann mithilfe des Moduls [!UICONTROL List Channels] abgerufen werden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nachrichten-ID]</td> 
   <td> <p> Geben Sie den Zeitstempel der Nachricht ein, die Sie löschen möchten, oder ordnen Sie ihn zu.</p> <p>Hinweis: Der Zeitstempel kann mit einem anderen Modul abgerufen werden, z. B. dem Modul "Privater Kanal überwachen".</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

<!--

### Files 

+++ **[!UICONTROL Watch Files]**

This trigger module starts a scenario when a new file is added.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Select the type of file that you want the module to watch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td> <p>Select the type of channel you want to watch for files, then select the channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Enter or map the maximum number of files you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL List Files]**

This action module returns a list of files based on the specified filter.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type] </td> 
   <td> <p>Select the type(s) of files you want to retrieve.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Channel type]</p> </td> 
   <td> <p>Select the type of channel representing the channel that you want to list files from, then select the channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Created by]</td> 
   <td> <p>Select a user to return only files created by that user.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Date from]</td> 
   <td>Enter the earliest date that you want to return files from. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Type coercion in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Date to]</td> 
   <td>Enter the latest date that you want to return files from. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Type coercion in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Enter or map the maximum number of files you want the module to return during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Get a File]**

This action module returns details about the specified file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td> <p>Enter or map the ID of the file that you want to retrieve. </p> <p>Note: The file ID can be retrieved using another module, such as the [!DNL Watch Files] Module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Download a File]**

This action module downloads a file from a URL. It must follow the [!UICONTROL Slack] >[!UICONTROL Get a File] module in a scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL private download]</td> 
   <td> <p>Map the <b>[!UICONTROL URL Private download]</b> value from the [!DNL Slack] >[!UICONTROL Get a File] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Upload a File]**

This action module creates or uploads a file to [!DNL Slack]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channels]</td> 
   <td> <p>For each channel you want to upload the file to, click <b>[!UICONTROL Add item]</b>, then select the channel type and channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>Enter a title for the file you want to upload</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Thread ID (timestamp)]</td> 
   <td> <p>If you are uploading the file as a reply, enter or map the time stamp of the message you want to reply to.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Initial Comment]</td> 
   <td> <p>Enter or map the text of the message that introduces the file.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Create a Text File]**

This action module creates a text file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channels]</td> 
   <td> <p>For each channel you want to upload the file to, click <b>[!UICONTROL Add item]</b>, then select the channel type and channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>Enter a title for the file you want to upload</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Thread ID (timestamp)]</td> 
   <td> <p>If you are uploading the file as a reply, enter or map the time stamp of the message you want to reply to.</p> <p>Note: The time stamp can be retrieved using another module, such as the[!UICONTROL  Watch Private Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Initial Comment]</td> 
   <td> <p>Enter or map the text of the message that introduces the file.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Delete a File]**

This action module returns deletes the specified file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td> <p>Enter or map the ID of the file that you want to delete. </p> <p>Note: The file ID can be retrieved using another module, such as the [!DNL Watch Files] Module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

-->

### Kanäle

+++ **[!UICONTROL Auflistungskanäle]**

Dieses Suchmodul gibt eine Liste aller Kanäle in einem Arbeitsbereich zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Slack]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Archiv ausschließen]</p> </td> 
   <td> <p>Wählen Sie [!UICONTROL Ja] aus, um archivierte Kanäle aus den Ergebnissen auszuschließen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Typ] </td> 
   <td> <p>Wählen Sie die Kanäle aus, die Sie abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Legen Sie die maximale Anzahl von Kanälen fest, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgibt.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Einen Kanal abrufen]**

Dieses Aktionsmodul gibt Informationen zu einem Workspace-Kanal zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Slack]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Kanal-ID]</p> </td> 
   <td> <p>Geben Sie die Kennung des Kanals ein oder ordnen Sie ihn zu, über den Sie Informationen abrufen möchten.</p> <p>Hinweis: Die Kanal-ID kann mithilfe des Moduls [!UICONTROL List Channels] abgerufen werden.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Listenmitglieder im Kanal]**

Dieses Suchmodul gibt eine Liste der Benutzer im ausgewählten Kanal zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Slack]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kanaltyp]</td> 
   <td>Wählen Sie den Kanal aus, der die Liste der Mitglieder enthält, die Sie auflisten möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private Channel]</td> 
   <td>Wählen Sie den Kanal aus, für den Sie Mitglieder auflisten möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Legen Sie die maximale Anzahl von Mitgliedern fest, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgibt.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

<!--

+++ **[!UICONTROL Set the Topic of a Channel]**

This action module changes the topic of a channel

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to change the topic for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM Channel] / [!UICONTROL User]</td> 
   <td>Select the channel or user that you want to change the topic for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Topic]</td> 
   <td>Enter or map the new topic of the channel. This field does not support formatting or links.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Set the Purpose of a Channel]**

This action module changes the purpose of a channel

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to change the purpose for.</td> 
  </tr> 
  <tr> 
>[!MORELIKETHIS]
>
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM Channel] / User</td> 

   <td>Select the channel or user that you want to change the purpose for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Purpose]</td> 
   <td>Enter or map the new purpose of the channel. This field does not support formatting or links.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Join a Channel]**

This action module joins the user to a channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Channel ID]</p> </td> 
   <td> <p>Enter or map the ID of the channel that you want to join.</p> <p>Note: The Channel ID can be retrieved using the [!UICONTROL List Channels] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Leave a Channel]**

This action module removes the user from a channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Channel ID]</p> </td> 
   <td> <p>Enter or map the ID of the channel that you want to leave.</p> <p>Note: The Channel ID can be retrieved using the [!UICONTROL List Channels] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Create a Channel]**

This action module creates a new channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
   <td> <p>Enter or map a name for the new channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Is private]</td> 
   <td>Enable this option to set the new channel as private.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Archive a Channel]**

This action module archives a  channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Channel ID]</p> </td> 
   <td> <p>Enter or map the ID of the channel that you want to archive.</p> <p>Note: The Channel ID can be retrieved using the [!UICONTROL List Channels] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Unarchive a Channel]**

This action module unarchives a channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Channel ID]</p> </td> 
   <td> <p>Enter or map the ID of the channel that you want to unarchive.</p> <p>Note: The Channel ID can be retrieved using the [!UICONTROL List Channels] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Reactions

+++ **[!UICONTROL List reactions]**

This action module returns reactions that a user made.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL User]</p> </td> 
   <td> <p>Select the user that made the reactions that you want to list.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of reactions you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Add a reaction]**

This action module adds a reaction to an item.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to add a reaction to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM channel] / [!UICONTROL User]</td> 
   <td>Select the channel or user that you want to add a reaction to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Enter or map the time stamp of the message you want to add a reaction to.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reaction (emoji) name]</td> 
   <td>Enter or map the name of the emoji that you want to use for a reaction. Example: <code>thumbsup</code>. </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Remove a reaction]**

This action module adds a reaction to an item.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to remove a reaction from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM channel] / [!UICONTROL User]</td> 
   <td>Select the channel or user that you want to add a reaction from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Enter or map the time stamp of the message you want to add a reaction to.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reaction (emoji) name]</td> 
   <td>Enter or map the name of the emoji that you want to remove from the message. Example: <code>thumbsup</code>. </td> 
  </tr> 
 </tbody> 
</table>

+++

### Stars 

+++ **[!UICONTROL Add a star]**

This action module makes a channel a starred channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to add a star to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL IM] / [!UICONTROL Multiple IM channel]</td> 
   <td>Select the channel or user that you want to add a star to.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Remove a star]**

This action module removed the star from a starred channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to add a star to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL IM] / [!UICONTROL Multiple IM channel]</td> 
   <td>Select the channel or user that you want to add a star to.</td> 
  </tr> 
 </tbody> 
</table>

+++

### Saved Items

+++ **[!UICONTROL Save an Item]**

This action module adds an item to saved items.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID (Time stamp)]</td> 
   <td> <p> Enter or map the time stamp of the message you want to save.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td> <p>Enter or map the file that you want to save.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Remove Saved Item]**

This action module adds an item to saved items.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID (Time stamp)]</td> 
   <td> <p> Enter or map the time stamp of the message you want to remove from saved items.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td> <p>Enter or map the file you want to remove from saved items.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Pins

+++ **[!UICONTROL Pin an Item]**

This action module pins an item, such as a file or file comment, to a channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to pin an item to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM channel] / [!UICONTROL User]</td> 
   <td>Select the channel or user that you want to pin an item to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Enter or map the time stamp of the message you want to pin.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Unpin an Item]**

This action module unpins an item from a channel. You can unpin files, file comments, channel messages, or group messages.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to unpin an item from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM channel] / [!UICONTROL User]</td> 
   <td>Select the channel or user that you want to unpin an item from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Enter or map the time stamp of the message you want to unpin.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Users 

+++ **[!UICONTROL Watch Users]**

This trigger module starts the scenario when a new user is added to the [!DNL Slack] workspace.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Set the maximum number of users [!DNL Workfront Fusion] will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Search for User]**

This action module retrieves details about a single user, by using their email address.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Email] </p> </td> 
   <td> <p>Enter or map the email address of the user you want to retrieve details about.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL List Users]**

This action module returns a list of all users in a workspace.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Limit]</p> </td> 
   <td> <p>Enter or map the maximum number of users you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Get a User]**

This action module retrieves details about a member of a workspace.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL User ID]</p> </td> 
   <td> <p>Enter or map the User ID of the user you want to retrieve details for.</p> <p>Note: The User ID can be retrieved using another module, such as the [!DNL List Users] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Invite Users]**

This action module invites 1-30 users to a public or private channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want invite users to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM channel] / [!UICONTROL User]</td> 
   <td>Select the channel or user that you want to invite users to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Users]</td> 
   <td> <p>Select the users that you want to add to the channel.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Kick a User]**

This action module removes a user from a channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want remove a user from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private channel]</td> 
   <td>Select the channel that you want to remove a user from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Users]</td> 
   <td> <p>Select the user that you want to remove from the channel.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Reminders

+++ **[!UICONTROL List Reminders]**

This action module returns a list of all reminders created by or given to the currently authenticated user.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Limit]</p> </td> 
   <td> <p>Enter or map the maximum number of reminders you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Get a Reminder]**

This action module retrieves details about a specific reminder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Reminder ID]</p> </td> 
   <td> <p>Enter or map the Reminder ID of the reminder you want to retrieve details for.</p> <p>Note: The Reminder ID can be retrieved using another module, such as the [!UICONTROL List Reminders] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Create a Reminder]**

This action module creates a reminder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td>Enter or map the content of the reminder</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Time]</td> 
   <td> <p>Enter or map the date and time when this reminder should happen. Enter one of the following: </p> 
    <ul> 
     <li> <p>The Unix timestamp (up to five years from now)</p> </li> 
     <li> <p>The number of seconds until the reminder (if within 24 hours) </p> </li> 
     <li> <p>A natural language description (Examples: "in 15 minutes" or "every Thursday")</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL User] </p> </td> 
   <td> <p>Select the user that receives the reminder.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Complete a Reminder]**

This action module completes a specific reminder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Reminder ID]</p> </td> 
   <td> <p>Enter or map the Reminder ID of the reminder you want to complete.</p> <p>Note: The Reminder ID can be retrieved using another module, such as the [!UICONTROL List Reminders] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Delete a Reminder]**

This action module deletes a specific reminder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Reminder ID]</p> </td> 
   <td> <p>Enter or map the Reminder ID of the reminder you want to delete.</p> <p>Note: The Reminder ID can be retrieved using another module, such as the [!UICONTROL List Reminders] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Events

+++ **[!UICONTROL New Event]**

This instant trigger starts a scenario when a new message or other event is created.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Webhook]</p> </td> 
   <td> <p>Select the webhook you want to use.</p> <p>Or</p> <p>Create a new webhook.</p> 
    <ol> 
     <li value="1"> <p>Click <b>[!UICONTROL Add]</b>.</p> </li> 
     <li value="2"> <p>Select the event type.</p> </li> 
     <li value="3"> <p>Select or add a connection. For instructions about connecting your [!DNL Slack] account to [!UICONTROL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!UICONTROL Adobe Workfront Fusion] - Basic instructions</a></p> </li> 
     <li value="4"> <p>If prompted, select the channel that you want to watch.</p> </li> 
     <li value="5"> <p>Click <b>[!UICONTROL Save]</b> to save the webhook and return to the module.</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Profile

+++ **[!UICONTROL Set a status]**

This action module updates a user's current status.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Status text]</p> </td> 
   <td> <p>Enter or map the status text. Consider the following:</p> 
    <ul> 
     <li> <p>You can enter up to 100 characters.</p> </li> 
     <li> <p>You can use markup or other formatting, such as user mentions.</p> </li> 
     <li> <p>You can include emojis in the status text by using the format <code>:emojiname:</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status Emoji]</td> 
   <td> <p>Enter or map the emoji that you want to use to represent your status. Use the format <code>:emojiname:</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status expiration]</td> 
   <td>Enter or map the date and time you want the status to expire. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Type coercion in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
 </tbody> 
</table>

+++

-->

### Sonstige

+++ **[!UICONTROL API-Aufruf durchführen]**

Mit diesem Aktionsmodul können Sie einen benutzerdefinierten authentifizierten Aufruf an die [!DNL Slack] -API durchführen. Auf diese Weise können Sie eine Datenflussautomatisierung erstellen, die von anderen [!DNL Slack] -Modulen nicht ausgeführt werden kann.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Slack]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Geben Sie einen Pfad relativ zu <code>https://slack.com/api/</code> ein. Beispiel: <code>/users/identity</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode]</td> 
   td&gt; <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
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
  <tr> 
   <td role="rowheader">[!UICONTROL Basis-URL]</td> 
   <td>Wählen Sie die Basis-URL aus, die Sie für den API-Aufruf verwenden möchten.</td> 
  </tr> 
 </tbody> 
</table>

+++

## Terminologie

Die folgende Terminologie kann beim Konfigurieren von [!DNL Slack] -Modulen nützlich sein:

* **DM**: [!UICONTROL Direktnachricht]
* **IM**: [!UICONTROL Instant Message]
* **Privater Kanal**: früher [!UICONTROL Gruppe]
* **Direktnachricht**: früher [!UICONTROL IM]
* **Kanal**: [!UICONTROL Konversation] in der API-Dokumentation, [!UICONTROL Kanal] in der [!DNL Slack]-App.