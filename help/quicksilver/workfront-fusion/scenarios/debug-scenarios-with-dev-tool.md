---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Debugging-Szenarien mit dem Adobe Workfront Fusion-Entwicklungstool
description: Mit dem Adobe Workfront Fusion Devtool können Sie Szenarien verstehen und Fehler beheben. Das Entwickler-Tool fügt den Chrome Developer Tools ein zusätzliches Bedienfeld hinzu. Mithilfe dieses Debugger-Bedienfelds können Sie alle manuellen Ausführungen Ihres Szenarios überprüfen, alle ausgeführten Vorgänge überprüfen und die Details jedes ausgeführten API-Aufrufs anzeigen. Sie können sehen, welches Modul, welcher Vorgang oder welche einzelne Antwort den Fehler verursacht hat, und dieses Wissen verwenden, um Ihr Szenario zu verfeinern.
author: Becky
feature: Workfront Fusion
exl-id: f7557214-3615-4797-b4cb-4af70e4797ac
source-git-commit: 6edcb5b826bdcf37b62396a926c923875a3a1436
workflow-type: tm+mt
source-wordcount: '1858'
ht-degree: 1%

---

# Debugging-Szenarien mit dem [!DNL Adobe Workfront Fusion] Entwickler-Tool

Mit dem Entwickler-Tool [!DNL Adobe Workfront Fusion] können Sie Szenarien verstehen und Fehler beheben. Das Entwickler-Tool fügt dem [!DNL Chrome Developer Tools] ein zusätzliches Bedienfeld hinzu. Mithilfe dieses Debugger-Bedienfelds können Sie alle manuellen Ausführungen Ihres Szenarios überprüfen, alle ausgeführten Vorgänge überprüfen und die Details jedes ausgeführten API-Aufrufs anzeigen. Sie können sehen, welches Modul, welcher Vorgang oder welche einzelne Antwort den Fehler verursacht hat, und dieses Wissen verwenden, um Ihr Szenario zu verfeinern.

>[!NOTE]
>
>Die Anmeldung im Debugger-Bedienfeld ist für vertrauliche Szenarien, automatische Ausführungen und erfolgreiche Vorgänge eingeschränkt oder nicht verfügbar.

Eine Videoeinführung und exemplarische Anleitung zum Fusion-Entwickler finden Sie unter

* [Fusion Development Tool](https://video.tv.adobe.com/v/3427031/){target=_blank}.
* [Entwickler-exemplarische Vorgehensweise](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/fusion/troubleshooting-and-error-handling/dev-tool-walkthrough.html?lang=en)

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
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
   </td>    </tr> 
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

## Zugriff auf das Workfront Fusion-Entwicklungstool

Der Zugriff auf das Entwickler-Tool hängt davon ab, ob Sie Fusion im [!DNL Adobe Unified Experience] verwenden.

* [Zugriff auf das Entwickler-Tool im Ordner [!DNL Adobe Unified Experience]](#access-the-devtool-in-the-adobe-unified-experience)
* [Zugriff auf das Entwickler-Tool im klassischen [!DNL Fusion] Erlebnis](#access-the-devtool-in-the-classic-fusion-experience)

### Zugriff auf das Entwickler-Tool im [!DNL Adobe Unified Experience] oder dem neuen Fusionserlebnis

Wenn Sie Fusion in der Adobe Unified Shell verwenden oder auf das neue Fusion-Erlebnis aktualisiert haben, können Sie über den Szenario-Editor auf das Dev-Tool zugreifen.

1. Klicken Sie unten auf dem Bildschirm auf das Symbol **Helper tools** ![Helper tools](assets/debugger-icon.png) .

Oder:

1. Wechseln Sie zum Szenario-Editor für das Szenario, das Sie debuggen möchten.

   Informationen zum Suchen des Szenario-Editors finden Sie unter [Szenario-Editor](/help/quicksilver/workfront-fusion/scenarios/scenario-editor.md).

1. Klicken Sie mit der rechten Maustaste in einen leeren Bereich der Seite (nicht auf ein Modul).
1. Wählen Sie **Entwickler öffnen** aus.

### Zugriff auf das Entwickler-Tool im klassischen Erlebnis [!DNL Fusion]

Um das Entwickler-Tool im klassischen [!DNL Fusion] -Erlebnis zu verwenden, müssen Sie eine [!DNL Chrome] -Erweiterung installieren. Sie können diese Erweiterung dann über die [!DNL Chrome] Entwicklertools verwenden.

* [Installieren Sie die Erweiterung [!DNL Chrome] Devtool installieren .](#install-the-chrome-devtool-extension)
* [Suchen Sie das  [!DNL Workfront Fusion] Entwickler-Tool](#locate-the-workfront-fusion-devtool)

#### Installieren der Erweiterung [!DNL Chrome] Devtool

Sie können das [!DNL Workfront Fusion] Entwickler-Tool über den [!UICONTROL [!DNL Chrome] Webspeicher] zu [!DNL Chrome] hinzufügen.

1. Klicken Sie auf [diesen Link](https://chromewebstore.google.com/u/1/detail/workfront-fusion-devtool/hkimbmkkmmejdnhbhoaefggkpkndfjnn) , um zum [!DNL Workfront Fusion] Entwickler-Tool im [!UICONTROL [!DNL Chrome] Webspeicher] zu wechseln.
1. Klicken Sie auf **[!UICONTROL Zu[!DNL Chrome]]** hinzufügen.
1. Überprüfen Sie im sich öffnenden Fenster die Berechtigungen. Wenn Sie mit den Berechtigungen einverstanden sind, klicken Sie auf **[!UICONTROL Erweiterung hinzufügen]**.

Die [!DNL Workfront Fusion] Devtool-Erweiterung wird Ihren [!DNL Chrome] -Erweiterungen hinzugefügt.


#### Suchen Sie das [!DNL Workfront Fusion]-Entwickler-Tool

Um das [!DNL Workfront Fusion]-Entwickler-Tool zu verwenden, müssen Sie die [!DNL Workfront Fusion] Entwickler-Tool-Erweiterung zu Ihrem [!DNL Chrome] -Browser hinzufügen, wie unter [Installieren der Chrome Devtool-Erweiterung](#install-the-chrome-Devtool-extension) beschrieben.

1. Öffnen Sie Ihr [!DNL Workfront Fusion]-Szenario.
1. Öffnen Sie [!DNL Chrome Developer Tools]:

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
      <td> <p>Strg + Umschalt + I</p> <p> Oder </p> <p>F12</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Es wird empfohlen, die [!DNL Chrome Developer Console] unten anzudocken, um eine bessere Ansicht Ihrer Module zu erhalten.

1. Klicken Sie auf die Registerkarte **[!DNL Workfront Fusion]** in [!DNL Chrome Dev Tools].

## Verwenden des [!DNL Workfront Fusion]-Entwicklungstools

Workfront Fusion Devtool ist in drei Hauptbereiche unterteilt. Sie finden diese im linken Bereich Ihres Entwickler-Tools-Fensters.

* [Live-Stream](#live-stream)
* [Szenario-Debugger](#scenario-debugger)
* [Instrumente](#tools)

### Live Stream

Live Stream zeigt an, was im Hintergrund passiert, wenn Sie in Ihrem Szenario auf &quot;Einmal ausführen&quot;klicken.

1. Klicken Sie auf das Symbol **[!UICONTROL Live-Stream]** ![](assets/live-stream-icon.png), um den Abschnitt &quot;Live-Stream&quot;zu öffnen.
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
        <li> <p>Anfragekopfzeilen (API-Endpunkt-URL, HTTP-Methode, Uhrzeit und Datum des Aufrufs der Anfrage, Anfragekopfzeilen und Abfragezeichenfolge)</p> </li> 
        <li> <p>Anfrageinhalt</p> </li> 
        <li> <p>Antwortheader</p> </li> 
        <li> <p>Response Body</p> </li> 
       </ul> <p>Um diese Informationen anzuzeigen, klicken Sie auf die entsprechende Registerkarte im rechten Bereich des [!DNL Workfront Fusion] Entwickler-Tools.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Suchanfragen und Antworten</p> </td> 
      <td> <p>Geben Sie den Suchbegriff in das Suchfeld im linken Bereich des [!DNL Workfront Fusion] Entwickler-Tools ein, um nur Anforderungen anzuzeigen, die den Suchbegriff enthalten.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Liste von Anforderungen entfernen </p> </td> 
      <td> <p>Klicken Sie auf das Papierkorbsymbol in der oberen rechten Ecke des linken Bedienfelds des Entwickler-Tools, um die Liste der vom Entwickler-Tool aufgezeichneten Anforderungen zu löschen.[!DNL Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Aktivieren der Konsolenprotokollierung</p> </td> 
      <td> <p>Klicken Sie auf das Computersymbol <img src="assets/console-computer-icon.png"> in der oberen rechten Ecke des linken Bedienfelds des Entwickler-Tools.</p> <p>Die Protokollierung in der Konsole ist aktiviert, wenn das Computersymbol grün ist.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Rufen Sie die Anforderung im JSON-Rohformat oder in der cURL ab</p> </td> 
      <td> 
       <ul> 
        <li> <p><strong>Roh JSON</strong> </p> <p>Klicken Sie oben rechts im rechten Bereich des Entwickler-Tools auf <strong>[!UICONTROL RAW kopieren]</strong>.</p> </li> 
        <li> <p><strong>cURL</strong> </p> <p>Klicken Sie oben rechts im rechten Bereich des Entwickler-Tools auf <strong>[!UICONTROL cURL kopieren]</strong>.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

### Szenario-Debugger

Der Szenario-Debugger ist für komplexere Szenarien nützlich. Er zeigt den Verlauf der ausgeführten Szenarien an und ermöglicht es Ihnen, Module nach ihrem Namen oder ihrer ID zu suchen.

1. Klicken Sie auf das Symbol **[!UICONTROL Szenario-Debugger]** ![](assets/scenario-debugger-icon.png), um den Szenario-Debugger zu öffnen.
1. (Optional) Geben Sie den Suchbegriff (Name oder Modul-ID) im Suchfeld im linken Bereich von [!DNL Workfront Fusion] Devtool im Abschnitt [!UICONTROL Szenario-Debugger] ein.
1. Doppelklicken Sie auf den Namen des Moduls, um seine Einstellungen im Szenario-Editor zu öffnen.
1. Zeigen Sie die Anfragedetails an, indem Sie auf den gewünschten Vorgang klicken.

### Instrumente

Das [!DNL Workfront Fusion]-Entwickler-Tool verfügt über Tools, die die Einrichtung Ihres Szenarios erleichtern.

1. Klicken Sie auf das Symbol **[!UICONTROL Tools]** ![](assets/console-tools-icon.png), um die Tools zu öffnen.
1. Wählen Sie das gewünschte Tool aus
1. Konfigurieren Sie die Felder wie unten beschrieben.
1. Klicken Sie auf **[!UICONTROL Ausführen]**.

Tools und ihre Felder:

* [Fokus auf ein Modul](#focus-a-module)
* [Module durch Zuordnung suchen](#find-modules-by-mapping)
* [App-Metadaten abrufen](#get-app-metadata)
* [Zuordnung kopieren](#copy-mapping)
* [Filter kopieren](#copy-filter)
* [Verbindung tauschen](#swap-connection)
* [Variable tauschen](#swap-variable)
* [App tauschen](#swap-app)
* [Base 64](#base-64)
* [Modulnamen kopieren](#copy-module-name)
* [Remap Source](#remap-source)
* [Anwendung markieren](#highlight-app)
* [Migrieren von GS](#migrate-gs)

#### [!UICONTROL Fokus auf ein Modul]

Öffnet die Einstellungen des angegebenen Moduls nach ID.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Modul-ID]</td>
        <td>Geben Sie die ID des Moduls ein, für das Sie Einstellungen öffnen möchten.</td>
    </tr>
</table>

#### [!UICONTROL Module durch Zuordnung suchen]

Ermöglicht die Suche nach Modulwerten für einen bestimmten Begriff. Die Ausgabe enthält IDs von Modulen, die den gesuchten Begriff enthalten.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Keyword]</td> 
   <td> <p> Geben Sie den Begriff ein, nach dem Sie suchen möchten. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Nur Werte verwenden]</p> </td> 
   <td> <p>Aktivieren Sie diese Option, um nur in den Werten der Modulfelder zu suchen.</p> <p>Deaktivieren Sie diese Option, um auch in den Namen der Modulfelder zu suchen.</p> <p>Die Suche wird über die Parameter name und label durchgeführt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL App-Metadaten abrufen]

Ruft Metadaten der App anhand des Modulnamens oder der ID der App ab. Dies ist beispielsweise nützlich, wenn Sie die Version der App kennen müssen, die in Ihrem Szenario verwendet wird.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
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
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Wählen Sie das Modul aus oder geben Sie die ID des Moduls ein, aus dem Sie Feldwerte kopieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Wählen Sie das Modul aus oder geben Sie die ID des Moduls ein, in das Sie die Quellmodulwerte einfügen möchten.</p> <p>Wichtig: Werte im Zielmodul werden überschrieben.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Filter kopieren]

Kopiert die Filtereinstellungen aus dem Quellmodul in das Zielmodul.

>[!NOTE]
>
>Die Kopieraktion wird für den Filter durchgeführt, der auf der linken Seite des ausgewählten Moduls platziert wird.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> Wählen Sie das Modul aus oder geben Sie die ID des Moduls ein, aus dem Sie Filterwerte kopieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Wählen Sie das Modul aus oder geben Sie die ID des Moduls ein, in das Sie die Filterwerte aus dem Quellmodul einfügen möchten.</p> <p>Wichtig: Werte im Zielmodul werden überschrieben.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Einstellung Fallback-Route beibehalten]</p> </td> 
   <td> <p>Der Quellfilter wird als Ausweichroute festgelegt. Aktivieren Sie diese Option, um auch festzulegen, dass der Zielfilter als Ausweichroute festgelegt ist.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Verbindung tauschen]

Dupliziert eine Verbindung vom Quellmodul zu jedem Modul im Szenario derselben App.

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Wählen Sie das Modul aus oder geben Sie die Kennung des Moduls ein, aus dem Sie die Verbindung duplizieren möchten.</td>
    </tr>
</table>

#### [!UICONTROL Variable tauschen]

Sucht nach bestimmten Variablen im Szenario und ersetzt sie durch eine neue Variable.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Variable zu suchen]</td> 
   <td> <p> Suchen Sie die Variable, die Sie ersetzen möchten, aus dem Modul in Ihrem Szenario und kopieren Sie sie in das Feld ([!UICONTROL Variable to Find]). Im Feld wird es mit doppelten geschweiften Klammern angezeigt. Beispiel: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Ersetzen durch]</p> </td> 
   <td> <p>Suchen Sie die Variable, die Sie durch ersetzen möchten, aus dem -Modul in Ihrem Szenario und kopieren Sie sie in dieses Feld ([!UICONTROL Variable to Find]). Im Feld wird es mit doppelten geschweiften Klammern angezeigt. Beispiel: <code>&#123;&#123;5.value&#125;&#125;</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Modul]</p> </td> 
   <td> <p>Wählen Sie das Modul aus, in dem Sie die Variable ersetzen möchten. Wenn kein Modul ausgewählt ist, wird die Variable im gesamten Szenario ersetzt.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL App tauschen]

Ersetzt die ausgewählte App-Version in Ihrem Szenario durch eine andere App-Version.

Dies kann beispielsweise verwendet werden, um die Module von Gmail- und E-Mail-Apps auf die neueste Version zu aktualisieren.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL App zu ersetzen]</td> 
   <td> <p> Wählen Sie die App aus, die Sie ersetzen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Ersetzen durch]</p> </td> 
   <td> <p>Wählen Sie die App aus, durch die Sie sie ersetzen möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Base 64]

Dient der Codierung der eingegebenen Daten in Base64 oder der Dekodierung von Base64. Einige Anforderungen sind in Base64 kodiert. Dieses Tool kann nützlich sein, wenn Sie in der kodierten Anforderung nach bestimmten Daten suchen möchten.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Vorgang] </td> 
   <td> <p>Wählen Sie aus, ob Sie die Daten aus dem [!UICONTROL Rohdaten]-Feld in Base64 kodieren oder Base64 in Rohdaten dekodieren möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Rohdaten]</p> </td> 
   <td> <p> Geben Sie die Daten ein, die Sie in Base64 oder Base64 kodieren möchten, wenn Sie die Dekodierung in Rohdaten durchführen möchten. Dies hängt von der im obigen Feld [!UICONTROL Vorgang] ausgewählten Option ab.</p> </td> 
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
   <td role="rowheader">[!UICONTROL Modul] </td> 
   <td> <p>Wählen Sie das Modul aus, dessen Namen Sie kopieren möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remap Source]

Ermöglicht die Änderung der Zuordnungsquelle von einem Modul zum anderen.

Sie müssen zunächst das Modul, das Sie als Quellmodul verwenden möchten, zur Route in Ihrem Szenario hinzufügen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module] </td> 
   <td> <p> Wählen Sie das Modul aus, das Sie als Zuordnungsquelle für andere Module in Ihrem Szenario ersetzen möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Target Module]</p> </td> 
   <td> <p>Wählen Sie das Modul aus, das Sie als neue Zuordnungsquelle verwenden möchten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Modul zu bearbeiten]</p> </td> 
   <td> <p>Wählen Sie das Modul aus, für das Sie die Zuordnung ändern möchten, wenn Sie die Zuordnung im gesamten Szenario nicht ändern möchten. </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Anwendung markieren]

Hebt Module der angegebenen App in Ihrem Szenario hervor.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL App zu markieren] </td> 
   <td> <p> Wählen Sie die App aus, die im Szenario hervorgehoben werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Version] </p> </td> 
   <td> <p>Wählen Sie die Version der App aus, die hervorgehoben werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Hervorhebungsfarbe]</p> </td> 
   <td> <p> Geben Sie den Farb-Hexadezimal ein, den Sie für die Hervorhebung von Modulen verwenden möchten.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Migrieren von GS]

Dieses Tool wurde speziell zum Aktualisieren der [!DNL Google Sheets] -Module (veraltet) auf die neueste [!DNL Google Sheets] -Version entwickelt. Eine neue Version des Moduls wird direkt nach der älteren Version des Moduls in der Szenarioroute hinzugefügt.

Für dieses Modul müssen Sie keine Parameter festlegen.
