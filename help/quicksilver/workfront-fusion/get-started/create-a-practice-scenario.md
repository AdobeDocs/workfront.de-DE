---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Erstellen eines Szenarios für die Integration von Verfahren in Adobe Workfront Fusion
description: In diesem Artikel wird beschrieben, wie Sie ein Integrationsszenario mit Adobe Workfront Fusion erstellen. Integrationsszenarios verbinden separate Apps miteinander, sodass Ihre Daten durch verschiedene Anwendungen fließen können.
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: f11af8d9d1e5fa65c2efb4d882d25f9e13784611
workflow-type: tm+mt
source-wordcount: '2139'
ht-degree: 0%

---

# Erstellen eines Szenarios für die Integration von Verfahren in Adobe Workfront Fusion

In diesem Artikel wird beschrieben, wie Sie ein Integrationsszenario mit Adobe Workfront Fusion erstellen. Integrationsszenarios verbinden separate Apps miteinander, sodass Ihre Daten durch verschiedene Anwendungen fließen können.

Um ein Integrationsszenario zu erstellen, muss Ihr Unternehmen über eine [!DNL Workfront Fusion for Work Automation and Integration] -Lizenz verfügen.

Anweisungen zum Erstellen eines Automatisierungsszenarios nur für Workfront finden Sie unter [Erstellen eines Szenarios für die Automatisierung von Verfahren in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

Weitere Informationen zu Workfront Fusion-Lizenzen finden Sie unter [Adobe Workfront Fusion-Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

>[!NOTE]
>
>Möglicherweise gestattet Ihr Unternehmen keinen Zugriff auf Google Tabellen. Ist dies der Fall, können Sie diese Integration nicht einrichten, aber die hier dargestellten Informationen können als allgemeines Beispiel für die Funktionsweise von Integrationsszenarien verwendet werden.

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

## Erstellen eines Praxisszenarios

Die Aufgabe von [!DNL Adobe Workfront Fusion] besteht darin, Ihre Prozesse zu automatisieren, sodass Sie sich auf neue Aufgaben konzentrieren können, anstatt dieselben Aufgaben immer wieder zu wiederholen. Es funktioniert durch die Verknüpfung von Aktionen innerhalb und zwischen Apps und Diensten, um ein Szenario zu erstellen, in dem Ihre Daten automatisch übertragen und transformiert werden. Das Szenario, in dem Sie Watches für Daten in einer App oder einem Dienst erstellen und diese Daten verarbeiten, um das gewünschte Ergebnis zu liefern.

Ein Szenario besteht aus einer Reihe von Modulen, die angeben, wie Daten in einer App umgewandelt oder zwischen Apps und Webdiensten übertragen werden sollen.

Um zu erklären, wie Sie ein Szenario erstellen und die Best Practices während der Verwendung von [!DNL Workfront Fusion] verbessern können, führt Sie dieser Artikel Schritt für Schritt durch den Prozess. Wir erstellen ein Szenario, das einen neuen Datensatz in [!DNL Workfront] für jede Zeile in einer [!DNL Google Sheets] Tabelle erstellt.

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>Ein solches Szenario wäre nützlich, wenn Sie eine Tabelle mit Projekten haben, die in [!DNL Workfront] bearbeitet werden müssen. Das Szenario könnte das Arbeitsblatt für neue Zeilen &quot;ansehen&quot;und für jede Zeile ein neues Projekt in [!DNL Workfront] hinzufügen.

Das Erstellen eines Szenarios umfasst mehrere Hauptaufgaben:

## Wählen Sie die Apps aus und benennen Sie das Szenario

1. Laden Sie dieses [Arbeitsblatt ](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx) herunter und laden Sie es dann in Ihr [!DNL Google Drive] hoch, um es während dieser Übung zu verwenden.

   Oder

   Erstellen oder finden Sie eine eigene einfache [!DNL Google Sheets] -Tabelle, die dieser ähnelt:

   ![](assets/spreadsheet-headers-350x55.png)

1. Melden Sie sich bei Ihrem [!DNL Workfront Fusion] -Konto an.
1. Klicken Sie im linken Bereich auf **[!UICONTROL Szenarios]** ![](assets/scenarios-icon.png) .

   >[!NOTE]
   >
   >Wenn das linke Navigationsfenster oder dessen Symbole nicht angezeigt werden, klicken Sie auf das Menü-Symbol ![Menü](assets/main-menu-icon-left-nav.png) .

   Im grauen Bereich [!UICONTROL Ordner] können Sie Ihre Szenarien in Ordnern organisieren.

   Oben im Hauptbereich auf der rechten Seite können Sie die von Ihnen erstellten Szenarien **[!UICONTROL Alle]**, Ihre **[!UICONTROL aktiven Szenarien]** und **[!UICONTROL inaktiven Szenarien]** und Ihre **[!UICONTROL Konzepte]** anzeigen, bei denen es sich um Szenarien handelt, die noch etwas mehr Arbeit erfordern, bevor [!DNL Workfront Fusion] sie als aktiv oder inaktiv klassifizieren kann.

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. Klicken Sie im Bedienfeld [!UICONTROL Ordner] auf das Symbol **[!UICONTROL Ordner hinzufügen]** ![](assets/add-folder-icon.png) und geben Sie dann einen Namen wie &quot;Practice scenarios&quot;für Ihren ersten Ordner ein.

1. Öffnen Sie den Ordner und klicken Sie dann oben rechts auf der Seite auf **[!UICONTROL Neues Szenario erstellen]** .

   Die angezeigte Landingpage ermöglicht das Vorausfüllen aller Apps, die Sie in dem Szenario verwenden möchten, das Sie erstellen möchten.

1. Suchen Sie für diese Übung nach der App **[!UICONTROL Google Tabellen]** und wählen Sie sie aus.
1. Klicken Sie oben rechts auf **[!UICONTROL Weiter]** .

   Der Szenario-Editor wird angezeigt. Er enthält ein leeres Modul in der Mitte, die vorab geladene [!DNL Google Sheets]-App und einige Optionen in der Symbolleiste am unteren Rand.

<!--
   ![](assets/scenario-editor-350x235.png)
-->

Wenn Sie mit der Erstellung eines neuen Szenarios beginnen, ist es empfehlenswert, einen Namen dafür zu erstellen.

1. Wählen Sie oben links den Platzhalternamen **[!UICONTROL Neues Szenario]** aus und geben Sie dann einen Namen wie &quot;Praxisszenario 1&quot;ein.
1. Fahren Sie mit [Hinzufügen und Konfigurieren des ersten Moduls](#add-and-configure-the-first-module) weiter unten.

## Hinzufügen und Konfigurieren des ersten Moduls

Das leere Modul mit einem Fragezeichen stellt das Trigger-Modul dar, das Sie hinzufügen müssen. Dieses Modul startet das Szenario bei jeder Ausführung. Das Uhrsymbol auf dem leeren Modul zeigt an, dass es sich um ein geplantes Modul handelt.

![](assets/empty-module.png)

Dieses Modul enthält die Daten, die das Szenario überwachen soll.

1. Klicken Sie auf das leere Modul, um die App auszuwählen, aus der Sie ein Modul auswählen.

   Die zuvor vorab geladene App wird neben dem leeren Modul angezeigt. Sie können alle anderen Apps mit Modulen über das Feld [!UICONTROL Suche] hinzufügen.

   ![](assets/pre-loaded-apps-350x139.png)

1. Klicken Sie auf **[!DNL Google Sheets]**.

   Die Liste ändert sich, sodass alle [!DNL Google Sheets] -Module angezeigt werden, die Sie als Trigger-Modul verwenden können.

1. Klicken Sie auf das Trigger-Modul **[!UICONTROL Auf Datensätze achten]**.

   Nun müssen Sie eine authentifizierte Verbindung zu Ihrem Google-Konto herstellen. Jedes Modul, das Sie einem Szenario hinzufügen, muss eine Verbindung zu seiner App haben.

1. Klicken Sie im Feld &quot;**[!DNL Google Sheets]**&quot;unter &quot;**[!UICONTROL Verbindung]**&quot;auf &quot;**[!UICONTROL Hinzufügen]**&quot;, geben Sie einen Namen für die Verbindung ein, z. B. &quot;Olivas Google-Konto&quot;und klicken Sie dann auf &quot;**[!UICONTROL Weiter]**&quot;.
1. Authentifizieren Sie die Verbindung im angezeigten Fenster.

   Der Prozess zum Authentifizieren einer Verbindung kann zwischen Apps etwas variieren. Möglicherweise müssen Sie sich bei der App anmelden. Normalerweise müssen Sie auf eine Schaltfläche **[!UICONTROL Zulassen]** klicken. Wenn Sie Hilfe benötigen, finden Sie weitere Informationen unter [Übersicht über Verbindungen](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Konfigurieren des ersten Moduls

Nachdem Sie [!DNL Workfront Fusion] mit Ihrem [!DNL Google Sheets] -Konto verbunden haben, können Sie eine [!DNL Google Sheets] -Tabelle angeben, auf die Sie Zugriff haben, sowie die Daten dort, auf die das erste Modul verarbeitet werden soll.

1. Klicken Sie auf das Feld **[!UICONTROL Tabelle]** und wählen Sie dann in der angezeigten Liste die Tabelle **[!UICONTROL Workfront Fusion practice scenario] #1** aus.

   Diese Tabelle enthält 2 Tabellenblätter (Registerkarten). Daher müssen wir angeben, welches Blatt die gewünschten Daten enthält:

1. Wählen Sie in der Dropdownliste **[!UICONTROL Blatt]** die Option **[!UICONTROL Projekte]** aus.

   Unsere Tabelle enthält Kopfzeilen und wir möchten, dass das -Modul sie verwendet, um die Daten zu identifizieren, die wir verarbeiten möchten:

   ![](assets/spreadsheet-headers-350x55.png)

1. Lassen Sie **[!UICONTROL Ja]** für **[!UICONTROL Tabelle enthält Kopfzeilen]** ausgewählt.

1. Im Feld **[!UICONTROL Zeile mit Kopfzeilen]** können Sie einen Zeilenbereich angeben, den Sie einschließen möchten, aber lassen wir die standardmäßige A1:Z1 für diese Übung dort.
1. Geben Sie in das Feld **[!UICONTROL Limit]** den Wert &quot;1&quot;ein.

   Auf diese Weise verarbeitet das Modul jedes Mal, wenn Sie das Szenario ausführen, nur eine Zeile im Arbeitsblatt. Dies ist nützlich, um Ihre Testläufe während der Erstellung des Szenarios zu vereinfachen.

1. Klicken Sie auf **[!UICONTROL OK]**.

   Im Feld **[!UICONTROL Festlegen, wo das Modul gestartet werden soll]** werden Sie aufgefordert, anzugeben, wo im Arbeitsblatt das Modul mit der Verarbeitung beginnen soll.

1. Klicken Sie auf **[!UICONTROL Manuell auswählen]**, wählen Sie die obere Option in der angezeigten Liste aus und klicken Sie dann auf **[!UICONTROL OK]**.
1. Klicken Sie mit der rechten Maustaste auf das Modul, klicken Sie auf **[!UICONTROL Umbenennen]**, geben Sie einen Namen ein, der beschreibt, was das Modul tun soll (z. B. &quot;Liste des Projekts ansehen&quot;), und klicken Sie dann auf **[!UICONTROL OK]**.

   Der Name erscheint direkt unter dem Modul. Darunter enthält [!DNL Workfront Fusion] eine kurze Beschreibung der Art der Aktion, die vom Modul ausgeführt wird.

   ![](assets/module-renamed-350x388.png)

1. Fahren Sie mit [Hinzufügen und Konfigurieren des zweiten Moduls](#add-and-configure-the-second-module) fort.

## Zweites Modul hinzufügen und konfigurieren

1. Klicken Sie auf den Teilkreis rechts neben dem Modul, um **[!UICONTROL ein weiteres Modul hinzufügen]** hinzuzufügen.

   Dieses zweite Modul muss ein [!DNL Workfront] -Modul sein, aber wir haben die [!DNL Workfront] -App nicht vorab geladen.

1. Um die [!DNL Workfront] -App zu finden, geben Sie &quot;[!DNL Workfront]&quot;ein und klicken Sie auf die App, sobald sie angezeigt wird.
1. Klicken Sie in der angezeigten Liste der [!DNL Workfront] -Module auf **[!UICONTROL Datensatz erstellen]**.

1. Klicken Sie wie bei der Google Tabellen-App zuvor im Feld [!DNL Workfront] auf **[!UICONTROL Hinzufügen]** , um eine Verbindung zwischen Workfront Fusion und Workfront hinzuzufügen.

   Jetzt legen wir fest, was wir mit den Daten aus der Tabelle machen möchten.

1. Klicken Sie auf **[!UICONTROL Record type]** und wählen Sie dann **[!UICONTROL Project]** aus, da wir ein Projekt in [!DNL Workfront] mit einer Zeile aus dem Arbeitsblatt erstellen möchten.

   >[!TIP]
   >
   >Sie können **[!UICONTROL Projekt]** in der Liste finden, wenn Sie mit der Eingabe des Wortes &quot;[!UICONTROL Projekt]&quot;beginnen.

   Das Feld wird erweitert und zeigt alle verfügbaren [!DNL Workfront] -Projektfelder an, in denen Sie die vom ersten Modul gefundenen Informationen ablegen können.

   Wir werden das Feld **[!UICONTROL Name]** verwenden: Wir möchten, dass dieses Modul jedes Projekt in [!DNL Workfront] mit dem Text in der entsprechenden Zeile [!UICONTROL Google Tabellen] benennt.

1. Klicken Sie auf das Feld **[!UICONTROL Name]**.

   >[!TIP]
   >
   >Sie können **Befehl+F** ([!DNL Mac] BS) oder **Strg+F** ([!DNL Windows] OS) verwenden, um ein Feld schnell zu finden.

   Dadurch wird die Liste der Variablen geöffnet, die Sie im Feld **[!UICONTROL Name]** verwenden können, um den Namen für jedes in Workfront erstellte Projekt zu definieren.

   ![](assets/list-of-available-variables-350x261.png)

   Beachten Sie, dass die Variablen oben in der Liste den Spaltenüberschriften im Arbeitsblatt entsprechen.

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. Klicken Sie auf die Variable &quot;**[!UICONTROL Mein Projektname (A)]**&quot;, um sie dem Feld **[!UICONTROL Name]** hinzuzufügen.

   Sie haben gerade Ihr erstes Datenelement für dieses Szenario zugeordnet.

   Zuordnen eines weiteren Datenelements aus der Tabelle zu [!DNL Workfront]: Das Startdatum für jedes Projekt.

1. Klicken Sie auf das Feld **[!UICONTROL Geplantes Startdatum]** und dann auf die Variable **[!UICONTROL Geplantes Anfangsdatum (E)]** , um Daten aus dieser Spalte in der Tabelle abzurufen.

1. Klicken Sie auf **[!UICONTROL OK]**.

   Jetzt haben Sie ein funktionierendes Szenario.

1. Geben Sie dem zweiten Modul einen Namen wie &quot;Workfront-Projekt erstellen&quot;und fahren Sie dann mit [Testen des Szenarios](#test-the-scenario) fort.

## Testen des Szenarios

Bevor Sie Ihr Szenario aktivieren, müssen Sie es testen, indem Sie es mindestens einmal ausführen und die Ergebnisse anzeigen. Auf diese Weise können Sie erkennen, wie Daten durch das Szenario fließen und Fehler finden.

Es wurde ausgewählt, dass 1 Zeile aus der Tabelle verarbeitet werden soll, um ein Projekt in Workfront zu erstellen. Wenn Sie das Szenario ausführen, sollte dies geschehen.

1. Klicken Sie in der linken unteren Ecke des Szenario-Editors auf **[!UICONTROL Einmal ausführen]** .
1. Nachdem das Szenario abgeschlossen ist, klicken Sie auf die Blase über dem [!DNL Google Sheets] -Modul.

   ![](assets/click-bubble.png)

   In dem angezeigten Feld können Sie Informationen zum Datenbündel, das das Modul verarbeitet hat, anzeigen, einschließlich der tatsächlichen Daten, die für die Zeile, mit der Sie begonnen haben, aus der Tabelle abgerufen wurden.

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. Klicken Sie auf den Ausführungsinspektor oberhalb des Moduls [!DNL Workfront] , um die Eingabe der Informationen und die Ausgabe anzuzeigen, d. h. die Kennung des Projekts, das jetzt in [!DNL Workfront] erstellt wurde.

   ![](assets/execution-inspector-wf-350x384.png)

   Weitere Informationen zum Lesen von Informationen zur Ausführung von Szenarien finden Sie in den folgenden Artikeln:

   * Allgemeine Informationen finden Sie unter [Ausführungsfluss eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Informationen zu verarbeiteten Bundles finden Sie unter [Ausführung, Zyklen und Phasen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Navigieren Sie zu &quot;[!DNL Workfront]&quot;und suchen Sie nach &quot;soho downtown loft&quot;, um das Projekt zu sehen, das das Szenario erstellt hat. Dies war die letzte Zeile im Arbeitsblatt.
1. Klicken Sie in [!DNL Workfront Fusion] unten links auf **[!UICONTROL Speichern]** ![](assets/save-icon.png) , um den Fortschritt des Szenarios zu speichern.

   >[!IMPORTANT]
   >
   >Speichern Sie oft, während Sie ein Szenario testen.

## Fertigstellen des Szenarios und erneutes Testen

Wir müssen das Szenario weiterhin konfigurieren, um Projekte für alle anderen Zeilen im Arbeitsblatt zu erstellen.

1. Klicken Sie auf das Modul **[!UICONTROL Zeilen ansehen]** , das Sie für Google Tabellen erstellt haben.
1. Ändern Sie die **[!UICONTROL Beschränkung]** in 100.

   Wenn Sie eine Zahl festlegen, die höher ist als die Anzahl der Zeilen, von denen Sie wissen, dass sie sich im Arbeitsblatt befinden, wird sichergestellt, dass alle Zeilen im Szenario erfasst werden.

1. Klicken Sie mit der rechten Maustaste auf das Modul **[!UICONTROL Zeilen ansehen]**, klicken Sie auf **[!UICONTROL Legen Sie fest, wo]** gestartet werden soll, klicken Sie auf **[!UICONTROL Alle]** und klicken Sie dann auf **[!UICONTROL OK]**.

1. Klicken Sie auf **[!UICONTROL Einmal ausführen]** und beobachten Sie, was in den Ausführungsinspektor-Blasen passiert.

   Das Modul [!DNL Google] Tabellen **[!UICONTROL Zeilen ansehen]** wird einmal ausgeführt, um alle Zeilen zu lesen. Anschließend wird das Workfront-Modul **[!UICONTROL Datensatz erstellen]** 20-mal ausgeführt, um ein Projekt für jede der 20 verbleibenden Zeilen im Arbeitsblatt zu erstellen.

1. Klicken Sie auf die Blase im Ausführungsinspektor für das Modul &quot;[!DNL Workfront]&quot;, um alle 20 Vorgänge anzuzeigen, und klicken Sie dann auf einen der Vorgänge, um die Informationen zum erstellten Projekt anzuzeigen.
1. Klicken Sie unten links auf **[!UICONTROL Speichern]** ![](assets/save-icon.png).
1. Wechseln Sie zu &quot;[!DNL Workfront]&quot;, um die Projekte anzuzeigen, die das Szenario erstellt hat.

>[!TIP]
>
>Wir empfehlen die optionale, aber nützliche Vorgehensweise, Hinweise zu jedem Modul hinzuzufügen.
>
>1. Klicken Sie mit der rechten Maustaste auf das Modul [!DNL Workfront] und klicken Sie dann auf **[!UICONTROL Notiz hinzufügen]**.
>1. Geben Sie in die angezeigte Notiz eine Übersicht für das Modul ein.
>
>    Dies ist hilfreich, da Sie das Modul nicht ständig öffnen müssen, um zu sehen, was es tut. Sie können beispielsweise &quot;Erstellt ein Projekt mit dem Namen, dem geplanten Startdatum und der aus einer Tabelle zugeordneten Priorität&quot;eingeben.
>
>    Für das Modul [!UICONTROL Google Tabellen] können Sie beispielsweise &quot;Projektliste für hinzugefügte neue Zeilen/Projekte ansehen&quot;eingeben.
>
>    Sie können mehrere Notizen für ein Modul hinzufügen.
>
>1. Schließen Sie den Bereich **[!UICONTROL Notizen]** .
>
>    Nachdem Sie einem Szenario eine Notiz hinzugefügt haben, wird am unteren Rand des Szenario-Editors auf dem Symbol **[!UICONTROL Notizen]** ![](assets/notes-icon-w-dot.png) ein orangefarbener Punkt angezeigt.
>
>1. Klicken Sie auf das Symbol **[!UICONTROL Notizen]** ![](assets/notes-icon-w-dot.png), um Ihre Notizen anzuzeigen.
>



## Aktivieren des Szenarios

Wenn dies ein Szenario wäre, das Sie für echte Daten verwenden würden, würden Sie es als Letztes aktivieren. Nachdem Sie ein Szenario aktiviert haben, wird es standardmäßig alle 15 Minuten ausgeführt. Sie können dies ändern, indem Sie festlegen, wann und wie oft die Anwendung ausgeführt werden soll.

Weitere Informationen zum Aktivieren von Szenarien finden Sie unter [Aktivieren oder Deaktivieren eines Szenarios in Adobe Workfront Fusion](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Informationen zu Zeitplänen finden Sie unter [Planen eines Szenarios in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).
