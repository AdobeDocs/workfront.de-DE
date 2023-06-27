---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: Frame.io-Module
description: Die [!DNL Adobe Workfront Fusion Frame].io modules enable you to monitor, create, update, retrieve, or delete assets and comments in your [!DNL Frame.io] -Konto.
author: Becky
feature: Workfront Fusion
exl-id: 373a86f6-fbba-4914-b08d-a3a035ac0ae4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2311'
ht-degree: 0%

---

# [!DNL Frame.io]-Module

Die [!DNL Adobe Workfront Fusion] [!DNL Frame.io] -Module ermöglichen es Ihnen, Assets und Kommentare in Ihrer [!DNL Frame.io] -Konto.

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
   <td>
   <p>Aktuelle Lizenzanforderungen: Nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Ältere Lizenzanforderungen: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderungen: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Ältere Produktanforderungen: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Verwendung [!DNL Frame.io] -Module, müssen Sie über eine [!DNL Frame.io] account

## Verbinden [!DNL Frame.io] nach [!UICONTROL Adobe Workfront Fusion]

Sie können eine Verbindung zu [!DNL Frame.io] Verwendung eines API-Tokens oder Verwendung von OAuth 2.0.

[Verbinden mit [!DNL Frame.io] Verwenden eines API-Tokens](#connect-to-frameio-using-an-api-token)

[Verbinden mit [!DNL Frame.io] Verwenden von OAuth 2.0 PKCE](#connect-to-frameio-using-oauth-20-pkce)

### Verbinden mit [!DNL Frame.io] Verwenden eines API-Tokens

Um eine Verbindung herzustellen [!DNL Frame.io] Konto [!DNL Workfront Fusion] mithilfe eines API-Tokens müssen Sie das API-Token in Ihrer [!DNL Frame.io] -Konto und fügen Sie es in die [!DNL Workfront Fusion] [!DNL Frame.io] [!UICONTROL Verbindung erstellen] angezeigt.

1. Melden Sie sich bei Ihrer [!DNL Frame.io] -Konto.
1. Navigieren Sie zu **[!UICONTROL Token]** in der [!DNL Frame.io] Entwickler.
1. Klicken **[!UICONTROL Neu]**.
1. Geben Sie den Namen des Tokens ein, wählen Sie die zu verwendenden Bereiche aus und klicken Sie auf **[!UICONTROL Erstellen]**.
1. Kopieren Sie das bereitgestellte Token.
1. Navigieren Sie zu [!DNL Workfront Fusion] und öffnen Sie die [!DNL Frame.io] -Modul **[!UICONTROL Verbindung erstellen]** angezeigt.
1. Im **[!UICONTROL Verbindungstyp]** Feld, wählen Sie **[!DNL Frame.io]**.
1. Geben Sie das Token ein, das Sie in Schritt 5 in die **[!UICONTROL Ihre [!DNL Frame.io] API-Schlüssel]** Feld und klicken Sie auf **[!UICONTROL Weiter]** um die Verbindung herzustellen.

Die Verbindung wurde hergestellt. Sie können mit der Einrichtung des Moduls fortfahren.

### Verbinden mit [!DNL Frame.io] Verwenden von OAuth 2.0 PKCE

Sie können eine Verbindung zu [!DNL Frame.io] Verwendung von OAuth 2.0 PKCE mit einer optionalen Client-ID. Wenn Sie eine Client-ID in Ihre Verbindung aufnehmen möchten, müssen Sie eine OAuth 2.0-App in Ihrer [!DNL Frame.io] -Konto.

* [Verbinden mit [!DNL Frame.io] Verwendung von OAuth 2.0 PKCE (ohne Client-ID)](#connect-to-frameio-using-using-oauth-20-pkce-without-client-id)
* [Verbinden mit [!DNL Frame.io] Verwendung von OAuth 2.0 PKCE (mit Client-ID)](#connect-to-frameio-using-using-oauth-20-pkce-with-client-id)

#### Verbinden mit [!DNL Frame.io] Verwendung von OAuth 2.0 PKCE (ohne Client-ID)

1. Navigieren Sie zu [!DNL Workfront Fusion] und öffnen Sie die [!DNL Frame.io] -Modul **[!UICONTROL Verbindung erstellen]** angezeigt.
1. Im **[!UICONTROL Verbindungstyp]** Feld, wählen Sie **[!UICONTROL [!DNL Frame.io]OAuth 2.0 PKCE]**.
1. Geben Sie einen Namen für die neue Verbindung im **[!UICONTROL Verbindungsname]** -Feld.
1. Klicken **[!UICONTROL Weiter]** um die Verbindung herzustellen.

Die Verbindung wurde hergestellt. Sie können mit der Einrichtung des Moduls fortfahren.

#### Verbinden mit [!DNL Frame.io] Verwendung von OAuth 2.0 PKCE (mit Client-ID)

1. Erstellen einer OAuth 2.0-App in [!DNL Frame.io]. Anweisungen finden Sie in der [!DNL Frame.io] Dokumentation zu [!UICONTROL OAuth 2.0 Code-Autorisierungsfluss].

   >[!IMPORTANT]
   >
   >Beim Erstellen der OAuth 2.0-App in [!DNL Frame.io]:
   >
   >* Geben Sie Folgendes als Umleitungs-URI ein:
   >   
   >  Amerika/APAC `https://app.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >  EMEA `https://app-eu.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >* Aktivieren Sie die Option PCKE .


1. Kopieren Sie die bereitgestellte `client_id`.
1. Navigieren Sie zu [!DNL Workfront Fusion] und öffnen Sie die [!DNL Frame.io] -Modul **[!UICONTROL Verbindung erstellen]** angezeigt.
1. Im **[!UICONTROL Verbindungstyp]** Feld, wählen Sie **[!UICONTROL [!DNL Frame.io]OAuth 2.0 PKCE]**.
1. Geben Sie einen Namen für die neue Verbindung im **[!UICONTROL Verbindungsname]** -Feld.
1. Klicken **[!UICONTROL Erweiterte Einstellungen anzeigen]**.
1. Geben Sie die `client_id` Sie haben in Schritt 2 zum **[!UICONTROL Client-ID]** -Feld.
1. Klicken **[!UICONTROL Weiter]** um die Verbindung herzustellen.

Die Verbindung wurde hergestellt. Sie können mit der Einrichtung des Moduls fortfahren.

## [!DNL Frame.io] Module und ihre Felder

Bei der Konfiguration [!DNL Frame.io] Module, [!DNL Workfront Fusion] zeigt die unten aufgeführten Felder an. Zusätzlich zu diesen [!DNL Frame.io] -Felder können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Ordnen Sie Informationen zwischen Modulen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Assets](#assets)
* [Kommentare](#comments)
* [Projekte](#projects)
* [Sonstige](#other)

### Assets

* [[!UICONTROL Erstellen eines Assets]](#create-an-asset)
* [[!UICONTROL Löschen von Assets]](#delete-an-asset)
* [[!UICONTROL Asset abrufen]](#get-an-asset)
* [[!UICONTROL Auflisten von Assets]](#list-assets)
* [[!UICONTROL Aktualisieren eines Assets]](#update-an-asset)
* [[!UICONTROL Asset löschen ansehen]](#watch-asset-deleted)
* [[!UICONTROL Asset-Bezeichnung ansehen aktualisiert]](#watch-asset-label-updated)
* [[!UICONTROL Neues Asset ansehen]](#watch-new-asset)

#### [!UICONTROL Erstellen eines Assets]

Dieses Aktionsmodul erstellt ein neues Asset.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Frame.io], siehe <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] nach [!DNL Adobe Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Wählen Sie das Team aus, dem das Projekt gehört, für das Sie ein Asset erstellen möchten, oder ordnen Sie es zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projekt-ID] </td> 
   <td> <p>Wählen Sie das Projekt aus oder ordnen Sie die ID des Projekts zu, für das Sie ein Asset erstellen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner-ID] </td> 
   <td> <p>Wählen Sie den Ordner aus oder ordnen Sie die ID des Ordners zu, in dem Sie ein Asset erstellen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Typ] </td> 
   <td> <p>Wählen Sie aus, ob ein Ordner oder eine Datei erstellt werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Geben Sie den Namen der neuen Datei oder des Ordners ein.</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Type </td> 
    <td> <p>Select the type of file you want to upload.</p> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Size </td> 
    <td> <p>The file size in bytes.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">[!UICONTROL Quell-URL] </td> 
   <td> <p>Geben Sie die URL der Datei ein, die Sie hochladen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beschreibung] </td> 
   <td> <p>Geben Sie eine kurze Beschreibung des Assets ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Löschen von Assets]

Dieses Aktionsmodul löscht ein bestimmtes Asset.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Frame.io], siehe <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] nach [!DNL Adobe Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Wählen Sie das Team aus, dem das Projekt gehört, das das Asset enthält, das Sie löschen möchten, oder ordnen Sie es zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projekt-ID]</td> 
   <td> <p> Wählen Sie das Projekt oder , das das Asset enthält, das Sie löschen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner-ID] </td> 
   <td> <p>Wählen Sie den Ordner aus, der das Asset enthält, das Sie löschen möchten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-ID] </td> 
   <td> <p>Wählen Sie das Asset aus oder ordnen Sie es zu, das Sie löschen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Asset abrufen]

Dieses Aktionsmodul ruft Asset-Details ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Frame.io], siehe <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] nach [!DNL Adobe Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Wählen Sie das Team aus, dem das Projekt gehört, das das Asset enthält, zu dem Sie Details abrufen möchten, oder ordnen Sie es zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projekt-ID]</td> 
   <td> <p> Wählen Sie das Projekt aus, das das Asset enthält, über das Sie Details abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner-ID] </td> 
   <td> <p>Wählen Sie den Ordner aus, der das Asset enthält, über das Sie Details abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-ID] </td> 
   <td> <p>Wählen Sie das Asset aus oder ordnen Sie die ID des Assets zu, zu dem Sie Details abrufen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Auflisten von Assets]

Dieses Suchmodul ruft alle Assets im Ordner des angegebenen Projekts ab.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Frame.io], siehe <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] nach [!DNL Adobe Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Wählen Sie das Team aus oder ordnen Sie es zu, dem das Projekt gehört, das den Ordner enthält, aus dem Sie Assets abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projekt-ID]</td> 
   <td> <p> Wählen Sie das Projekt aus, das den Ordner enthält, aus dem Sie Assets abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner-ID] </td> 
   <td> <p>Wählen Sie den Ordner aus, aus dem Sie Assets auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Maximale Anzahl von Assets festlegen [!DNL Workfront Fusion] wird während eines Ausführungszyklus zurückgegeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### `[!UICONTROL Update an Asset]`

Mit diesem Aktionsmodul können Sie den Namen, die Beschreibung oder die benutzerdefinierten Felder eines vorhandenen Assets aktualisieren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Frame.io], siehe <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] nach [!DNL Adobe Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Wählen Sie das Team aus, dem das Projekt gehört, für das Sie ein Asset aktualisieren möchten, oder ordnen Sie es zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projekt-ID] </td> 
   <td> <p>Wählen Sie das Projekt aus oder ordnen Sie die ID des Projekts zu, für das Sie ein Asset aktualisieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner-ID] </td> 
   <td> <p>Wählen Sie den Ordner aus oder ordnen Sie die ID des Ordners zu, in dem Sie ein Asset aktualisieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Geben Sie den Namen der aktualisierten Datei ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Beschreibung] </td> 
   <td> <p>Geben Sie eine kurze Beschreibung des aktualisierten Assets ein.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Asset löschen ansehen]

Dieses Trigger-Modul startet ein Szenario, wenn ein Asset gelöscht wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> Geben Sie den Namen des Webhooks ein, z. B. Asset gelöscht.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Frame.io], siehe <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] nach [!DNL Adobe Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Wählen Sie das Team aus, für das dieser Webhook erstellt wurde.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Asset-Bezeichnung ansehen aktualisiert]

Dieses Trigger-Modul startet ein Szenario, in dem der Status eines Assets festgelegt, geändert oder entfernt wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> Geben Sie den Namen des Webhooks ein, z. B. Asset-Status aktualisiert.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Frame.io], siehe <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] nach [!DNL Adobe Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Wählen Sie das Team aus, für das dieser Webhook erstellt wurde.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Neues Asset ansehen]

Dieses Trigger-Modul startet ein Szenario, wenn ein neues Asset erstellt wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> Geben Sie den Namen des Webhooks ein, z. B. erstelltes Asset.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Frame.io], siehe <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] nach [!DNL Adobe Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Wählen Sie das Team aus, für das dieser Webhook erstellt wurde.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Kommentare

* [[!UICONTROL Kommentar erstellen]](#create-a-comment)
* [[!UICONTROL Löschen eines Kommentars]](#delete-a-comment)
* [[!UICONTROL Kommentar abrufen]](#get-a-comment)
* [[!UICONTROL Kommentare auflisten]](#list-comments)
* [[!UICONTROL Kommentar aktualisieren]](#update-a-comment)
* [[!UICONTROL Überwachungskommentar aktualisiert]](#watch-comment-updated)
* [[!UICONTROL Neuen Kommentar ansehen]](#watch-new-comment)

#### [!UICONTROL Kommentar erstellen]

Dieses Aktionsmodul fügt dem Asset einen neuen Kommentar oder eine neue Antwort hinzu.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Frame.io], siehe <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] nach [!DNL Adobe Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Typ] </td> 
   <td> <p>Wählen Sie aus, ob Sie einen Kommentar oder eine Antwort auf einen Kommentar erstellen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Wählen Sie das Team aus, dem das Projekt gehört, das das Asset enthält, dem Sie einen Kommentar hinzufügen möchten, oder ordnen Sie es zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projekt-ID] </td> 
   <td> <p>Wählen Sie das Projekt aus oder ordnen Sie die ID des Projekts zu, das das Asset enthält, dem Sie einen Kommentar hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner-ID] </td> 
   <td> <p>Wählen Sie den Ordner aus oder ordnen Sie die ID des Ordners zu, der das Asset enthält, dem Sie einen Kommentar hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-ID] </td> 
   <td> <p>Wählen Sie das Asset aus oder ordnen Sie es zu, dem Sie einen Kommentar hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kommentar-ID] </td> 
   <td> <p>Wählen Sie den Kommentar aus oder ordnen Sie ihn zu, dem Sie eine Antwort hinzufügen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td> <p> Geben Sie den Textinhalt des Kommentars oder der Antwort ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zeitstempel] </td> 
   <td> <p>Geben Sie die Bildnummer im Video ein, mit der der Kommentar verknüpft werden soll.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Löschen eines Kommentars]

Dieses Aktionsmodul löscht einen vorhandenen Kommentar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Frame.io], siehe <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] nach [!DNL Adobe Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID]</td> 
   <td> <p> Wählen Sie das Team aus, dem das Projekt gehört, das das Asset enthält, aus dem Sie einen Kommentar löschen möchten, oder ordnen Sie es zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projekt-ID]</td> 
   <td> <p> Wählen Sie das Projekt aus oder ordnen Sie die ID des Projekts zu, das das Asset enthält, aus dem Sie einen Kommentar löschen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner-ID]</td> 
   <td> <p> Wählen Sie den Ordner aus, der das Asset enthält, aus dem Sie einen Kommentar löschen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-ID] </td> 
   <td> <p>Wählen Sie das Asset aus, das den zu löschenden Kommentar enthält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kommentar-ID] </td> 
   <td> <p>Wählen Sie den Kommentar aus, den Sie löschen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kommentar abrufen]

Dieses Aktionsmodul ruft Details zum angegebenen Kommentar ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Frame.io], siehe <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] nach [!DNL Adobe Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Wählen Sie das Team aus oder ordnen Sie es zu, dem das Projekt gehört, das den Ordner enthält, aus dem Sie Assets abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projekt-ID] </td> 
   <td> <p>Wählen Sie das Projekt aus, das den Ordner enthält, aus dem Sie Assets abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner-ID] </td> 
   <td> <p>Wählen Sie den Ordner aus, aus dem Sie Assets auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-ID] </td> 
   <td> <p>Wählen Sie das Asset aus, das den Kommentar enthält, den Sie abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kommentar-ID] </td> 
   <td> <p>Wählen Sie den Kommentar aus, zu dem Sie Details abrufen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kommentare auflisten]

Dieses Suchmodul ruft alle Kommentare des angegebenen Assets ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Frame.io], siehe <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] nach [!DNL Adobe Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Wählen Sie das Team aus, dem das Projekt gehört, das den Ordner enthält, aus dem Sie Kommentare abrufen möchten, oder ordnen Sie es zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projekt-ID] </td> 
   <td> <p>Wählen Sie das Projekt aus, das den Ordner enthält, aus dem Sie Kommentare abrufen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner-ID] </td> 
   <td> <p>Wählen Sie den Ordner aus, der das Asset enthält, aus dem Sie Kommentare auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-ID] </td> 
   <td> <p>Wählen Sie das Asset aus, für das Sie Kommentare auflisten möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Maximale Anzahl an Kommentaren festlegen [!DNL Workfront Fusion] wird während eines Ausführungszyklus zurückgegeben.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Kommentar aktualisieren]

Dieses Aktionsmodul bearbeitet einen vorhandenen Kommentar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Frame.io], siehe <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] nach [!DNL Adobe Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Wählen Sie das Team aus, dem das Projekt gehört, das das Asset enthält, für das Sie einen Kommentar aktualisieren möchten, oder ordnen Sie es zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projekt-ID] </td> 
   <td> <p>Wählen Sie das Projekt \ aus, das das Asset enthält, für das Sie einen Kommentar aktualisieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Ordner-ID] </td> 
   <td> <p>Wählen Sie den Ordner aus, der das Asset enthält, für das Sie einen Kommentar aktualisieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset-ID] </td> 
   <td> <p>Wählen Sie das Asset aus, für das Sie einen Kommentar aktualisieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kommentar-ID] </td> 
   <td> <p>Wählen Sie den Kommentar aus, den Sie aktualisieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td> <p> Geben Sie den Textinhalt des Kommentars ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Zeitstempel] </td> 
   <td> <p>Geben Sie die Bildnummer im Video ein, mit der der Kommentar verknüpft ist.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Überwachungskommentar aktualisiert]

Dieses Trigger-Modul startet ein Szenario, wenn ein Kommentar bearbeitet wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name] </td> 
   <td> <p>Geben Sie den Namen des Webhooks ein, z. B. Kommentar bearbeitet.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Frame.io], siehe <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] nach [!DNL Adobe Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Wählen Sie das Team aus, für das dieser Webhook erstellt wurde.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Neuen Kommentar ansehen]

Dieses Trigger-Modul startet ein Szenario, wenn ein neuer Kommentar oder eine neue Antwort erstellt wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name] </td> 
   <td> <p>Geben Sie den Namen des Webhooks ein, z. B. neuen Kommentar.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Frame.io], siehe <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] nach [!DNL Adobe Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Wählen Sie das Team aus, für das dieser Webhook erstellt wurde.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Projekte

#### [!UICONTROL Projekte auflisten]

Dieses Suchmodul ruft alle Projekte für das angegebene Team ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Frame.io], siehe <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] nach [!DNL Adobe Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>Wählen Sie das Team aus, für das Sie Projekte abrufen möchten, oder ordnen Sie es zu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Maximale Anzahl an Projekten festlegen [!DNL Workfront Fusion] wird während eines Ausführungszyklus zurückgegeben.</p> </td> 
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
    <td role="rowheader">[!UICONTROL Verbindung] </td> 
   <td>Anweisungen zum Erstellen einer Verbindung zu [!DNL Frame.io], siehe <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">Verbinden [!DNL Frame.io] nach [!DNL Adobe Workfront Fusion]</a> in diesem Artikel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Geben Sie einen Pfad relativ zu ein <code>https://api.frame.io</code>. Beispiel: <code> /v2/teams</code></p> <p>Hinweis: Die Liste der verfügbaren Endpunkte finden Sie im Abschnitt [!DNL Frame.io] API-Referenz.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Methode]</p> </td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] fügt automatisch Autorisierungskopfzeilen hinzu.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Abfragezeichenfolge] </td> 
   <td> <p>Geben Sie die Abfragezeichenfolge der Anfrage ein. Klicken Sie für jeden Parameter, den Sie in die Abfragezeichenfolge aufnehmen möchten, auf <b>[!UICONTROL Element hinzufügen]</b> und geben Sie den Namen des Felds sowie den gewünschten Wert ein.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Fügen Sie den Textinhalt für den API-Aufruf in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Notiz:  <p>Bei Verwendung von bedingten Anweisungen wie <code>if</code> Fügen Sie die Anführungszeichen in Ihre JSON-Datei außerhalb der bedingten Anweisung ein.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**Beispiel:** Der folgende API-Aufruf gibt alle Teams und deren Details in Ihrer [!DNL Frame.io] Konto:

URL: `/v2/teams`

Methode: `GET`

![](assets/api-call-example.png)

Das Ergebnis finden Sie in der Ausgabe des Moduls unter Bundle > Hauptteil.

In unserem Beispiel wurden die Details von 1 Team zurückgegeben:

![](assets/api-call-output.png)
