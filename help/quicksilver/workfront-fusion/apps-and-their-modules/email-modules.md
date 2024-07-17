---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: E-Mail-Module
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Ihr E-Mail-Konto mit mehreren Anwendungen und Diensten von Drittanbietern verbinden. So können Sie E-Mails über IMAP herunterladen, E-Mails über SMTP versenden, neue Entwürfe erstellen, E-Mails von einem Ordner in einen anderen verschieben und kopieren, E-Mails als gelesen oder ungelesen markieren und E-Mails löschen.
author: Becky
feature: Workfront Fusion
exl-id: 384ba60a-d79e-4126-a247-6d67b5154ede
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '2626'
ht-degree: 0%

---

# E-Mail-Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Ihr E-Mail-Konto mit mehreren Anwendungen und Diensten von Drittanbietern verbinden. Dadurch können Sie E-Mails über IMAP herunterladen, E-Mails über SMTP versenden, neue Entwürfe erstellen, E-Mails von einem Ordner in einen anderen verschieben und kopieren, E-Mails als gelesen oder ungelesen markieren und E-Mails löschen.

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

## E-Mail mit Workfront Fusion verbinden {#connect-your-email-to-workfront-fusion}

* [Verbindung zu Google herstellen](#connect-to-google)
* [Verbindung zu anderen E-Mail-Diensten herstellen (SMAP)](#connect-to-other-email-services-smap)

### Mit [!DNL Google] verbinden

Verwenden Sie diese Option, um Szenarien mit E-Mail-Modulen zu erstellen, die eine Verbindung zu Ihrem [!DNL Google]-Konto erfordern. Dies ist ein Konto mit eingeschränktem Umfang.

Sie können eine Verbindung zu Ihrem [!DNL Google]-Konto direkt aus einem E-Mail-Modul erstellen.

1. Klicken Sie in einem beliebigen E-Mail-Modul neben dem Feld [!UICONTROL Verbindung] auf **[!UICONTROL Hinzufügen]** .
1. Wählen Sie **[!DNL Google]** als Verbindungstyp aus.
1. Geben Sie einen Namen für die Verbindung ein.
1. (Optional) Geben Sie Ihre [!UICONTROL [!DNL Google] Client-ID] und Ihren [!UICONTROL Client-Geheimnis] ein.
1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

### Verbindung zu anderen E-Mail-Diensten herstellen (SMAP)

Mit der SMAP-Verbindung können Sie remote auf Ihr Postfach zugreifen und Nachrichten in Ihrem Postfach lesen oder bearbeiten. Die SMAP-Verbindung wird von den meisten E-Mail-Modulen verwendet.

1. Klicken Sie in einem beliebigen E-Mail-Modul neben dem Feld [!UICONTROL Verbindung] auf **[!UICONTROL Hinzufügen]** .
1. Wählen Sie **[!UICONTROL Sonstige (SMTP)]** als Verbindungstyp aus.
1. Geben Sie einen **[!UICONTROL Namen]** für die Verbindung ein.
1. Wählen Sie Ihren **[!UICONTROL E-Mail-Anbieter]** aus der Liste aus. Wenn Ihr E-Mail-Anbieter nicht in der Liste aufgeführt ist, wählen Sie &quot;Sonstige&quot;.
1. Geben Sie Ihre **[!UICONTROL E-Mail-Adresse]**, **[!UICONTROL Ihren vollständigen Namen]**, Ihren **[!UICONTROL Benutzernamen]** und Ihr **[!UICONTROL Kennwort]** ein.
1. (Bedingt) Wenn Ihr Provider nicht in der Liste aufgeführt ist, geben Sie Ihren **[!UICONTROL SMTP-Server]** und den **[!UICONTROL Port]** ein und geben Sie an, ob Sie **[!UICONTROL eine sichere Verbindung (TLS) verwenden möchten]**. Um diese Informationen zu erhalten, lesen Sie den Abschnitt [!UICONTROL Hilfe] für Ihr Postfach. Wenn Sie diese Informationen nicht zur Verfügung haben, wenden Sie sich an Ihren E-Mail-Dienstleister.
1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.

## [!UICONTROL E-Mail] -Module und ihre Felder

Wenn Sie die Module [!UICONTROL E-Mail] konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Einige E-Mail-Felder enthalten möglicherweise bereits Daten, da Sie sie in einem anderen Modul des Szenarios verwendet haben. Weitere Informationen dazu finden Sie in der Dokumentation zur E-Mail-Hilfe .

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>Die eindeutige E-Mail-ID &quot;[!UICONTROL E-Mail-ID (UID)]&quot; ist die E-Mail-Kennung. Die E-Mail-ID ist für jeden Ordner der E-Mail spezifisch.

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Iteratoren](#iterators)

### Trigger

#### [!UICONTROL E-Mails ansehen]

Trigger, in denen eine neue E-Mail zur Verarbeitung gemäß bestimmten Kriterien empfangen wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres E-Mail-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Verbinden Ihrer E-Mail mit [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den Ordner aus, der E-Mails enthält, die Sie ansehen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Kriterien]</p> </td> 
   <td> <p>Wählen Sie die Kriterien aus, nach denen E-Mails angesehen werden sollen:</p> 
    <ul> 
     <li>[!UICONTROL Alle E-Mails]</li> 
     <li>[!UICONTROL Schreibgeschützte E-Mails]</li> 
     <li>[!UICONTROL Only Unread Email]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sender Email Address] </td> 
   <td> <p>Geben Sie die E-Mail-Adresse des Absenders ein, dessen E-Mails Sie ansehen möchten.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Empfänger-E-Mail-Adresse]</td> 
   <td> <p> Geben Sie die E-Mail-Adresse des Empfängers ein, dessen E-Mails Sie ansehen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Betreff] </td> 
   <td> <p>Geben Sie den Betreff der E-Mail ein, die Sie sehen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Wortgruppe] </td> 
   <td> <p>Geben Sie Suchbegriffe ein, um nur E-Mails mit bestimmten Ausdrücken zu sehen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Markieren Sie die Nachricht(en) als gelesen beim Abrufen]</td> 
   <td> <p>Aktivieren Sie diese Option, um die ungelesene E-Mail nach dem Abrufen der Details als gelesen zu markieren.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Ergebnisanzahl]</td> 
   <td> <p> Die maximale Anzahl von E-Mails [!DNL Workfront Fusion] sollte während eines Szenario-Ausführungszyklus zurückgegeben werden.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL E-Mail senden]](#send-an-email)
* [[!UICONTROL Erstellen eines Entwurfs]](#create-a-draft)
* [[!UICONTROL Markieren einer E-Mail als &quot;Gelesen&quot;]](#mark-an-email-as-read)
* [[!UICONTROL Kennzeichnen einer E-Mail als &quot;Ungelesen&quot;]](#mark-an-email-as-unread)
* [[!UICONTROL Verschieben einer E-Mail]](#move-an-email)
* [[!UICONTROL E-Mail kopieren]](#copy-an-email)
* [[!UICONTROL E-Mail löschen]](#delete-an-email)
* [[!UICONTROL E-Mails abrufen]](#get-emails)

#### [!UICONTROL E-Mail senden]

Sendet eine neue E-Mail.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres E-Mail-Kontos mit [!DNL Workfront Fusion] finden Sie unter <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Verbinden Ihrer E-Mail mit [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nachricht nach dem Versand speichern]</td> 
   <td>Nachdem die E-Mail gesendet wurde, wird sie in Ihrem Postfach gespeichert. Aktivieren Sie diese Option, wenn Sie mit [!DNL Workfront Fusion] gesendete E-Mails im Ordner <i>[!UICONTROL Gesendet Mail]</i> oder in einem anderen Ordner in Ihrem Postfach speichern möchten. Einige E-Mail-Dienste wie [!DNL Gmail] speichern die gesendeten Nachrichten automatisch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL To] </td> 
   <td> <p>Fügen Sie die E-Mail-Adressen hinzu, an die Sie die E-Mail senden möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Betreff] </td> 
   <td> <p>Geben Sie die Betreffzeile der E-Mail ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Content-Typ]</p> </td> 
   <td> <p>Wählen Sie den Inhaltstyp [!UICONTROL für die E-Mail aus:</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Plaintext]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content] </td> 
   <td> <p>Geben Sie den E-Mail-Inhalt mithilfe von HTML-Tags im HTML-Format ein oder ordnen Sie ihn im Klartext zu, je nachdem, was Sie im Feld [!UICONTROL Content Type] ausgewählt haben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Anlage hinzufügen:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Dateiname]</strong> </p> <p>Geben Sie den Dateinamen ein. Beispiel: sample.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Geben Sie den Pfad zum Ordner ein, in den der Anhang hochgeladen werden soll.</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>Geben Sie die [!UICONTROL Inhalts-ID] ein, um den Anhang (Bild) in den Inhalt einzufügen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Empfänger kopieren </td> 
   <td> <p>Geben Sie eine oder mehrere E-Mail-Adressen ein oder ordnen Sie sie zu, an die Sie eine Kopie dieser E-Mail senden möchten. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Blind Copy-Empfänger]</td> 
   <td> <p> Geben Sie eine oder mehrere E-Mail-Adressen ein oder ordnen Sie sie zu, an die Sie eine Kopie dieser E-Mail senden möchten, ohne dass die E-Mail-Adresse in der E-Mail erscheint.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Von] </td> 
   <td> <p>Geben Sie die E-Mail-Adresse (und ggf. den Namen) ein oder ordnen Sie sie zu, die im Feld [!UICONTROL Von] in der E-Mail angezeigt wird. </p> <p>Wichtig: Verwenden Sie die richtige Syntax: <code>name@email.com</code> oder <code>"Name" name@email.com</code>.</p> <p>Hinweis: Normalerweise verwendet [!DNL Workfront Fusion] die E-Mail-Adresse, die Sie beim Erstellen der Verbindung eingegeben haben, als Absenderadresse. Wenn Sie eine andere E-Mail-Adresse eingeben, kann beim Senden einer Nachricht ein Fehler auftreten, da Ihr Konto möglicherweise nicht über die Berechtigung zum Senden von E-Mails von einer anderen Adresse als Ihrer eigenen verfügt. Beispiel: <code>test@mail.com</code> oder "<code>John Bush" test@email.com</code>".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>Geben Sie die E-Mail-Adresse ein oder ordnen Sie sie zu, die im Feld [!UICONTROL Sender] in der E-Mail angezeigt wird.</p> <p>Tipp: Wenn Sie nicht sicher sind, ob Sie dieses Feld oder das Feld Von verwenden möchten, empfehlen wir Ihnen, das Feld Von zu auszuwählen.</p> <p>Wichtig: Verwenden Sie die richtige Syntax: <code>name@email.com</code> oder <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Antwort]</td> 
   <td> <p> Wenn Sie Antworten auf diese E-Mail an eine andere Adresse als die "Von"-Adresse senden möchten, geben Sie die E-Mail-Adresse ein, an die Sie Antworten auf diese E-Mail senden möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL In-Response-To]</td> 
   <td> <p> Wenn Sie auf eine bestimmte E-Mail reagieren, geben Sie die Kennung der E-Mail, auf die Sie antworten, ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Referenzen] </td> 
   <td> <p>Geben Sie die Nachrichten-IDs aller Antworten im Thread ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Priority]</p> </td> 
   <td> <p>Wählen Sie die Priorität der E-Mail aus:</p> 
    <ul> 
     <li>[!UICONTROL Hoch]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Niedrig]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Header]</p> </td> 
   <td> <p>Fügen Sie die Kopfzeilen hinzu:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Schlüssel]</strong> </p> <p>Fügen Sie den Schlüssel hinzu. Beispiel: [!UICONTROL Sender], [!UICONTROL Date], [!UICONTROL To] usw.</p> </li> 
     <li> <p><strong>[!UICONTROL Wert]</strong> </p> <p>Geben Sie den Wert für den Schlüssel ein.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen eines Entwurfs]

Erstellt einen neuen Entwurf und fügt ihn einem ausgewählten Ordner hinzu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres E-Mail-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Verbinden Ihrer E-Mail mit [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner]</td> 
   <td>Wählen Sie den Ordner aus, in dem Sie den E-Mail-Entwurf erstellen möchten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL To] </td> 
   <td> <p>Geben Sie die E-Mail-Adresse ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Betreff] </td> 
   <td> <p>Geben Sie die Betreffzeile der E-Mail ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Content-Typ]</p> </td> 
   <td> <p>Wählen Sie den Inhaltstyp für die E-Mail aus:</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Klartext]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content] </td> 
   <td> <p>Geben Sie den E-Mail-Inhalt mithilfe von HTML-Tags im HTML-Format ein oder ordnen Sie ihn im Klartext zu, je nachdem, was Sie im Feld [!UICONTROL Content Type] ausgewählt haben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>Anlage hinzufügen:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Dateiname]</strong> </p> <p>Geben Sie den Dateinamen ein. Beispiel: sample.doc.</p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>Geben Sie den Pfad zum Ordner ein, in den der Anhang hochgeladen werden soll.</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>Geben Sie die Inhalts-ID ein, um den Anhang (Bild) in den Inhalt einzufügen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Empfänger kopieren </td> 
   <td> <p>Geben Sie eine oder mehrere E-Mail-Adressen ein oder ordnen Sie sie zu, an die Sie eine Kopie dieser E-Mail senden möchten. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Blind Copy-Empfänger]</td> 
   <td> <p> Geben Sie eine oder mehrere E-Mail-Adressen ein oder ordnen Sie sie zu, an die Sie eine Kopie dieser E-Mail senden möchten, ohne dass die E-Mail-Adresse in der E-Mail erscheint.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Von] </td> 
   <td> <p>Geben Sie die E-Mail-Adresse (und ggf. den Namen) ein oder ordnen Sie sie zu, die im Feld [!UICONTROL Von] in der E-Mail angezeigt wird. </p> <p>Wichtig: Verwenden Sie die richtige Syntax: <code>name@email.com</code> oder <code>"Name" name@email.com</code>.</p> <p>Hinweis: Normalerweise verwendet [!DNL Workfront Fusion] die E-Mail-Adresse, die Sie beim Erstellen der Verbindung eingegeben haben, als Absenderadresse. Wenn Sie eine andere E-Mail-Adresse eingeben, kann beim Senden einer Nachricht ein Fehler auftreten, da Ihr Konto möglicherweise nicht über die Berechtigung zum Senden von E-Mails von einer anderen Adresse als Ihrer eigenen verfügt. Beispiel: <code>test@mail.com</code> oder "<code>John Bush" test@email.com</code>".</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>Geben Sie die E-Mail-Adresse ein oder ordnen Sie sie zu, die im Feld [!UICONTROL Sender] in der E-Mail angezeigt wird.</p> <p>Tipp: Wenn Sie nicht sicher sind, ob Sie dieses Feld oder das Feld Von verwenden möchten, empfehlen wir Ihnen, das Feld Von zu auszuwählen.</p> <p>Wichtig: Verwenden Sie die richtige Syntax: <code>name@email.com</code> oder <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Antwort]</td> 
   <td> <p> Wenn Sie Antworten auf diese E-Mail an eine andere Adresse als die Adresse "[!UICONTROL von]" senden möchten, geben Sie die E-Mail-Adresse ein, an die Antworten auf diese E-Mail gesendet werden sollen.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL In-Response-To]</td> 
   <td> <p> Wenn Sie auf eine bestimmte E-Mail reagieren, geben Sie die Kennung der E-Mail, auf die Sie antworten, ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Referenzen] </td> 
   <td> <p>Geben Sie die Nachrichten-IDs aller Antworten im Thread ein.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Priority]</p> </td> 
   <td> <p>Wählen Sie die Priorität der E-Mail aus:</p> 
    <ul> 
     <li>[!UICONTROL Hoch]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Niedrig]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Header]</p> </td> 
   <td> <p>Fügen Sie die Kopfzeilen hinzu:</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Schlüssel]</strong> </p> <p>Fügen Sie den Schlüssel hinzu. Beispiel: Sender, Datum, An usw.</p> </li> 
     <li> <p><strong>[!UICONTROL Wert]</strong> </p> <p>Geben Sie den Wert für den Schlüssel ein.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Markieren einer E-Mail als &quot;Gelesen&quot;]

Markiert eine E-Mail oder einen Entwurf in einem ausgewählten Ordner als gelesen, indem die Markierung [!UICONTROL Lesen] gesetzt wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres E-Mail-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Verbinden Ihrer E-Mail mit [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner]</td> 
   <td>Wählen Sie den Ordner der E-Mail aus, die Sie als gelesen markieren möchten. Beispiel: Primär.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL E-Mail-ID (UID)]</p> </td> 
   <td> <p>Geben Sie die E-Mail-UID der E-Mail ein, die Sie als gelesen markieren möchten.</p> <p>Sie können die UID der E-Mail über das Modul [!UICONTROL Email] &gt;[!UICONTROL Watch Email] oder das Modul [!UICONTROL Search Email] abrufen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kennzeichnen einer E-Mail als &quot;Ungelesen&quot;]

Markiert eine E-Mail oder einen Entwurf in einem ausgewählten Ordner als ungelesen, indem das Flag Ungelesen gesetzt wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres E-Mail-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Verbinden Ihrer E-Mail mit [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner]</td> 
   <td>Wählen Sie den Ordner der E-Mail aus, die als ungelesen gekennzeichnet werden soll. Beispiel: Primär.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL E-Mail-ID (UID)]</p> </td> 
   <td> <p>Geben Sie die E-Mail-UID der E-Mail ein, die als ungelesen gekennzeichnet werden soll.</p> <p>Sie können die UID der E-Mail über das Modul [!UICONTROL Email] &gt;[!UICONTROL Watch Email] oder das Modul [!UICONTROL Search Email] abrufen.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres E-Mail-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Verbinden Ihrer E-Mail mit [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner Source]</td> 
   <td>Wählen Sie den Ordner aus, der die E-Mail enthält, aus der Sie die E-Mail verschieben möchten. Beispiel: Primär.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zielordner]</td> 
   <td> <p> Wählen Sie den Ordner aus, dem Sie die E-Mail hinzufügen möchten. Beispiel: Arbeit.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL E-Mail-ID (UID)]</p> </td> 
   <td> <p>Geben Sie die E-Mail-UID der E-Mail ein, die Sie in den Zielordner verschieben möchten.</p> <p>Sie können die UID der E-Mail über das Modul [!UICONTROL Email] &gt;[!UICONTROL Watch Email] oder das Modul [!UICONTROL Search Email] abrufen.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL E-Mail kopieren]

Kopiert eine E-Mail oder einen Entwurf in einen ausgewählten Ordner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres E-Mail-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Verbinden Ihrer E-Mail mit [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner Source]</td> 
   <td>Wählen Sie den Ordner aus, aus dem Sie die E-Mail kopieren möchten. Beispiel: Primär.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zielordner]</td> 
   <td> <p> Wählen Sie den Ordner aus, in den Sie die E-Mail kopieren möchten. Beispiel: Arbeit.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL E-Mail-ID (UID)]</p> </td> 
   <td> <p>Geben Sie die E-Mail-UID der E-Mail ein, die Sie in den Zielordner kopieren möchten.</p> <p>Sie können die UID der E-Mail über das Modul [!UICONTROL Email] &gt;[!UICONTROL Watch Email] oder das Modul [!UICONTROL Search Email] abrufen.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres E-Mail-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Verbinden Ihrer E-Mail mit [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner]</td> 
   <td>Wählen Sie den Ordner der E-Mail aus, die Sie löschen möchten. Beispiel: Primär.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL E-Mail-ID (UID)]</p> </td> 
   <td> <p>Geben Sie die E-Mail-UID der E-Mail ein, die Sie löschen möchten.</p> <p>Sie können die UID der E-Mail über das Modul [!UICONTROL Email] &gt;[!UICONTROL Watch Email] oder das Modul [!UICONTROL Search Email] abrufen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expunge]</td> 
   <td> <p>Aktivieren Sie diese Option, damit das Modul alle Nachrichten, die im derzeit geöffneten Postfach als [!UICONTROL gelöscht] gekennzeichnet sind, dauerhaft entfernen kann.</p> <p>Hinweis: In [!DNL Gmail] wird dieses Verhalten durch die Einstellung im Abschnitt [!UICONTROL Einstellungen] &gt;[!UICONTROL Weiterleitung von POP/IMAP im IMAP-Zugriff] gesteuert.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres E-Mail-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">Verbinden Ihrer E-Mail mit [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den Ordner aus, der die abzurufenden E-Mails enthält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Markieren Sie die Nachricht(en) als gelesen beim Abrufen] </td> 
   <td> <p>Aktivieren Sie diese Option, wenn Sie die ungelesene E-Mail nach dem Abrufen der Details als gelesen markieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Kriterien]</p> </td> 
   <td> <p>Wählen Sie die Kriterien der E-Mails aus, die Sie abrufen möchten:</p> 
    <ul> 
     <li>[!UICONTROL Alle E-Mails]</li> 
     <li>[!UICONTROL Schreibgeschützte E-Mails]</li> 
     <li>[!UICONTROL Only Unread Email]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sender Email Address] </td> 
   <td> <p>Geben Sie die E-Mail-Adresse des Absenders ein oder ordnen Sie sie zu, dessen E-Mails Sie abrufen möchten.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Empfänger-E-Mail-Adresse]</td> 
   <td> <p> Geben Sie die E-Mail-Adresse des Empfängers ein oder ordnen Sie sie zu, dessen E-Mails Sie abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ab Datum] </td> 
   <td> <p>Geben Sie das Datum ein oder ordnen Sie es zu, um die am oder nach dem angegebenen Datum verarbeiteten E-Mails abzurufen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vor Datum]</td> 
   <td> <p> Geben Sie das Datum ein oder ordnen Sie es zu, um die am oder vor dem angegebenen Datum verarbeiteten E-Mails abzurufen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Betreff] </td> 
   <td> <p>Geben Sie den Betreff der E-Mail ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Wortgruppe] </td> 
   <td> <p>Geben Sie Suchbegriffe ein oder ordnen Sie sie zu, um nur die E-Mails abzurufen, die bestimmte Begriffe enthalten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL E-Mail-ID (UID)]</td> 
   <td> <p> Geben Sie die E-Mail-ID (UID) der E-Mail ein, deren Details Sie abrufen möchten.</p> <p>Sie können die UID der E-Mail mit dem Modul [!UICONTROL Watch Email] oder dem Modul [!UICONTROL Search Email] von [!DNL Workfront Fusion] abrufen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximale Ergebnisanzahl]</td> 
   <td> <p> Die maximale Anzahl von E-Mails [!DNL Workfront Fusion] sollte während eines Szenario-Ausführungszyklus zurückgegeben werden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fortfahren der Routenausführung, selbst wenn das Modul keine Ergebnisse zurückgibt]</td> 
   <td> <p> Wählen Sie aus, ob Sie das Modul auch dann weiterhin ausführen möchten, wenn keine Ergebnisse zurückgegeben werden.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Iteratoren

#### [!UICONTROL Iterate Attachments]

Iterate empfangen Anlagen einzeln.

Mit dem E-Mail-Iterator-Modul können Sie E-Mail-Anhänge separat verwalten. Sie können beispielsweise E-Mails beobachten, um E-Mails mit Anhängen zu iterieren und Warnungen zu erhalten.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Modul]</td> 
   <td> <p>Wählen Sie das Modul aus, das die E-Mail mit den Anlagen ausgibt, durch die Sie iterieren möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu Iteratoren finden Sie unter [Iterator-Modul in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
