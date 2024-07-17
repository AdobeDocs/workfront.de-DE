---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;calendars
keywords: Connector
navigation-topic: apps-and-their-modules
title: Google-Kalendermodule
description: In einem [!DNL Adobe Workfront Fusion] szenario können Sie Workflows automatisieren, die den Google-Kalender verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 168e8fce-645d-4108-84b7-46a113c83f41
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '3817'
ht-degree: 0%

---

# [!DNL Google Calendar] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!UICONTROL Google-Kalender] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

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

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Um [!DNL Google Calendar] -Module zu verwenden, müssen Sie über ein [!DNL Google] -Konto verfügen.

## [!DNL Google Calendar] Module und ihre Felder

Wenn Sie [!DNL Google Calendar] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Google Calendar] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Veranstaltungen](#events)
* [Kalender](#calendars)
* [Zugriffskontrollregeln](#access-control-rules)
* [Iteratoren (nicht mehr unterstützt)](#iterators-deprecated)
* [Sonstige](#other)

### Veranstaltungen

* [[!UICONTROL Ereignisse ansehen]](#watch-events)
* [[!UICONTROL Suchereignisse]](#search-events)
* [[!UICONTROL Ereignis abrufen]](#get-an-event)
* [[!UICONTROL Ereignis erstellen]](#create-an-event)
* [[!UICONTROL Ereignis aktualisieren]](#update-an-event)
* [[!UICONTROL Ereignis löschen]](#delete-an-event)


#### [!UICONTROL Ereignisse ansehen]

Dieses Trigger-Modul führt ein Szenario aus, wenn ein neues Ereignis im angegebenen Kalender hinzugefügt, aktualisiert, gelöscht, gestartet oder beendet wird. Das Modul gibt alle mit dem Datensatz oder den Datensätzen verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalender] </td> 
   <td> <p>Wählen Sie den Kalender aus, mit dem das Modul arbeiten soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Überwachungsereignisse]</td> 
   <td> <p>Wählen Sie aus, ob Sie Ereignisse nach Erstellungsdatum, Aktualisierungsdatum, Startdatum oder Enddatum verfolgen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gelöschte Ereignisse anzeigen]</td> 
   <td> <p>Aktivieren Sie diese Option, um gelöschte Ereignisse einzuschließen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abfrage] </td> 
   <td> <p>Geben Sie den Text ein, nach dem Sie suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Ereignissen fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeitet (die Anzahl der Wiederholungen pro Szenario-Ausführung). Wenn der Wert zu hoch eingestellt ist, kann die Verbindung auf der Seite des angegebenen Drittanbieterdienstes unterbrochen werden (Timeout). [!DNL Workfront Fusion] hat keinen Einfluss darauf. Es wird empfohlen, einen niedrigeren Wert festzulegen und entweder einen höheren Wert für die maximale Anzahl von Zyklen zu definieren oder das Szenario häufiger auszuführen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Suchereignisse]

Dieses Aktionsmodul sucht im ausgewählten Kalender nach einem Ereignis.

Sie geben den Kalender und die Suchparameter an.

Das Modul gibt die ID des Ereignisses sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit Workfront Fusion finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe Workfront Fusion - Grundlegende Anweisungen</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalender-ID]</td> 
   <td> <p>Wählen Sie den Kalender aus, den Sie suchen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Startdatum]</td> 
   <td> <p> Geben Sie das Datum für den Beginn des Ereignisses ein oder ordnen Sie es zu. Dieses Modul ruft auch Ereignisse ab, die vor diesem Datum beginnen und noch am eingegebenen Startdatum auftreten. </p> <p>Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enddatum]</td> 
   <td> <p> Geben Sie das Datum zum Ende des Ereignisses ein oder ordnen Sie es zu. </p> <p> Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Einzelereignisse]</td> 
   <td> <p> Aktivieren Sie diese Option, um wiederkehrende Ereignisse als einzelne Instanzen zu behandeln. Wenn Sie beispielsweise ein wöchentliches Meeting haben und diese Option aktiviert ist, gibt das Modul das Meeting jeder Woche als separate Veranstaltung zurück.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Abfrage]</td> 
   <td> <p>Geben Sie den Suchbegriff, nach dem Sie suchen möchten, ein oder ordnen Sie ihn zu. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reihenfolge nach]</td> 
   <td> <p>Wählen Sie die Reihenfolge der im Ergebnis zurückgegebenen Ereignisse aus.</p> 
    <ul> 
     <li><strong>[!UICONTROL Startzeit]</strong>: Reihenfolge nach Startdatum und -zeit (aufsteigend). Dies ist nur bei der Abfrage einzelner Ereignisse verfügbar.</li> 
     <li><strong>[!UICONTROL Aktualisierte Zeit]</strong>: Reihenfolge der letzten Änderung (aufsteigend).</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p>Legen Sie die maximale Anzahl von Ereignissen fest, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgibt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ereignis abrufen]

Dieses Aktionsmodul gibt die Metadaten für ein einzelnes Ereignis im angegebenen Kalender zurück.

Sie geben den Kalender und das Ereignis an.

Das Modul gibt die ID des Ereignisses und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalender-ID]</td> 
   <td> <p>Geben Sie die Kennung des Kalenders ein oder ordnen Sie sie zu, der das gewünschte Ereignis enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ereignis-ID] </td> 
   <td> <p>Geben Sie die Ereignis-ID des vorhandenen [!DNL Google Calendar] -Ereignisses ein, das Sie abrufen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ereignis erstellen]

Dieses Aktionsmodul erstellt ein Ereignis.

Sie geben den Kalender und die Parameter für das Ereignis an.

Das Modul gibt die ID des Ereignisses sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit Workfront Fusion finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe Workfront Fusion - Grundlegende Anweisungen</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ereignis erstellen]</td> 
   <td> <p>Wählen Sie aus, wie das Ereignis erstellt werden soll.</p> 
    <ul> 
     <li><b>[!UICONTROL im Detail]</b><p>Mit dieser Option können Sie detailliertere Informationen zum Ereignis bereitstellen.<br></p></li> 
     <li><b>[!UICONTROL Schnell]</b><p>Sie müssen nur den Kalender auswählen und einen Namen für das Ereignis eingeben. Sie können Zeit- und Ortsdetails in den Namen einschließen und [!DNL Google Calendar] plant das Ereignis für diesen Ort und diese Uhrzeit.</p></li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalender-ID]</td> 
   <td> <p>Wählen Sie den Kalender aus, in dem das Ereignis angezeigt werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Farbe]</td> 
   <td>Wählen Sie die Farbe aus, die das Ereignis im Kalender anzeigt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ereignisname]</td> 
   <td> <p> Geben Sie einen Namen für das Ereignis ein oder ordnen Sie ihn zu. </p> <p>Hinweis: Wenn Sie [!UICONTROL Quick Add] im Feld [!UICONTROL Ereignis erstellen] ausgewählt haben, können Sie das Datum und die Uhrzeit des Ereignisses angeben und [!DNL Workfront Fusion] erstellt das Ereignis für dieses Datum und diese Uhrzeit. Beispiel: <code>Appointment at Capitol Hill on June 3rd 10am-10:25am</code>. Wenn Sie [!UICONTROL Quick Add] ausgewählt haben, aber kein Datum und keine Uhrzeit in den Ereignisnamen einschließen, wird das Ereignis von der aktuellen Zeit aus erstellt und dauert eine Stunde.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ganztägiges Ereignis]</td> 
   <td>Aktivieren Sie diese Option, wenn es sich bei dem Ereignis um ein ganztägiges Ereignis handelt (keine Start- und Endzeiten erforderlich sind).</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Startdatum]</td> 
   <td> <p>Wenn es sich um ein ganztägiges Ereignis handelt, geben Sie das Startdatum des Ereignisses ein. </p> <p>Eine Liste der unterstützten Datumsformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Enddatum]</td> 
   <td> <p> Wenn es sich um ein ganztägiges Ereignis handelt, geben Sie das Enddatum des Ereignisses ein. </p> <p>Eine Liste der unterstützten Datumsformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Beschreibung]</td> 
   <td>Geben Sie eine Beschreibung für das Ereignis ein oder ordnen Sie es zu. Dieses Feld unterstützt HTML.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Standort]</td> 
   <td>Geben Sie einen Ort für das Ereignis im Textformular ein.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Verwenden Sie die standardmäßigen Erinnerungseinstellungen für dieses Ereignis]</td> 
   <td>Aktivieren Sie diese Option, um die standardmäßigen Erinnerungseinstellungen zu verwenden. Wenn Sie eine benutzerdefinierte Erinnerung im Feld [!UICONTROL Erinnerung] festlegen, wird dieser Wert auf "Nein"gesetzt.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Reminder] </td> 
   <td> <p>Fügen Sie eine Erinnerung für das Ereignis hinzu. Wählen Sie für jede Erinnerung die Methode aus, an die Sie erinnert werden möchten, und definieren Sie, wie lange (in Minuten) vor dem Ereignis, an das Sie erinnert werden möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Teilnehmer]</td> 
   <td>Fügen Sie die Teilnehmer zum Ereignis hinzu. Geben Sie für jeden Teilnehmer seinen Namen und seine E-Mail-Adresse ein oder ordnen Sie sie zu.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Anzeigen als]</td> 
   <td>Wählen Sie aus, ob Personen, die Ihren Kalender anzeigen, Sie während dieser Veranstaltung als beschäftigt oder verfügbar anzeigen sollen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sichtbarkeit] </td> 
   <td> <p>Wählen Sie die Sichtbarkeit dieses Ereignisses aus. </p> 
    <ul> 
     <li> <p><b>[!UICONTROL Standard]</b></p> <p>Das Ereignis hat die Sichtbarkeit, die Sie in Ihren Kalendereinstellungen festgelegt haben.</p> </li> 
     <li> <p><b>[!UICONTROL Public]</b></p> <p>Jeder, für den der Kalender freigegeben ist, kann dieses Ereignis sehen.</p> </li> 
     <li> <p><b>[!UICONTROL Private]</b></p> <p>Dieses Ereignis kann nur von Teilnehmern angezeigt werden.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benachrichtigung zur Ereigniserstellung senden]</td> 
   <td> <p>Wählen Sie aus, ob Benachrichtigungen über die Erstellung eines neuen Ereignisses an alle Gäste, Nicht-[!DNL Google Calendar]-Gäste oder an niemanden gesendet werden sollen.</p> <p>Tipp: Es wird empfohlen, die Option [!UICONTROL None] nur für Migrationsanwendungsfälle zu verwenden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Gäste können das Ereignis ändern]</td> 
   <td> <p>Aktivieren Sie diese Option, wenn Sie möchten, dass Gäste dieses Ereignis ändern können.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Recurence]</td> 
   <td>Fügen Sie alle Wiederholungsregeln hinzu, die Sie auf dieses Ereignis anwenden möchten. Für jede Regel ist eine Liste der Zeilen [!UICONTROL RRULE], [!UICONTROL EXRULE], [!UICONTROL RDATE] und [!UICONTROL EXDATE] für ein wiederkehrendes Ereignis erforderlich. Beachten Sie, dass die Zeilen [!UICONTROL DTSTART] und [!UICONTROL DTEND] in diesem Feld nicht zulässig sind. Start- und Endzeiten von Ereignissen werden in den Start- und Endfeldern angegeben. Dieses Feld wird für einzelne Ereignisse oder Instanzen wiederkehrender Ereignisse weggelassen. Weitere Informationen finden Sie unter <a href="https://tools.ietf.org/html/rfc5545#section-3.8.5">RFC5545</a>.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Ereignis aktualisieren]

Dieses Aktionsmodul ändert ein vorhandenes Ereignis.

Sie geben den Kalender und die Ereignis-ID an.

Das Modul gibt die ID des Ereignisses sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalender] </td> 
   <td> <p>Wählen Sie den Kalender aus, mit dem Sie arbeiten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ereignis-ID] </td> 
   <td> <p>Geben Sie die Ereignis-ID aus dem zuvor erstellten [!DNL Google Calendar] -Ereignis ein, das Sie aktualisieren möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

Sie können die Ereignisinformationen aktualisieren, indem Sie neue Werte in das gewünschte Feld eingeben. Weitere Informationen zu den einzelnen Feldern finden Sie unter [[!UICONTROL Ereignis erstellen]](#create-an-event).

#### [!UICONTROL Ereignis löschen]

Dieses Aktionsmodul löscht ein Ereignis.

Sie geben den Kalender und die Ereignis-ID an.

Das Modul gibt die ID des Ereignisses sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalender-ID]</td> 
   <td> <p>Wählen Sie den Kalender aus, der das Ereignis enthält, das Sie löschen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ereignis-ID]</td> 
   <td> <p> Geben Sie die Ereignis-ID aus einem zuvor erstellten [!DNL Google Calendar] -Ereignis ein, das Sie löschen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benachrichtigung zum Löschen des Ereignisses senden]</td> 
   <td>Wählen Sie aus, ob Sie Benachrichtigungen zum Löschen des Ereignisses an alle Gäste, Gäste, die nicht [!DNL Google Calendar] verwenden, oder an niemanden senden möchten.</td> 
  </tr> 
 </tbody> 
</table>

### Kalender

* [[!UICONTROL Listenkalender]](#list-calendars)
* [[!UICONTROL Einen Kalender abrufen]](#get-a-calendar)
* [[!UICONTROL Erstellen eines Kalenders]](#create-a-calendar)
* [[!UICONTROL Aktualisieren eines Kalenders]](#update-a-calendar)
* [[!UICONTROL Löschen eines Kalenders]](#delete-a-calendar)
* [[!UICONTROL Löschen eines Kalenders]](#clear-a-calendar)

#### [!UICONTROL Listenkalender]

Dieses Aktionsmodul gibt die Kalender in der Kalenderliste eines Benutzers zurück.

Das Modul gibt die Kennung des Kalenders sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mindestzugriffsrolle]</td> 
   <td> <p>Wählen Sie die Mindestzugriffsrolle für den Benutzer aus. Das Modul gibt Kalender basierend auf dieser minimalen Zugriffsrolle zurück.</p> 
    <ul> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong>: Der Benutzer kann freie/geschäftige Informationen lesen. </li> 
     <li><strong>[!UICONTROL Inhaber]</strong>: Der Benutzer kann Ereignisse lesen und ändern und auf Kontrolllisten zugreifen. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: Der Benutzer kann Ereignisse lesen, die nicht privat sind. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: Der Benutzer kann Ereignisse lesen und ändern.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verborgene Kalender anzeigen]</td> 
   <td>Aktivieren Sie diese Option, um ausgeblendete Kalender in die Liste einzuschließen, die das Modul zurückgibt.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Legen Sie die maximale Anzahl von Kalendern fest, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgibt.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Einen Kalender abrufen]

Dieses Aktionsmodul ruft einen Kalender ab.

Sie geben die Kennung des Kalenders an, den Sie abrufen möchten.

Das Modul gibt die Kennung des Datensatzes und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalender-ID]</td> 
   <td> <p>Wählen Sie den Kalender aus, den Sie abrufen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen eines Kalenders]

Dieses Aktionsmodul erstellt einen neuen Kalender.

Sie geben einen Namen für den Kalender an.

Das Modul gibt die Kennung des Kalenders sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalendername]</td> 
   <td> <p> Geben Sie einen Namen für den neuen Kalender ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aktualisieren eines Kalenders]

Dieses Aktionsmodul aktualisiert einen Kalender.

Sie geben die Kennung des Kalenders an, den Sie aktualisieren möchten.

Das Modul gibt die Kennung des Kalenders sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalender-ID]</td> 
   <td> <p>Wählen Sie den zu aktualisierenden Kalender aus.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalendername]</td> 
   <td> <p> Geben Sie einen neuen Namen für den Kalender ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Löschen eines Kalenders]

Dieses Aktionsmodul löscht einen Kalender.

Sie geben die Kennung des Kalenders an, den Sie löschen möchten.

Das Modul gibt die Kennung des Kalenders sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalender-ID]</td> 
   <td> <p>Geben Sie die Kennung des Kalenders ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Löschen eines Kalenders]

Dieses Aktionsmodul entfernt alle Ereignisse aus dem primären Kalender eines Kontos.

Sie geben die Verbindung an, die eine Verbindung zu dem Konto herstellt, das den Kalender enthält, den Sie löschen möchten.

Das Modul gibt die Kennung des Kalenders sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
 </tbody> 
</table>

### Zugriffskontrollregeln

* [[!UICONTROL Zugriffssteuerungsregeln auflisten]](#list-access-control-rules)
* [[!UICONTROL Abrufen einer Zugriffssteuerungsregel]](#get-an-access-control-rule)
* [[!UICONTROL Erstellen einer Zugriffssteuerungsregel]](#create-an-access-control-rule)
* [[!UICONTROL Aktualisieren einer Zugriffssteuerungsregel]](#update-an-access-control-rule)
* [[!UICONTROL Eine Zugriffssteuerungsregel löschen]](#delete-an-access-control-rule)

#### [!UICONTROL Zugriffssteuerungsregeln auflisten]

Dieses Aktionsmodul gibt die Regeln in der Zugriffssteuerungsliste eines Kalenders zurück.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalender-ID]</td> 
   <td> <p>Wählen Sie den Kalender aus, der die Zugriffssteuerungsregeln enthält, die Sie abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Legen Sie die maximale Anzahl von Ergebnissen fest, die [!DNL Workfront Fusion] während eines Ausführungszyklus zurückgibt.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Abrufen einer Zugriffssteuerungsregel]

Dieses Aktionsmodul gibt die Metadaten einer Zugriffssteuerungsregel zurück.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kalender-ID]</td> 
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

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalender-ID]</td> 
   <td> <p>Wählen Sie den Kalender aus, in dem Sie eine Zugriffssteuerungsregel erstellen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rolle]</td> 
   <td> <p>Wählen Sie die Rolle aus, die der Zugriffsregel zugewiesen werden soll. </p> 
    <ul> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong>: Der Benutzer kann freie/geschäftige Informationen lesen. </li> 
     <li><strong>[!UICONTROL Inhaber]</strong>: Der Benutzer kann Ereignisse lesen und ändern und auf Kontrolllisten zugreifen. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: Der Benutzer kann Ereignisse lesen, die nicht privat sind. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: Der Benutzer kann Ereignisse lesen und ändern.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Typ]</td> 
   <td> <p>Wählen Sie den Perimeter aus. </p> 
    <ul> 
     <li><strong>[!UICONTROL Standard]</strong>: Der öffentliche Bereich. Dies ist der Standardwert. </li> 
     <li><strong>[!UICONTROL Benutzer]</strong>: Beschränkt den Umfang auf einen einzelnen Benutzer. </li> 
     <li><strong>[!UICONTROL Group]</strong>: Beschränkt den Umfang auf eine Gruppe. </li> 
     <li><strong>[!UICONTROL Domain]</strong>: Beschränkt den Umfang auf eine Domäne. </li> 
    </ul> <p>Hinweis: Die Berechtigungen, die dem [!UICONTROL Standard] oder dem öffentlichen Bereich gewährt werden, gelten für alle Benutzer, ob authentifiziert oder nicht.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Wert]</td> 
   <td>Geben Sie je nach Perimeter die E-Mail-Adresse eines Benutzers oder einer Gruppe oder den Namen einer Domain an.</td> 
  </tr> 
  <tr> 
   <td>Benachrichtigungen senden:</td> 
   <td> <p>Aktivieren Sie diese Option, um Benachrichtigungen über die Zugriffsänderung zu senden. </p> <p>Hinweis: Es gibt keine Benachrichtigungen zum Entfernen des Zugriffs. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Aktualisieren einer Zugriffssteuerungsregel]

Dieses Aktionsmodul aktualisiert eine Zugriffssteuerungsregel.

Sie geben einen Namen für den Kalender an.

Das Modul gibt die ID der Zugriffssteuerungsregel und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalender-ID]</td> 
   <td> <p>Wählen Sie den Kalender aus, der die zu aktualisierende Zugriffssteuerungsregel enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zugriffssteuerungsregel-ID]</td> 
   <td>Wählen Sie die Zugriffssteuerungsregel aus, die Sie aktualisieren möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Rolle]</td> 
   <td> <p>Wählen Sie die Rolle aus, die der Zugriffsregel zugewiesen werden soll. </p> 
    <ul> 
     <li><strong>[!UICONTROL None]</strong>: Diese Rolle bietet keinen Zugriff.</li> 
     <li><strong>[!UICONTROL Free Busy Reader]</strong>: Der Benutzer kann freie/geschäftige Informationen lesen. </li> 
     <li><strong>[!UICONTROL Inhaber]</strong>: Der Benutzer kann Ereignisse lesen und ändern und auf Kontrolllisten zugreifen. </li> 
     <li><strong>[!UICONTROL Reader]</strong>: Der Benutzer kann Ereignisse lesen, die nicht privat sind. </li> 
     <li><strong>[!UICONTROL Writer]</strong>: Der Benutzer kann Ereignisse lesen und ändern.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Benachrichtigungen senden:</td> 
   <td> <p>Aktivieren Sie diese Option, um Benachrichtigungen über die Zugriffsänderung zu senden. </p> <p>Hinweis: Es gibt keine Benachrichtigungen zum Entfernen des Zugriffs. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eine Zugriffssteuerungsregel löschen]

Dieses Aktionsmodul löscht eine Zugriffssteuerungsregel.

Sie geben einen Namen für den Kalender an.

Das Modul gibt die ID der Zugriffssteuerungsregel und alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalender-ID]</td> 
   <td> <p>Wählen Sie die ID des Kalenders aus oder ordnen Sie sie zu, der die Zugriffssteuerungsregel enthält, die Sie löschen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zugriffssteuerungsregel-ID]</td> 
   <td>Wählen Sie die ID der Zugriffssteuerungsregel aus, die Sie löschen möchten, oder ordnen Sie sie zu.</td> 
  </tr> 
 </tbody> 
</table>

### Iteratoren (nicht mehr unterstützt)

Die Module [!UICONTROL iterate attachments] und [!UICONTROL iterate attendes] wurden nicht mehr unterstützt. Verwenden Sie zum Iterieren von Anlagen oder Teilnehmern das Modul [!UICONTROL Flusssteuerung] > [!UICONTROL Iterator] . Weitere Informationen finden Sie unter [Iterator-Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md)

### Sonstige

* [[!UICONTROL API-Aufruf durchführen]](#make-an-api-call)
* [[!UICONTROL Kostenlose/beladene Informationen abrufen]](#get-freebusy-information)

#### [!UICONTROL API-Aufruf durchführen]

Mit diesem Modul können Sie einen benutzerdefinierten API-Aufruf ausführen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe [!DNL Workfront Fusion] - Grundlegende Anweisungen</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td>Geben Sie einen Pfad relativ zu <code>https://www.googleapis.com/calendar</code> ein. Beispiel: <code>/v3/users/me/calendarList</code></td> 
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

#### [!UICONTROL Kostenlose/beladene Informationen abrufen]

Dieses Aktionsmodul gibt kostenlose und vielseitige Informationen für eine Reihe von Kalendern zurück.

Das Modul gibt die Kennung des Kalenders sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Verbinden Ihres [!DNL Google Calendar]-Kontos mit Workfront Fusion finden Sie unter <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Erstellen einer Verbindung mit Adobe Workfront Fusion - Grundlegende Anweisungen</a></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mindestzeit]</td> 
   <td> <p> Geben Sie den Beginn des Intervalls ein, für das Sie Informationen abrufen möchten.</p> <p> Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum time]</td> 
   <td> <p> Geben Sie das Ende des Intervalls ein, für das Sie Informationen abrufen möchten. </p> <p>Eine Liste der unterstützten Datums- und Uhrzeitformate finden Sie unter <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typerzwingung in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kalender]</td> 
   <td> <p>Klicken Sie für jeden Kalender, aus dem Sie Informationen abrufen möchten, auf <strong>Hinzufügen</strong> und geben Sie die Kalender-ID ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Trigger eines Szenarios vor einem Ereignis

Mithilfe von standardmäßigen [!DNL Google Calendar] E-Mail-Erinnerungen und dem Modul [!UICONTROL Webhooks] >[!UICONTROL Benutzerspezifischer Mailhook] können Sie ein Szenario einen bestimmten Zeitpunkt vor einem Ereignis Trigger haben.

1. Verwenden Sie das Modul [!UICONTROL Google-Kalender] >[!UICONTROL Ereignis aktualisieren] , um Ihrem Ereignis eine E-Mail-Erinnerung hinzuzufügen:

   ![](assets/trigger-scen-before-event-350x209.png)

1. Erstellen Sie ein neues Szenario, das mit dem Modul [!UICONTROL Webhooks] >[!UICONTROL Benutzerspezifischer Mailhook] beginnt.

   1. Kopieren Sie die E-Mail-Adresse des Postfachs.
   1. Speichern Sie das Szenario und führen Sie es aus.

1. Führen Sie in [!DNL Gmail] die [!DNL Google Calendar]-E-Mail-Erinnerungen an die E-Mail-Adresse des Postfachs um:

   1. Öffnen Sie Ihre **[!UICONTROL [!DNL Gmail]-Einstellungen]**.
   1. Öffnen Sie die Registerkarte **[!UICONTROL Weiterleitung und POP/IMAP]**.
   1. Klicken Sie auf **[!UICONTROL Weiterleitungsadresse hinzufügen].**
   1. Fügen Sie die E-Mail-Adresse des kopierten Mailhooks ein, klicken Sie auf &#x200B;**[!UICONTROL Weiter]**, bestätigen Sie die Eingabe durch Drücken von **[!UICONTROL Weiter]** im Popup-Fenster und klicken Sie dann auf **[!UICONTROL OK]**.

   1. Wechseln Sie in [!DNL Workfront Fusion] zum neuen Szenario, dessen Ausführung durch Erhalt der Bestätigungs-E-Mail abgeschlossen werden soll.
   1. Klicken Sie auf die Blase über dem Modul, um die Ausgabe des Moduls zu überprüfen.
   1. Erweitern Sie das Element `Text` und kopieren Sie den Bestätigungscode:

      ![](assets/confirmation-code-350x252.png)

   1. Fügen Sie in Gmail den Bestätigungscode in das Bearbeitungsfeld ein und klicken Sie auf &#x200B;**[!UICONTROL Verify]**:

      ![](assets/paste-code-350x46.png)

   1. Öffnen Sie die Registerkarte **[!UICONTROL Filter und Blockierte Adressen]** .
   1. Klicken Sie auf **[!UICONTROL Neuen Filter erstellen]**.
   1. Richten Sie einen Filter für alle E-Mails ein, die von `     calendar-notification@google.com` kommen, und klicken Sie auf &#x200B;**[!UICONTROL Filter erstellen]**:
   1. Wählen Sie **[!UICONTROL Weiterleiten an]** und wählen Sie die E-Mail-Adresse des Postfachs aus der Liste aus.
   1. Klicken Sie auf **[!UICONTROL Filter erstellen]** , um den Filter zu erstellen.

1. (Optional) Fügen Sie in [!DNL Workfront Fusion] das Modul [!UICONTROL Text parser] > [!UICONTROL Match pattern] nach dem Modul [!UICONTROL Webhooks] >[!UICONTROL Benutzerspezifischer Mailhook] hinzu, um den HTML-Code der E-Mail zu analysieren, um die benötigten Informationen abzurufen.

   Sie können das Modul beispielsweise wie folgt konfigurieren, um die ID des Ereignisses abzurufen:

   *Muster*: `<meta itemprop="eventId/googleCalendar" content="(?<evenitID>.*?)"/>`

   *Text*: Das aus dem Modul [!UICONTROL Webhooks] >[!UICONTROL Benutzerspezifischer Mailhook] ausgegebene Element `HTML content`.
