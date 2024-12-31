---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Erstellen eines Szenarios in Adobe Workfront Fusion
description: In den folgenden Aufgaben wird beschrieben, wie Sie ein Szenario  [!DNL Adobe Workfront Fusion] .
author: Becky
feature: Workfront Fusion
exl-id: adf66cfc-ccaf-4b29-9199-c13260695569
source-git-commit: ee2283ac159ca26ca473cac28ec4bed85d1dea04
workflow-type: tm+mt
source-wordcount: '1406'
ht-degree: 0%

---

# Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]

In den folgenden Aufgaben wird beschrieben, wie Sie ein [!DNL Adobe Workfront Fusion] erstellen.

Eine praktische Übung, die Sie durch das Erstellen eines Automatisierungsszenarios führt, finden Sie unter [Erstellen eines Automatisierungsszenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md).

Eine Übungsübung, die Sie durch die Erstellung eines Integrationsszenarios mit den von uns bereitgestellten Daten führt, finden [ unter „Erstellen eines Übungsintegrationsszenarios in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

>[!NOTE]
>
>Informationen zum Erstellen eines Szenarios aus einer Vorlage finden Sie unter [Erstellen von Szenarios mit  [!DNL Adobe Workfront Fusion]  Vorlagen](../../workfront-fusion/scenarios/templates/create-scenarios-with-fusion-templates.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Adobe Workfront-Plan</td>  
      <td>Beliebig</td>  
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
        Aktuell: Keine Workfront Fusion-Lizenzanforderung.<br>
        Oder<br>
        Legacy: Beliebig
      </td>  
    </tr>  
    <tr>  
      <td>Produkt</td>  
      <td> 
        Neu: Wählen Sie oder Prime Workfront Plan: Ihr Unternehmen muss Adobe Workfront Fusion erwerben.<br>
        Ultimate Workfront Plan: Workfront Fusion ist enthalten.<br>
        Oder<br>
        Aktuell: Ihr Unternehmen muss Adobe Workfront Fusion erwerben.
      </td>  
    </tr> 
  </tbody>  
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Erstellen eines Szenarios

1. Klicken Sie **[!UICONTROL linken Bedienfeld]** Szenarios![](assets/scenarios-icon.png).

1. Klicken **[!UICONTROL oben rechts auf]** Seite auf „Neues Szenario erstellen“.
1. Wenn Sie im angezeigten Bildschirm (dem Szenario-Editor) ein neues Szenario erstellen, klicken Sie auf **[!UICONTROL Neues Szenario]** in der oberen linken Ecke und geben Sie einen Namen für das Szenario ein.
1. Fahren Sie fort mit [Modul in einem Szenario hinzufügen](#add-a-module-in-a-scenario).

## Hinzufügen eines Moduls in einem Szenario

1. Um das erste Modul zum Szenario hinzuzufügen, klicken Sie auf das Fragezeichen-Symbol. ![](assets/question-mark-icon.gif)

   Oder

   Um dem Szenario zusätzliche Module hinzuzufügen, klicken Sie auf den Ziehgriff auf der rechten Seite des Moduls, dem das Szenario folgen soll.

1. Suchen Sie in dem angezeigten Feld nach der App oder dem Service, mit der bzw. dem Sie beginnen möchten, und klicken Sie darauf.

   Alle zuvor ausgewählten Apps werden in dem Feld für einfachen Zugriff und im Abschnitt **[!UICONTROL Favoriten]** unten auf dem Bildschirm angezeigt.

   Wenn Sie auf **[!UICONTROL Weiteres Modul hinzufügen]** klicken, hängen die angezeigten Module davon ab, wo im Szenario Sie das Modul hinzufügen. Einige Module können nur zwischen anderen Modulen platziert werden, andere nur am Anfang des Szenarios.

   >[!TIP]
   >
   >Die beiden häufigsten Modultypen sind Aktionen und Trigger. Weitere Informationen finden Sie unter [Modultypen](../../workfront-fusion/modules/module-types.md).

1. Klicken Sie in der angezeigten Modulliste auf das erste Modul, das Sie dem Szenario hinzufügen möchten.

   Welche Module angezeigt werden, hängt davon ab, wo Sie ein Modul in Ihrem Szenario hinzufügen möchten. Einige Module können nur zwischen anderen Modulen platziert werden, andere nur am Anfang des Szenarios.

   Die beiden häufigsten Modultypen sind Aktionen und Trigger. Weitere Informationen finden Sie unter [Modultypen](../../workfront-fusion/modules/module-types.md).

1. Fahren Sie fort mit [Verbinden der App oder des Webservices des Moduls mit [!DNL Workfront Fusion]](#connect-the-modules-app-or-web-service-to-workfront-fusion).

## Verbinden der App oder des Webservices des Moduls mit [!DNL Workfront Fusion] {#connect-the-modules-app-or-web-service-to-workfront-fusion}

Workfront Fusion-Module, die eine Verbindung zu einer App herstellen (z. B. [!DNL Workfront], [!DNL Salesforce] oder [!DNL Jira)]), verfügen über das Feld [!UICONTROL Verbindung] . Hier können Sie die Verbindung angeben, die dieses Modul für die Verbindung mit der App verwenden soll. Sie können eine vorhandene Verbindung aus dem Dropdown-Menü auswählen oder eine neue Verbindung erstellen.

Wenn Sie in einem Szenario eine Verbindung für eine App auswählen oder erstellen, verwenden andere Module für diese App automatisch dieselbe Verbindung, es sei denn, Sie wählen beim Einrichten der späteren Module eine andere Verbindung aus.

Weitere Informationen finden Sie unter [Verbindungen - Übersicht](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

![](assets/connection-field-350x169.png)

So erstellen Sie eine Verbindung innerhalb eines [!DNL Workfront Fusion]:

1. Klicken Sie **[!UICONTROL Hinzufügen]**, um das Feld **[!UICONTROL Verbindung erstellen]** zu öffnen.
1. (Optional) Ändern Sie den Standard **[!UICONTROL Verbindungsnamen]**.
1. (Bedingt) Wenn für die App erweiterte Verbindungseinstellungen wie eine ID, ein Schlüssel oder ein [!UICONTROL Geheimnis] erforderlich sind, geben Sie diese Informationen ein.

   Möglicherweise müssen Sie auf **[!UICONTROL Erweiterte Einstellungen anzeigen]** klicken, um die Felder anzuzeigen, in die Sie diese Art von Informationen eingeben können.

1. Klicken Sie **[!UICONTROL Weiter]**.
1. Geben Sie im angezeigten Anmeldefenster Ihre Anmeldedaten ein, um sich bei der App anzumelden, falls Sie dies noch nicht getan haben.
1. (Bedingt) Wenn eine Schaltfläche **[!UICONTROL Zulassen]** angezeigt wird, überprüfen Sie die Aktionen, die der Connector ausführen kann, und klicken Sie dann auf die Schaltfläche, um die App mit [!DNL Workfront Fusion] zu verbinden.
1. Fahren Sie fort mit [Konfigurieren des Moduls](#configure-the-module).


## Konfigurieren des Moduls

1. Konfigurieren Sie in den Feldern unter dem Feld Verbindung die Einstellungen für das Modul und klicken Sie dann auf **[!UICONTROL OK]**.

   ![](assets/conf-settigs-mod-350x547.png)

   Diese Einstellungen sind für jedes Modul unterschiedlich. Ein fett gedruckter Titel zeigt eine erforderliche Einstellung an.

   >[!TIP]
   >
   >Während Sie an Ihrem Szenario arbeiten, können Sie auf das Modul klicken, um dieses Feld mit den Einstellungen jederzeit anzuzeigen.
   >
   >
   >Wenn ein Modul einen schwarzen Kreis aufweist, ist die Konfiguration der Einstellungen noch nicht abgeschlossen. Klicken Sie auf das Modul, um es zu öffnen und mit der Konfiguration fortzufahren.
   >
   >
   >![](assets/black-error-circle-on-module.png)

1. Wenn Sie das erste Modul in Ihrem Szenario hinzufügen, wählen Sie eine Option aus, um anzugeben, wo das Szenario bei jeder Ausführung starten soll.

   ![](assets/choose-where-start-350x194.png)

1. Wiederholen Sie die Schritte in den Abschnitten [Hinzufügen eines Moduls in einem Szenario](#add-a-module-in-a-scenario) und [Konfigurieren des Moduls](#configure-the-module), um dem Szenario weitere Module hinzuzufügen.

1. (Optional) Kopieren Sie ein Modul oder eine Gruppe von Modulen und fügen Sie es ein.

   Weitere Informationen finden Sie unter [Module oder Szenarien in Adobe Workfront Fusion kopieren](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md).

1. Fahren Sie mit [Konfigurieren und Arbeiten mit Ihrem Szenario“ ](#configure-and-work-with-your-scenario).

## Konfigurieren und Verwenden Ihres Szenarios

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
        <li><strong>[!UICONTROL Filter einrichten]</strong>: Legt fest, welche Bundles zu bestimmten Zeitpunkten im Szenario verwendet werden.</li> 
        <li><strong>[!UICONTROL unlink]</strong>: Entfernt eine Route.</li> 
        <li><strong>[!UICONTROL Router hinzufügen]</strong>: Fügt einen Router zwischen den Modulen hinzu. </li> 
        <li><strong>[!UICONTROL Modul hinzufügen]</strong>: Fügt ein neues Modul zwischen den Modulen hinzu.</li> 
        <li><strong>[!UICONTROL Anmerkung hinzufügen]</strong>: Fügt der Route eine Anmerkung hinzu.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Konfigurieren der Szenario-Einstellungen</td> 
      <td>Klicken Sie auf das Symbol [!UICONTROL Szenario-Einstellungen]. <img src="assets/gear-icon-settings.png"> Diese Einstellungen richten sich in erster Linie an fortgeschrittene Benutzer. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Das Bedienfeld „Szenario-Einstellungen“ in [!DNL Adobe Workfront Fusion]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Konfigurieren der Einstellungen für die Flusssteuerung</td> 
      <td> <p>Klicken Sie auf das Symbol [!UICONTROL Flow Control]. <img src="assets/flow-control-icon.gif"> Sie können eine Aufgabe so einrichten, dass sie eine bestimmte Anzahl von Malen wiederholt, ein Array in eine Reihe von Bundles konvertiert und mehrere Bundles in einem Bundle zusammenführt. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Flusskontrolle in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Verbessern des Szenarios mit erweiterten Tools</td> 
      <td>Klicken Sie auf das Symbol [!DNL Tools] . <img src="assets/tools-icon.gif"> Sie können Trigger, Aktionen, Aggregatoren und Transformatoren erstellen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Tools</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tools zum Parsen von Benutzertexten</td> 
      <td>Klicken Sie auf das [!DNL Text parser]-Symbol <img src="assets/text-parser-icon.gif">. Sie können Elemente aus HTML-Code abrufen, Zeichenfolgenelemente, die einem Suchmuster entsprechen, suchen und ersetzen und Daten von einer Website abkratzen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Tools</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Führen Sie einen der folgenden Schritte aus, um mit Ihrem Szenario zu arbeiten:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Protokoll der Ereignisse anzeigen, die bei Ausführung des Szenarios auftreten</td> 
      <td> <p>Klicken Sie auf den Pfeil [!UICONTROL Bearbeiten beenden] <img src="assets/exit-editing-arrow.png"> im Szenario-Editor, um die Seite mit den Szenario-Details anzuzeigen. Das Protokoll wird unten im Fenster oder in der unteren rechten Ecke angezeigt. Er enthält Informationen zu den einzelnen Phasen und allen Fehlern, die bei der Ausführung des Szenarios aufgetreten sind.</p> <p>Um mit Ihrem Szenario in der [!DNL scenario editor] wieder zu arbeiten, klicken Sie auf eine beliebige Stelle auf der Seite mit den Szenario-Details.</p> <p>Weitere Informationen zur Seite mit den Szenario-Details finden Sie unter <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Szenario-Details in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Zugreifen auf Ihre am häufigsten verwendeten Apps und Services</td> 
      <td> Klicken Sie auf ein Symbol im Abschnitt <strong>[!UICONTROL Favorites]</strong> unten auf dem Bildschirm. Symbole werden in diesem Abschnitt automatisch angezeigt, wenn Sie Ihrem Szenario Apps und Services hinzufügen. Sie können auch auf das Symbol [!UICONTROL Hinzufügen] <img src="assets/add-icon.gif"> klicken, um diesem Bereich manuell Apps und Services hinzuzufügen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Animation anzeigen, die den Datenfluss durch das Szenario zeigt</td> 
      <td>Klicken Sie auf das Symbol [!UICONTROL Fluss erläutern] <img src="assets/explain-flow-airplane-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatische Ausrichtung des Layouts der Module </td> 
      <td>Klicken Sie auf das Symbol [!UICONTROL Auto-align] <img src="assets/auto-align-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Geben Sie Notizen zum Szenario ein oder zeigen Sie sie an</td> 
      <td>Klicken Sie auf das Symbol [!UICONTROL Notes] <img src="assets/notes-icon.gif">.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Modul entfernen</td> 
      <td>Klicken Sie mit der rechten Maustaste auf das Modul und dann auf <strong>[!UICONTROL Delete module]</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Um das Szenario erneut auszuführen, klicken Sie auf &quot;**[!UICONTROL ausführen]**.

   Bevor Sie das Szenario aktivieren, müssen Sie sicherstellen, dass es erwartungsgemäß ausgeführt wird. Nach der Aktivierung wird das Szenario gemäß seinem Zeitplan ausgeführt. Wenn nicht alles erwartungsgemäß ausgeführt wird, finden Sie weitere Informationen unter [Fehlerbehandlung in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).

1. Wenn Sie die Bearbeitung des Szenarios abgeschlossen haben (oder zu einem beliebigen Zeitpunkt während der Bearbeitung), klicken Sie auf [!UICONTROL Speichern]-Symbol am unteren Rand des ![](assets/save-icon.gif).

Informationen zum Aktivieren eines Szenarios finden Sie unter [Aktivieren oder Deaktivieren eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

## Tastaturbefehle für das Workfront Fusion-Szenario

Beim Erstellen oder Bearbeiten eines Szenarios können die folgenden Tastaturbefehle verwendet werden:

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
   <td role="rowheader">[!UICONTROL Speichern] </td> 
   <td>Strg+Umschalt+S</td> 
   <td><span style="font-weight: normal;">Befehl+Umschalt+S</span> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Einmal ausführen]</td> 
   <td>Strg+Umschalt+Eingabe</td> 
   <td><span style="font-weight: normal;">Befehl+Umschalt+Eingabe</span> </td> 
  </tr> 
 </tbody> 
</table>
