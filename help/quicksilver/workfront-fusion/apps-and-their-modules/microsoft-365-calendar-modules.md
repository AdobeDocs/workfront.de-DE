---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: Microsoft Office 365-Kalender
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 814c285e-c106-458a-a0b1-760677634f4f
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '2074'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Calendar]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Microsoft Office 365-Kalender](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/microsoft-365-calendar-modules.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die [!DNL Microsoft Office 365 Calendar] verwenden, und sie mit mehreren Anwendungen und Services von Drittanbietern verbinden.

Um [!DNL Office 365 Calendar] mit [!DNL Adobe Workfront Fusion] verwenden zu können, muss ein [!DNL Office 365 Excel] Konto vorhanden sein. Sie können einen unter [www.office.com](https://www.office.com/) erstellen.

Anweisungen zum Verbinden Ihres Office 365-Kontos mit [!DNL Workfront Fusion] finden Sie unter [Verbindung zum Adobe herstellen [!DNL Workfront Fusion]  - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

Nachdem Sie Ihr Einverständnis erteilt haben, werden Sie zurück zur Verwaltungsseite von [!UICONTROL Workfront Fusion] weitergeleitet, wo Sie Ihr Szenario weiter erstellen können.

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

Um [!DNL Microsoft Office 365 Calendar]-Module verwenden zu können, müssen Sie über ein [!DNL Microsoft Office 365 Calendar]-Konto verfügen.

## Informationen zur Microsoft Office 365-Kalender-API

Der Microsoft Office 365-Kalender-Connector verwendet Folgendes:

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

## Verbinden des [!DNL Office 365 Calendar]-Services mit [!DNL Workfront Fusion]

Anweisungen zum Verbinden Ihres [!DNL Office 365 Calendar]-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter [Erstellen einer Verbindung mit [!UICONTROL Adobe Workfront Fusion] - Grundlegende Anweisungen](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Einige Microsoft-Apps verwenden dieselbe Verbindung, die an individuelle Benutzerberechtigungen gebunden ist. Daher werden beim Erstellen einer Verbindung im Einverständnisbildschirm für Berechtigungen alle Berechtigungen angezeigt, die zuvor der Verbindung dieses Benutzers gewährt wurden, zusätzlich zu den neuen Berechtigungen, die für die aktuelle Anwendung erforderlich sind.
>
>Wenn ein Benutzer beispielsweise über die über den Excel-Connector gewährten Berechtigungen zum Lesen von Tabellen verfügt und dann im Outlook-Connector eine Verbindung zum Lesen von E-Mails erstellt, zeigt der Einverständnisbildschirm für Berechtigungen sowohl die bereits erteilte Berechtigung zum Lesen von Tabellen als auch die neu erforderliche Berechtigung zum Schreiben von E-Mails an.

## [!DNL Microsoft Office 365 Calendar] Module und ihre Felder

Beim Konfigurieren [!DNL Microsoft Office 365 Calendar] Module zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service weitere [!DNL Microsoft Office 365 Calendar] angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Ereignis](#event)
* [Kalender](#calendar)
* [Sonstige](#other)

### Ereignis

* [[!UICONTROL Ereignisse ansehen]](#watch-events)
* [[!UICONTROL Ereignisse suchen]](#search-events)
* [[!UICONTROL Ereignis abrufen]](#get-an-event)
* [[!UICONTROL Ereignis erstellen]](#create-an-event)
* [[!UICONTROL Ereignis aktualisieren]](#update-an-event)
* [[!UICONTROL Ereignis löschen]](#delete-an-event)

#### [!UICONTROL Ereignisse ansehen]

Dieses Kalendermodul ruft Details zu einem Trigger ab, wenn das Ereignis im ausgewählten Kalender erstellt, aktualisiert, gelöscht, gestartet oder beendet wird.

>[!NOTE]
>
>Um nach gelöschten Vorkommen einer Ereignisreihe zu suchen, wählen Sie [!UICONTROL Nach Aktualisierungszeit] im Feld [!UICONTROL Ereignisse ]. Dieses Modul überwacht nicht auf gelöschte einzelne Ereignisse oder gelöschte Ereignisreihen.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ereignisse beobachten]</td> 
   <td> <p>Wählen Sie aus, wie Sie Ereignisse ansehen möchten.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL nach Erstellungszeit]</strong> </p> <p>Achten Sie auf neue Ereignisse.</p> </li> 
     <li> <p><strong>[!UICONTROL nach Aktualisierungszeit]</strong> </p> <p>Auf aktualisierte Ereignisse achten.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalendergruppen-ID]</td> 
   <td>Wählen Sie die [!UICONTROL Kalendergruppe] aus, die den Kalender enthält, in dem Sie Ereignisse beobachten möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Kalender]</td> 
   <td> <p>Wählen Sie den spezifischen Kalender aus, den Sie beobachten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL filter]</td> 
   <td>Filterbedingungen festlegen, um Ergebnisse nach Betreff, Ereignis-ID oder Hauptteil zu filtern.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Geben Sie die maximale Anzahl an Nachrichten ein, die [!DNL Workfront Fusion] während eines Szenario-Ausführungszyklus zurückgeben sollen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ereignisse suchen]

Dieses Suchmodul ruft Details zu einem Ereignis ab, wenn das Ereignis im ausgewählten Kalender erstellt, aktualisiert, gelöscht, gestartet oder beendet wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalendergruppen-ID]</td> 
   <td>Wählen Sie die [!UICONTROL Kalendergruppe] aus, die den Kalender enthält, in dem Sie Ereignisse beobachten möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Kalender]</td> 
   <td> <p>Wählen Sie den spezifischen Kalender aus, den Sie beobachten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL filter]</td> 
   <td> <p>Filterbedingungen festlegen, um Ergebnisse zu filtern. Sie können nach den folgenden Eigenschaften filtern:</p> 
    <ul> 
     <li>[!UICONTROL Betreff]</li> 
     <li>[!UICONTROL Ereignis-ID]</li> 
     <li>[!UICONTROL Erstellungsdatum Uhrzeit]</li> 
     <li>[!UICONTROL Datum der letzten Änderung]</li> 
     <li>[!UICONTROL Textvorschau]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sortieren nach]</td> 
   <td> <p>Wählen Sie aus, wie Sie die Ergebnisse sortieren möchten.</p> 
    <ul> 
     <li><strong>[!UICONTROL subject]</strong>, aufsteigend oder absteigend</li> 
     <li><strong>[!UICONTROL Erstellungsdatum Uhrzeit]</strong>, aufsteigend oder absteigend</li> 
     <li><strong>[!UICONTROL Datum der letzten Änderung]</strong>, aufsteigend oder absteigend</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl an Ereignissen ein, die [!DNL Workfront Fusion] während eines Szenario-Ausführungszyklus zurückgeben sollen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ereignis abrufen]

Dieses Aktionsmodul ruft Details des angegebenen Ereignisses ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ereignis-ID]</td> 
   <td> <p>Geben Sie die ID des Ereignisses ein, zu dem Sie Details abrufen möchten, oder ordnen Sie sie zu.</p> </td> 
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
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Betreff]</td> 
   <td> <p>Geben Sie einen Titel für das erstellte Ereignis ein oder mappen Sie ihn.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Startdatum]</td> 
   <td> Geben Sie einen einzigen Zeitpunkt ein, zu dem das Ereignis in einer kombinierten Datums- und Uhrzeitdarstellung beginnt. Verwenden Sie den <code>({date}T{time}</code> Format , z. B. <code>2017-08-29T04:00:00.0000000</code>. Eine Liste der unterstützten Datums- und Zeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typzwang in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enddatum]</td> 
   <td> Geben Sie einen einzigen Zeitpunkt ein, zu dem das Ereignis in einer kombinierten Datums- und Uhrzeitdarstellung endet. Verwenden Sie den <code>{date}T{time}</code> Format , z. B. <code>2017-08-29T04:00:00.0000000</code>. Eine Liste der unterstützten Datums- und Zeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typzwang in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL reminder on]</td> 
   <td>Wählen Sie aus, ob eine Erinnerung für dieses Ereignis aktiviert werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL reminder]</td> 
   <td>Anzahl der Minuten vor Ereignisbeginn eingeben oder zuordnen, nach denen die Erinnerung Trigger werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Wichtigkeit]</td> 
   <td> <p>Die Wichtigkeit dieses Ereignisses auswählen.</p> 
    <ul> 
     <li>[!UICONTROL Niedrig]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL Hoch]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensitivity] </td> 
   <td> <p>Wählen Sie die Empfindlichkeit dieses Ereignisses aus.</p> 
    <ul> 
     <li><strong>[!UICONTROL normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>Der Empfänger sieht die Nachricht "[!UICONTROL Please treat as Personal]".</p> </li> 
     <li> <p><strong>[!UICONTROL Privat]</strong> </p> <p>Der Empfänger sieht die Nachricht "[!UICONTROL Bitte als privat behandeln]". Dieses Ereignis wird von den Posteingangsregeln des Empfängers nicht weitergeleitet oder umgeleitet.</p> </li> 
     <li> <p><strong>[!UICONTROL VERTRAULICH]</strong> </p> <p>Der Empfänger sieht die Nachricht "[!UICONTROL Bitte als vertraulich behandeln]". </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Hauptteil-Inhaltstyp]</td> 
   <td>Wählen Sie aus, ob der Textinhalt Nur-Text oder HTML ist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Hauptteilinhalt]</td> 
   <td>Geben Sie den Text der Nachricht ein, die mit dem Ereignis verknüpft ist, oder mappen Sie ihn. Sie kann im HTML- oder Textformat vorliegen (wie im Feld [!UICONTROL Hauptteil Inhaltstyp] weiter oben angegeben).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Speicherort]</td> 
   <td> <p>Details zum Veranstaltungsort eingeben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Antwort angefordert]</td> 
   <td>Wählen Sie <strong>[!UICONTROL Yes]</strong> aus, um den Einladenden aufzufordern, eine Antwort auf die Ereigniseinladung zu senden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anzeigen als]</td> 
   <td> <p>Wählen Sie aus, wie das Ereignis den Personen angezeigt werden soll, die Ihren Kalender anzeigen.</p> 
    <ul> 
     <li>[!UICONTROL FREE]</li> 
     <li>[!UICONTROL Tentative]</li> 
     <li>[!UICONTROL Besetzt]</li> 
     <li>[!UICONTROL Abwesend]</li> 
     <li>[!UICONTROL, anderswo arbeiten]</li> 
     <li>[!UICONTROL unbekannt]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attendees]</p> </td> 
   <td> <p>Fügen Sie Teilnehmer der Veranstaltung hinzu.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL name]</strong> </p> <p>Geben Sie den Namen des Teilnehmers ein.</p> </li> 
     <li> <p><strong>[!UICONTROL email]</strong> </p> <p>Geben Sie die E-Mail-Adresse des Teilnehmers ein.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kategorie]</td> 
   <td>Geben Sie die Kategorien ein, die das Ereignis wie im Kalender angezeigt werden soll, oder ordnen Sie sie zu.</td> 
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
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ereignis-ID]</td> 
   <td>Geben Sie die ID des Ereignisses ein, das Sie aktualisieren möchten, ordnen Sie sie zu oder wählen Sie sie aus.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Betreff]</td> 
   <td> <p>Geben Sie einen Titel für das erstellte Ereignis ein oder mappen Sie ihn.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Startdatum]</td> 
   <td> Geben Sie einen einzigen Zeitpunkt ein, zu dem das Ereignis in einer kombinierten Datums- und Uhrzeitdarstellung beginnt. Verwenden Sie den <code>{date}T{time}</code> Format , z. B. <code>2017-08-29T04:00:00.0000000</code>. Eine Liste der unterstützten Datums- und Zeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typzwang in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enddatum]</td> 
   <td> Geben Sie einen einzigen Zeitpunkt ein, zu dem das Ereignis in einer kombinierten Datums- und Uhrzeitdarstellung endet. Verwenden Sie den <code>({date}T{time}</code> Format , z. B. <code>2017-08-29T04:00:00.0000000</code>. Eine Liste der unterstützten Datums- und Zeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typzwang in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL reminder on]</td> 
   <td>Wählen Sie aus, ob eine Erinnerung für dieses Ereignis aktiviert werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL reminder]</td> 
   <td>Anzahl der Minuten vor Ereignisbeginn eingeben oder zuordnen, nach denen die Erinnerung Trigger werden soll.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Wichtigkeit]</td> 
   <td> <p>Die Wichtigkeit dieses Ereignisses auswählen.</p> 
    <ul> 
     <li>[!UICONTROL Niedrig]</li> 
     <li>[!UICONTROL Medium]</li> 
     <li>[!UICONTROL Hoch]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sensitivity] </td> 
   <td> <p>Wählen Sie die Empfindlichkeit dieses Ereignisses aus.</p> 
    <ul> 
     <li><strong>[!UICONTROL normal]</strong> </li> 
     <li> <p><strong>[!UICONTROL Personal]</strong> </p> <p>Der Empfänger sieht die Nachricht "[!UICONTROL Please treat as Personal]".</p> </li> 
     <li> <p><strong>[!UICONTROL Privat]</strong> </p> <p>Der Empfänger sieht die Nachricht "[!UICONTROL Bitte als privat behandeln]". Dieses Ereignis wird von den Posteingangsregeln des Empfängers nicht weitergeleitet oder umgeleitet.</p> </li> 
     <li> <p><strong>[!UICONTROL VERTRAULICH]</strong> </p> <p>Der Empfänger sieht die Nachricht "[!UICONTROL Bitte als vertraulich behandeln]". </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Hauptteil-Inhaltstyp]</td> 
   <td>Wählen Sie aus, ob der Hauptteil der Nachricht, die mit dem Ereignis verknüpft ist, Nur-Text oder HTML ist.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Hauptteilinhalt]</td> 
   <td>Geben Sie den Text der Nachricht ein, die mit dem Ereignis verknüpft ist, oder mappen Sie ihn. Sie kann im HTML- oder Textformat vorliegen (wie im Feld [!UICONTROL Hauptteil Inhaltstyp] weiter oben angegeben).</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Speicherort]</td> 
   <td> <p>Details zum Veranstaltungsort eingeben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Antwort angefordert]</td> 
   <td>Wählen Sie <strong>[!UICONTROL Yes]</strong> aus, um den Einladenden aufzufordern, eine Antwort auf die Ereigniseinladung zu senden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Anzeigen als]</td> 
   <td> <p>Wählen Sie aus, wie das Ereignis den Personen angezeigt werden soll, die Ihren Kalender anzeigen.</p> 
    <ul> 
     <li>[!UICONTROL FREE]</li> 
     <li>[!UICONTROL Tentative]</li> 
     <li>[!UICONTROL Besetzt]</li> 
     <li>[!UICONTROL Abwesend]</li> 
     <li>[!UICONTROL, anderswo arbeiten]</li> 
     <li>[!DNL Unknown]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attendees]</p> </td> 
   <td> <p>Fügen Sie Teilnehmer der Veranstaltung hinzu.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL name]</strong> </p> <p>Geben Sie den Namen des Teilnehmers ein.</p> </li> 
     <li> <p><strong>[!UICONTROL email]</strong> </p> <p>Geben Sie die E-Mail-Adresse des Teilnehmers ein.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kategorie]</td> 
   <td>Geben Sie die Kategorien ein, die das Ereignis wie im Kalender angezeigt werden soll, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ereignis löschen]

Dieses Aktionsmodul löscht ein vorhandenes Ereignis.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ereignis-ID]</td> 
   <td> <p>Geben Sie die ID des Ereignisses ein, das Sie löschen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Kalender

* [[!UICONTROL Kalender auflisten]](#list-calendars)
* [[!UICONTROL Kalender abrufen]](#get-a-calendar)
* [[!UICONTROL Kalender erstellen]](#create-a-calendar)
* [[!UICONTROL Aktualisieren eines Kalenders]](#update-a-calendar)
* [[!UICONTROL Löschen eines Kalenders]](#delete-a-calendar)

#### [!UICONTROL Kalender auflisten]

Dieses Suchmodul ruft eine Liste aller Kalender der authentifizierten Benutzenden ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalendergruppen-ID]</td> 
   <td>Wählen Sie die [!UICONTROL Kalendergruppe] aus, die die Kalender enthält, die Sie auflisten möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Geben Sie die maximale Anzahl an Kalendern ein, die [!DNL Workfront Fusion] während eines Szenario-Ausführungszyklus zurückgeben sollen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kalender abrufen]

Dieses Aktionsmodul ruft Details zu einem einzelnen Kalender ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalenderkennung]</td> 
   <td> <p>Geben Sie die ID des Kalenders ein, zu dem Sie Details abrufen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kalender erstellen]

Dieses Aktionsmodul erstellt einen neuen Kalender in Ihrem Google-Konto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalendername]</td> 
   <td> <p>Geben Sie einen Namen für den neuen Kalender ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aktualisieren eines Kalenders]

Dieses Aktionsmodul bearbeitet einen vorhandenen Kalender.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalenderkennung]</td> 
   <td>Geben Sie die [!UICONTROL Kalender-ID] für den Kalender ein, den Sie aktualisieren möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Neuer Kalendername]</td> 
   <td> <p>Geben Sie einen Namen für den neuen Kalender ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Löschen eines Kalenders]

Dieses Aktionsmodul löscht einen vorhandenen Kalender.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalenderkennung]</td> 
   <td>Geben Sie die [!UICONTROL Calendar]-ID für den Kalender ein, den Sie löschen möchten.</td> 
  </tr> 
 </tbody> 
</table>

### Sonstige

#### [!UICONTROL Erstellen eines API-Aufrufs]

Mit diesem Modul können Sie einen benutzerdefinierten API-Aufruf durchführen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Office 365]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu [!DNL Adobe Workfront Fusion] - Grundlegende Anweisungen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Geben Sie einen Pfad relativ zu <code>https://graph.microsoft.com</code> ein. Beispiel:<code> /v1.0/me/events</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Methode]</p> </td> 
   td&gt; <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anfragemethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Kopfzeilen]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu, z. B. <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] fügt die Autorisierungskopfzeilen für Sie hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge]</td> 
   <td> <p> Fügen Sie die Abfrage für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL body]</td> 
   <td> <p>Fügen Sie den Hauptteil des Inhalts für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Hinweis:   <p>Wenn Sie bedingte Anweisungen wie <code>if</code> in Ihrer JSON-Datei verwenden, setzen Sie die Anführungszeichen außerhalb der bedingten Anweisung.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
