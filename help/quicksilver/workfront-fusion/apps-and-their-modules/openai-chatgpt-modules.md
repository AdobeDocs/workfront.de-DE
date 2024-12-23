---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Connector
navigation-topic: apps-and-their-modules
title: OpenAI-Module (ChatGPT)
description: In einem Adobe Workfront Fusion-Szenario können Sie Workflows automatisieren, die OpenAIT (ChatGPT) verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.
author: Becky
feature: Workfront Fusion
exl-id: 3a747013-5fb6-4416-8d95-d656dfeeb7db
source-git-commit: 2e91e9a4c691430f3c98e3cbddb30706ea57f84a
workflow-type: tm+mt
source-wordcount: '1339'
ht-degree: 0%

---

# [!DNL OpenAI (ChatGPT & DALL-E)] Module

In einem [!DNL Adobe Workfront Fusion] -Szenario können Sie Workflows automatisieren, die [!DNL OpenAI (ChatGPT & DALL-E)] verwenden, und sie mit mehreren Anwendungen und Diensten von Drittanbietern verbinden.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Voraussetzungen

Um [!DNL OpenAI (ChatGPT & DALL-E)] -Module zu verwenden, müssen Sie über ein [!DNL OpenAI] -Konto verfügen, das einen API-Schlüssel und eine Organisations-ID enthält.

## API-Informationen zu OpenAI (ChatGPT &amp; DALL-E)

Der OpenAI-Connector (ChatGPT &amp; DALL-E) verwendet Folgendes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">API-Version</td> 
   <td> v1 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-Tag</td> 
   <td>v1.11.1</td> 
  </tr>
 </tbody> 
 </table>

## Verbinden von [!DNL OpenAI (ChatGPT & DALL-E)] mit [!DNL Workfront Fusion]

Sie können eine Verbindung zu Ihrem [!DNL OpenAI (ChatGPT & DALL-E)]-Konto direkt aus einem [!DNL OpenAI (ChatGPT & DALL-E)]-Modul erstellen.

1. Klicken Sie in einem beliebigen [!DNL OpenAI (ChatGPT & DALL-E)]-Modul neben dem Feld [!UICONTROL Verbindung] auf **[!UICONTROL Hinzufügen]** .
1. Geben Sie die folgenden Informationen ein:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Verbindungsname]</p> </td> 
      <td> <p>Geben Sie einen Namen für die neue Verbindung ein.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL API-Schlüssel]</td> 
      <td>Sie finden Ihren API-Schlüssel in Ihren OpenAI-Benutzereinstellungen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Organisations-ID] </td> 
      <td>Sie finden Ihre Organisations-ID auf Ihrer Seite mit den Unternehmenseinstellungen in OpenAI.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Weiter]** , um die Verbindung zu erstellen und zum Modul zurückzukehren.


## [!DNL OpenAI (ChatGPT & DALL-E)] Module und ihre Felder

Wenn Sie [!DNL OpenAI (ChatGPT & DALL-E)] -Module konfigurieren, zeigt [!DNL Workfront Fusion] die unten aufgeführten Felder an. Darüber hinaus können abhängig von Faktoren wie Ihrer Zugriffsebene in der App oder im Dienst zusätzliche [!DNL OpenAI (ChatGPT & DALL-E)] -Felder angezeigt werden. Ein fett hervorgehobener Titel in einem Modul zeigt ein erforderliches Feld an.

Wenn Sie die Zuordnungsschaltfläche über einem Feld oder einer Funktion sehen, können Sie damit Variablen und Funktionen für dieses Feld festlegen. Weitere Informationen finden Sie unter [Informationen von einem Modul einem anderen zuordnen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Erstellen eines Abschlusses

>[!IMPORTANT]
>
>Dieses Modul wird nicht mehr unterstützt.

<!--

This action module creates a completion for the provided prompt or chat.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL OpenAI (ChatGPT & DALL-E)] account to Workfront Fusion, see <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connecting [!DNL OpenAI (ChatGPT & DALL-E)] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Model]</td> 
   <td> Enter or map the ID of the model to use. You can use the Get models module to see all of your available models. </td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL Temperature]</td> 
   <td> This value must be between 0 and 2, and determines the randomness of the output. Higher values produce output that is more random, while lower values produce more focused output. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>For information about the optional advanced settings in this module, see the information about creating completions in the <a href="https://platform.openai.com/docs/api-reference/completions/create" class="MCXref xref">OpenAI API documentation</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

### Erstellen einer Moderation

Dieses Aktionsmodul ermittelt, ob Text gegen die Inhaltsrichtlinie von OpenAI verstößt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL OpenAI (ChatGPT & DALL-E)]-Kontos mit Workfront Fusion finden Sie in diesem Artikel unter <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL OpenAI (ChatGPT & DALL-E)] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Input]</td> 
   <td> Klicken Sie für jedes Beispiel von Text, den Sie einbeziehen möchten, auf <b>Element hinzufügen</b> und geben Sie den Text ein oder ordnen Sie ihn zu. Schließen Sie das gesamte Textbeispiel ein.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Modell]</td> 
   <td> Geben Sie die Kennung des zu verwendenden Modells ein oder ordnen Sie sie zu. Sie können das Modul Modelle abrufen verwenden, um alle verfügbaren Modelle anzuzeigen. </td> 
  </tr> 
 </tbody> 
</table>

### Erstellen einer Bearbeitung

Dieses Aktionsmodul gibt eine bearbeitete Version einer von Ihnen angegebenen Eingabeaufforderung zurück, die Ihren Anweisungen entspricht.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL OpenAI (ChatGPT & DALL-E)]-Kontos mit Workfront Fusion finden Sie in diesem Artikel unter <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL OpenAI (ChatGPT & DALL-E)] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Modell]</td> 
   <td> Geben Sie die Kennung des zu verwendenden Modells ein oder ordnen Sie sie zu. Sie können das Modul Modelle abrufen verwenden, um alle verfügbaren Modelle anzuzeigen. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Input]</td> 
   <td> Geben Sie den Text ein oder ordnen Sie ihn zu, den Sie bearbeiten möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Instruction]</td> 
   <td> Geben Sie die Anweisungen für die Bearbeitung ein oder ordnen Sie sie zu. Beispiel: "Korrigieren Sie die Rechtschreibfehler." </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Erweiterte Einstellungen</td> 
   <td> <p>Informationen zu den optionalen erweiterten Einstellungen in diesem Modul finden Sie in den Informationen zum Erstellen von Bearbeitungen in der <a href="https://platform.openai.com/docs/api-reference/edits/create" class="MCXref xref">OpenAI API-Dokumentation</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Erstellen einer Einbettung

Dieses Aktionsmodul erstellt einen eingebetteten Vektor, der den Eingabetext darstellt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL OpenAI (ChatGPT & DALL-E)]-Kontos mit Workfront Fusion finden Sie in diesem Artikel unter <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL OpenAI (ChatGPT & DALL-E)] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Modell]</td> 
   <td> Geben Sie die Kennung des zu verwendenden Modells ein oder ordnen Sie sie zu. Sie können das Modul Modelle abrufen verwenden, um alle verfügbaren Modelle anzuzeigen. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Einfügetext]</td> 
   <td> Geben Sie den Text ein oder ordnen Sie ihn zu, den Sie einbetten möchten. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Benutzer-ID]</td> 
   <td> Eingeben oder Zuordnen einer eindeutigen Kennung, die Ihren Endbenutzer darstellt und OpenAI bei der Überwachung und Erkennung von Missbrauch unterstützen kann </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> Geben Sie die maximale Anzahl von Bearbeitungen ein oder ordnen Sie sie zu, mit denen das Modul während der einzelnen Szenario-Ausführungszyklen arbeiten soll.</td> 
  </tr> 
 </tbody> 
</table>

### Erstellen eines Chat-Abschlusses

Bei einer Liste von Nachrichten, die eine Konversation beschreiben, gibt dieses Aktionsmodul eine Antwort zurück.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL OpenAI (ChatGPT & DALL-E)]-Kontos mit Workfront Fusion finden Sie in diesem Artikel unter <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL OpenAI (ChatGPT & DALL-E)] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Modell]</td> 
   <td> Geben Sie die Kennung des zu verwendenden Modells ein oder ordnen Sie sie zu. Sie können das Modul Modelle abrufen verwenden, um alle verfügbaren Modelle anzuzeigen. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Messages]</td> 
   <td>Nachrichten beschreiben die Konversation bisher. Klicken Sie für jede Nachricht, die Sie hinzufügen möchten, auf <b>Element hinzufügen</b> und geben Sie Folgendes ein:
   <ul>
   <li> <b>Rolle</b>: Wählen Sie die Rolle des Autors dieser Nachricht aus.</li>
   <li> <b>Inhalt</b>: Geben Sie den Inhalt dieser Nachricht ein oder ordnen Sie ihn zu.</li>
   <li> <b>Name</b>: Geben Sie den Namen des Autors dieser Nachricht ein oder ordnen Sie ihn zu. Der Name kann Groß- und Kleinbuchstaben, Zahlen und Unterstriche enthalten. Die maximale Länge des Namens beträgt 64 Zeichen.</li>
   </ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Erweiterte Einstellungen</td> 
   <td> <p>Informationen zu den optionalen erweiterten Einstellungen in diesem Modul finden Sie in der Dokumentation zur <a href="https://platform.openai.com/docs/api-reference/chat/create" class="MCXref xref">OpenAI-API-Dokumentation</a> in den Informationen zum Erstellen von Chat-Abschlüssen.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--

### Edit image

This action module makes edits or creates variations of existing images.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL OpenAI (ChatGPT & DALL-E)] account to Workfront Fusion, see <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connecting [!DNL OpenAI (ChatGPT & DALL-E)] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select the operation]</td> 
   <td> Select whether you want to create edits or variations of the image.
   <p>NOTE: Images must be a valid PNG file, less than 4MB, and square. If mask is not provided, the image must have transparency, which will be used as the mask.</p> 
 </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Text description of desired image]</td> 
   <td> <p>If editing an image, enter or map a description of the edits you want to create. Maximum length is 1000 characters.</p> </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>For information about the optional advanced settings in this module, see the information about creating image edits or variations in the <a href="https://platform.openai.com/docs/api-reference/images/createEdit" class="MCXref xref">OpenAI API documentation</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

### Bilder generieren

Dieses Aktionsmodul generiert oder bearbeitet Bilder mit Dall-E-Modellen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL OpenAI (ChatGPT & DALL-E)]-Kontos mit Workfront Fusion finden Sie in diesem Artikel unter <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL OpenAI (ChatGPT & DALL-E)] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Textbeschreibung des gewünschten Bildes]</td> 
   <td> Geben Sie eine Beschreibung des gewünschten Bildes ein oder ordnen Sie es zu. Die maximale Länge der Beschreibung beträgt 1000 Zeichen. 
 </td> 
  </tr> 
   <tr> 
   <td role="rowheader">Erweiterte Einstellungen</td> 
   <td> <p>Informationen zu den optionalen erweiterten Einstellungen in diesem Modul finden Sie in den Informationen zum Erstellen von Bildern in der <a href="https://platform.openai.com/docs/api-reference/images/create" class="MCXref xref">OpenAI API-Dokumentation</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Modelle abrufen

In diesem Modul werden die verschiedenen in der OpenAI-API verfügbaren Modelle aufgelistet und beschrieben.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL OpenAI (ChatGPT & DALL-E)]-Kontos mit Workfront Fusion finden Sie in diesem Artikel unter <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL OpenAI (ChatGPT & DALL-E)] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aktion]</td> 
   <td> Wählen Sie aus, ob Sie eine Liste aller Modelle erhalten oder ein bestimmtes Modell abrufen möchten.
    <ul>
    <li><p><b>Listenmodelle </b></p><p>Diese Aktion listet die derzeit verfügbaren Modelle auf und liefert grundlegende Informationen zu jedem Modell, wie dem Eigentümer und der Verfügbarkeit.</p></li>
    <li><p><b>Modell abrufen </b></p><p>Geben Sie die Kennung des Modells ein, das Sie abrufen möchten, oder ordnen Sie sie zu. </p></li>
   </ul>
 </td> 
  </tr>
 </tbody> 
</table>

### Benutzerdefinierter API-Aufruf

Dieses Aktionsmodul enthält eine benutzerdefinierte HTTP-Anforderung an die OpenAI-API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL OpenAI (ChatGPT & DALL-E)]-Kontos mit Workfront Fusion finden Sie in diesem Artikel unter <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL OpenAI (ChatGPT & DALL-E)] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Pfad relativ zu <code>https://api.openai.com/v1/</code> eingeben </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Methode]</td> 
   <td> <p>Wählen Sie die HTTP-Anfragemethode aus, die Sie zum Konfigurieren des API-Aufrufs benötigen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-Anforderungsmethoden in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Header]</td> 
   <td> <p>Fügen Sie die Header der Anfrage in Form eines standardmäßigen JSON-Objekts hinzu.</p> <p>Beispiel: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion fügt die Autorisierungskopfzeilen automatisch hinzu.</p> </td> 
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
 </tbody> 
</table>

<!--

### Manage Audio

This action modules converts audio to text.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL OpenAI (ChatGPT & DALL-E)] account to Workfront Fusion, see <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Connecting [!DNL OpenAI (ChatGPT & DALL-E)] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Select the operation]</td> 
   <td> Select whether you want to transcribe the audio into the input language, or into English.
   <p>If transcribing into the input language, you can select the language in this module's advanced settings. </td> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> Enter or map the maximum number of edits you want the module to work with during each scenario execution cycle.</td> 
   <tr> 
   <td role="rowheader">[!UICONTROL Advanced settings]</td> 
   <td> <p>For information about the optional advanced settings in this module, see the information about creating transcriptions in the <a href="https://platform.openai.com/docs/api-reference/audio/createTranscription" class="MCXref xref">OpenAI API documentation</a>.</p> </td> 
  </tr> 
  </tr> 
 </tbody> 
</table>

-->

### Dateien verwalten

Dieses Aktionsmodul listet, löscht oder ruft Dateien oder Dateiinhalte ab.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL OpenAI (ChatGPT & DALL-E)]-Kontos mit Workfront Fusion finden Sie in diesem Artikel unter <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL OpenAI (ChatGPT & DALL-E)] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Aktion]</td> 
   <td> Wählen Sie die Aktion aus, die Sie ausführen möchten. 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Datei-ID]</td> 
   <td> Wenn Sie eine Datei löschen oder einen Datei- oder Dateiinhalt abrufen, geben Sie die Kennung der Datei ein oder ordnen Sie sie zu. 
  </tr> 
</tbody>
</table>

### Verwalten von Feinabstimmungen

Verwalten Sie Optimierungsaufträge, um ein Modell auf Ihre spezifischen Trainings-Daten anzupassen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Verbindung]</td> 
   <td> <p>Anweisungen zum Verbinden Ihres [!DNL OpenAI (ChatGPT & DALL-E)]-Kontos mit Workfront Fusion finden Sie in diesem Artikel unter <a href="#connecting-openaichatgpt-to-workfront-fusion" class="MCXref xref">Verbinden von [!DNL OpenAI (ChatGPT & DALL-E)] mit [!DNL Workfront Fusion]</a> .</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vorgang auswählen]</td> 
   <td> Wählen Sie die Aktion aus, die Sie ausführen möchten.
   <ul>
   <li><p>Modell aus einem Datensatz optimieren</p><p>Geben Sie eine Beschreibung für das gewünschte Bild ein oder ordnen Sie es zu.</p>
     <li><p>Abrufen von Informationen zu einem Feinsteuerungsauftrag</p><p>Geben Sie die Kennung des Auftrags ein oder ordnen Sie sie zu.</p>
   <li><p>Abbrechen eines Feinsteuerungsauftrags</p><p>Geben Sie die Kennung des Auftrags ein oder ordnen Sie sie zu.</p>
   <li><p>Abbrechen eines Feinsteuerungsauftrags</p><p>Geben Sie die Kennung des Auftrags ein oder ordnen Sie sie zu.</p>
   <li><p>Statusaktualisierungen für einen Feinsteuerungsauftrag abrufen</p><p>Geben Sie die ID des Auftrags ein oder ordnen Sie sie zu und wählen Sie aus, ob Sie diese Aktualisierungen streamen möchten.</p>
   <li><p>Feinabstimmungsmodell löschen</p><p>Geben Sie die Kennung des Modells ein, das Sie löschen möchten, oder ordnen Sie sie zu.</p>
 </ul> 
  </tr> 
   <tr> 
   <td role="rowheader">[!UICONTROL Datei-ID]</td> 
   <td> Wenn Sie eine Datei löschen oder einen Datei- oder Dateiinhalt abrufen, geben Sie die Kennung der Datei ein oder ordnen Sie sie zu. 
  </tr> 
</tbody>
