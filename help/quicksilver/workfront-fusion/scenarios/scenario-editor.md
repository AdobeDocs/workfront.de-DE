---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Der Szenario-Editor in  [!DNL Adobe] Workfront Fusion
description: Mit dem Szenario-Editor können Sie Szenarien in einer visuellen Benutzeroberfläche erstellen und bearbeiten.
author: Becky
feature: Workfront Fusion
exl-id: 4377303d-7615-41eb-b0cc-4bf884899361
source-git-commit: cb4edb02aad8a0738ea80f058fcc2bc016832ce1
workflow-type: tm+mt
source-wordcount: '1108'
ht-degree: 0%

---

# Der Szenario-Editor in [!DNL Adobe Workfront Fusion]

Mit dem Szenario-Editor können Sie Szenarien in einer visuellen Benutzeroberfläche erstellen und bearbeiten.

![](assets/scenario-editor.jpg)

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] Lizenz**</td> 
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

## Öffnen Sie den Szenario-Editor:

1. Klicken Sie **[!UICONTROL linken Bedienfeld]** Szenarios![](assets/scenarios-icon.png).

1. Wenn Sie ein Szenario erstellen möchten, klicken **[!UICONTROL oben rechts]** der Seite auf „Neues Szenario erstellen“.

   Oder

   Wenn Sie ein vorhandenes Szenario bearbeiten möchten, klicken Sie auf das Szenario.

   Im angezeigten Szenario-Editor können Sie alle in der folgenden Tabelle aufgeführten Vorgänge ausführen. Weitere Informationen finden Sie unter [Erstellen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Wenn Sie die Bearbeitung eines Szenarios abgeschlossen haben (oder zu einem beliebigen Zeitpunkt während der Bearbeitung), klicken Sie auf das Symbol [!UICONTROL Speichern]. ![](assets/save-icon.gif)

   >[!NOTE]
   >
   >Nach dem Speichern Ihres Szenarios wird eine neue Version unter dem Dreipunkt-Menü verfügbar sein, falls Sie in Zukunft darauf zugreifen müssen. Zuvor gespeicherte Szenario-Versionen sind nur für 60 Tage verfügbar.

## Verfügbare Szenario-Editor-Aktionen

Die folgenden Aktionen sind im Szenario-Editor verfügbar:

<table style="table-layout:auto"> 
<tbody>
  <tr>
     <td role="rowheader">Erstes Modul hinzufügen</td>
     <td> <p>Klicken Sie auf das Fragezeichen-Symbol. <img src="assets/question-mark-full-size.png"></p> <p> Suchen Sie dann die App oder den Service, mit der bzw. dem Sie beginnen möchten, und klicken Sie darauf. Wenn Sie in Schritt 2 Apps ausgewählt haben, werden diese hier angezeigt, um einen einfachen Zugriff zu ermöglichen (und im Abschnitt <strong>[!UICONTROL Favoriten]</strong> am unteren Bildschirmrand).</p> </td>
  </tr>
  <tr>
     <td role="rowheader">Modul hinzufügen</td>
     <td>Bewegen Sie den Mauszeiger über ein Modul, klicken Sie auf das Pluszeichen auf der rechten Seite und klicken Sie dann im angezeigten Menü auf das gewünschte Modul.</td>
  </tr>  
  <tr>   
     <td role="rowheader">Geben Sie an, wann und wie oft das Szenario ausgeführt wird</td>  
      <td> <p>Klicken Sie auf das Uhrensymbol. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Planen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td>
  </tr>  
  <tr>
     <td role="rowheader">Einrichten einer Route</td>   
     <td> <p>Klicken Sie auf das Symbol [!UICONTROL Wrench] <img src="assets/wrench-icon.gif"> zwischen den beiden Modulen und verwenden Sie eine der folgenden Optionen:</p>    
       <ul>
         <li><strong>[!UICONTROL Filter einrichten]</strong>: Legt fest, welche Bundles zu bestimmten Zeitpunkten im Szenario verwendet werden. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Hinzufügen eines Filters zu einem Szenario in [!DNL Adobe Workfront Fusion]</a>.</li>     
         <li><strong>[!UICONTROL unlink]</strong>: Entfernt eine Route.</li>     
         <li><strong>[!UICONTROL Router hinzufügen]</strong>: Fügt einen Router zwischen den Modulen hinzu. </li>     
         <li><strong>[!UICONTROL Modul hinzufügen]</strong>: Fügt ein neues Modul zwischen den Modulen hinzu.</li>     
         <li><strong>[!UICONTROL Anmerkung hinzufügen]</strong>: Fügt der Route eine Anmerkung hinzu.</li>   
       </ul> 
     </td>  
  </tr>  
  <tr>  
     <td role="rowheader">Modul entfernen</td>   
     <td>Klicken Sie mit der rechten Maustaste auf das Modul und dann auf <strong>[!UICONTROL Delete module]</strong>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Anzeigen eines Ereignisprotokolls als Szenario</td>     
     <td> 
       <p>Führen Sie ein Szenario aus. Wenn das Szenario abgeschlossen ist, wird das Protokoll in der rechten unteren Ecke des [!UICONTROL Szenario-Editors] angezeigt. </p> <p> <img src="assets/log-350x189.png" style="width: 350;height: 189;"> </p> <p>Je nach Szenario kann das Protokoll Informationen über die Schwierigkeit jeder Phase und alle Fehler enthalten, die bei der Ausführung des Szenarios aufgetreten sind.</p> 
     </td>  
   </tr>  
   <tr>   
     <td role="rowheader">Konfigurieren der Szenario-Einstellungen</td>   
     <td>Klicken Sie auf das Symbol [!UICONTROL Szenario-Einstellungen]. <img src="assets/gear-icon-settings.png"> Diese Einstellungen richten sich in erster Linie an fortgeschrittene Benutzer.</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Geben Sie Notizen zum Szenario ein oder zeigen Sie sie an</td>   
     <td>Klicken Sie auf das Symbol [!UICONTROL Notes]. <img src="assets/notes-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Automatische Ausrichtung des Layouts der Module </td>   
     <td>Klicken Sie auf das Symbol [!UICONTROL Auto-align]. <img src="assets/auto-align-icon.gif"></td>  </tr>  <tr>   <td role="rowheader">Animation anzeigen, die den Datenfluss durch das Szenario zeigt</td>   <td>Klicken Sie auf das Symbol [!UICONTROL Fluss erläutern]. <img src="assets/explain-flow-airplane-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Szenario als Blueprint auf den Computer exportieren</td>   
     <td>Klicken Sie auf die <img src="assets/more-icon.png"> [!UICONTROL Mehr] und dann auf [!UICONTROL Blueprint exportieren].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Szenario-Blueprint von Ihrem Computer importieren</td>   
     <td>Klicken Sie auf die <img src="assets/more-icon.png"> [!UICONTROL Mehr] und dann auf [!UICONTROL Blueprint importieren].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Wiederherstellen einer früheren Version des Szenarios</td>   
     <td>Siehe den Artikel <a href="../../workfront-fusion/scenarios/restore-a-scenario-version.md" class="MCXref xref">Wiederherstellen einer Szenario-Version in [!DNL Adobe Workfront Fusion]</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Konfigurieren der Einstellungen für [!UICONTROL Flow Control]</td>   
     <td> <p>Klicken Sie auf das Symbol [!UICONTROL Flow Control]. <img src="assets/flow-control-icon.gif"> Sie können eine Aufgabe so einrichten, dass sie eine bestimmte Anzahl von Malen wiederholt, ein Array in eine Reihe von Bundles konvertiert und mehrere Bundles in einem Bundle zusammenführt. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Flusskontrolle in [!DNL Adobe Workfront Fusion]</a>.</p> </td>  
   </tr>  
   <tr> 
     <td role="rowheader">Verbessern des Szenarios mit erweiterten Tools</td>   
     <td>Klicken Sie auf das Symbol [!UICONTROL Tools]. <img src="assets/tools-icon.gif"> Sie können Trigger, Aktionen, Aggregatoren und Transformatoren erstellen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Tools</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Textanalysetools verwenden</td>   
     <td>Klicken Sie auf das Symbol [!UICONTROL Text Parser]. <img src="assets/text-parser-icon.gif"> Sie können Elemente aus HTML-Code abrufen, Zeichenfolgenelemente, die einem Suchmuster entsprechen, suchen und ersetzen und Daten von einer Website abkratzen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Tools</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Zugreifen auf Ihre am häufigsten verwendeten Apps und Services</td>   
     <td> Klicken Sie auf ein Symbol im Abschnitt <strong>[!UICONTROL Favorites]</strong> unten auf dem Bildschirm. Symbole werden in diesem Abschnitt automatisch angezeigt, wenn Sie Ihrem Szenario Apps und Services hinzufügen. Sie können auch auf das Symbol Hinzufügen klicken, <img src="assets/add-icon.gif"> diesem Bereich manuell Programme und Services hinzuzufügen.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Testlauf des Szenarios</td>   
     <td>Klicken Sie auf <strong>[!UICONTROL Einmal ausführen]</strong>, um zu überprüfen, ob das Szenario wie erwartet ausgeführt wird, bevor Sie es aktivieren. Nach der Aktivierung wird das Szenario gemäß seinem Zeitplan ausgeführt. Wenn nicht alles wie erwartet ausgeführt wird, können Sie unseren Abschnitt zur Fehlerbehandlung aufrufen, um zu erfahren, wie Sie mit Fehlern umgehen.</td> 
   </tr> 
   <tr> 
     <td role="rowheader">Verwenden des DevTools zum Debuggen des Szenarios</td>   
     <td>Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/debug-scenarios-with-dev-tool.md" class="MCXref xref">Debugging-Szenarien mit dem [!DNL Adobe Workfront Fusion] DevTool</a>.
</td> 
   </tr> 
<tr>
<td>Überprüfen des Status des Szenarios</td>
<td>Szenarien können aktiv oder inaktiv sein. Sie können den Szenario-Status ändern, indem Sie im Szenario-Detail auf die Schaltfläche Ein/Aus klicken.

Weitere Informationen finden Sie in den folgenden Artikeln:
<ul>
<li><a href="../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md">Aktivieren oder Deaktivieren eines Szenarios in Adobe Workfront Fusion</a></li>
<li><a href="../../workfront-fusion/scenarios/scenario-detail.md">Szenariodetails in Adobe Workfront Fusion</a></li>
</ul>
</td>
</tr>
<tr>
<td>Ändern des Zeitplans des Szenarios</td>
<td>Aktive Szenarien werden nach einem Zeitplan ausgeführt. Standardmäßig wird ein Szenario alle 15 Minuten ausgeführt. Sie können dies ändern, indem Sie festlegen, wann und wie oft ein aktiviertes Szenario ausgeführt wird. Fusionsszenarien können so geplant werden, dass sie alle 5 Minuten ausgeführt werden.

Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md">Planen eines Szenarios in Adobe Workfront Fusion</a>.
</td>
</tr>
<tr>
<td>Szenario umbenennen</td>
<td>Um ein Szenario umzubenennen, öffnen Sie das Szenario, klicken Sie oben links auf den Namen des Szenarios und bearbeiten Sie es. Drücken Sie die Eingabetaste oder klicken Sie außerhalb des bearbeiteten Felds, um den Szenarionamen zu speichern.</td>
</tr>
<tr>
<td>Das erste Bundle auswählen</td>
<td>Bei einigen Trigger-Modulen können Sie das erste Bundle auswählen, von dem aus das Abrufen von Bundles beginnen soll.

Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/choose-where-trigger-module-starts.md">Auswählen, wo ein Trigger-Modul in Adobe Workfront Fusion beginnt</a>.</td>
</tr>
<tr>
<td>Anzahl der zurückgegebenen Bundles festlegen</td>
<td>-Module geben standardmäßig immer nur zwei Bundles zurück. Dies kann in den Moduleinstellungen im Feld [!UICONTROL Maximale Anzahl der zurückgegebenen Bundles] geändert werden.</td>
</tr>
<tr>
<td>Konfigurieren der erweiterten Szenarioeinstellungen</td>
<td>[!DNL Adobe Workfront Fusion] bietet Ihnen die Möglichkeit, eine Reihe anderer erweiterter Einstellungen zu konfigurieren.

Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md">Bedienfeld „Szenarioeinstellungen“ in Adobe Workfront Fusion</a>.</td>
</tr>
</tbody>
</table>
