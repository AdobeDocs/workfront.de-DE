---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Fehlerbehebungsszenarien mit dem Adobe Workfront Fusion DevTool
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1861'
ht-degree: 1%

---

# Debugging-Szenarien mit dem [!DNL Adobe Workfront Fusion] DevTool

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Debuggen eines Szenarios](https://experienceleague.adobe.com/docs/workfront-fusion/using/manage-scenarios/debug-a-scenario.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Mit dem [!DNL Adobe Workfront Fusion] DevTool können Sie Szenarien verstehen und Fehler beheben. Das DevTool fügt dem [!DNL Chrome Developer Tools] ein zusätzliches Bedienfeld hinzu. Mithilfe dieses Debugger-Bedienfelds können Sie alle manuellen Ausführungen Ihres Szenarios überprüfen, alle ausgeführten Vorgänge überprüfen und die Details jedes durchgeführten API-Aufrufs anzeigen. Sie können sehen, welches Modul, welcher Vorgang oder welche einzelne Antwort den Fehler verursacht hat, und dieses Wissen verwenden, um Ihr Szenario zu verfeinern.

>[!NOTE]
>
>Die Protokollierung im Debugger-Bedienfeld ist für vertrauliche Szenarien, automatische Ausführungen und erfolgreiche Vorgänge eingeschränkt oder nicht verfügbar.

Eine Videoeinführung und exemplarische Anleitung für das Fusion DevTool finden Sie unter

* [Fusion-Entwicklungstool](https://video.tv.adobe.com/v/3427031/){target=_blank}.
* [Anleitung zu Devtool](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/troubleshooting-and-error-handling/dev-tool-walkthrough.html)

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
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
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

## Zugriff auf das Workfront Fusion DevTool

Der Zugriff auf das DevTool unterscheidet sich je nachdem, ob Sie Fusion in der [!DNL Adobe Unified Experience] verwenden.

* [Greifen Sie auf das DevTool in der  [!DNL Adobe Unified Experience]](#access-the-devtool-in-the-adobe-unified-experience)
* [Zugriff auf das DevTool in der klassischen  [!DNL Fusion] ](#access-the-devtool-in-the-classic-fusion-experience)

### Zugriff auf das DevTool im [!DNL Adobe Unified Experience] oder im neuen Fusion-Erlebnis

Wenn Sie Fusion in der Adobe Unified Shell verwenden oder auf das neue Fusion-Erlebnis aktualisiert haben, können Sie über den Szenario-Editor auf das Dev Tool zugreifen.

1. Klicken Sie auf **Helper-Tools** ![Helper-Tools](assets/debugger-icon.png) unten auf dem Bildschirm.

Oder:

1. Wechseln Sie zum Szenario-Editor für das Szenario, das Sie debuggen möchten.

   Den Szenario-Editor finden Sie unter [Szenario-Editor](/help/quicksilver/workfront-fusion/scenarios/scenario-editor.md).

1. Klicken Sie mit der rechten Maustaste in einen leeren Bereich der Seite (nicht auf ein Modul).
1. Wählen Sie **DevTool öffnen**.

### Zugriff auf das DevTool im klassischen [!DNL Fusion]

Um das DevTool in der klassischen [!DNL Fusion]-Version zu verwenden, müssen Sie eine [!DNL Chrome]-Erweiterung installieren. Sie können diese Erweiterung dann über die [!DNL Chrome] Entwickler-Tools verwenden.

* [Installieren der Erweiterung  [!DNL Chrome] .Devtool](#install-the-chrome-devtool-extension)
* [Suchen Sie das  [!DNL Workfront Fusion] -Devtool](#locate-the-workfront-fusion-devtool)

#### Installieren der [!DNL Chrome] Devtool-Erweiterung

Sie können das [!DNL Workfront Fusion] DevTool [!DNL Chrome] über den [!UICONTROL [!DNL Chrome] Web Store hinzufügen].

1. Klicken Sie [diesen Link](https://chromewebstore.google.com/u/1/detail/workfront-fusion-devtool/hkimbmkkmmejdnhbhoaefggkpkndfjnn), um zum [!DNL Workfront Fusion] DevTool im [!UICONTROL [!DNL Chrome] Web Store zu ].
1. Klicken Sie auf **[!UICONTROL Zu[!DNL Chrome]]** hinzufügen.
1. Überprüfen Sie im sich öffnenden Fenster die Berechtigungen. Wenn Sie den Berechtigungen zustimmen, klicken Sie auf **[!UICONTROL Erweiterung hinzufügen]**.

Die [!DNL Workfront Fusion] Devtool-Erweiterung wird Ihren [!DNL Chrome]-Erweiterungen hinzugefügt.


#### Suchen Sie das [!DNL Workfront Fusion] DevTool

Um das [!DNL Workfront Fusion] Devtool zu verwenden, müssen Sie die [!DNL Workfront Fusion] Devtool-Erweiterung zu Ihrem [!DNL Chrome] hinzufügen, wie in [Installieren der Chrome Devtool-Erweiterung](#install-the-chrome-Devtool-extension) beschrieben.

1. Öffnen Sie Ihr [!DNL Workfront Fusion].
1. [!DNL Chrome Developer Tools] öffnen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Mac]</td> 
      <td>Befehl + Option + I</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Windows]</td> 
      <td> <p>Strg+Umsch+I</p> <p> Oder </p> <p>F12</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Es wird empfohlen, die [!DNL Chrome Developer Console] am unteren Rand anzudocken, um eine bessere Ansicht Ihrer Module zu erhalten.

1. Klicken Sie in [!DNL Chrome Dev Tools] auf die Registerkarte **[!DNL Workfront Fusion]** .

## Verwenden des [!DNL Workfront Fusion] DevTools

Workfront Fusion Devtool ist in drei Hauptabschnitte unterteilt. Sie finden diese im linken Bereich Ihres DevTool-Fensters.

* [Live-Stream](#live-stream)
* [Szenario-Debugger](#scenario-debugger)
* [Tools](#tools)

### Live-Stream

Live Stream zeigt an, was im Hintergrund passiert, wenn Sie in Ihrem Szenario einmal auf Ausführen klicken.

1. Klicken Sie auf das **[!UICONTROL Live-Stream]**-Symbol ![](assets/live-stream-icon.png), um den Abschnitt Live-Stream zu öffnen.
1. Führen Sie einen der folgenden Schritte aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Aktion</th> 
      <th>Anleitung</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anfrageinformationen anzeigen</td> 
      <td> <p>Sie können die folgenden Informationen für jedes Modul in Ihrem Szenario anzeigen</p> 
       <ul> 
        <li> <p>Anfragekopfzeilen (API-Endpunkt-URL, HTTP-Methode, Uhrzeit und Datum, an dem die Anfrage aufgerufen wurde, Anfragekopfzeilen und Abfragezeichenfolge)</p> </li> 
        <li> <p>Anfragetext</p> </li> 
        <li> <p>Antwort-Header</p> </li> 
        <li> <p>Antworttext</p> </li> 
       </ul> <p>Um diese Informationen anzuzeigen, klicken Sie auf die entsprechende Registerkarte im rechten Bedienfeld des [!DNL Workfront Fusion] DevTools.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Suchanfragen und Antworten</p> </td> 
      <td> <p>Geben Sie den Suchbegriff in das Suchfeld im linken Bereich des [!DNL Workfront Fusion] DevTools ein, um nur Anfragen anzuzeigen, die den Suchbegriff enthalten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Liste der Anfragen entfernen </p> </td> 
      <td> <p>Klicken Sie auf das Papierkorb-Symbol in der oberen rechten Ecke des linken Bedienfelds des DevTools, um die Liste der vom [!DNL Workfront Fusion] DevTool aufgezeichneten Anfragen zu löschen. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Konsolenprotokollierung aktivieren</p> </td> 
      <td> <p>Klicken Sie auf das Computersymbol <img src="assets/console-computer-icon.png"> in der oberen rechten Ecke des linken Bedienfelds von DevTool.</p> <p>Die Protokollierung in der Konsole ist aktiviert, wenn das Computersymbol grün ist.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Rufen Sie die Anfrage im rohen JSON-Format oder cURL ab.</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>Roh-JSON</strong> </p> <p>Klicken Sie auf <strong>[!UICONTROL Copy RAW]</strong> in der oberen rechten Ecke des rechten Fensterbereichs von Devtool.</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>Klicken Sie auf <strong>[!UICONTROL Copy cURL]</strong> in der oberen rechten Ecke des rechten Bereichs des Devtools.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Szenario-Debugger

Der Szenario-Debugger ist für komplexere Szenarien nützlich. Es zeigt den Verlauf der Szenario-Ausführungen an und ermöglicht es Ihnen, Module anhand ihres Namens oder ihrer ID zu durchsuchen.

1. Klicken Sie auf **[!UICONTROL Symbol]** Szenario-Debugger![](assets/scenario-debugger-icon.png), um den Szenario-Debugger zu öffnen.
1. (Optional) Geben Sie den Suchbegriff (Name oder Modul-ID) in das Suchfeld im linken Bereich [!DNL Workfront Fusion] DevTool im Abschnitt [!UICONTROL Szenario-]&quot; ein.
1. Doppelklicken Sie auf den Namen des Moduls, um seine Einstellungen im Szenario-Editor zu öffnen.
1. Zeigen Sie Anfragedetails an, indem Sie auf den gewünschten Vorgang klicken.

### Tools

Das [!DNL Workfront Fusion] DevTool bietet Tools, die die Einrichtung Ihres Szenarios erleichtern.

1. Klicken Sie auf das **[!UICONTROL Tools]**-Symbol ![](assets/console-tools-icon.png), um die Tools zu öffnen.
1. Wählen Sie das gewünschte Tool aus
1. Konfigurieren Sie die Felder wie unten beschrieben.
1. Klicken Sie auf **[!UICONTROL Ausführen]**.

Tools und ihre Felder:

* [Fokussieren eines Moduls](#focus-a-module)
* [Module nach Zuordnung suchen](#find-modules-by-mapping)
* [Abrufen von App-Metadaten](#get-app-metadata)
* [Zuordnung kopieren](#copy-mapping)
* [Filter kopieren](#copy-filter)
* [Wechseln der Verbindung](#swap-connection)
* [Swap-Variable](#swap-variable)
* [App austauschen](#swap-app)
* [Base 64](#base-64)
* [Modulnamen kopieren](#copy-module-name)
* [Source neu zuordnen](#remap-source)
* [Programm hervorheben](#highlight-app)
* [Migrieren von GS](#migrate-gs)

#### [!UICONTROL Fokussieren eines Moduls]

Öffnet die Einstellungen des angegebenen Moduls nach ID.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Modul-ID]</td>
        <td>Geben Sie die ID des Moduls ein, für das Sie die Einstellungen öffnen möchten.</td>
    </tr>
</table>

#### [!UICONTROL Module nach Zuordnung suchen]

Ermöglicht die Suche nach den Modulwerten für einen bestimmten Begriff. Die Ausgabe enthält IDs von Modulen, die den gesuchten Begriff enthalten.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Schlüsselwort]</td> 
   <td> <p> Geben Sie den Begriff ein, nach dem Sie suchen möchten. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nur Werte verwenden]</p> </td> 
   <td> <p>Aktivieren Sie diese Option, um nur in den Werten der Modulfelder zu suchen.</p> <p>Deaktivieren Sie diese Option, um auch nach den Namen der Modulfelder zu suchen.</p> <p>Die Suche wird über die Parameter Name und Titel durchgeführt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Abrufen von App-Metadaten]

Ruft Metadaten der App anhand des Modulnamens oder der ID der App ab. Dies ist beispielsweise nützlich, wenn Sie die Version der in Ihrem Szenario verwendeten App kennen müssen.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source-Modul]</td>
        <td>Wählen Sie das Modul aus, für das Sie Metadaten abrufen möchten.</td>
    </tr>
</table>

#### [!UICONTROL Zuordnung kopieren]

Kopiert Werte aus dem Quellmodul in das Zielmodul.

>[!CAUTION]
>
>Stellen Sie sicher, dass Sie die richtigen Quell- und Zielmodule festlegen. Wenn Sie einen anderen Modultyp auswählen, werden die Werte im Zielmodul gelöscht.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Modul]</td> 
   <td> <p> Wählen Sie das Modul aus oder geben Sie die ID des Moduls ein, aus dem Sie die Feldwerte kopieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target-Modul]</p> </td> 
   <td> <p>Wählen Sie das Modul aus oder geben Sie die ID des Moduls ein, in das Sie die Werte des Quellmoduls einfügen möchten.</p> <p>Wichtig: Die Werte im Zielmodul werden überschrieben.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Filter kopieren]

Kopiert die Filtereinstellungen vom Quell- zum Zielmodul.

>[!NOTE]
>
>Die Kopieraktion wird für den Filter ausgeführt, der auf der linken Seite des ausgewählten Moduls platziert ist.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Modul]</td> 
   <td> <p> Wählen Sie das Modul aus oder geben Sie die ID des Moduls ein, aus dem Sie Filterwerte kopieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target-Modul]</p> </td> 
   <td> <p>Wählen Sie das Modul aus oder geben Sie die ID des Moduls ein, in das Sie die Filterwerte aus dem Quellmodul einfügen möchten.</p> <p>Wichtig: Die Werte im Zielmodul werden überschrieben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Einstellung der Ausweichroute beibehalten]</p> </td> 
   <td> <p>Der Quellfilter wird als Fallback-Route festgelegt. Aktivieren Sie diese Option, um auch festzulegen, dass der Zielfilter als Ausweichroute festgelegt wird.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Wechseln der Verbindung]

Dupliziert eine Verbindung vom Quellmodul zu jedem Modul im Szenario derselben App.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source-Modul]</td>
        <td>Wählen Sie das Modul aus oder geben Sie die ID des Moduls ein, aus dem Sie die Verbindung duplizieren möchten.</td>
    </tr>
</table>

#### [!UICONTROL Swap-Variable]

Sucht im Szenario nach angegebenen Variablen und ersetzt sie durch eine neue Variable.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variable zum Suchen]</td> 
   <td> <p> Suchen Sie die Variable Pille, die Sie aus dem Modul in Ihrem Szenario ersetzen möchten, und kopieren Sie sie in dieses Feld ([!UICONTROL Variable zum Suchen]). Im Feld wird sie mit doppelten geschweiften Klammern angezeigt. Beispiel: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL durch] ersetzen</p> </td> 
   <td> <p>Suchen Sie die Variable Pille, mit der Sie die Variable ersetzen möchten, aus dem Modul in Ihrem Szenario und kopieren Sie sie in dieses Feld ([!UICONTROL Variable zum Suchen]). Im Feld wird sie mit doppelten geschweiften Klammern angezeigt. Beispiel: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Modul]</p> </td> 
   <td> <p>Wählen Sie das Modul aus, in dem Sie die Variable ersetzen möchten. Wenn kein Modul ausgewählt ist, wird die Variable im gesamten Szenario ersetzt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL App austauschen]

Ersetzt die ausgewählte Programmversion in Ihrem Szenario durch eine andere Programmversion.

Dies kann beispielsweise verwendet werden, um die Module von Gmail und Email Apps auf die neueste Version zu aktualisieren.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-App, die ersetzt werden soll]</td> 
   <td> <p> Wählen Sie die App aus, die Sie ersetzen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Ersetzen durch]</p> </td> 
   <td> <p>Wählen Sie die App aus, durch die Sie sie ersetzen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Base 64]

Ermöglicht die Kodierung der eingegebenen Daten in Base64 oder die Dekodierung von Base64. Einige Anfragen sind mit Base64 codiert. Dieses Tool kann nützlich sein, wenn Sie in der kodierten Anfrage nach bestimmten Daten suchen möchten.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Vorgang] </td> 
   <td> <p>Wählen Sie aus, ob die Daten aus dem Feld [!UICONTROL Raw Data] in Base64 kodiert oder Base64 in Raw Data dekodiert werden sollen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Rohdaten]</p> </td> 
   <td> <p> Geben Sie die Daten, die Sie für Base64 codieren möchten, oder Base64 ein, wenn Sie für Rohdaten decodieren möchten, je nach der im Feld [!UICONTROL-Vorgang] oben ausgewählten Option.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Modulnamen kopieren]

Kopiert den Namen des ausgewählten Moduls in die Zwischenablage.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-Modul] </td> 
   <td> <p>Wählen Sie das Modul aus, dessen Namen Sie kopieren möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Source neu zuordnen]

Ermöglicht das Ändern der Zuordnungsquelle von einem Modul zu einem anderen.

Zunächst müssen Sie das Modul, das Sie als Quellmodul verwenden möchten, zur Route in Ihrem Szenario hinzufügen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source-Modul] </td> 
   <td> <p> Wählen Sie das Modul aus, das Sie als Zuordnungsquelle für andere Module in Ihrem Szenario ersetzen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target-Modul]</p> </td> 
   <td> <p>Wählen Sie das Modul aus, das Sie als neue Zuordnungsquelle verwenden möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL-Modul zum Bearbeiten]</p> </td> 
   <td> <p>Wählen Sie das Modul aus, für das Sie die Zuordnung ändern möchten, wenn Sie die Zuordnung nicht im gesamten Szenario ändern möchten. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Programm hervorheben]

Zeigt Module der angegebenen App in Ihrem Szenario an.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL-App, die hervorgehoben werden soll] </td> 
   <td> <p> Wählen Sie die App aus, die Sie in Ihrem Szenario hervorheben möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Version] </p> </td> 
   <td> <p>Wählen Sie die Version der App aus, die Sie hervorheben möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Hervorhebungsfarbe]</p> </td> 
   <td> <p> Geben Sie den Farbhex ein, den Sie für Hervorhebungsmodule verwenden möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Migrieren von GS]

Dieses Tool wurde speziell für die Aktualisierung von [!DNL Google Sheets] (alten) -Modulen auf die neueste [!DNL Google Sheets]-Version entwickelt. Eine neue Version des Moduls wird direkt nach der älteren Version des Moduls in der Szenarioroute hinzugefügt.

Für dieses Modul müssen keine Parameter festgelegt werden.
