---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Gmail-Module
description: In einem [!DNL Adobe Workfront Fusion] Szenario können Sie Workflows automatisieren, die Gmail verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '1821'
ht-degree: 0%

---

# [!DNL Gmail] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL Gmail] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

Wenn Sie Anweisungen zum Erstellen eines Szenarios benötigen, finden Sie weitere Informationen unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Weitere Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

Um [!DNL Gmail] -Module zu verwenden, müssen Sie über ein [!DNL Gmail] -Konto verfügen.

## [!DNL Gmail] mit [!DNL Workfront Fusion] verbinden {#connect-gmail-to-workfront-fusion}

* [Verbinden Sie [!DNL Gmail] mit [!DNL Workfront Fusion] mit [!DNL Google Workspace]](#connect-gmail-to-workfront-fusion-usingg-suite)
* [Verbinden Sie [!DNL Gmail] mit [!DNL Workfront Fusion] mit [!DNL gmail.com] oder [!DNL googlemail].com](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### [!DNL Gmail] mit [!DNL  Google Workspace] an [!DNL Workfront Fusion] anbinden {#connect-gmail-to-workfront-fusion-using-g-suite}

Anweisungen zum Verbinden Ihres [!DNL Google Workspace]-Kontos mit [!UICONTROL Workfront Fusion] finden Sie unter [Verbinden der App oder des Webdiensts des Moduls mit  [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) im Artikel [Erstellen eines Szenarios in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Verbinden Sie [!DNL Gmail] mit [!DNL Workfront Fusion] mit [!DNL gmail.com] oder [!DNL googlemail].com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

Wenn Sie Benutzer [!DNL @gmail.com] oder [!DNL @googlemail.com] sind, müssen Sie einen OAuth-Client auf [dem  [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) erstellen, um eine [!UICONTROL Client-ID] und einen [!UICONTROL Client-Geheimnis] zu erhalten.

Eine schrittweise Anleitung zum Erstellen des OAuth-Clients und zum Abrufen einer [!UICONTROL Client-ID] und eines [!UICONTROL Client-Geheimnisses] finden Sie unter [Verbinden von Adobe Workfront Fusion mit Google-Diensten mit einem benutzerdefinierten OAuth-Client](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## [!DNL Gmail] Module und ihre Felder

Wenn Sie [!DNL Gmail] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL Gmail] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger](#triggers)
* [Aktionen](#actions)
* [Iteratoren](#iterators)

### Trigger

#### [!UICONTROL E-Mails ansehen]

Dieses Trigger-Modul führt ein Szenario aus, wenn eine neue E-Mail zur Verarbeitung empfangen wird.

Das Modul gibt alle mit dem Datensatz oder den Datensätzen verknüpften Standardfelder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Gmail]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Gmail] mit [!UICONTROL Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den E-Mail-Ordner aus, den Sie überwachen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Filtertyp] </td> 
   <td> <p>Wählen Sie den Filtertyp aus, den Sie für E-Mails verwenden möchten</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Einfacher Filter]</strong> </p> <p>Füllen Sie die Felder [!UICONTROL Kriterien], [!UICONTROL Sender Email Address], [!UICONTROL Subject] und [!UICONTROL Search Phrase] aus.</p> </li> 
     <li> <p> <strong>[!UICONTROL Gmail filter]</strong> </p> <p>Geben Sie im Feld [!UICONTROL Abfrage] die Abfrage ein, die zum Filtern von E-Mails verwendet werden soll.</p> <p>Weitere Informationen zu [!DNL Gmail] Filtern finden Sie unter <a href="https://support.google.com/mail/answer/7190">Suchoperatoren</a> in der Dokumentation zu [!DNL Gmail].</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kriterien]</td> 
   <td>Wählen Sie aus, ob Sie [!UICONTROL alle E-Mails], [!UICONTROL nur gelesene E-Mails] oder [!UICONTROL nur ungelesene] E-Mails ansehen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sender email address]</td> 
   <td> <p> Geben Sie eine E-Mail-Adresse ein, um nur E-Mails zu sehen, die von dieser Adresse gesendet werden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Betreff]</td> 
   <td>Geben Sie eine Textzeichenfolge ein, um nur E-Mails mit dieser Textzeichenfolge im Betreff zu sehen.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Suchbegriff]</td> 
   <td>Geben Sie eine Textzeichenfolge ein, damit nur E-Mails mit dieser Textzeichenfolge an einer beliebigen Stelle in der E-Mail angezeigt werden.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL E-Mail-Nachricht(en) als gelesen markieren, wenn sie abgerufen wurde]</td> 
   <td> <p> Aktivieren Sie diese Option, um abgerufene E-Mails als gelesen zu markieren.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximale Ergebnisanzahl]</td> 
   <td> <p> Legen Sie die maximale Anzahl von Ergebnissen fest, mit denen [!DNL Workfront Fusion] während eines Zyklus arbeiten soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL E-Mail senden]](#send-an-email)
* [[!UICONTROL Erstellen eines Entwurfs]](#create-a-draft)
* [[!UICONTROL Markieren Sie eine E-Mail als gelesen]](#mark-an-email-as-read)
* [[!UICONTROL Kennzeichnen einer E-Mail als ungelesen]](#mark-an-email-as-unread)
* [[!UICONTROL Verschieben einer E-Mail]](#move-an-email)
* [[!UICONTROL E-Mail kopieren]](#copy-an-email)
* [[!UICONTROL E-Mail löschen]](#delete-an-email)
* [[!UICONTROL E-Mail-Titel ändern]](#modify-email-labels)

#### [!UICONTROL E-Mail senden]

Dieses Aktionsmodul sendet eine neue E-Mail.

Geben Sie den Empfänger der E-Mail an.

Das Modul gibt die E-Mail-ID sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Gmail]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Gmail] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Von]</td> 
   <td> <p>Geben Sie eine Absender-E-Mail-Adresse ein oder ordnen Sie sie zu.</p> <p>Hinweis: Wenn Sie eine falsche E-Mail-Adresse eingeben, kann beim Senden einer Nachricht ein Fehler auftreten, da Ihr Konto möglicherweise nicht über die Berechtigung zum Senden von E-Mails von einer anderen Adresse als Ihrer verfügt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To] </td> 
   <td> <p>Klicken Sie auf <strong>[!UICONTROL Hinzufügen]</strong> und geben Sie die E-Mail-Adresse für jeden Empfänger ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Betreff] </td> 
   <td> <p>Geben Sie den Betreff der E-Mail ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>Geben Sie den E-Mail-Inhalt (Nachrichtentext) ein oder ordnen Sie ihn zu. HTML-Tags sind zulässig.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attachments] </td> 
   <td> <p>Klicken Sie auf <strong>[!UICONTROL Add]</strong> , um eine Anlage hinzuzufügen. Sie können eine Datei aus den vorherigen Modulen zuordnen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Empfänger kopieren]</td> 
   <td> <p> Klicken Sie auf <strong>[!UICONTROL Hinzufügen]</strong> und geben Sie die E-Mail-Adresse für jeden Kopierempfänger ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Blind Copy-Empfänger]</td> 
   <td> <p> Klicken Sie auf <strong>[!UICONTROL Hinzufügen]</strong> und geben Sie die E-Mail-Adresse für jeden blinden Kopierempfänger ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Erstellen eines Entwurfs]

Dieses Aktionsmodul erstellt einen neuen E-Mail-Entwurf und fügt ihn zu einem von Ihnen angegebenen Ordner hinzu.

Sie geben den Ordner an, in dem Sie einen Entwurf erstellen möchten.

Das Modul gibt die ID des E-Mail-Entwurfs und der zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Gmail]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Gmail] mit [!UICONTROL Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den Ordner [!DNL Gmail] aus, in dem Sie einen Entwurf erstellen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To] </td> 
   <td> <p>Klicken Sie auf <strong>[!UICONTROL Hinzufügen]</strong> und geben Sie die E-Mail-Adresse für jeden Empfänger ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Betreff] </td> 
   <td> <p>Geben Sie den Betreff der E-Mail ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>Geben Sie den E-Mail-Inhalt (Nachrichtentext) ein oder ordnen Sie ihn zu. HTML-Tags sind zulässig.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attachments] </td> 
   <td> <p>Klicken Sie auf <strong>[!UICONTROL Add]</strong> , um eine Anlage hinzuzufügen. Sie können eine Datei aus den vorherigen Modulen zuordnen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Empfänger kopieren]</td> 
   <td> <p> Klicken Sie auf <strong>[!UICONTROL Hinzufügen]</strong> und geben Sie die E-Mail-Adresse für jeden Kopierempfänger ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Blind Copy-Empfänger]</td> 
   <td> <p> Klicken Sie auf <strong>[!UICONTROL Hinzufügen]</strong> und geben Sie die E-Mail-Adresse für jeden blinden Kopierempfänger ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Markieren Sie eine E-Mail als gelesen]

Dieses Aktionsmodul markiert eine E-Mail als gelesen.

Geben Sie die E-Mail-Adresse und den Ordner an.

Das Modul gibt die E-Mail-ID sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Gmail]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Gmail] mit [!UICONTROL Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den Ordner [!DNL Gmail] aus, der die E-Mail enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL E-Mail-ID (UID)]</td> 
   <td> <p> Geben Sie die E-Mail-ID ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kennzeichnen einer E-Mail als ungelesen]

Dieses Aktionsmodul markiert eine E-Mail oder einen E-Mail-Entwurf als ungelesen.

Geben Sie die E-Mail-Adresse und den Ordner an.

Das Modul gibt die E-Mail-ID sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Gmail]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Gmail] mit [!UICONTROL Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den Ordner [!DNL Gmail] aus, der die E-Mail enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL E-Mail-ID (UID)] </td> 
   <td> <p>Geben Sie die E-Mail-ID der E-Mail-Adresse ein, die Sie als ungelesen markieren möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Verschieben einer E-Mail]

Dieses Aktionsmodul verschiebt eine E-Mail oder einen E-Mail-Entwurf in einen von Ihnen angegebenen Ordner.

Sie geben den Ordner, den Zielordner und die E-Mail-Adresse an.

Das Modul gibt die E-Mail-ID sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Gmail]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Gmail] mit [!UICONTROL Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den Quellordner [!DNL Gmail] aus, der die zu verschiebende E-Mail enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zielordner]</td> 
   <td> <p> Wählen Sie den Zielordner [!DNL Gmail] aus, in den Sie die E-Mail verschieben möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL E-Mail-ID (UID)]</td> 
   <td> <p> Geben Sie die E-Mail-ID der E-Mail ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL E-Mail kopieren]

Dieses Aktionsmodul kopiert einen E-Mail- oder E-Mail-Entwurf in einen von Ihnen angegebenen Ordner.

Sie geben den Ordner, den Zielordner und die E-Mail-Adresse an.

Das Modul gibt die E-Mail-ID sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Gmail]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Gmail] mit [!UICONTROL Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den Quellordner [!DNL Gmail] aus, der die zu kopierende E-Mail enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zielordner]</td> 
   <td> <p>Wählen Sie den Zielordner [!DNL Gmail] aus, in den Sie die E-Mail kopieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL E-Mail-ID (UID)]</td> 
   <td> <p>Geben Sie die E-Mail-ID der E-Mail ein, die Sie kopieren möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL E-Mail löschen]

Dieses Aktionsmodul entfernt eine E-Mail oder einen E-Mail-Entwurf aus einem von Ihnen angegebenen Ordner.

Das Modul gibt die E-Mail-ID sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Gmail]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Gmail] mit [!UICONTROL Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL [!DNL Gmail] Nachrichten-ID]</p> </td> 
   <td> <p>Geben Sie die E-Mail-ID der E-Mail-Adresse ein, die Sie löschen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Dauerhaft] </td> 
   <td> <p>Aktivieren Sie diese Option, damit das Modul die E-Mail dauerhaft löschen kann, anstatt sie in den Papierkorb zu verschieben.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL E-Mail-Titel ändern]

Dieses Aktionsmodul ändert den Titel einer von Ihnen angegebenen E-Mail-Nachricht.

Das Modul gibt die E-Mail-ID sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

Wenn Sie dieses Modul konfigurieren, werden die folgenden Felder angezeigt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL Gmail]-Kontos mit [!DNL Workfront Fusion] finden Sie in diesem Artikel unter <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL Gmail] mit [!UICONTROL Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Gmail] Nachrichten-ID]</td> 
   <td> <p> Geben Sie die E-Mail-ID der E-Mail-Adresse ein, die Sie löschen möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Beschriftungen zum Hinzufügen]</p> </td> 
   <td> <p>Wählen Sie den Titel aus oder ordnen Sie ihn der ausgewählten E-Mail-Nachricht zu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Beschriftungen zum Entfernen]</td> 
   <td> <p> Wählen Sie den Titel aus oder ordnen Sie ihn der ausgewählten E-Mail-Nachricht zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>[!UICONTROL Beschriftung zum Hinzufügen von ] und [!UICONTROL Beschriftung zum Entfernen von ] Feldern laden nur vom Benutzer erstellte Beschriftungen.

### Iteratoren

#### [!UICONTROL Iterate attachments]

Sie können E-Mail-Anhänge iterieren. Jeder Anhang ist ein separates Bundle in der Ausgabe des Moduls. Weitere Informationen finden Sie unter [Iterator-Modul in Adobe Workfront Fusion](../../workfront-fusion/modules/iterator-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source-Modul] </td> 
   <td> <p>Wählen Sie das Modul aus, aus dem Sie Anlagen iterieren möchten. </p> </td> 
  </tr> 
 </tbody> 
</table>
