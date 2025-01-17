---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Steckverbinder
navigation-topic: apps-and-their-modules
title: E-Mail-Module
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 384ba60a-d79e-4126-a247-6d67b5154ede
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '2651'
ht-degree: 0%

---

# E-Mail-Module

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [E-Mail-Module](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/email-modules.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Ihr E-Mail-Konto mit mehreren Anwendungen und Services von Drittanbietern verbinden. Damit können Sie E-Mails über IMAP herunterladen, E-Mails über SMTP senden, neue Entwürfe erstellen, E-Mails von einem Ordner in einen anderen verschieben und kopieren, E-Mails als gelesen oder ungelesen markieren und E-Mails löschen.

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

## Verbinden Ihrer E-Mail mit Workfront Fusion {#connect-your-email-to-workfront-fusion}

* [Verbindung mit Google herstellen](#connect-to-google)
* [Herstellen einer Verbindung zu anderen E-Mail-Services (SMAP)](#connect-to-other-email-services-smap)

### Mit [!DNL Google] verbinden

Verwenden Sie diese Option, um Szenarien mit E-Mail-Modulen zu erstellen, für die eine Verbindung zu Ihrem [!DNL Google]-Konto erforderlich ist. Dies ist ein Konto mit eingeschränkten Gültigkeitsbereichen.

Sie können direkt aus einem E-Mail-Modul heraus eine Verbindung zu Ihrem [!DNL Google]-Konto herstellen.

1. Klicken Sie in einem beliebigen E **[!UICONTROL Mail-Modul]** dem Feld [!UICONTROL Verbindung] auf „Hinzufügen“.
1. Wählen Sie **[!DNL Google]** als Verbindungstyp aus.
1. Geben Sie einen Namen für die Verbindung ein.
1. (Optional) Geben Sie Ihre [!UICONTROL [!DNL Google]-Client]ID und [!UICONTROL Client-Geheimnis] ein.
1. Klicken Sie **[!UICONTROL Fortfahren]**, um die Verbindung zu erstellen, und kehren Sie zum Modul zurück.

### Herstellen einer Verbindung zu anderen E-Mail-Services (SMAP)

Mit der SMAP-Verbindung können Sie aus der Ferne auf Ihre Mailbox zugreifen und Nachrichten in Ihrer Mailbox lesen oder bearbeiten. Die SMAP-Verbindung wird von den meisten E-Mail-Modulen verwendet.

1. Klicken Sie in einem beliebigen E **[!UICONTROL Mail-Modul]** dem Feld [!UICONTROL Verbindung] auf „Hinzufügen“.
1. Wählen Sie **[!UICONTROL Sonstige (SMTP)]** als Verbindungstyp aus.
1. Geben Sie einen **[!UICONTROL Namen]** für die Verbindung ein.
1. Wählen Sie Ihren **[!UICONTROL E-Mail]** Anbieter) aus der Liste aus. Wenn Ihr E-Mail-Anbieter nicht in der Liste aufgeführt ist, wählen Sie Sonstige aus.
1. Geben Sie Ihre **[!UICONTROL E]** Mail-Adresse **[!UICONTROL Ihren]**, Ihren **[!UICONTROL Benutzernamen]** und Ihr **[!UICONTROL Kennwort]** ein.
1. (Bedingt) Wenn sich Ihr Provider nicht auf der Liste befindet, geben Sie Ihren **[!UICONTROL SMTP-Server]** und **[!UICONTROL Port]** ein und geben an, ob Sie **[!UICONTROL Sichere Verbindung (TLS) verwenden)]**. Diese Informationen finden Sie im Abschnitt [!UICONTROL Hilfe] für Ihr Postfach. Wenn Sie nicht über diese Informationen verfügen, wenden Sie sich an Ihren E-Mail-Dienstanbieter.
1. Klicken Sie **[!UICONTROL Fortfahren]**, um die Verbindung zu erstellen, und kehren Sie zum Modul zurück.

## [!UICONTROL E]Mail-Module und ihre Felder

Beim Konfigurieren von [!UICONTROL E]Mail-Modulen zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können je nach Faktoren wie Ihrer Zugriffsebene in der App oder im Service weitere Felder angezeigt werden. Ein fett gedruckter Titel in einem Modul gibt ein erforderliches Feld an.

Einige der E-Mail-Felder enthalten möglicherweise bereits Daten, da Sie diese in einem anderen Modul im Szenario verwendet haben. Weitere Informationen finden Sie in der E-Mail-Hilfe.

Wenn die Zuordnungsschaltfläche über einem Feld oder einer Funktion angezeigt wird, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Zuordnen von Informationen zu einem anderen Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>Die eindeutige E-Mail-ID [!UICONTROL E-Mail-ID (UID)] ist die Kennung der E-Mail. Die E-Mail-ID ist für jeden Ordner der E-Mail spezifisch.

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Iteratoren](#iterators)

### Trigger

#### [!UICONTROL E-Mails ansehen]

Trigger beim Empfang einer neuen E-Mail zur Verarbeitung gemäß den angegebenen Kriterien.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres E-Mail-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Verbinden Ihrer E-Mail mit [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Ordner] </td> 
   <td> <p>Wählen Sie den Ordner aus, der E-Mails enthält, die Sie beobachten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Kriterien]</p> </td> 
   <td> <p>Wählen Sie die Kriterien aus, nach denen Sie E-Mails ansehen möchten:</p> 
    <ul> 
     <li>[!UICONTROL Alle E-Mails]</li> 
     <li>[!UICONTROL Nur E-Mails lesen]</li> 
     <li>[!UICONTROL only Unread Emails]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Absender-E-Mail-Adresse] </td> 
   <td> <p>Geben Sie die E-Mail-Adresse des Absenders ein, dessen E-Mails Sie beobachten möchten.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Empfänger-E-Mail-Adresse]</td> 
   <td> <p> Geben Sie die E-Mail-Adresse des Empfängers ein, dessen E-Mails Sie beobachten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Betreff] </td> 
   <td> <p>Geben Sie den Betreff der E-Mail ein, die Sie beobachten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Phrase] </td> 
   <td> <p>Geben Sie Schlüsselwörter ein, um nur E-Mails mit bestimmten Phrasen anzusehen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nachricht(en) beim Abrufen als gelesen markieren]</td> 
   <td> <p>Aktivieren Sie diese Option, um die ungelesene E-Mail nach dem Abrufen der Details als gelesen zu markieren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl an Ergebnissen]</td> 
   <td> <p> Die maximale Anzahl von E-Mails, die [!DNL Workfront Fusion] während eines Szenario-Ausführungszyklus zurückgeben sollten.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL E-Mail senden]](#send-an-email)
* [[!UICONTROL Entwurf erstellen]](#create-a-draft)
* [[!UICONTROL Markieren einer E-Mail als gelesen]](#mark-an-email-as-read)
* [[!UICONTROL Markieren einer E-Mail als ungelesen]](#mark-an-email-as-unread)
* [[!UICONTROL Verschieben einer E-Mail]](#move-an-email)
* [[!UICONTROL Kopieren einer E-Mail]](#copy-an-email)
* [[!UICONTROL E-Mail löschen]](#delete-an-email)
* [[!UICONTROL E-Mails abrufen]](#get-emails)

#### [!UICONTROL E-Mail senden]

Sendet eine neue E-Mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres E-Mail-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Verbinden Ihrer E-Mail mit [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nachricht nach dem Senden speichern]</td> 
   <td>Nachdem die E-Mail gesendet wurde, wird sie in Ihrem Postfach gespeichert. Aktivieren Sie diese Option, wenn Sie die mit [!DNL Workfront Fusion] gesendeten E-Mails im <i>[!UICONTROL Sent Mail]</i>-Ordner oder einem anderen Ordner in Ihrem Postfach speichern möchten. Einige E-Mail-Dienste, z. B. [!DNL Gmail], speichern gesendete Nachrichten automatisch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL nach] </td> 
   <td> <p>Fügen Sie die E-Mail-Adressen hinzu, an die Sie die E-Mail senden möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Betreff] </td> 
   <td> <p>Geben Sie die Betreffzeile der E-Mail ein oder mappen Sie sie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Content-Typ]</p> </td> 
   <td> <p>Wählen Sie den [!UICONTROL content]-Typ für die E-Mail aus:</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL plaintext]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Inhalt] </td> 
   <td> <p>Geben Sie den E-Mail-Inhalt im HTML-Format mithilfe von HTML-Tags ein oder mappen Sie ihn im Klartext, je nachdem, was Sie im Feld [!UICONTROL Content-Typ] ausgewählt haben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Anlagen]</p> </td> 
   <td> <p>Anlage hinzufügen:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Dateiname]</strong> </p> <p>Geben Sie den Dateinamen ein. Beispiel: sample.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL-Daten]</strong> </p> <p>Geben Sie den Pfad zum Ordner ein, in den die Anlage hochgeladen werden soll.</p> </li> 
     <li> <p><strong>[!UICONTROL content-ID]</strong> </p> <p>Geben Sie die [!UICONTROL Inhalts-ID] ein, um den Anhang (das Bild) in den Inhalt einzufügen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Empfänger kopieren] </td> 
   <td> <p>Geben Sie eine oder mehrere E-Mail-Adressen ein, an die Sie eine Kopie dieser E-Mail senden möchten, oder ordnen Sie sie zu. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Blind Copy-Empfänger]</td> 
   <td> <p> Geben Sie eine oder mehrere E-Mail-Adressen ein, an die Sie eine Kopie dieser E-Mail senden möchten, ohne dass die E-Mail-Adresse in der E-Mail angezeigt wird, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL from] </td> 
   <td> <p>Geben Sie die E-Mail-Adresse (und ggf. den Namen) ein, die im Feld [!UICONTROL Von] in der E-Mail angezeigt wird, oder ordnen Sie sie zu. </p> <p>Wichtig: Verwenden Sie die richtige Syntax: <code>name@email.com</code> oder <code>"Name" name@email.com</code>.</p> <p>Hinweis: Normalerweise verwendet [!DNL Workfront Fusion] die E-Mail-Adresse, die Sie beim Erstellen der Verbindung eingegeben haben, als Absenderadresse. Wenn Sie eine andere E-Mail-Adresse eingeben, kann beim Senden einer Nachricht ein Fehler auftreten, da Ihr Konto möglicherweise nicht berechtigt ist, E-Mails von einer anderen Adresse als Ihrer eigenen zu senden. Z. B. <code>test@mail.com</code> oder "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>Geben Sie die E-Mail-Adresse ein, die im Feld [!UICONTROL Absender] in der E-Mail angezeigt wird, oder ordnen Sie sie zu.</p> <p>Tipp: Wenn Sie sich nicht sicher sind, ob Sie dieses Feld oder das Feld „Von“ verwenden sollen, empfehlen wir die Auswahl des Felds „Von“.</p> <p>Wichtig: Verwenden Sie die richtige Syntax: <code>name@email.com</code> oder <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Antwort-An]</td> 
   <td> <p> Wenn Antworten auf diese E-Mail an eine andere Adresse als die Absenderadresse gesendet werden sollen, geben Sie die E-Mail-Adresse ein, an die Antworten auf diese E-Mail gesendet werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL in-response-to]</td> 
   <td> <p> Wenn Sie auf eine bestimmte E-Mail antworten, geben Sie die ID der E-Mail, auf die Sie antworten, ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verweise] </td> 
   <td> <p>Geben Sie die Nachrichten-IDs aller Antworten im Thread ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Priorität]</p> </td> 
   <td> <p>Priorität der E-Mail auswählen:</p> 
    <ul> 
     <li>[!UICONTROL Hoch]</li> 
     <li>[!UICONTROL normal]</li> 
     <li>[!UICONTROL Niedrig]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Kopfzeilen]</p> </td> 
   <td> <p>Fügen Sie die Kopfzeilen hinzu:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL key]</strong> </p> <p>Fügen Sie den Schlüssel hinzu. Beispielsweise [!UICONTROL Sender], [!UICONTROL Date], [!UICONTROL To] usw.</p> </li> 
     <li> <p><strong>[!UICONTROL value]</strong> </p> <p>Geben Sie den Wert für den Schlüssel ein.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Entwurf erstellen]

Erstellt einen neuen Entwurf und fügt ihn einem ausgewählten Ordner hinzu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres E-Mail-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Verbinden Ihrer E-Mail mit [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Ordner]</td> 
   <td>Wählen Sie den Ordner aus, in dem Sie den E-Mail-Entwurf erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL nach] </td> 
   <td> <p>Geben Sie die E-Mail-Adresse ein, an die Sie die E-Mail senden möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Betreff] </td> 
   <td> <p>Geben Sie die Betreffzeile der E-Mail ein oder mappen Sie sie.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Content-Typ]</p> </td> 
   <td> <p>Content-Typ für die E-Mail auswählen:</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Nur Text]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Inhalt] </td> 
   <td> <p>Geben Sie den E-Mail-Inhalt im HTML-Format mithilfe von HTML-Tags ein oder mappen Sie ihn im Klartext, je nachdem, was Sie im Feld [!UICONTROL Content-Typ] ausgewählt haben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Anlagen]</p> </td> 
   <td> <p>Anlage hinzufügen:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Dateiname]</strong> </p> <p>Geben Sie den Dateinamen ein. Beispiel: sample.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL-Daten]</strong> </p> <p>Geben Sie den Pfad zum Ordner ein, in den die Anlage hochgeladen werden soll.</p> </li> 
     <li> <p><strong>[!UICONTROL content-ID]</strong> </p> <p>Geben Sie die Inhalts-ID ein, um den Anhang (Bild) in den Inhalt einzufügen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Empfänger kopieren] </td> 
   <td> <p>Geben Sie eine oder mehrere E-Mail-Adressen ein, an die Sie eine Kopie dieser E-Mail senden möchten, oder ordnen Sie sie zu. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Blind Copy-Empfänger]</td> 
   <td> <p> Geben Sie eine oder mehrere E-Mail-Adressen ein, an die Sie eine Kopie dieser E-Mail senden möchten, ohne dass die E-Mail-Adresse in der E-Mail angezeigt wird, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL from] </td> 
   <td> <p>Geben Sie die E-Mail-Adresse (und ggf. den Namen) ein, die im Feld [!UICONTROL Von] in der E-Mail angezeigt wird, oder ordnen Sie sie zu. </p> <p>Wichtig: Verwenden Sie die richtige Syntax: <code>name@email.com</code> oder <code>"Name" name@email.com</code>.</p> <p>Hinweis: Normalerweise verwendet [!DNL Workfront Fusion] die E-Mail-Adresse, die Sie beim Erstellen der Verbindung eingegeben haben, als Absenderadresse. Wenn Sie eine andere E-Mail-Adresse eingeben, kann beim Senden einer Nachricht ein Fehler auftreten, da Ihr Konto möglicherweise nicht berechtigt ist, E-Mails von einer anderen Adresse als Ihrer eigenen zu senden. Z. B. <code>test@mail.com</code> oder "<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>Geben Sie die E-Mail-Adresse ein, die im Feld [!UICONTROL Absender] in der E-Mail angezeigt wird, oder ordnen Sie sie zu.</p> <p>Tipp: Wenn Sie sich nicht sicher sind, ob Sie dieses Feld oder das Feld „Von“ verwenden sollen, empfehlen wir die Auswahl des Felds „Von“.</p> <p>Wichtig: Verwenden Sie die richtige Syntax: <code>name@email.com</code> oder <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Antwort-An]</td> 
   <td> <p> Wenn Antworten auf diese E-Mail an eine andere Adresse als die Adresse "[!UICONTROL from]" gesendet werden sollen, geben Sie die E-Mail-Adresse ein, an die Antworten auf diese E-Mail gesendet werden sollen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL in-response-to]</td> 
   <td> <p> Wenn Sie auf eine bestimmte E-Mail antworten, geben Sie die ID der E-Mail, auf die Sie antworten, ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL-Verweise] </td> 
   <td> <p>Geben Sie die Nachrichten-IDs aller Antworten im Thread ein.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL-Priorität]</p> </td> 
   <td> <p>Priorität der E-Mail auswählen:</p> 
    <ul> 
     <li>[!UICONTROL Hoch]</li> 
     <li>[!UICONTROL normal]</li> 
     <li>[!UICONTROL Niedrig]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL-Kopfzeilen]</p> </td> 
   <td> <p>Fügen Sie die Kopfzeilen hinzu:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL key]</strong> </p> <p>Fügen Sie den Schlüssel hinzu. Beispielsweise „Absender“, „Datum“, „An“ usw.</p> </li> 
     <li> <p><strong>[!UICONTROL value]</strong> </p> <p>Geben Sie den Wert für den Schlüssel ein.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Markieren einer E-Mail als gelesen]

Markiert eine E-Mail oder einen Entwurf in einem ausgewählten Ordner als gelesen, indem die Markierung [!UICONTROL Lesen] festgelegt wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres E-Mail-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Verbinden Ihrer E-Mail mit [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Ordner]</td> 
   <td>Wählen Sie den Ordner der E-Mail aus, den Sie als gelesen markieren möchten. Beispiel: Primär.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL E-Mail-ID (UID)]</p> </td> 
   <td> <p>Geben Sie die E-Mail-UID der E-Mail ein, die Sie als gelesen markieren möchten.</p> <p>Sie können die UID der E-Mail mit dem Modul [!UICONTROL E-Mail] &gt;[!UICONTROL E-Mail ansehen] oder dem Modul [!UICONTROL E-Mail suchen] abrufen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Markieren einer E-Mail als ungelesen]

Markiert eine E-Mail oder einen Entwurf in einem ausgewählten Ordner als ungelesen, indem die Markierung Ungelesen gesetzt wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres E-Mail-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Verbinden Ihrer E-Mail mit [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Ordner]</td> 
   <td>Wählen Sie den Ordner der E-Mail aus, den Sie als ungelesen markieren möchten. Beispiel: Primär.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL E-Mail-ID (UID)]</p> </td> 
   <td> <p>Geben Sie die E-Mail-UID der E-Mail ein, die Sie als ungelesen markieren möchten.</p> <p>Sie können die UID der E-Mail mit dem Modul [!UICONTROL E-Mail] &gt;[!UICONTROL E-Mail ansehen] oder dem Modul [!UICONTROL E-Mail suchen] abrufen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Verschieben einer E-Mail]

Verschiebt eine ausgewählte E-Mail oder einen Entwurf in einen ausgewählten Ordner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres E-Mail-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Verbinden Ihrer E-Mail mit [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Ordner]</td> 
   <td>Wählen Sie den Ordner aus, der die E-Mail enthält, von der Sie die E-Mail verschieben möchten. Beispiel: Primär.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zielordner]</td> 
   <td> <p> Wählen Sie den Ordner aus, dem Sie die E-Mail hinzufügen möchten. Beispiel: Arbeit.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL E-Mail-ID (UID)]</p> </td> 
   <td> <p>Geben Sie die E-Mail-UID der E-Mail ein, die Sie in den Zielordner verschieben möchten.</p> <p>Sie können die UID der E-Mail mit dem Modul [!UICONTROL E-Mail] &gt;[!UICONTROL E-Mail ansehen] oder dem Modul [!UICONTROL E-Mail suchen] abrufen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kopieren einer E-Mail]

Kopiert eine E-Mail oder einen Entwurf in einen ausgewählten Ordner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres E-Mail-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Verbinden Ihrer E-Mail mit [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Ordner]</td> 
   <td>Wählen Sie den Ordner aus, aus dem Sie die E-Mail kopieren möchten. Beispiel: Primär.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zielordner]</td> 
   <td> <p> Wählen Sie den Ordner aus, in den Sie die E-Mail kopieren möchten. Beispiel: Arbeit.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL E-Mail-ID (UID)]</p> </td> 
   <td> <p>Geben Sie die E-Mail-UID der E-Mail ein, die Sie in den Zielordner kopieren möchten.</p> <p>Sie können die UID der E-Mail mit dem Modul [!UICONTROL E-Mail] &gt;[!UICONTROL E-Mail ansehen] oder dem Modul [!UICONTROL E-Mail suchen] abrufen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL E-Mail löschen]

Entfernt eine E-Mail oder einen Entwurf aus dem ausgewählten Ordner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres E-Mail-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Verbinden Ihrer E-Mail mit [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Ordner]</td> 
   <td>Wählen Sie den Ordner der E-Mail aus, die Sie löschen möchten. Beispiel: Primär.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL E-Mail-ID (UID)]</p> </td> 
   <td> <p>Geben Sie die E-Mail-UID der E-Mail ein, die Sie löschen möchten.</p> <p>Sie können die UID der E-Mail mit dem Modul [!UICONTROL E-Mail] &gt;[!UICONTROL E-Mail ansehen] oder dem Modul [!UICONTROL E-Mail suchen] abrufen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL löschen]</td> 
   <td> <p>Aktivieren Sie diese Option, damit das Modul alle Nachrichten, die als [!UICONTROL Deleted] gekennzeichnet sind, in der aktuell geöffneten Mailbox dauerhaft entfernen kann.</p> <p>Hinweis: In [!DNL Gmail] wird dieses Verhalten durch die Einstellung im Abschnitt [!UICONTROL-Einstellungen] &gt;[!UICONTROL-Weiterleitung POP/IMAP im IMAP-Zugriff] gesteuert.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL E-Mails abrufen]

Gibt E-Mails zurück, die den angegebenen Kriterien entsprechen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres E-Mail-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Verbinden Ihrer E-Mail mit [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Ordner] </td> 
   <td> <p>Wählen Sie den Ordner aus, der die abzurufenden E-Mails enthält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nachricht(en) beim Abrufen als gelesen markieren] </td> 
   <td> <p>Aktivieren Sie diese Option, wenn Sie die ungelesene E-Mail nach dem Abrufen der Details als gelesen markieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Kriterien]</p> </td> 
   <td> <p>Wählen Sie die Kriterien der E-Mails aus, die Sie abrufen möchten:</p> 
    <ul> 
     <li>[!UICONTROL Alle E-Mails]</li> 
     <li>[!UICONTROL Nur E-Mails lesen]</li> 
     <li>[!UICONTROL only Unread Emails]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Absender-E-Mail-Adresse] </td> 
   <td> <p>Geben Sie die E-Mail-Adresse des Absenders ein, dessen E-Mails Sie abrufen möchten, oder mappen Sie sie.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Empfänger-E-Mail-Adresse]</td> 
   <td> <p> Geben Sie die E-Mail-Adresse des Empfängers ein, dessen E-Mails Sie abrufen möchten, oder mappen Sie sie.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Von Datum] </td> 
   <td> <p>Geben Sie das Datum ein, an dem die am oder nach dem angegebenen Datum verarbeiteten E-Mails abgerufen werden sollen, oder mappen Sie es.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL vor Datum]</td> 
   <td> <p> Datum eingeben oder zuordnen, an dem die am oder vor dem angegebenen Datum verarbeiteten E-Mails abgerufen werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Betreff] </td> 
   <td> <p>Geben Sie den Betreff der E-Mail ein, die Sie abrufen möchten, oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Phrase] </td> 
   <td> <p>Geben Sie Schlüsselwörter ein oder ordnen Sie sie zu, um nur die E-Mails abzurufen, die bestimmte Phrasen enthalten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL E-Mail-ID (UID)]</td> 
   <td> <p> Geben Sie die E-Mail-ID (UID) der E-Mail ein, deren Details Sie abrufen möchten.</p> <p>Sie können die UID der E-Mail abrufen, indem Sie das Modul [!UICONTROL E-Mail beobachten] oder das Modul [!UICONTROL E-Mail suchen] von [!DNL Workfront Fusion] verwenden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Anzahl an Ergebnissen]</td> 
   <td> <p> Die maximale Anzahl von E-Mails, die [!DNL Workfront Fusion] während eines Szenario-Ausführungszyklus zurückgeben sollten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Die Routenausführung auch dann fortsetzen, wenn das Modul keine Ergebnisse zurückgibt]</td> 
   <td> <p> Wählen Sie aus, ob Sie das Modul auch dann weiter ausführen möchten, wenn keine Ergebnisse zurückgegeben wurden.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Iteratoren

#### [!UICONTROL Iterieren von Anhängen]

Iteriert empfangene Anhänge einzeln.

Mit dem Modul E-Mail-Iterator können Sie E-Mail-Anhänge separat verwalten. Sie können beispielsweise einrichten, dass E-Mails überwacht werden, um die E-Mails mit Anhängen zu durchlaufen und Warnhinweise zu erhalten.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Modul]</td> 
   <td> <p>Wählen Sie das Modul aus, das die E-Mail mit den Anhängen ausgibt, durch die Sie iterieren möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu Iteratoren finden Sie unter [Iteratormodul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
