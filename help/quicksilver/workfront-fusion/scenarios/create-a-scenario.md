---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Erstellen eines Szenarios in Adobe Workfront Fusion
description: Die folgenden Aufgaben erläutern, wie Sie eine [!DNL Adobe Workfront Fusion] Szenario.
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '1428'
ht-degree: 0%

---

# Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]

Die folgenden Aufgaben erläutern, wie Sie eine [!DNL Adobe Workfront Fusion] Szenario.

Eine Übung, die Sie durch die Erstellung eines Automatisierungsszenarios führt, finden Sie unter [Erstellen Sie ein Automatisierungsszenario für Vorgehensweisen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md).

Eine Übung, die Sie durch die Erstellung eines Integrationsszenarios mit von uns bereitgestellten Daten führt, finden Sie unter [Erstellen eines Szenarios für die Integration von Verfahren in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

>[!NOTE]
>
>Informationen zum Erstellen eines Szenarios aus einer Vorlage finden Sie unter [Erstellen von Szenarien mit [!DNL Adobe Workfront Fusion] templates](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p><p>[!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Erstellen eines Szenarios beginnen

1. Klicken **[!UICONTROL Szenarien]** ![](assets/scenarios-icon.png) im linken Bereich.

1. Klicken **[!UICONTROL Neues Szenario erstellen]** in der oberen rechten Ecke der Seite.
1. (Optional) Unter **[!UICONTROL Welche Dienste möchten Sie integrieren?]** Wenn Sie ein neues Szenario erstellen, wählen Sie Apps aus, mit denen Sie in dem Szenario arbeiten möchten, und klicken Sie dann auf **[!UICONTROL Weiter]**.

   Oder

   Klicken **[!UICONTROL Überspringen]** , wenn Sie die Apps im Szenario-Editor auswählen möchten.

1. Wenn Sie ein neues Szenario erstellen, klicken Sie im angezeigten Bildschirm (im Szenario-Editor) auf **[!UICONTROL Neues Szenario]** in der linken oberen Ecke ein und geben Sie einen Namen für das Szenario ein.
1. Fahren Sie fort mit [Hinzufügen eines Moduls in einem Szenario](#add-a-module-in-a-scenario).

## Hinzufügen eines Moduls in einem Szenario

1. Um das erste Modul zum Szenario hinzuzufügen, klicken Sie auf das Fragezeichen-Symbol. ![](assets/question-mark-icon.gif)

   Oder

   Um dem Szenario weitere Module hinzuzufügen, klicken Sie auf das Handle auf der rechten Seite des Moduls, dem Sie folgen möchten.

1. Klicken Sie im angezeigten Feld auf die App oder den Dienst, mit der/dem Sie beginnen möchten.

   Alle zuvor ausgewählten Apps werden im Feld für einfachen Zugriff und im **[!UICONTROL Favoriten]** unten auf dem Bildschirm.

   Wenn Sie auf **[!UICONTROL Hinzufügen eines weiteren Moduls]**, hängen die angezeigten Module davon ab, wo Sie im Szenario das Modul hinzufügen. Einige Module können nur zwischen anderen Modulen platziert werden, andere nur am Anfang des Szenarios.

   >[!TIP]
   >
   >Die beiden häufigsten Modultypen sind Aktionen und Trigger. Weitere Informationen finden Sie unter [Modultypen](../../workfront-fusion/modules/module-types.md).

1. Klicken Sie in der Liste der angezeigten Module auf das erste Modul, das Sie zum Szenario hinzufügen möchten.

   Die angezeigten Module hängen davon ab, wo Sie ein Modul in Ihrem Szenario hinzufügen möchten. Einige Module können nur zwischen anderen Modulen platziert werden, andere nur am Anfang des Szenarios.

   Die beiden häufigsten Modultypen sind Aktionen und Trigger. Weitere Informationen finden Sie unter [Modultypen](../../workfront-fusion/modules/module-types.md).

1. Fahren Sie fort mit [Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion).

## Verbinden Sie die App oder den Webdienst des Moduls mit [!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

Workfront Fusion-Module, die eine Verbindung zu einer App herstellen (z. B. [!DNL Workfront], [!DNL Salesforce]oder [!DNL Jira)] Funktion [!UICONTROL Verbindung] -Feld. Hier können Sie die Verbindung angeben, über die dieses Modul eine Verbindung zur App herstellen soll. Sie können eine vorhandene Verbindung aus dem Dropdown-Menü auswählen oder eine neue Verbindung erstellen.

Wenn Sie in einem Szenario eine Verbindung für eine App auswählen oder erstellen, verwenden andere Module für diese App automatisch dieselbe Verbindung, es sei denn, Sie wählen beim Einrichten der späteren Module eine andere Verbindung aus.

Weitere Informationen finden Sie unter [Über die Verbindung [!DNL Adobe Workfront Fusion] an eine App oder einen Dienst](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

![](assets/connection-field-350x169.png)

So erstellen Sie eine Verbindung innerhalb einer [!DNL Workfront Fusion] -Modul:

1. Klicken **[!UICONTROL Hinzufügen]** , um **[!UICONTROL Verbindung erstellen]** ankreuzen.
1. (Optional) Ändern Sie die Standardeinstellung **[!UICONTROL Verbindungsname]**.
1. (Bedingt) Wenn für die App erweiterte Verbindungseinstellungen erforderlich sind, z. B. eine ID, einen Schlüssel oder [!UICONTROL secret]eingeben.

   Möglicherweise müssen Sie auf **[!UICONTROL Erweiterte Einstellungen anzeigen]** um die Felder anzuzeigen, in die Sie diese Art von Informationen eingeben können.

1. Klicken **[!UICONTROL Weiter]**.
1. Geben Sie im angezeigten Anmeldefenster Ihre Anmeldedaten ein, um sich bei der App anzumelden, falls noch nicht geschehen.
1. (Bedingt) Wenn eine **[!UICONTROL Zulassen]** angezeigt wird, untersuchen Sie die Aktionen, die der Connector ausführen kann, und klicken Sie dann auf die Schaltfläche, um die App mit [!DNL Workfront Fusion].
1. Fahren Sie fort mit [Modul konfigurieren](#configure-the-module).


## Modul konfigurieren

1. Konfigurieren Sie in den Feldern unter dem Feld Verbindung die Einstellungen für das Modul und klicken Sie auf **[!UICONTROL OK]**.

   ![](assets/conf-settigs-mod-350x547.png)

   Diese Einstellungen sind für jedes Modul unterschiedlich. Ein fett hervorgehobener Titel zeigt eine erforderliche Einstellung an.

   >[!TIP]
   >
   >Während Sie an Ihrem Szenario arbeiten, können Sie auf das Modul klicken, um dieses Feld mit Einstellungen jederzeit anzuzeigen.
   >
   >
   >Wenn ein schwarzer Kreis auf einem Modul angezeigt wird, haben Sie die Konfiguration der Einstellungen noch nicht abgeschlossen. Klicken Sie auf das Modul, um es zu öffnen und mit der Konfiguration fortzufahren.
   >
   >
   >![](assets/black-error-circle-on-module.png)

1. Wenn Sie das erste Modul in Ihrem Szenario hinzufügen, wählen Sie eine Option aus, um bei jeder Ausführung anzugeben, wo das Szenario beginnen soll.

   ![](assets/choose-where-start-350x194.png)

1. Wiederholen Sie die Schritte in den Abschnitten . [Hinzufügen eines Moduls in einem Szenario](#add-a-module-in-a-scenario) und [Modul konfigurieren](#configure-the-module) , um weitere Module zum Szenario hinzuzufügen.

1. (Optional) Kopieren Sie ein Modul oder eine Gruppe von Modulen und fügen Sie es ein.

   Weitere Informationen finden Sie unter [Kopieren von Modulen oder Szenarien in Adobe Workfront Fusion](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

1. Fahren Sie fort mit [Konfigurieren und Arbeiten mit Ihrem Szenario](#configure-and-work-with-your-scenario).

## Konfigurieren und Arbeiten mit Ihrem Szenario

1. Führen Sie einen der folgenden Schritte aus, um Ihr Szenario zu konfigurieren:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Geben Sie an, wann und wie oft das Szenario ausgeführt wird</td> 
      <td> <p>Klicken Sie auf das Uhrensymbol. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Planen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Einrichten einer Route</td> 
      <td> <p>Klicken Sie auf das Schraubenschlüsselsymbol <img src="assets/wrench-icon.gif"> zwischen den beiden Modulen und verwenden Sie eine der folgenden Optionen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Hinzufügen eines Filters zu einem Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> 
       <ul> 
        <li><strong>[!UICONTROL Filter einrichten]</strong>: Legen Sie fest, welche Bundles an bestimmten Punkten im Szenario verwendet werden.</li> 
        <li><strong>[!UICONTROL Unlink]</strong>: Entfernt eine Route.</li> 
        <li><strong>[!UICONTROL Router hinzufügen]</strong>: Fügt einen Router zwischen Modulen hinzu. </li> 
        <li><strong>[!UICONTROL Modul hinzufügen]</strong>: Fügt ein neues Modul zwischen Modulen hinzu.</li> 
        <li><strong>[!UICONTROL Notiz hinzufügen]</strong>: Fügt der Route einen Hinweis hinzu.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Konfigurieren der Szenario-Einstellungen</td> 
      <td>Klicken Sie auf das Symbol [!UICONTROL Szenario-Einstellungen]. <img src="assets/gear-icon-settings.png"> Diese Einstellungen richten sich in erster Linie an fortgeschrittene Benutzer. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Das Bedienfeld für die Szenario-Einstellungen in [!DNL Adobe Workfront Fusion]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Flusssteuerungseinstellungen konfigurieren</td> 
      <td> <p>Klicken Sie auf das Symbol [!UICONTROL Flusssteuerung] . <img src="assets/flow-control-icon.gif"> Sie können eine Aufgabe so einrichten, dass eine bestimmte Anzahl von Malen wiederholt, ein Array in eine Reihe von Bundles konvertiert und mehrere Bundles zu einem Bundle zusammengeführt werden. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Flusssteuerung in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erweitern des Szenarios mit erweiterten Tools</td> 
      <td>Klicken Sie auf [!DNL Tools] Symbol. <img src="assets/tools-icon.gif"> Sie können Trigger, Aktionen, Aggregatoren und Transformatoren erstellen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Instrumente</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Analyse von Benutzertext</td> 
      <td>Klicken Sie auf [!DNL Text parser] icon <img src="assets/text-parser-icon.gif">. Sie können Elemente aus dem HTML-Code abrufen, Zeichenfolgen-Elemente suchen und extrahieren, die einem Suchmuster entsprechen,-Text suchen und ersetzen und Daten von einer Website "auseinanderziehen". Weitere Informationen finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Instrumente</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Führen Sie einen der folgenden Schritte aus, um mit Ihrem Szenario zu arbeiten:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anzeigen eines Protokolls der Ereignisse, die beim Ausführen des Szenarios auftreten</td> 
      <td> <p>Klicken Sie auf den Pfeil [!UICONTROL Beenden bearbeiten] <img src="assets/exit-editing-arrow.png"> im Szenario-Editor, um die Detailseite des Szenarios anzuzeigen. Das Protokoll wird unten im Fenster oder in der rechten unteren Ecke angezeigt. Er enthält Informationen zu jeder Phase sowie zu Fehlern, die während der Ausführung des Szenarios aufgetreten sind.</p> <p>So kehren Sie zur Arbeit mit Ihrem Szenario im [!DNL scenario editor]klicken Sie auf eine beliebige Stelle auf der Detailseite "Szenario".</p> <p>Weitere Informationen zur Detailseite des Szenarios finden Sie unter <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Details zum Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zugriff auf die am häufigsten verwendeten Apps und Dienste</td> 
      <td> Klicken Sie auf ein Symbol im <strong>[!UICONTROL Favoriten]</strong> unten auf dem Bildschirm. In diesem Abschnitt werden automatisch Symbole angezeigt, wenn Sie Ihrem Szenario Apps und Dienste hinzufügen. Sie können auch auf das Symbol [!UICONTROL Hinzufügen] klicken <img src="assets/add-icon.gif"> , um diesem Bereich manuell Apps und Dienste hinzuzufügen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eine Animation anzeigen, die zeigt, wie Daten durch das Szenario fließen</td> 
      <td>Klicken Sie auf das Symbol [!UICONTROL Fluss erläutern] <img src="assets/explain-flow-airplane-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Layout der Module automatisch ausrichten </td> 
      <td>Klicken Sie auf das Symbol [!UICONTROL Automatische Ausrichtung] . <img src="assets/auto-align-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Typ- oder Ansichtsnotizen zum Szenario</td> 
      <td>Klicken Sie auf das Symbol [!UICONTROL Notizen <img src="assets/notes-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entfernen von Modulen</td> 
      <td>Klicken Sie mit der rechten Maustaste auf das Modul und klicken Sie dann auf <strong>[!UICONTROL Löschmodul]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Um das Szenario zu testen, klicken Sie auf **[!UICONTROL Einmal ausführen]**.

   Es ist wichtig zu überprüfen, ob das Szenario erwartungsgemäß ausgeführt wird, bevor Sie es aktivieren. Nach der Aktivierung wird das Szenario gemäß seinem Zeitplan ausgeführt. Wenn alles nicht wie erwartet ausgeführt wird, lesen Sie [Umgang mit Fehlern in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).

1. Wenn Sie die Bearbeitung des Szenarios (oder zu einem beliebigen Zeitpunkt während der Bearbeitung) abgeschlossen haben, klicken Sie auf die Schaltfläche [!UICONTROL Speichern] Symbol unten im Fenster ![](assets/save-icon.gif).

Informationen zum Aktivieren eines Szenarios finden Sie unter [Aktivieren oder deaktivieren Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

## Tastaturbefehle für das Workfront Fusion-Szenario

Sie können beim Erstellen oder Bearbeiten eines Szenarios die folgenden Tastaturbefehle verwenden:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p>Aktion</p> </th> 
   <th>[!DNL Windows]</th> 
   <th> <p>[!DNL MacOS]</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Save] </td> 
   <td>Strg+Umschalt+S</td> 
   <td><span style="font-weight: normal;">Befehl+Umschalt+S</span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Einmal ausführen]</td> 
   <td>Strg+Umschalt+Eingabetaste</td> 
   <td><span style="font-weight: normal;">Befehl+Umschalt+Eingabetaste</span> </td> 
  </tr> 
 </tbody> 
</table>
