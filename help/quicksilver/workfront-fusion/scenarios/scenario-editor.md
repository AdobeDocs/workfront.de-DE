---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Der Szenario-Editor in [!DNL Adobe] Workfront Fusion
description: Mit dem Szenario-Editor können Sie Szenarien in einer visuellen Benutzeroberfläche erstellen und bearbeiten.
author: Becky
feature: Workfront Fusion
exl-id: 4377303d-7615-41eb-b0cc-4bf884899361
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# Der Szenario-Editor in [!DNL Adobe Workfront Fusion]

Mit dem Szenario-Editor können Sie Szenarien in einer visuellen Benutzeroberfläche erstellen und bearbeiten.

![](assets/scenario-editor-350x228.jpg)

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

## Öffnen Sie den Szenario-Editor:

1. Klicken **[!UICONTROL Szenarien]** ![](assets/scenarios-icon.png) im linken Bereich.

1. Wenn Sie ein Szenario erstellen möchten, klicken Sie auf **[!UICONTROL Neues Szenario erstellen]** in der oberen rechten Ecke der Seite.

   Oder

   Wenn Sie ein vorhandenes Szenario bearbeiten möchten, klicken Sie auf das Szenario.

   Im angezeigten Szenario-Editor können Sie alles tun, was in der unten stehenden Tabelle aufgeführt ist. Weitere Informationen finden Sie unter [Erstellen Sie ein Szenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Wenn Sie die Bearbeitung eines Szenarios abgeschlossen haben (oder zu einem beliebigen Zeitpunkt während der Bearbeitung), klicken Sie auf [!UICONTROL Speichern] Symbol. ![](assets/save-icon.gif)

   >[!NOTE]
   >
   >Nach dem Speichern des Szenarios wird eine neue Version unter dem Menü mit drei Punkten verfügbar sein, falls Sie in Zukunft darauf zugreifen müssen. Zuvor gespeicherte Szenario-Versionen sind nur für 60 Tage verfügbar.

## Verfügbare Szenario-Editor-Aktionen

Die folgenden Aktionen sind im Szenario-Editor verfügbar:

<table style="table-layout:auto"> 
<tbody>
  <tr>
     <td role="rowheader">Das erste Modul hinzufügen</td>
     <td> <p>Klicken Sie auf das Fragezeichen-Symbol. <img src="assets/question-mark-full-size.png"></p> <p> Klicken Sie dann auf die App oder den Dienst, mit der/dem Sie beginnen möchten. Wenn Sie in Schritt 2 Apps ausgewählt haben, werden diese hier für einfachen Zugriff angezeigt (und im <strong>[!UICONTROL Favoriten]</strong> unten auf dem Bildschirm).</p> </td>
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
     <td> <p>Klicken Sie auf das Symbol [!UICONTROL Schraubenschlüssel] . <img src="assets/wrench-icon.gif"> zwischen den beiden Modulen stehen und eine der folgenden Optionen verwenden:</p>    
       <ul>
         <li><strong>[!UICONTROL Filter einrichten]</strong>: Legen Sie fest, welche Bundles an bestimmten Punkten im Szenario verwendet werden. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Hinzufügen eines Filters zu einem Szenario in [!DNL Adobe Workfront Fusion]</a>.</li>     
         <li><strong>[!UICONTROL Unlink]</strong>: Entfernt eine Route.</li>     
         <li><strong>[!UICONTROL Router hinzufügen]</strong>: Fügt einen Router zwischen Modulen hinzu. </li>     
         <li><strong>[!UICONTROL Modul hinzufügen]</strong>: Fügt ein neues Modul zwischen Modulen hinzu.</li>     
         <li><strong>[!UICONTROL Notiz hinzufügen]</strong>: Fügt der Route einen Hinweis hinzu.</li>   
       </ul> 
     </td>  
  </tr>  
  <tr>  
     <td role="rowheader">Entfernen von Modulen</td>   
     <td>Klicken Sie mit der rechten Maustaste auf das Modul und klicken Sie dann auf <strong>[!UICONTROL Löschmodul]</strong>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Anzeigen eines Protokolls von Ereignissen, die in einem Szenario auftreten</td>     
     <td> 
       <p>Führen Sie ein Szenario aus. Wenn das Szenario abgeschlossen ist, wird das Protokoll in der rechten unteren Ecke des [!UICONTROL Szenario-Editors] angezeigt. </p> <p> <img src="assets/log-350x189.png" style="width: 350;height: 189;"> </p> <p>Je nach Szenario kann das Protokoll Informationen über die Schwierigkeit jeder Phase und etwaige Fehler enthalten, die bei der Ausführung des Szenarios aufgetreten sind.</p> 
     </td>  
   </tr>  
   <tr>   
     <td role="rowheader">Konfigurieren der Szenario-Einstellungen</td>   
     <td>Klicken Sie auf das Symbol [!UICONTROL Szenario-Einstellungen]. <img src="assets/gear-icon-settings.png"> Diese Einstellungen richten sich in erster Linie an fortgeschrittene Benutzer.</td>  
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
     <td>Klicken Sie auf das Menü [!UICONTROL Mehr] . <img src="assets/more-icon.png">und klicken Sie dann auf [!UICONTROL Export Blueprint].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Importieren eines Szenario-Blueprints von Ihrem Computer</td>   
     <td>Klicken Sie auf das Menü [!UICONTROL Mehr] . <img src="assets/more-icon.png">und klicken Sie dann auf [!UICONTROL Blueprint importieren].</td>  
   </tr>  
   <tr>   
     <td role="rowheader">Wiederherstellen einer früheren Version des Szenarios</td>   
     <td>Siehe Artikel <a href="../../workfront-fusion/scenarios/restore-a-scenario-version.md" class="MCXref xref">Wiederherstellen einer Szenario-Version in [!DNL Adobe Workfront Fusion]</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Einstellungen der [!UICONTROL Flusssteuerung konfigurieren]</td>   
     <td> <p>Klicken Sie auf das Symbol [!UICONTROL Flusssteuerung] . <img src="assets/flow-control-icon.gif"> Sie können eine Aufgabe so einrichten, dass eine bestimmte Anzahl von Malen wiederholt, ein Array in eine Reihe von Bundles konvertiert und mehrere Bundles zu einem Bundle zusammengeführt werden. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/flow-control.md" class="MCXref xref">Flusssteuerung in [!DNL Adobe Workfront Fusion]</a>.</p> </td>  
   </tr>  
   <tr> 
     <td role="rowheader">Erweitern des Szenarios mit erweiterten Tools</td>   
     <td>Klicken Sie auf das Symbol [!UICONTROL Tools] . <img src="assets/tools-icon.gif"> Sie können Trigger, Aktionen, Aggregatoren und Transformatoren erstellen. Weitere Informationen finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Instrumente</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Verwenden von Textanalysewerkzeugen</td>   
     <td>Klicken Sie auf das Symbol [!UICONTROL Text-Parser] . <img src="assets/text-parser-icon.gif"> Sie können Elemente aus dem HTML-Code abrufen, Zeichenfolgen-Elemente suchen und extrahieren, die einem Suchmuster entsprechen,-Text suchen und ersetzen und Daten von einer Website "auseinanderziehen". Weitere Informationen finden Sie unter <a href="../../workfront-fusion/apps-and-their-modules/tools-modules.md" class="MCXref xref">Instrumente</a>.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Zugriff auf die am häufigsten verwendeten Apps und Dienste</td>   
     <td> Klicken Sie auf ein Symbol im <strong>[!UICONTROL Favoriten]</strong> unten auf dem Bildschirm. In diesem Abschnitt werden automatisch Symbole angezeigt, wenn Sie Ihrem Szenario Apps und Dienste hinzufügen. Sie können auch auf das Symbol Hinzufügen klicken <img src="assets/add-icon.gif"> , um diesem Bereich manuell Apps und Dienste hinzuzufügen.</td>  
   </tr>  
   <tr> 
     <td role="rowheader">Testen des Szenarios</td>   
     <td>Klicken <strong>[!UICONTROL Einmal ausführen]</strong> , um zu überprüfen, ob das Szenario wie erwartet ausgeführt wird, bevor Sie es aktivieren. Nach der Aktivierung wird das Szenario gemäß seinem Zeitplan ausgeführt. Wenn nicht alles wie erwartet ausgeführt wird, erfahren Sie in unserem Abschnitt zur Fehlerbehebung , wie Fehler zu handhaben sind.</td> 
   </tr> 
</tbody>
</table>
