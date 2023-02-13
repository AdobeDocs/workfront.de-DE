---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Gmail-Module
description: In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die Gmail verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1785'
ht-degree: 0%

---

# [!DNL Gmail]-Module

In einer [!DNL Adobe Workfront Fusion] können Sie Workflows automatisieren, die [!DNL Gmail], und stellen Sie eine Verbindung zu mehreren Drittanbieteranwendungen und -diensten her.

Informationen zum Erstellen eines Szenarios finden Sie unter [Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Informationen zu Modulen finden Sie unter [Module in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td>
  <td> <p>[!UICONTROL Pro] oder höher</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Verwendung [!DNL Gmail] -Module, müssen Sie über eine [!DNL Gmail] -Konto.

## Verbinden [!DNL Gmail] nach [!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion}

* [Verbinden [!DNL Gmail] nach [!DNL Workfront Fusion] Verwenden von [!DNL G Suite]](#connect-gmail-to-workfront-fusion-usingg-suite)
* [Verbinden [!DNL Gmail] nach [!DNL Workfront Fusion] using [!DNL gmail.com] oder [!DNL googlemail].com](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### Verbinden [!DNL Gmail] nach [!DNL Workfront Fusion] using[!DNL  G Suite] {#connect-gmail-to-workfront-fusion-using-g-suite}

Anweisungen zum Verbinden der [!DNL G Suite] Konto [!UICONTROL Workfront Fusion], siehe [Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) im Artikel [Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### Verbinden [!DNL Gmail] nach [!DNL Workfront Fusion] using [!DNL gmail.com] oder [!DNL googlemail].com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

Wenn Sie [!DNL @gmail.com] oder [!DNL @googlemail.com] Benutzer, für den Sie einen OAuth-Client erstellen müssen [die [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) um eine [!UICONTROL Client-ID] und [!UICONTROL Client Secret].

Eine schrittweise Anleitung zum Erstellen des OAuth-Clients und zum Abrufen einer [!UICONTROL Client-ID] und [!UICONTROL Client Secret], siehe [Verbinden von Adobe Workfront Fusion mit Google Services mithilfe eines benutzerdefinierten OAuth-Clients](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## [!DNL Gmail] Module und ihre Felder

Bei der Konfiguration [!DNL Gmail] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Gmail] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

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
   <td> <p>Anweisungen zum Verbinden der [!DNL Gmail] Konto [!DNL Workfront Fusion], siehe <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Gmail] nach [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie den E-Mail-Ordner aus, den Sie überwachen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Filtertyp] </td> 
   <td> <p>Wählen Sie den Filtertyp aus, den Sie für E-Mails verwenden möchten</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Einfacher Filter]</strong> </p> <p>Füllen Sie die Felder [!UICONTROL Kriterien], [!UICONTROL Absender-E-Mail-Adresse], [!UICONTROL Betreff] und [!UICONTROL Suchbegriff] aus.</p> </li> 
     <li> <p> <strong>[!UICONTROL Gmail-Filter]</strong> </p> <p>Geben Sie im Feld [!UICONTROL Abfrage] die Abfrage ein, die zum Filtern von E-Mails verwendet werden soll.</p> <p>Weitere Informationen finden Sie unter [!DNL Gmail] Filter, siehe <a href="https://support.google.com/mail/answer/7190">Suchoperatoren</a> im [!DNL Gmail] Dokumentation.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Kriterien]</td> 
   <td>Wählen Sie aus, ob Sie [!UICONTROL alle E-Mails], [!UICONTROL nur gelesene E-Mails] oder [!UICONTROL nur ungelesene] E-Mails ansehen möchten.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Absender-E-Mail-Adresse]</td> 
   <td> <p> Geben Sie eine E-Mail-Adresse ein, um nur E-Mails zu sehen, die von dieser Adresse gesendet werden.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject]</td> 
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
   <td> <p> Legen Sie die maximale Anzahl von Ergebnissen fest, die [!DNL Workfront Fusion] wird während eines Zyklus mit arbeiten.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Aktionen

* [[!UICONTROL E-Mail senden]](#send-an-email)
* [[!UICONTROL Entwurf erstellen]](#create-a-draft)
* [[!UICONTROL E-Mail als gelesen markieren]](#mark-an-email-as-read)
* [[!UICONTROL E-Mail als ungelesen markieren]](#mark-an-email-as-unread)
* [[!UICONTROL E-Mail verschieben]](#move-an-email)
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
   <td> <p>Anweisungen zum Verbinden der [!DNL Gmail] Konto [!DNL Workfront Fusion], siehe <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Gmail] nach [!DNL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Von]</td> 
   <td> <p>Geben Sie eine Absender-E-Mail-Adresse ein oder ordnen Sie sie zu.</p> <p>Hinweis: Wenn Sie eine falsche E-Mail-Adresse eingeben, kann beim Senden einer Nachricht ein Fehler auftreten, da Ihr Konto möglicherweise nicht über die Berechtigung zum Senden von E-Mails von einer anderen Adresse als Ihrer verfügt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To] </td> 
   <td> <p>Klicken <strong>[!UICONTROL Hinzufügen]</strong>, geben Sie die E-Mail-Adresse für jeden Empfänger ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject] </td> 
   <td> <p>Geben Sie den Betreff der E-Mail ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>Geben Sie den E-Mail-Inhalt (Nachrichtentext) ein oder ordnen Sie ihn zu. HTML-Tags sind zulässig.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attachments] </td> 
   <td> <p>Klicken <strong>[!UICONTROL Hinzufügen]</strong> , um eine Anlage hinzuzufügen. Sie können eine Datei aus den vorherigen Modulen zuordnen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Empfänger kopieren]</td> 
   <td> <p> Klicken <strong>[!UICONTROL Hinzufügen]</strong>, geben Sie die E-Mail-Adresse für jeden Kopierempfänger ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Blind Copy-Empfänger]</td> 
   <td> <p> Klicken <strong>[!UICONTROL Hinzufügen]</strong>, geben Sie die E-Mail-Adresse für jeden Empfänger der Blindkopie ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Entwurf erstellen]

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
   <td> <p>Anweisungen zum Verbinden der [!DNL Gmail] Konto [!DNL Workfront Fusion], siehe <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Gmail] nach [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie die [!DNL Gmail] Ordner, in dem Sie einen Entwurf erstellen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To] </td> 
   <td> <p>Klicken <strong>[!UICONTROL Hinzufügen]</strong>, geben Sie die E-Mail-Adresse für jeden Empfänger ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject] </td> 
   <td> <p>Geben Sie den Betreff der E-Mail ein oder ordnen Sie ihn zu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>Geben Sie den E-Mail-Inhalt (Nachrichtentext) ein oder ordnen Sie ihn zu. HTML-Tags sind zulässig.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attachments] </td> 
   <td> <p>Klicken <strong>[!UICONTROL Hinzufügen]</strong> , um eine Anlage hinzuzufügen. Sie können eine Datei aus den vorherigen Modulen zuordnen.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Empfänger kopieren]</td> 
   <td> <p> Klicken <strong>[!UICONTROL Hinzufügen]</strong>, geben Sie die E-Mail-Adresse für jeden Kopierempfänger ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Blind Copy-Empfänger]</td> 
   <td> <p> Klicken <strong>[!UICONTROL Hinzufügen]</strong>, geben Sie die E-Mail-Adresse für jeden Empfänger der Blindkopie ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL E-Mail als gelesen markieren]

Dieses Aktionsmodul markiert eine E-Mail als gelesen.

Geben Sie die E-Mail-Adresse und den Ordner an.

Das Modul gibt die E-Mail-ID sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Gmail] Konto [!DNL Workfront Fusion], siehe <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Gmail] nach [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie die [!DNL Gmail] Ordner, der die E-Mail enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL E-Mail-ID (UID)]</td> 
   <td> <p> Geben Sie die E-Mail-ID ein oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL E-Mail als ungelesen markieren]

Dieses Aktionsmodul markiert eine E-Mail oder einen E-Mail-Entwurf als ungelesen.

Geben Sie die E-Mail-Adresse und den Ordner an.

Das Modul gibt die E-Mail-ID sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Gmail] Konto [!DNL Workfront Fusion], siehe <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Gmail] nach [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie die [!DNL Gmail] Ordner, der die E-Mail enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL E-Mail-ID (UID)] </td> 
   <td> <p>Geben Sie die E-Mail-ID der E-Mail-Adresse ein, die Sie als ungelesen markieren möchten, oder ordnen Sie sie zu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL E-Mail verschieben]

Dieses Aktionsmodul verschiebt eine E-Mail oder einen E-Mail-Entwurf in einen von Ihnen angegebenen Ordner.

Sie geben den Ordner, den Zielordner und die E-Mail-Adresse an.

Das Modul gibt die E-Mail-ID sowie alle zugehörigen Felder sowie alle benutzerdefinierten Felder und Werte zurück, auf die die Verbindung zugreift. Sie können diese Informationen in nachfolgenden Modulen im Szenario zuordnen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Verbindung] </td> 
   <td> <p>Anweisungen zum Verbinden der [!DNL Gmail] Konto [!DNL Workfront Fusion], siehe <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Gmail] nach [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie die [!DNL Gmail] Quellordner, der die zu verschiebende E-Mail enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zielordner]</td> 
   <td> <p> Wählen Sie die [!DNL Gmail] Zielordner, in den Sie die E-Mail verschieben möchten.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL E-Mail-ID (UID)]</td> 
   <td> <p> Geben Sie die E-Mail-ID der E-Mail-Adresse ein, die Sie verschieben möchten, oder ordnen Sie sie zu.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden der [!DNL Gmail] Konto [!DNL Workfront Fusion], siehe <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Gmail] nach [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Ordner] </td> 
   <td> <p>Wählen Sie die [!DNL Gmail] Quellordner, der die zu kopierende E-Mail enthält.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Zielordner]</td> 
   <td> <p>Wählen Sie die [!DNL Gmail] Zielordner, in den Sie die E-Mail kopieren möchten.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden der [!DNL Gmail] Konto [!DNL Workfront Fusion], siehe <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Gmail] nach [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
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
   <td> <p>Anweisungen zum Verbinden der [!DNL Gmail] Konto [!DNL Workfront Fusion], siehe <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">Verbinden [!DNL Gmail] nach [!UICONTROL Workfront Fusion]</a> in diesem Artikel.</p> </td> 
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
>[!UICONTROL Beschriftung zum Hinzufügen] und [!UICONTROL Beschriftung zum Entfernen] -Felder laden nur von Benutzern erstellte Bezeichnungen.

### Iteratoren

#### [!UICONTROL Anhänge itterieren]

Sie können E-Mail-Anhänge iterieren. Jeder Anhang ist ein separates Bundle in der Ausgabe des Moduls. Weitere Informationen finden Sie unter [Iteratormodul in Adobe Workfront Fusion](../../workfront-fusion/modules/iterator-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Quellmodul] </td> 
   <td> <p>Wählen Sie das Modul aus, aus dem Sie Anlagen iterieren möchten. </p> </td> 
  </tr> 
 </tbody> 
</table>
