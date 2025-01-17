---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: Google-Kalendermodule
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 168e8fce-645d-4108-84b7-46a113c83f41
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '3889'
ht-degree: 0%

---

# [!DNL Google Calendar]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Google-Kalendermodule](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

In einem [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die den [!UICONTROL Google-Kalender] verwenden, und ihn mit mehreren Anwendungen und Services von Drittanbietern verbinden.

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

Um [!DNL Google Calendar]-Module verwenden zu können, müssen Sie über ein [!DNL Google]-Konto verfügen.

## Google Calendar-API-Informationen

Der Google-Kalender-Connector verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Basis-URL</td> 
   <td> https://www.googleapis.com/calendar/v3</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Version</td> 
   <td> v3 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v5.4.5</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Google Calendar] Module und ihre Felder

Beim Konfigurieren [!DNL Google Calendar] Module zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder dem Service weitere [!DNL Google Calendar] angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [-Events](#events)
* [Kalender](#calendars)
* [Zugriffssteuerungsregeln](#access-control-rules)
* [Iteratoren (veraltet)](#iterators-deprecated)
* [Sonstige](#other)

### -Events

* [[!UICONTROL Ereignisse ansehen]](#watch-events)
* [[!UICONTROL Ereignisse suchen]](#search-events)
* [[!UICONTROL Ereignis abrufen]](#get-an-event)
* [[!UICONTROL Ereignis erstellen]](#create-an-event)
* [[!UICONTROL Ereignis aktualisieren]](#update-an-event)
* [[!UICONTROL Ereignis löschen]](#delete-an-event)


#### [!UICONTROL Ereignisse ansehen]

Dieses Kalendermodul führt ein Trigger aus, wenn ein neues Ereignis in dem von Ihnen angegebenen Kalender hinzugefügt, aktualisiert, gelöscht, gestartet oder beendet wird. Das Modul gibt alle Standardfelder zurück, die mit dem Datensatz oder den Datensätzen verknüpft sind, sowie alle benutzerdefinierten Felder und Werte, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Kalender] </td> 
   <td> <p>Wählen Sie den Kalender aus, mit dem das Modul arbeiten soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ereignisse beobachten]</td> 
   <td> <p>Wählen Sie aus, ob Sie Ereignisse nach Erstellungsdatum, Aktualisierungsdatum, Startdatum oder Enddatum beobachten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gelöschte Ereignisse anzeigen]</td> 
   <td> <p>Aktivieren Sie diese Option, um gelöschte Ereignisse einzuschließen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Abfrage] </td> 
   <td> <p>Geben Sie den Text ein, nach dem Sie suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Ereignissen fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeitet (die Anzahl der Wiederholungen pro Szenario-Ausführung). Wenn der Wert zu hoch eingestellt ist, kann die Verbindung auf der Seite des angegebenen Drittanbieterdienstes unterbrochen werden (Zeitüberschreitung). [!DNL Workfront Fusion] hat darauf keinen Einfluss. Es wird empfohlen, einen niedrigeren Wert festzulegen und entweder einen höheren Wert für die maximale Anzahl an Zyklen zu definieren oder das Szenario häufiger auszuführen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ereignisse suchen]

Dieses Aktionsmodul sucht im ausgewählten Kalender nach einem Ereignis.

Sie geben den Kalender und die Parameter der Suche an.

Das Modul gibt die ID des Ereignisses und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit Workfront Fusion finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbindung zu Adobe Workfront Fusion herstellen - Grundanweisungen</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalenderkennung]</td> 
   <td> <p>Wählen Sie den Kalender aus, den Sie durchsuchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Startdatum]</td> 
   <td> <p> Datum des Starts des Ereignisses eingeben oder zuordnen. Dieses Modul ruft auch Ereignisse ab, die vor diesem Datum beginnen und noch am eingegebenen Startdatum auftreten. </p> <p>Eine Liste der unterstützten Datums- und Zeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typzwang in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enddatum]</td> 
   <td> <p> Datum eingeben oder zuordnen, an dem das Ereignis endet. </p> <p> Eine Liste der unterstützten Datums- und Zeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typzwang in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Einzel-Ereignisse]</td> 
   <td> <p> Aktivieren Sie diese Option, um wiederkehrende Ereignisse als einzelne Instanzen zu behandeln. Wenn Sie beispielsweise eine wöchentliche Besprechung haben und diese Option aktiviert ist, gibt das Modul jede wöchentliche Besprechung als separates Ereignis zurück.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Abfrage]</td> 
   <td> <p>Geben Sie den Suchbegriff ein, nach dem Sie suchen möchten, oder ordnen Sie ihn zu. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sortieren nach]</td> 
   <td> <p>Auswahl der Reihenfolge der im Ergebnis zurückgegebenen Ereignisse.</p> 
    <ul> 
     <li><strong>[!UICONTROL Startzeit]</strong>: Sortieren Sie nach dem Startdatum und der Startzeit (aufsteigend). Dies ist nur bei der Abfrage einzelner Ereignisse verfügbar.</li> 
     <li><strong>[!UICONTROL Aktualisierungszeit]</strong>: Sortieren nach der Zeit der letzten Änderung (aufsteigend).</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Legen Sie die maximale Anzahl von Ereignissen fest, [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgegeben werden.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ereignis abrufen]

Dieses Aktionsmodul gibt die Metadaten für ein einzelnes Ereignis im angegebenen Kalender zurück.

Sie geben den Kalender und das Ereignis an.

Das Modul gibt die ID des Ereignisses und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalenderkennung]</td> 
   <td> <p>Geben Sie die ID des Kalenders ein, der das Ereignis enthält, das Sie erhalten möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ereignis-ID] </td> 
   <td> <p>Geben Sie die Ereignis-ID des vorhandenen [!DNL Google Calendar] ein, das Sie erhalten möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ereignis erstellen]

Dieses Aktionsmodul erstellt ein Ereignis.

Sie geben den Kalender und die Parameter für das Ereignis an.

Das Modul gibt die ID des Ereignisses und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit Workfront Fusion finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbindung zu Adobe Workfront Fusion herstellen - Grundanweisungen</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ereignis erstellen]</td> 
   <td> <p>Wählen Sie aus, wie Sie das Ereignis erstellen möchten.</p> 
    <ul> 
     <li><b>[!UICONTROL im Detail]</b><p>Mit dieser Option können Sie weitere Details zum Ereignis eingeben.<br></p></li> 
     <li><b>[!UICONTROL Quick]</b><p>Sie müssen nur den Kalender auswählen und einen Namen für das Ereignis eingeben. Sie können Zeit- und Ortsangaben in den Namen aufnehmen, und [!DNL Google Calendar] planen das Ereignis für diesen Ort und diese Uhrzeit.</p></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalenderkennung]</td> 
   <td> <p>Wählen Sie den Kalender aus, in dem das Ereignis angezeigt werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL color]</td> 
   <td>Wählen Sie die Farbe aus, die das Ereignis im Kalender anzeigt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ereignisname]</td> 
   <td> <p> Geben Sie einen Namen für das Ereignis ein oder mappen Sie ihn. </p> <p>Hinweis: Wenn Sie [!UICONTROL Quick Add] im Feld [!UICONTROL Ereignis erstellen] ausgewählt haben, können Sie Datum und Uhrzeit des Ereignisses einbeziehen und [!DNL Workfront Fusion] das Ereignis für dieses Datum und diese Uhrzeit erstellen. Beispiel: <code>Appointment at Capitol Hill on June 3rd 10am-10:25am</code>. Wenn Sie [!UICONTROL Quick Add] ausgewählt haben, aber im Ereignisnamen kein Datum und keine Uhrzeit angeben, wird das Ereignis aus der aktuellen Zeit erstellt und dauert eine Stunde.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ganztägiges Ereignis]</td> 
   <td>Aktivieren Sie diese Option, wenn das Ereignis ein ganztägiges Ereignis ist (keine Start- und Endzeiten erfordert).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Startdatum]</td> 
   <td> <p>Wenn es sich um ein ganztägiges Ereignis handelt, geben Sie das Startdatum des Ereignisses ein. </p> <p>Eine Liste der unterstützten Datumsformate finden Sie unter "<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref"> in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enddatum]</td> 
   <td> <p> Wenn es sich um ein ganztägiges Ereignis handelt, geben Sie das Enddatum des Ereignisses ein. </p> <p>Eine Liste der unterstützten Datumsformate finden Sie unter "<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref"> in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Beschreibung]</td> 
   <td>Geben Sie eine Beschreibung für das Ereignis ein oder mappen Sie sie. Dieses Feld unterstützt das HTML.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Speicherort]</td> 
   <td>Geben Sie einen Ort für das Ereignis im Textformular ein.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Standardeinstellungen für Erinnerungen an dieses Ereignis verwenden]</td> 
   <td>Aktivieren Sie diese Option, um die standardmäßigen Erinnerungseinstellungen zu verwenden. Wenn Sie eine benutzerdefinierte Erinnerung im Feld [!UICONTROL Reminder] festlegen, wird dieser Wert auf Nein gesetzt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL reminder] </td> 
   <td> <p>Erinnerung für das Ereignis hinzufügen. Wählen Sie für jede Erinnerung die Methode aus, mit der Sie erinnert werden möchten, und legen Sie fest, wie lange (in Minuten) das Ereignis dauern soll, an das Sie erinnert werden möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attendees]</td> 
   <td>Fügen Sie die Teilnehmer zum Ereignis hinzu. Geben Sie für jeden Teilnehmer seinen Namen und seine E-Mail-Adresse ein bzw. mappen Sie diese.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anzeigen als]</td> 
   <td>Wählen Sie aus, ob Personen, die Ihren Kalender anzeigen, Sie während dieses Ereignisses als beschäftigt oder verfügbar anzeigen sollen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sichtbarkeit] </td> 
   <td> <p>Sichtbarkeit dieses Ereignisses auswählen. </p> 
    <ul> 
     <li> <p><b>[!UICONTROL Standard]</b></p> <p>Das Ereignis hat die Sichtbarkeit, die Sie in Ihren Kalendereinstellungen festgelegt haben.</p> </li> 
     <li> <p><b>[!UICONTROL Öffentlich]</b></p> <p>Jeder, für den der Kalender freigegeben ist, kann dieses Ereignis sehen.</p> </li> 
     <li> <p><b>[!UICONTROL Privat]</b></p> <p>Nur Teilnehmer können diese Veranstaltung sehen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benachrichtigung über die Erstellung des Ereignisses senden]</td> 
   <td> <p>Wählen Sie aus, ob Benachrichtigungen über die Erstellung eines neuen Ereignisses an alle Gäste, nicht [!DNL Google Calendar] Gäste oder an niemanden gesendet werden sollen.</p> <p>Tipp: Es wird empfohlen, die Option [!UICONTROL None] nur für Anwendungsfälle der Migration zu verwenden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gäste können das Ereignis ändern]</td> 
   <td> <p>Aktivieren Sie diese Option, wenn Gäste dieses Ereignis ändern können sollen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Wiederholung]</td> 
   <td>Fügen Sie alle Wiederholungsregeln hinzu, die Sie auf dieses Ereignis anwenden möchten. Für jede Regel ist eine Liste von [!UICONTROL RULE], [!UICONTROL EXRULE], [!UICONTROL RDATE] und [!UICONTROL EXDATE] Zeilen für ein wiederkehrendes Ereignis erforderlich. Beachten Sie, dass [!UICONTROL DTSTART]- und [!UICONTROL DTEND]-Zeilen in diesem Feld nicht zulässig sind. Start- und Endzeiten von Ereignissen werden in den Start- und Endfeldern angegeben. Dieses Feld wird für einzelne Ereignisse oder Instanzen wiederkehrender Ereignisse weggelassen. Weitere Informationen finden Sie unter <a href="https://tools.ietf.org/html/rfc5545#section-3.8.5">RFC5545</a>.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ereignis aktualisieren]

Dieses Aktionsmodul ändert ein vorhandenes Ereignis.

Kalender und Ereignis-ID angeben.

Das Modul gibt die ID des Ereignisses und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Kalender] </td> 
   <td> <p>Wählen Sie den Kalender aus, mit dem Sie arbeiten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ereignis-ID] </td> 
   <td> <p>Geben Sie die Ereignis-ID aus dem zuvor erstellten [!DNL Google Calendar] ein, das Sie aktualisieren möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

Sie können die Ereignisinformationen aktualisieren, indem Sie neue Werte in das gewünschte Feld eingeben. Einzelheiten zu den einzelnen Feldern finden Sie unter [[!UICONTROL Erstellen eines Ereignisses]](#create-an-event).

#### [!UICONTROL Ereignis löschen]

Dieses Aktionsmodul löscht ein Ereignis.

Kalender und Ereignis-ID angeben.

Das Modul gibt die ID des Ereignisses und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalenderkennung]</td> 
   <td> <p>Wählen Sie den Kalender aus, der das Ereignis enthält, das Sie löschen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ereignis-ID]</td> 
   <td> <p> Geben Sie die Ereignis-ID aus einem zuvor erstellten [!DNL Google Calendar] ein, das Sie löschen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benachrichtigung über das Löschen des Ereignisses senden]</td> 
   <td>Wählen Sie aus, ob Sie Benachrichtigungen über die Löschung des Ereignisses an alle Gäste, Gäste, die [!DNL Google Calendar] nicht verwenden, oder an niemanden senden möchten.</td> 
  </tr> 
 </tbody> 
</table>

### Kalender

* [[!UICONTROL Kalender auflisten]](#list-calendars)
* [[!UICONTROL Kalender abrufen]](#get-a-calendar)
* [[!UICONTROL Kalender erstellen]](#create-a-calendar)
* [[!UICONTROL Aktualisieren eines Kalenders]](#update-a-calendar)
* [[!UICONTROL Löschen eines Kalenders]](#delete-a-calendar)
* [[!UICONTROL Löschen eines Kalenders]](#clear-a-calendar)

#### [!UICONTROL Kalender auflisten]

Dieses Aktionsmodul gibt die Kalender aus der Kalenderliste eines Benutzers zurück.

Das Modul gibt die ID des Kalenders und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Minimum access role]</td> 
   <td> <p>Wählen Sie die Mindestzugriffsrolle für den Benutzer aus. Das Modul gibt Kalender zurück, die auf dieser Mindestzugriffsrolle basieren.</p> 
    <ul> 
     <li><strong>[!UICONTROL Frei/Gebucht-Reader]</strong>: Der Benutzer kann Frei/Gebucht-Informationen lesen. </li> 
     <li><strong>[!UICONTROL Inhaber]</strong>: Der Benutzer kann Ereignisse lesen und ändern und auf Kontrolllisten zugreifen. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: Der Benutzer kann nicht private Ereignisse lesen. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: Der Benutzer kann Ereignisse lesen und ändern.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ausgeblendete Kalender anzeigen]</td> 
   <td>Aktivieren Sie diese Option, um ausgeblendete Kalender in die vom Modul zurückgegebene Liste aufzunehmen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Legen Sie die maximale Anzahl von Kalendern fest, [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgegeben werden.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kalender abrufen]

Dieses Aktionsmodul ruft einen Kalender ab.

Sie geben die ID des Kalenders an, den Sie abrufen möchten.

Das Modul gibt die ID des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalenderkennung]</td> 
   <td> <p>Wählen Sie den Kalender aus, den Sie abrufen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kalender erstellen]

Dieses Aktionsmodul erstellt einen neuen Kalender.

Sie geben einen Namen für den Kalender an.

Das Modul gibt die ID des Kalenders und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalendername]</td> 
   <td> <p> Geben Sie einen Namen für den neuen Kalender ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aktualisieren eines Kalenders]

Dieses Aktionsmodul aktualisiert einen Kalender.

Sie geben die ID des Kalenders an, den Sie aktualisieren möchten.

Das Modul gibt die ID des Kalenders und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalenderkennung]</td> 
   <td> <p>Wählen Sie den Kalender aus, den Sie aktualisieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalendername]</td> 
   <td> <p> Geben Sie einen neuen Namen für den Kalender ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Löschen eines Kalenders]

Dieses Aktionsmodul löscht einen Kalender.

Sie geben die ID des Kalenders an, den Sie löschen möchten.

Das Modul gibt die ID des Kalenders und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalenderkennung]</td> 
   <td> <p>Geben Sie die ID des Kalenders ein, den Sie löschen möchten, oder mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Löschen eines Kalenders]

Dieses Aktionsmodul entfernt alle Ereignisse aus dem primären Kalender eines Kontos.

Sie geben die Verbindung an, die eine Verbindung zu dem Konto herstellt, das den Kalender enthält, den Sie löschen möchten.

Das Modul gibt die ID des Kalenders und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
 </tbody> 
</table>

### Zugriffssteuerungsregeln

* [[!UICONTROL Regeln für die Zugriffssteuerung auflisten]](#list-access-control-rules)
* [[!UICONTROL Zugriffssteuerungsregel abrufen]](#get-an-access-control-rule)
* [[!UICONTROL Erstellen einer Zugriffssteuerungsregel]](#create-an-access-control-rule)
* [[!UICONTROL Aktualisieren einer Zugriffssteuerungsregel]](#update-an-access-control-rule)
* [[!UICONTROL Löschen einer Zugriffssteuerungsregel]](#delete-an-access-control-rule)

#### [!UICONTROL Regeln für die Zugriffssteuerung auflisten]

Dieses Aktionsmodul gibt die Regeln in der Zugriffssteuerungsliste für einen Kalender zurück.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalenderkennung]</td> 
   <td> <p>Wählen Sie den Kalender aus, der die Zugriffssteuerungsregeln enthält, die Sie abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Legen Sie die maximale Anzahl von Ergebnissen fest, [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgegeben werden.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Zugriffssteuerungsregel abrufen]

Dieses Aktionsmodul gibt die Metadaten einer Zugriffssteuerungsregel zurück.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalenderkennung]</td> 
   <td> <p>Wählen Sie den Kalender aus, der die Zugriffssteuerungsregel enthält, die Sie abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zugriffssteuerungsregel-ID]</td> 
   <td>Wählen Sie die Zugriffssteuerungsregel aus, die Sie abrufen möchten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen einer Zugriffssteuerungsregel]

Dieses Aktionsmodul erstellt eine neue Zugriffssteuerungsregel.

Sie geben einen Namen für den Kalender an.

Das Modul gibt die ID der Zugriffssteuerungsregel und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalenderkennung]</td> 
   <td> <p>Wählen Sie den Kalender aus, in dem Sie eine Zugriffssteuerungsregel erstellen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td> <p>Wählen Sie die Rolle aus, die der Zugriffsregel zugewiesen werden soll. </p> 
    <ul> 
     <li><strong>[!UICONTROL Frei/Gebucht-Reader]</strong>: Der Benutzer kann Frei/Gebucht-Informationen lesen. </li> 
     <li><strong>[!UICONTROL Inhaber]</strong>: Der Benutzer kann Ereignisse lesen und ändern und auf Kontrolllisten zugreifen. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: Der Benutzer kann nicht private Ereignisse lesen. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: Der Benutzer kann Ereignisse lesen und ändern.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Typ]</td> 
   <td> <p>Wählen Sie den Typ des Umfangs aus. </p> 
    <ul> 
     <li><strong>[!UICONTROL default]</strong>: Der öffentliche Bereich. Dies ist der Standardwert. </li> 
     <li><strong>[!UICONTROL User]</strong>: Beschränkt den Gültigkeitsbereich auf einen einzelnen Benutzer. </li> 
     <li><strong>[!UICONTROL Group]</strong>: Beschränkt den Gültigkeitsbereich auf eine Gruppe. </li> 
     <li><strong>[!UICONTROL Domain]</strong>: Beschränkt den Gültigkeitsbereich auf eine Domain. </li> 
    </ul> <p>Hinweis: Die dem [!UICONTROL Default]-Bereich oder dem öffentlichen Bereich gewährten Berechtigungen gelten für alle Benutzer, unabhängig davon, ob sie authentifiziert sind oder nicht.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Wert]</td> 
   <td>Geben Sie je nach Bereichstyp die E-Mail-Adresse eines Benutzers oder einer Gruppe oder den Namen einer Domain ein.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benachrichtigungen senden]</td> 
   <td> <p>Aktivieren Sie diese Option, um Benachrichtigungen über die Zugriffsänderung zu senden. </p> <p>Hinweis: Es gibt keine Benachrichtigungen zum Entfernen des Zugriffs. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aktualisieren einer Zugriffssteuerungsregel]

Dieses Aktionsmodul aktualisiert eine Zugriffssteuerungsregel.

Sie geben einen Namen für den Kalender an.

Das Modul gibt die ID der Zugriffssteuerungsregel und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalenderkennung]</td> 
   <td> <p>Wählen Sie den Kalender aus, der die Zugriffssteuerungsregel enthält, die Sie aktualisieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zugriffssteuerungsregel-ID]</td> 
   <td>Wählen Sie die Zugriffssteuerungsregel aus, die Sie aktualisieren möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Role]</td> 
   <td> <p>Wählen Sie die Rolle aus, die der Zugriffsregel zugewiesen werden soll. </p> 
    <ul> 
     <li><strong>[!UICONTROL None]</strong>: Diese Rolle bietet keinen Zugriff.</li> 
     <li><strong>[!UICONTROL Frei/Gebucht-Reader]</strong>: Der Benutzer kann Frei/Gebucht-Informationen lesen. </li> 
     <li><strong>[!UICONTROL Inhaber]</strong>: Der Benutzer kann Ereignisse lesen und ändern und auf Kontrolllisten zugreifen. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: Der Benutzer kann nicht private Ereignisse lesen. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: Der Benutzer kann Ereignisse lesen und ändern.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benachrichtigungen senden]</td> 
   <td> <p>Aktivieren Sie diese Option, um Benachrichtigungen über die Zugriffsänderung zu senden. </p> <p>Hinweis: Es gibt keine Benachrichtigungen zum Entfernen des Zugriffs. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Löschen einer Zugriffssteuerungsregel]

Dieses Aktionsmodul löscht eine Zugriffssteuerungsregel.

Sie geben einen Namen für den Kalender an.

Das Modul gibt die ID der Zugriffssteuerungsregel und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalenderkennung]</td> 
   <td> <p>Wählen Sie die ID des Kalenders aus, der die zu löschende Zugriffssteuerungsregel enthält, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zugriffssteuerungsregel-ID]</td> 
   <td>Wählen Sie die ID der Zugriffssteuerungsregel aus, die Sie löschen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

### Iteratoren (veraltet)

Die Module [!UICONTROL Anlagen ] und [!UICONTROL Teilnehmer ]) werden nicht mehr unterstützt. Um Anlagen oder Teilnehmer zu iterieren, verwenden Sie das Modul [!UICONTROL Flusskontrolle] > [!UICONTROL Iterator]. Weitere Informationen finden Sie unter [Iterator-Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)

### Sonstige

* [[!UICONTROL Erstellen eines API-Aufrufs]](#make-an-api-call)
* [[!UICONTROL Erhalten Sie Frei/Gebucht-Informationen]](#get-freebusy-information)

#### [!UICONTROL Erstellen eines API-Aufrufs]

Mit diesem Modul können Sie einen benutzerdefinierten API-Aufruf durchführen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung zu Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>Geben Sie einen Pfad relativ zu <code>https://www.googleapis.com/calendar</code> ein. Beispiel: <code>/v3/users/me/calendarList</code></td> 
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

#### [!UICONTROL Erhalten Sie Frei/Gebucht-Informationen]

Dieses Aktionsmodul gibt Frei- und Belegt-Informationen für eine Reihe von Kalendern zurück.

Das Modul gibt die ID des Kalenders und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Beim Konfigurieren dieses Moduls werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL-Verbindung] </td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit Workfront Fusion finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Verbindung zu Adobe Workfront Fusion herstellen - Grundanweisungen</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mindestzeit]</td> 
   <td> <p> Geben Sie den Beginn des Intervalls ein, für das Sie Informationen abrufen möchten.</p> <p> Eine Liste der unterstützten Datums- und Zeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typzwang in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Zeit]</td> 
   <td> <p> Geben Sie das Ende des Intervalls ein, für das Sie Informationen abrufen möchten. </p> <p>Eine Liste der unterstützten Datums- und Zeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typzwang in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL-Kalender]</td> 
   <td> <p>Klicken Sie für jeden Kalender, aus dem Sie Informationen abrufen möchten, auf <strong>Hinzufügen</strong> und geben Sie die Kalender-ID ein oder mappen Sie sie.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Trigger eines Szenarios vor einem Ereignis

Trigger Sie können ein Szenario zu einer bestimmten Zeit vor einem Ereignis mithilfe von standardmäßigen [!DNL Google Calendar]-E-Mail-Erinnerungen und dem Modul [!UICONTROL Webhooks] >[!UICONTROL Benutzerdefinierter ]).

1. Verwenden Sie das Modul [!UICONTROL Google] >[!UICONTROL Ereignis aktualisieren], um eine E-Mail-Erinnerung zu Ihrem Ereignis hinzuzufügen:

   ![](assets/trigger-scen-before-event-350x209.png)

1. Erstellen Sie ein neues Szenario, das mit dem Modul [!UICONTROL Webhooks] > [!UICONTROL Benutzerdefinierter Mailhook] beginnt.

   1. Kopieren Sie die E-Mail-Adresse des Postfachs.
   1. Speichern Sie das Szenario und führen Sie es aus.

1. Leiten Sie [!DNL Gmail] die E-Mail-Erinnerungen an die E-Mail-Adresse des E-Mail-Hooks [!DNL Google Calendar]:

   1. Öffnen Sie Ihre **[!UICONTROL [!DNL Gmail]Einstellungen]**.
   1. Öffnen Sie die **[!UICONTROL „Weiterleitung und POP/IMAP]** .
   1. Klicken Sie **[!UICONTROL Weiterleitungsadresse hinzufügen].**
   1. Fügen Sie die kopierte E-Mail-Adresse der Mailhooks ein, klicken Sie auf &#x200B;**[!UICONTROL Weiter]**, bestätigen Sie, indem Sie **[!UICONTROL Fortfahren]** im Popup-Fenster drücken, und klicken Sie dann auf **[!UICONTROL OK]**.

   1. Wechseln Sie [!DNL Workfront Fusion] zu dem neuen Szenario, das seine Ausführung abschließen soll, indem Sie die Bestätigungs-E-Mail erhalten.
   1. Klicken Sie auf die Blase über dem Modul, um die Ausgabe des Moduls zu überprüfen.
   1. Erweitern Sie das `Text` und kopieren Sie den Bestätigungs-Code:

      ![](assets/confirmation-code-350x252.png)

   1. Fügen Sie in Gmail den Bestätigungs-Code in das Bearbeitungsfeld ein und klicken Sie auf &#x200B;**[!UICONTROL Überprüfen]**:

      ![](assets/paste-code-350x46.png)

   1. Öffnen Sie die **[!UICONTROL Filter und blockierte Adressen]**.
   1. Klicken Sie **[!UICONTROL Neuen Filter erstellen]**.
   1. Richten Sie einen Filter für alle E-Mails ein, die von `     calendar-notification@google.com` stammen, und klicken &#x200B;**[!UICONTROL Filter erstellen]**:
   1. Wählen **[!UICONTROL Weiterleiten an]** und wählen Sie die E-Mail-Adresse der E-Mail-Hooks aus der Liste aus.
   1. Klicken Sie **[!UICONTROL Filter erstellen]**, um den Filter zu erstellen.

1. (Optional) Fügen Sie [!DNL Workfront Fusion] das Modul [!UICONTROL Text-Parser] > [!UICONTROL Match Pattern] nach dem Modul [!UICONTROL Webhooks] > [!UICONTROL Custom Mailhook] hinzu, um den HTML-Code der E-Mail zu analysieren und alle benötigten Informationen zu erhalten.

   Sie können beispielsweise das Modul wie folgt konfigurieren, um die Ereignis-ID abzurufen:

   *Muster*: `<meta itemprop="eventId/googleCalendar" content="(?<evenitID>.*?)"/>`

   *Text*: Das `HTML content` Element, das vom Modul [!UICONTROL Webhooks] >[!UICONTROL Benutzerdefinierter Mailhook] ausgegeben wird.
