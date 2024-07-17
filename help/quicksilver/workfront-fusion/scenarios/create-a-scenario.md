---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Erstellen eines Szenarios in Adobe Workfront Fusion
description: Die folgenden Aufgaben erläutern, wie ein [!DNL Adobe Workfront Fusion] Szenario erstellt wird.
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: ee2283ac159ca26ca473cac28ec4bed85d1dea04
workflow-type: tm+mt
source-wordcount: '1406'
ht-degree: 0%

---

# Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]

Die folgenden Aufgaben erläutern, wie ein [!DNL Adobe Workfront Fusion] -Szenario erstellt wird.

Eine Übung, die Sie durch die Erstellung eines Automatisierungsszenarios führt, finden Sie unter [Erstellen eines Szenarios für die Automatisierung von Verfahren in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md).

Eine Übung, die Sie durch die Erstellung eines Integrationsszenarios mit von uns bereitgestellten Daten führt, finden Sie unter [Erstellen eines Szenarios für die Praxisintegration in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

>[!NOTE]
>
>Informationen zum Erstellen eines Szenarios aus einer Vorlage finden Sie unter [Erstellen von Szenarien mit  [!DNL Adobe Workfront Fusion] Vorlagen](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md) .

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Adobe Workfront-Abo</td>  
      <td>Alle</td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront-Lizenz</td>  
      <td>
        Neu: Standard<br>
        Oder<br>
        Aktuell: Arbeit oder höher
      </td>  
    </tr>  
    <tr>  
      <td>Adobe Workfront Fusion-Lizenz</td>  
      <td> 
        Aktuell: Keine Workfront Fusion-Lizenzanforderungen.<br>
        Oder<br>
        Veraltet: Beliebig
      </td>  
    </tr>  
    <tr>  
      <td>Produkt</td>  
      <td> 
        Neu: Wählen Sie den Workfront-Plan aus oder führen Sie ihn aus: Ihr Unternehmen muss Adobe Workfront Fusion erwerben.<br>
        Ultimate Workfront Plan: Workfront Fusion ist im Lieferumfang enthalten.<br>
        Oder<br>
        Aktuell: Ihr Unternehmen muss Adobe Workfront Fusion erwerben.
      </td>  
    </tr> 
  </tbody>  
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Erstellen eines Szenarios beginnen

1. Klicken Sie im linken Bereich auf **[!UICONTROL Szenarios]** ![](assets/scenarios-icon.png) .

1. Klicken Sie oben rechts auf der Seite auf **[!UICONTROL Neues Szenario erstellen]** .
1. Wenn Sie im angezeigten Bildschirm (im Szenario-Editor) ein neues Szenario erstellen, klicken Sie oben links auf **[!UICONTROL Neues Szenario]** und geben Sie einen Namen für das Szenario ein.
1. Fahren Sie mit [Hinzufügen eines Moduls in einem Szenario](#add-a-module-in-a-scenario) fort.

## Hinzufügen eines Moduls in einem Szenario

1. Um das erste Modul zum Szenario hinzuzufügen, klicken Sie auf das Fragezeichen-Symbol. ![](assets/question-mark-icon.gif)

   Oder

   Um dem Szenario weitere Module hinzuzufügen, klicken Sie auf das Handle auf der rechten Seite des Moduls, dem Sie folgen möchten.

1. Klicken Sie im angezeigten Feld auf die App oder den Dienst, mit der/dem Sie beginnen möchten.

   Alle zuvor ausgewählten Apps werden im Feld für einfachen Zugriff und im Abschnitt **[!UICONTROL Favoriten]** unten auf dem Bildschirm angezeigt.

   Wenn Sie auf **[!UICONTROL Add another module]** klicken, hängen die angezeigten Module davon ab, wo Sie das Modul im Szenario hinzufügen. Einige Module können nur zwischen anderen Modulen platziert werden, andere nur am Anfang des Szenarios.

   >[!TIP]
   >
   >Die beiden häufigsten Modultypen sind Aktionen und Trigger. Weitere Informationen finden Sie unter [Modultypen](../../workfront-fusion/modules/module-types.md).

1. Klicken Sie in der Liste der angezeigten Module auf das erste Modul, das Sie zum Szenario hinzufügen möchten.

   Die angezeigten Module hängen davon ab, wo Sie ein Modul in Ihrem Szenario hinzufügen möchten. Einige Module können nur zwischen anderen Modulen platziert werden, andere nur am Anfang des Szenarios.

   Die beiden häufigsten Modultypen sind Aktionen und Trigger. Weitere Informationen finden Sie unter [Modultypen](../../workfront-fusion/modules/module-types.md).

1. Fahren Sie mit [Verbinden Sie die App oder den Webdienst des Moduls mit  [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion) fort.

## Verbinden der App oder des Webdiensts des Moduls mit [!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

Workfront Fusion-Module, die eine Verbindung zu einer App herstellen (z. B. [!DNL Workfront], [!DNL Salesforce] oder [!DNL Jira)], weisen das Feld [!UICONTROL Verbindung] auf. Hier können Sie die Verbindung angeben, über die dieses Modul eine Verbindung zur App herstellen soll. Sie können eine vorhandene Verbindung aus dem Dropdown-Menü auswählen oder eine neue Verbindung erstellen.

Wenn Sie in einem Szenario eine Verbindung für eine App auswählen oder erstellen, verwenden andere Module für diese App automatisch dieselbe Verbindung, es sei denn, Sie wählen beim Einrichten der späteren Module eine andere Verbindung aus.

Weitere Informationen finden Sie unter [Übersicht über Verbindungen](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

![](assets/connection-field-350x169.png)

So erstellen Sie eine Verbindung innerhalb eines [!DNL Workfront Fusion]-Moduls:

1. Klicken Sie auf **[!UICONTROL Hinzufügen]** , um das Feld **[!UICONTROL Verbindung erstellen]** zu öffnen.
1. (Optional) Ändern Sie den standardmäßigen **[!UICONTROL Verbindungsnamen]**.
1. (Bedingt) Wenn für die App erweiterte Verbindungseinstellungen erforderlich sind, z. B. eine ID, einen Schlüssel oder [!UICONTROL secret], geben Sie diese Informationen ein.

   Möglicherweise müssen Sie auf **[!UICONTROL Erweiterte Einstellungen anzeigen]** klicken, um die Felder anzuzeigen, in die Sie diese Informationen eingeben können.

1. Klicken Sie auf **[!UICONTROL Weiter]**.
1. Geben Sie im angezeigten Anmeldefenster Ihre Anmeldedaten ein, um sich bei der App anzumelden, falls noch nicht geschehen.
1. (Bedingt) Wenn eine Schaltfläche **[!UICONTROL Zulassen]** angezeigt wird, untersuchen Sie die Aktionen, die der Connector ausführen kann, und klicken Sie dann auf die Schaltfläche , um die App mit [!DNL Workfront Fusion] zu verbinden.
1. Fahren Sie mit [Konfigurieren des Moduls](#configure-the-module) fort.


## Modul konfigurieren

1. Konfigurieren Sie in den Feldern unter dem Feld Verbindung die Einstellungen für das Modul und klicken Sie dann auf **[!UICONTROL OK]**.

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

1. Wiederholen Sie die Schritte in den Abschnitten [Modul in einem Szenario hinzufügen](#add-a-module-in-a-scenario) und [Modul konfigurieren](#configure-the-module) , um dem Szenario weitere Module hinzuzufügen.

1. (Optional) Kopieren Sie ein Modul oder eine Gruppe von Modulen und fügen Sie es ein.

   Weitere Informationen finden Sie unter [Kopieren von Modulen oder Szenarien in Adobe Workfront Fusion](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

1. Fahren Sie mit [Konfigurieren und Arbeiten mit Ihrem Szenario](#configure-and-work-with-your-scenario) fort.

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
        <li><strong>[!UICONTROL Filter einrichten]</strong>: Steuert, welche Bundles an bestimmten Punkten im Szenario verwendet werden.</li> 
        <li><strong>[!UICONTROL Unlink]</strong>: Entfernt eine Route.</li> 
        <li><strong>[!UICONTROL Router hinzufügen]</strong>: Fügt einen Router zwischen Modulen hinzu. </li> 
        <li><strong>[!UICONTROL Modul hinzufügen]</strong>: Fügt ein neues Modul zwischen Modulen hinzu.</li> 
        <li><strong>[!UICONTROL Notiz hinzufügen]</strong>: Fügt der Route einen Hinweis hinzu.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Konfigurieren der Szenario-Einstellungen</td> 
      <td>Klicken Sie auf das Symbol [!UICONTROL Szenario-Einstellungen]. <img src="assets/gear-icon-settings.png"> Diese Einstellungen sind hauptsächlich für fortgeschrittene Benutzer gedacht. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Das Bedienfeld mit den Szenario-Einstellungen in [!DNL Adobe Workfront Fusion]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Einstellungen zur Flusssteuerung konfigurieren</td> 
      <td> <p>Klicken Sie auf das Symbol [!UICONTROL Flusssteuerung] . <img src="assets/flow-control-icon.gif"> Sie können eine Aufgabe so einrichten, dass eine bestimmte Anzahl von Malen wiederholt, ein Array in eine Reihe von Bundles konvertiert und mehrere Bundles zu einem Bundle zusammengeführt werden. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Flusssteuerung in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erweitern des Szenarios mit erweiterten Tools</td> 
      <td>Klicken Sie auf das Symbol "[!DNL Tools]". <img src="assets/tools-icon.gif"> Sie können Trigger, Aktionen, Aggregatoren und Transformatoren erstellen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Tools</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Analyse von Benutzertext</td> 
      <td>Klicken Sie auf das Symbol [!DNL Text parser] <img src="assets/text-parser-icon.gif">. Sie können Elemente aus dem HTML-Code abrufen, Zeichenfolgen-Elemente suchen und extrahieren, die einem Suchmuster entsprechen,-Text suchen und ersetzen und Daten von einer Website "auseinanderziehen". Weitere Informationen finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Tools</a>.</td> 
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
      <td> <p>Klicken Sie im Szenario-Editor auf den Pfeil "[!UICONTROL Bearbeitung beenden]"<img src="assets/exit-editing-arrow.png"> , um die Detailseite des Szenarios anzuzeigen. Das Protokoll wird unten im Fenster oder in der rechten unteren Ecke angezeigt. Er enthält Informationen zu jeder Phase sowie zu Fehlern, die während der Ausführung des Szenarios aufgetreten sind.</p> <p>Um mit Ihrem Szenario in [!DNL scenario editor] wieder zu arbeiten, klicken Sie auf eine beliebige Stelle auf der Detailseite "Szenario".</p> <p>Weitere Informationen zur Detailseite "Szenario"finden Sie unter <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Details zum Szenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zugriff auf die am häufigsten verwendeten Apps und Dienste</td> 
      <td> Klicken Sie unten auf dem Bildschirm auf ein Symbol im Abschnitt <strong>[!UICONTROL Favoriten]</strong> . In diesem Abschnitt werden automatisch Symbole angezeigt, wenn Sie Ihrem Szenario Apps und Dienste hinzufügen. Sie können auch auf das Symbol [!UICONTROL Hinzufügen] <img src="assets/add-icon.gif"> klicken, um diesem Bereich manuell Apps und Dienste hinzuzufügen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Eine Animation anzeigen, die zeigt, wie Daten durch das Szenario fließen</td> 
      <td>Klicken Sie auf das Symbol [!UICONTROL Fluss erläutern] <img src="assets/explain-flow-airplane-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Layout der Module automatisch ausrichten </td> 
      <td>Klicken Sie auf das Symbol [!UICONTROL Automatische Ausrichtung] <img src="assets/auto-align-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Typ- oder Ansichtsnotizen zum Szenario</td> 
      <td>Klicken Sie auf das Symbol [!UICONTROL Notizen] <img src="assets/notes-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Entfernen von Modulen</td> 
      <td>Klicken Sie mit der rechten Maustaste auf das Modul und klicken Sie dann auf <strong>[!UICONTROL Modul löschen]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Um das Szenario zu testen, klicken Sie auf **[!UICONTROL Einmal ausführen]**.

   Es ist wichtig zu überprüfen, ob das Szenario erwartungsgemäß ausgeführt wird, bevor Sie es aktivieren. Nach der Aktivierung wird das Szenario gemäß seinem Zeitplan ausgeführt. Wenn nicht alles wie erwartet ausgeführt wird, lesen Sie den Abschnitt [Umgang mit Fehlern in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).

1. Wenn Sie die Bearbeitung des Szenarios (oder zu einem beliebigen Zeitpunkt während der Bearbeitung) abgeschlossen haben, klicken Sie auf das Symbol [!UICONTROL Speichern] unten im Fenster ![](assets/save-icon.gif).

Informationen zum Aktivieren eines Szenarios finden Sie unter [Aktivieren oder Deaktivieren eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

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
   <td>Strg+Umschalt+Enter</td> 
   <td><span style="font-weight: normal;">Befehl+Umschalt+Eingabetaste</span> </td> 
  </tr> 
 </tbody> 
</table>
