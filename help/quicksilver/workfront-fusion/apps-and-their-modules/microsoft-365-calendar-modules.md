---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: Connector
navigation-topic: apps-and-their-modules
title: Microsoft Office 365-Kalender
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die Microsoft Office 365 Calendar verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 814c285e-c106-458a-a0b1-760677634f4f
source-git-commit: 2e91e9a4c691430f3c98e3cbddb30706ea57f84a
workflow-type: tm+mt
source-wordcount: '2023'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Calendar]

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Microsoft Office 365 Calendar] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

Um [!DNL Office 365 Calendar] mit [!DNL Adobe Workfront Fusion] zu verwenden, ist ein [!DNL Office 365 Excel] -Konto erforderlich. Sie können eine unter [www.office.com](https://www.office.com/) erstellen.

Anweisungen zum Verbinden Ihres Office 365-Kontos mit [!DNL Workfront Fusion] finden Sie unter [Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion]  - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

Nachdem Sie die Einwilligung erteilt haben, werden Sie zur Administrationsseite von [!UICONTROL Workfront Fusion] zurückgeleitet, auf der Sie das Szenario weiter erstellen können.

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

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Um [!DNL Microsoft Office 365 Calendar] -Module zu verwenden, müssen Sie über ein [!DNL Microsoft Office 365 Calendar] -Konto verfügen.

## Microsoft Office 365 Calendar API-Informationen

Der Microsoft Office 365 Calendar-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td> https://graph.microsoft.com/v1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Version</td> 
   <td> v1.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v2.0.10</td> 
  </tr>
 </tbody> 
 </table>

## Verbinden des [!DNL Office 365 Calendar]-Dienstes mit [!DNL Workfront Fusion]

Anweisungen zum Verbinden Ihres [!DNL Office 365 Calendar]-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter [Erstellen einer Verbindung mit [!UICONTROL Adobe Workfront Fusion] - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Einige Microsoft-Apps verwenden dieselbe Verbindung, die an individuelle Benutzerberechtigungen gebunden ist. Daher werden beim Erstellen einer Verbindung im Bildschirm für die Genehmigung von Berechtigungen alle Berechtigungen angezeigt, die zuvor für die Verbindung dieses Benutzers gewährt wurden, zusätzlich zu den neuen Berechtigungen, die für die aktuelle Anwendung erforderlich sind.
>
>Wenn beispielsweise ein Benutzer über den Excel-Connector über die Berechtigung &quot;Tabelle lesen&quot;verfügt und dann im Outlook-Connector eine Verbindung zum Lesen von E-Mails erstellt, zeigt der Bildschirm für die Genehmigung der Berechtigungen sowohl die bereits erteilte Berechtigung &quot;Tabelle lesen&quot;als auch die neu erforderliche Berechtigung &quot;E-Mail schreiben&quot;an.

## [!DNL Microsoft Office 365 Calendar] Module und ihre Felder

Wenn Sie [!DNL Microsoft Office 365 Calendar] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Microsoft Office 365 Calendar] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Ereignis](#event)
* [Kalender](#calendar)
* [Sonstige](#other)

### Ereignis

* [[!UICONTROL Ereignisse ansehen]](#watch-events)
* [[!UICONTROL Suchereignisse]](#search-events)
* [[!UICONTROL Ereignis abrufen]](#get-an-event)
* [[!UICONTROL Ereignis erstellen]](#create-an-event)
* [[!UICONTROL Ereignis aktualisieren]](#update-an-event)
* [[!UICONTROL Löschen eines Ereignisses]](#delete-an-event)

#### [!UICONTROL Ereignisse ansehen]

Dieses Ereignismodul ruft Details zu einem Trigger ab, wenn das Ereignis im Kalender erstellt, aktualisiert, gelöscht, gestartet oder beendet wird.

>[!NOTE]
>
>Um auf gelöschte Vorkommen einer Ereignisreihe zu achten, wählen Sie im Feld [!UICONTROL Ereignisse überwachen] die Option [!UICONTROL Durch aktualisierte Zeit] aus. Dieses Modul überwacht nicht auf gelöschte einzelne Ereignisse oder gelöschte Ereignisreihen.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ereignisse ansehen]</td> 
   <td> <p>Wählen Sie aus, wie Sie Ereignisse anzeigen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Nach Erstellungszeit]</strong> </p> <p>Auf neue Ereignisse achten.</p> </li> 
     <li> <p><strong>[!UICONTROL Nach Aktualisierungszeit]</strong> </p> <p>Auf aktualisierte Ereignisse achten.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalendergruppen-ID]</td> 
   <td>Wählen Sie die [!UICONTROL Kalendergruppe] aus, die den Kalender enthält, in dem Sie Ereignisse anzeigen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalender]</td> 
   <td> <p>Wählen Sie den gewünschten Kalender aus.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Legen Sie die Filterbedingungen fest, um die Ergebnisse nach Betreff, Ereignis-ID oder Text zu filtern.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl von Nachrichten ein, die [!DNL Workfront Fusion] während eines Szenario-Ausführungszyklus zurückgeben soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suchereignisse]

Dieses Suchmodul ruft Details zu einem Ereignis zurück, wenn das Ereignis im ausgewählten Kalender erstellt, aktualisiert, gelöscht, gestartet oder beendet wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalendergruppen-ID]</td> 
   <td>Wählen Sie die [!UICONTROL Kalendergruppe] aus, die den Kalender enthält, in dem Sie Ereignisse anzeigen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalender]</td> 
   <td> <p>Wählen Sie den gewünschten Kalender aus.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Legen Sie die Filterbedingungen fest, um die Ergebnisse zu filtern. Sie können nach den folgenden Eigenschaften filtern:</p> 
    <ul> 
     <li>[!UICONTROL Betreff]</li> 
     <li>[!UICONTROL Ereignis-ID]</li> 
     <li>[!UICONTROL Erstellungsdatumszeit]</li> 
     <li>[!UICONTROL Last Modified Date Time]</li> 
     <li>[!UICONTROL Textkörper-Vorschau]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reihenfolge nach]</td> 
   <td> <p>Wählen Sie aus, wie die Ergebnisse sortiert werden sollen.</p> 
    <ul> 
     <li><strong>[!UICONTROL Subject]</strong>, aufsteigend oder absteigend</li> 
     <li><strong>[!UICONTROL Erstellungsdatumszeit]</strong>, aufsteigend oder absteigend</li> 
     <li><strong>[!UICONTROL Last Modified Date Time]</strong>, aufsteigend oder absteigend</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl von Ereignissen an, die [!DNL Workfront Fusion] während eines Szenario-Ausführungszyklus zurückgeben soll.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ereignis abrufen]

Dieses Aktionsmodul ruft Details zum angegebenen Ereignis ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ereignis-ID]</td> 
   <td> <p>Geben Sie die ID des Ereignisses ein oder ordnen Sie es zu, zu dem Sie Details abrufen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ereignis erstellen]

Dieses Aktionsmodul erstellt ein neues Ereignis.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Betreff]</td> 
   <td> <p>Geben Sie einen Titel für das erstellte Ereignis ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Startdatum]</td> 
   <td> Geben Sie einen einzelnen Zeitpunkt ein, zu dem das Ereignis in einer kombinierten Datums- und Uhrzeitdarstellung beginnt. Verwenden Sie das Format <code>({date}T{time}</code>, z. B. <code>2017-08-29T04:00:00.0000000</code>. Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enddatum]</td> 
   <td> Geben Sie einen einzelnen Zeitpunkt ein, zu dem das Ereignis in einer kombinierten Datums- und Uhrzeitdarstellung endet. Verwenden Sie das Format <code>{date}T{time}</code>, z. B. <code>2017-08-29T04:00:00.0000000</code>. Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reminder on]</td> 
   <td>Wählen Sie aus, ob Sie eine Erinnerung für dieses Ereignis aktivieren möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reminder]</td> 
   <td>Geben Sie die Anzahl der Minuten vor Ereignisbeginn ein oder ordnen Sie sie zu, wenn die Erinnerung Trigger werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Wichtigkeit]</td> 
   <td> <p>Wählen Sie die Wichtigkeit dieses Ereignisses aus.</p> 
    <ul> 
     <li>[!UICONTROL Niedrig]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL Hoch]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensitivität] </td> 
   <td> <p>Wählen Sie die Empfindlichkeit dieses Ereignisses aus.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>Dem Empfänger wird die Nachricht "[!UICONTROL Bitte behandeln Sie diese als persönlich]" angezeigt.</p> </li> 
     <li> <p><strong>[!UICONTROL Private]</strong> </p> <p>Dem Empfänger wird die Nachricht "[!UICONTROL Bitte behandeln Sie diese als privat]" angezeigt. Dieses Ereignis wird nicht von den Posteingangsregeln des Empfängers weitergeleitet oder weitergeleitet.</p> </li> 
     <li> <p><strong>[!UICONTROL Vertraulich]</strong> </p> <p>Der Empfänger erhält die Nachricht "[!UICONTROL Bitte behandeln Sie diese als vertraulich]". </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inhaltstyp des Textkörpers]</td> 
   <td>Wählen Sie aus, ob es sich bei dem Hauptteilinhalt um Text oder HTML handelt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Textkörper]</td> 
   <td>Geben Sie den Hauptteil der mit dem Ereignis verknüpften Nachricht ein oder ordnen Sie ihn zu. Sie kann im HTML- oder Textformat vorliegen (wie im Feld [!UICONTROL Body Content Type] oben angegeben).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Standort]</td> 
   <td> <p>Geben Sie die Details zum Ereignisspeicherort ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Antwort angefordert]</td> 
   <td>Wählen Sie <strong>[!UICONTROL Yes]</strong> aus, um die Einladung zum Senden einer Antwort auf die Ereigniseinladung anzufordern.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anzeigen als]</td> 
   <td> <p>Wählen Sie aus, wie das Ereignis Personen angezeigt werden soll, die den Kalender ansehen.</p> 
    <ul> 
     <li>[!UICONTROL Free]</li> 
     <li>[!UICONTROL Tentative]</li> 
     <li>[!UICONTROL beschäftigt]</li> 
     <li>[!UICONTROL Abwesenheit]</li> 
     <li>[!UICONTROL Anderswo arbeiten]</li> 
     <li>[!UICONTROL Unbekannt]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Teilnehmer]</p> </td> 
   <td> <p>Fügen Sie Teilnehmer des Ereignisses hinzu.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Geben Sie den Namen des Teilnehmers ein.</p> </li> 
     <li> <p><strong>[!UICONTROL Email]</strong> </p> <p>Geben Sie die E-Mail-Adresse des Teilnehmers ein.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kategorie]</td> 
   <td>Geben Sie die Kategorien ein oder ordnen Sie sie zu, als die das Ereignis im Kalender angezeigt werden soll.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ereignis aktualisieren]

Dieses Aktionsmodul aktualisiert ein vorhandenes Ereignis.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ereignis-ID]</td> 
   <td>Geben Sie die ID des Ereignisses ein, das Sie aktualisieren möchten, ordnen Sie sie zu oder wählen Sie sie aus.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Betreff]</td> 
   <td> <p>Geben Sie einen Titel für das erstellte Ereignis ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Startdatum]</td> 
   <td> Geben Sie einen einzelnen Zeitpunkt ein, zu dem das Ereignis in einer kombinierten Datums- und Uhrzeitdarstellung beginnt. Verwenden Sie das Format <code>{date}T{time}</code>, z. B. <code>2017-08-29T04:00:00.0000000</code>. Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enddatum]</td> 
   <td> Geben Sie einen einzelnen Zeitpunkt ein, zu dem das Ereignis in einer kombinierten Datums- und Uhrzeitdarstellung endet. Verwenden Sie das Format <code>({date}T{time}</code>, z. B. <code>2017-08-29T04:00:00.0000000</code>. Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reminder on]</td> 
   <td>Wählen Sie aus, ob Sie eine Erinnerung für dieses Ereignis aktivieren möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reminder]</td> 
   <td>Geben Sie die Anzahl der Minuten vor Ereignisbeginn ein oder ordnen Sie sie zu, wenn die Erinnerung Trigger werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Wichtigkeit]</td> 
   <td> <p>Wählen Sie die Wichtigkeit dieses Ereignisses aus.</p> 
    <ul> 
     <li>[!UICONTROL Niedrig]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL Hoch]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensitivität] </td> 
   <td> <p>Wählen Sie die Empfindlichkeit dieses Ereignisses aus.</p> 
    <ul> 
     <li><strong>[!UICONTROL Normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>Dem Empfänger wird die Nachricht "[!UICONTROL Bitte behandeln Sie diese als persönlich]" angezeigt.</p> </li> 
     <li> <p><strong>[!UICONTROL Private]</strong> </p> <p>Dem Empfänger wird die Nachricht "[!UICONTROL Bitte behandeln Sie diese als privat]" angezeigt. Dieses Ereignis wird nicht von den Posteingangsregeln des Empfängers weitergeleitet oder weitergeleitet.</p> </li> 
     <li> <p><strong>[!UICONTROL Vertraulich]</strong> </p> <p>Der Empfänger erhält die Nachricht "[!UICONTROL Bitte behandeln Sie diese als vertraulich]". </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Inhaltstyp des Textkörpers]</td> 
   <td>Wählen Sie aus, ob der Hauptteilinhalt der Nachricht, die mit dem Ereignis verknüpft ist, Nur-Text oder HTML ist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Textkörper]</td> 
   <td>Geben Sie den Hauptteil der mit dem Ereignis verknüpften Nachricht ein oder ordnen Sie ihn zu. Sie kann im HTML- oder Textformat vorliegen (wie im Feld [!UICONTROL Body Content Type] oben angegeben).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Standort]</td> 
   <td> <p>Geben Sie die Details zum Ereignisspeicherort ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Antwort angefordert]</td> 
   <td>Wählen Sie <strong>[!UICONTROL Yes]</strong> aus, um die Einladung zum Senden einer Antwort auf die Ereigniseinladung anzufordern.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anzeigen als]</td> 
   <td> <p>Wählen Sie aus, wie das Ereignis Personen angezeigt werden soll, die den Kalender ansehen.</p> 
    <ul> 
     <li>[!UICONTROL Free]</li> 
     <li>[!UICONTROL Tentative]</li> 
     <li>[!UICONTROL beschäftigt]</li> 
     <li>[!UICONTROL Abwesenheit]</li> 
     <li>[!UICONTROL Anderswo arbeiten]</li> 
     <li>[!DNL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Teilnehmer]</p> </td> 
   <td> <p>Fügen Sie Teilnehmer des Ereignisses hinzu.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>Geben Sie den Namen des Teilnehmers ein.</p> </li> 
     <li> <p><strong>[!UICONTROL Email]</strong> </p> <p>Geben Sie die E-Mail-Adresse des Teilnehmers ein.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kategorie]</td> 
   <td>Geben Sie die Kategorien ein oder ordnen Sie sie zu, als die das Ereignis im Kalender angezeigt werden soll.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Löschen eines Ereignisses]

Dieses Aktionsmodul löscht ein vorhandenes Ereignis.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ereignis-ID]</td> 
   <td> <p>Geben Sie die ID des Ereignisses ein, das Sie löschen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Kalender

* [[!UICONTROL Listenkalender]](#list-calendars)
* [[!UICONTROL Einen Kalender abrufen]](#get-a-calendar)
* [[!UICONTROL Einen Kalender erstellen]](#create-a-calendar)
* [[!UICONTROL Kalender aktualisieren]](#update-a-calendar)
* [[!UICONTROL Einen Kalender löschen]](#delete-a-calendar)

#### [!UICONTROL Listenkalender]

Dieses Suchmodul ruft eine Liste aller Kalender des authentifizierten Benutzers ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalendergruppen-ID]</td> 
   <td>Wählen Sie die [!UICONTROL Kalendergruppe] aus, die die aufzulistenden Kalender enthält.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl von Kalendern ein, die [!DNL Workfront Fusion] während eines Szenario-Ausführungszyklus zurückgeben soll.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Einen Kalender abrufen]

Dieses Aktionsmodul ruft Details zu einem einzelnen Kalender ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalender-ID]</td> 
   <td> <p>Geben Sie die Kennung des Kalenders ein oder ordnen Sie ihn zu, über den Sie Details abrufen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Einen Kalender erstellen]

Dieses Aktionsmodul erstellt einen neuen Kalender in Ihrem Google-Konto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalendername]</td> 
   <td> <p>Geben Sie einen Namen für den neuen Kalender ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kalender aktualisieren]

Dieses Aktionsmodul bearbeitet einen vorhandenen Kalender.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalender-ID]</td> 
   <td>Geben Sie die [!UICONTROL Kalender-ID] für den Kalender ein, den Sie aktualisieren möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Neuer Kalendername]</td> 
   <td> <p>Geben Sie einen Namen für den neuen Kalender ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Einen Kalender löschen]

Dieses Aktionsmodul löscht einen vorhandenen Kalender.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalender-ID]</td> 
   <td>Geben Sie die [!UICONTROL Kalender]-ID für den Kalender ein, den Sie löschen möchten.</td> 
  </tr> 
 </tbody> 
</table>

### Sonstige

#### [!UICONTROL API-Aufruf durchführen]

Mit diesem Modul können Sie einen benutzerdefinierten API-Aufruf ausführen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Geben Sie einen Pfad relativ zu <code>https://graph.microsoft.com</code> ein. Beispiel:<code> /v1.0/me/events</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Methode]</p> </td> 
   td&gt; <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu, z. B. <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p> Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:   <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> in Ihrer JSON platzieren Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
