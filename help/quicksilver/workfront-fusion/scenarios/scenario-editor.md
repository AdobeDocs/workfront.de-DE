---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Der Szenario-Editor in  [!DNL Adobe] Workfront Fusion
description: Mit dem Szenario-Editor können Sie Szenarien in einer visuellen Benutzeroberfläche erstellen und bearbeiten.
author: Becky
feature: Workfront Fusion
exl-id: 4377303d-7615-41eb-b0cc-4bf884899361
source-git-commit: 75cf9af858e90a640c45b211d36f35b684128c2f
workflow-type: tm+mt
source-wordcount: '1108'
ht-degree: 0%

---

# Der Szenario-Editor in [!DNL Adobe Workfront Fusion]

Mit dem Szenario-Editor können Sie Szenarien in einer visuellen Benutzeroberfläche erstellen und bearbeiten.

![](assets/scenario-editor-350x228.jpg)

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz*</td> 
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

## Öffnen Sie den Szenario-Editor:

1. Klicken Sie im linken Bereich auf **[!UICONTROL Szenarios]** ![](assets/scenarios-icon.png) .

1. Wenn Sie ein Szenario erstellen möchten, klicken Sie oben rechts auf der Seite auf **[!UICONTROL Neues Szenario erstellen]** .

   Oder

   Wenn Sie ein vorhandenes Szenario bearbeiten möchten, klicken Sie auf das Szenario.

   Im angezeigten Szenario-Editor können Sie alles tun, was in der unten stehenden Tabelle aufgeführt ist. Weitere Informationen finden Sie unter [Erstellen eines Szenarios in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Wenn Sie die Bearbeitung eines Szenarios abgeschlossen haben (oder zu einem beliebigen Zeitpunkt während der Bearbeitung), klicken Sie auf das Symbol [!UICONTROL Speichern] . ![](assets/save-icon.gif)

   >[!NOTE]
   >
   >Nach dem Speichern des Szenarios wird eine neue Version unter dem Menü mit drei Punkten verfügbar sein, falls Sie in Zukunft darauf zugreifen müssen. Zuvor gespeicherte Szenario-Versionen sind nur für 60 Tage verfügbar.

## Verfügbare Szenario-Editor-Aktionen

Die folgenden Aktionen sind im Szenario-Editor verfügbar:

<table style="table-layout:auto"> 
<tbody>
  <tr>
     <td role="rowheader">Das erste Modul hinzufügen</td>
     <td> <p>Klicken Sie auf das Fragezeichen-Symbol. <img src="assets/question-mark-full-size.png"></p> <p> Klicken Sie dann auf die App oder den Dienst, mit der/dem Sie beginnen möchten. Wenn Sie in Schritt 2 Apps ausgewählt haben, werden diese hier für einfachen Zugriff angezeigt (und im Abschnitt <strong>[!UICONTROL Favoriten]</strong> unten auf dem Bildschirm).</p> </td>
  </tr>
  <tr>
     <td role="rowheader">Modul hinzufügen</td>
     <td>Bewegen Sie den Mauszeiger über ein Modul, klicken Sie auf das Pluszeichen rechts und klicken Sie dann auf das gewünschte Modul im angezeigten Menü.</td>
  </tr>  
  <tr>   
     <td role="rowheader">Geben Sie an, wann und wie oft das Szenario ausgeführt wird</td>  
      <td> <p>Klicken Sie auf das Uhrensymbol. </p> <p> <img src="assets/clock-icon.gif"> </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md" class="MCXref xref">Planen eines Szenarios in [!DNL Adobe Workfront Fusion]</a>.</p> </td>
  </tr>  
  <tr>
     <td role="rowheader">Einrichten einer Route</td>   
     <td> <p>Klicken Sie zwischen den beiden Modulen auf das [!UICONTROL Schraubenschlüsselsymbol] <img src="assets/wrench-icon.gif"> und verwenden Sie eine der folgenden Optionen:</p>    
       <ul>
         <li><strong>[!UICONTROL Filter einrichten]</strong>: Steuert, welche Bundles an bestimmten Punkten im Szenario verwendet werden. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Hinzufügen eines Filters zu einem Szenario in [!DNL Adobe Workfront Fusion]</a>.</li>     
         <li><strong>[!UICONTROL Unlink]</strong>: Entfernt eine Route.</li>     
         <li><strong>[!UICONTROL Router hinzufügen]</strong>: Fügt einen Router zwischen Modulen hinzu. </li>     
         <li><strong>[!UICONTROL Modul hinzufügen]</strong>: Fügt ein neues Modul zwischen Modulen hinzu.</li>     
         <li><strong>[!UICONTROL Notiz hinzufügen]</strong>: Fügt der Route einen Hinweis hinzu.</li>   
       </ul> 
     </td>  
  </tr>  
  <tr>  
     <td role="rowheader">Entfernen von Modulen</td>   
     <td>Klicken Sie mit der rechten Maustaste auf das Modul und klicken Sie dann auf <strong>[!UICONTROL Modul löschen]</strong>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Anzeigen eines Protokolls von Ereignissen, die in einem Szenario auftreten</td>     
     <td> 
       <p>Führen Sie ein Szenario aus. Wenn das Szenario abgeschlossen ist, wird das Protokoll in der rechten unteren Ecke des [!UICONTROL Szenario-Editors] angezeigt. </p> <p> <img src="assets/log-350x189.png" style="width: 350;height: 189;"> </p> <p>Je nach Szenario kann das Protokoll Informationen über die Schwierigkeit jeder Phase und etwaige Fehler enthalten, die bei der Ausführung des Szenarios aufgetreten sind.</p> 
     </td>  
   </tr>  
   <tr>   
     <td role="rowheader">Konfigurieren der Szenario-Einstellungen</td>   
     <td>Klicken Sie auf das Symbol [!UICONTROL Szenario-Einstellungen]. <img src="assets/gear-icon-settings.png"> Diese Einstellungen sind hauptsächlich für fortgeschrittene Benutzer gedacht.</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Typ- oder Ansichtsnotizen zum Szenario</td>   
     <td>Klicken Sie auf das Symbol [!UICONTROL Notizen]. <img src="assets/notes-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Layout der Module automatisch ausrichten </td>   
     <td>Klicken Sie auf das Symbol [!UICONTROL Automatische Ausrichtung] . <img src="assets/auto-align-icon.gif"></td>  </tr>  <tr>   <td role="rowheader">Eine Animation anzeigen, die zeigt, wie Daten durch das Szenario fließen</td>   <td>Klicken Sie auf das Symbol [!UICONTROL Fluss erläutern]. <img src="assets/explain-flow-airplane-icon.gif"></td>  
   </tr>  
   <tr> 
     <td role="rowheader">Exportieren Sie das Szenario als Blueprint auf Ihren Computer</td>   
     <td>Klicken Sie auf das [!UICONTROL Mehr] Menü <img src="assets/more-icon.png"> und dann auf [!UICONTROL Export Blueprint].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Importieren eines Szenario-Blueprints von Ihrem Computer</td>   
     <td>Klicken Sie auf das [!UICONTROL Mehr] Menü <img src="assets/more-icon.png"> und dann auf [!UICONTROL Import Blueprint].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Wiederherstellen einer früheren Version des Szenarios</td>   
     <td>Weitere Informationen finden Sie im Artikel <a href="../../workfront-fusion/scenarios/restore-a-scenario-version.md" class="MCXref xref">Wiederherstellen einer Szenario-Version in [!DNL Adobe Workfront Fusion]</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Einstellungen der [!UICONTROL Flusssteuerung konfigurieren]</td>   
     <td> <p>Klicken Sie auf das Symbol [!UICONTROL Flusssteuerung] . <img src="assets/flow-control-icon.gif"> Sie können eine Aufgabe so einrichten, dass eine bestimmte Anzahl von Malen wiederholt, ein Array in eine Reihe von Bundles konvertiert und mehrere Bundles zu einem Bundle zusammengeführt werden. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Flusssteuerung in [!DNL Adobe Workfront Fusion]</a>.</p> </td>  
   </tr>  
   <tr> 
     <td role="rowheader">Erweitern des Szenarios mit erweiterten Tools</td>   
     <td>Klicken Sie auf das Symbol [!UICONTROL Tools] . <img src="assets/tools-icon.gif"> Sie können Trigger, Aktionen, Aggregatoren und Transformatoren erstellen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Tools</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Verwenden von Textanalysewerkzeugen</td>   
     <td>Klicken Sie auf das Symbol [!UICONTROL Text-Parser] . <img src="assets/text-parser-icon.gif"> Sie können Elemente aus dem HTML-Code abrufen, Zeichenfolgenelemente suchen und extrahieren, die einem Suchmuster entsprechen, suchen und ersetzen und Daten von einer Website "abreißen". Weitere Informationen finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Tools</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Zugriff auf die am häufigsten verwendeten Apps und Dienste</td>   
     <td> Klicken Sie unten auf dem Bildschirm auf ein Symbol im Abschnitt <strong>[!UICONTROL Favoriten]</strong> . In diesem Abschnitt werden automatisch Symbole angezeigt, wenn Sie Ihrem Szenario Apps und Dienste hinzufügen. Sie können auch auf das Symbol "Hinzufügen"<img src="assets/add-icon.gif"> klicken, um diesem Bereich manuell Apps und Dienste hinzuzufügen.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Testen des Szenarios</td>   
     <td>Klicken Sie auf <strong>[!UICONTROL Einmal ausführen]</strong> , um zu überprüfen, ob das Szenario wie erwartet ausgeführt wird, bevor Sie es aktivieren. Nach der Aktivierung wird das Szenario gemäß seinem Zeitplan ausgeführt. Wenn nicht alles wie erwartet ausgeführt wird, erfahren Sie in unserem Abschnitt zur Fehlerbehebung , wie Fehler zu handhaben sind.</td> 
   </tr> 
   <tr> 
     <td role="rowheader">Debugging des Szenarios mit dem Entwickler-Tool</td>   
     <td>Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/debug-scenarios-with-dev-tool.md" class="MCXref xref">Debugszenarien mit dem [!DNL Adobe Workfront Fusion] Entwickler-Tool</a> .
</td> 
   </tr> 
<tr>
<td>Status des Szenarios überprüfen</td>
<td>Szenarien können aktiv oder inaktiv sein. Sie können den Status des Szenarios ändern, indem Sie in den Details des Szenarios auf die Schaltfläche Ein/Aus klicken.

Weitere Informationen finden Sie in den folgenden Artikeln:
<ul>
<li><a href="../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md">Aktivieren oder Deaktivieren eines Szenarios in Adobe Workfront Fusion</a></li>
<li><a href="../../workfront-fusion/scenarios/scenario-detail.md">Szenariodetails in Adobe Workfront Fusion</a></li>
</ul>
</td>
</tr>
<tr>
<td>Ändern Sie den Zeitplan des Szenarios</td>
<td>Aktive Szenarien werden nach einem Zeitplan ausgeführt. Standardmäßig wird ein Szenario alle 15 Minuten ausgeführt. Sie können dies ändern, indem Sie festlegen, wann und wie oft ein aktiviertes Szenario ausgeführt wird. Fusionsszenarien können so oft wie alle 5 Minuten ausgeführt werden.

Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/schedule-a-scenario.md">Planen eines Szenarios in Adobe Workfront Fusion</a>.
</td>
</tr>
<tr>
<td>Umbenennen des Szenarios</td>
<td>Um ein Szenario umzubenennen, öffnen Sie das Szenario, klicken Sie auf den Namen des Szenarios in der oberen linken Ecke und bearbeiten Sie es. Drücken Sie die Eingabetaste oder klicken Sie außerhalb des bearbeiteten Felds, um den Namen des Szenarios zu speichern.</td>
</tr>
<tr>
<td>Auswählen des ersten Bundles</td>
<td>Einige Trigger-Module ermöglichen es Ihnen, das erste Bundle auszuwählen, aus dem das Abrufen von Bundles beginnen soll.

Weitere Informationen finden Sie unter <a href="../../workfront-fusion/modules/choose-where-trigger-module-starts.md">Auswählen, wo ein Trigger-Modul in Adobe Workfront Fusion gestartet wird</a>.</td>
</tr>
<tr>
<td>Anzahl der zurückgegebenen Bundles festlegen</td>
<td>Module geben standardmäßig immer nur zwei Bundles zurück. Dies kann in den Moduleinstellungen im Feld [!UICONTROL Maximale Anzahl der zurückgegebenen Bundles] geändert werden.</td>
</tr>
<tr>
<td>Erweiterte Szenario-Einstellungen konfigurieren</td>
<td>[!DNL Adobe Workfront Fusion] bietet Ihnen die Möglichkeit, eine Reihe weiterer erweiterter Einstellungen zu konfigurieren.

Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md">Das Bedienfeld mit den Szenario-Einstellungen in Adobe Workfront Fusion</a>.</td>
</tr>
</tbody>
</table>
