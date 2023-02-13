---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Erstellen eines Szenarios für die Integration von Verfahren in Adobe Workfront Fusion
description: In diesem Artikel wird beschrieben, wie Sie ein Integrationsszenario mit Adobe Workfront Fusion erstellen. Integrationsszenarios verbinden separate Apps miteinander, sodass Ihre Daten durch verschiedene Anwendungen fließen können.
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '2076'
ht-degree: 0%

---

# Erstellen eines Szenarios für die Integration von Verfahren in Adobe Workfront Fusion

In diesem Artikel wird beschrieben, wie Sie ein Integrationsszenario mit Adobe Workfront Fusion erstellen. Integrationsszenarios verbinden separate Apps miteinander, sodass Ihre Daten durch verschiedene Anwendungen fließen können.

Um ein Integrationsszenario zu erstellen, muss Ihr Unternehmen über eine [!DNL Workfront Fusion for Work Automation and Integration] Lizenz.

Anweisungen zum Erstellen eines reinen Workfront-Automatisierungsszenarios finden Sie unter [Erstellen eines Szenarios für die Automatisierung von Verfahren in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

Weitere Informationen zu Workfront Fusion-Lizenzen finden Sie unter [Adobe Workfront Fusion-Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

>[!NOTE]
>
>Möglicherweise gestattet Ihr Unternehmen keinen Zugriff auf Google Tabellen. Ist dies der Fall, können Sie diese Integration nicht einrichten, aber die hier dargestellten Informationen können als allgemeines Beispiel für die Funktionsweise von Integrationsszenarien verwendet werden.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Erstellen eines Praxisszenarios

Die Rolle von [!DNL Adobe Workfront Fusion] ist es, Ihre Prozesse zu automatisieren, sodass Sie sich auf neue Aufgaben konzentrieren können, anstatt dieselben Aufgaben immer wieder zu wiederholen. Es funktioniert durch die Verknüpfung von Aktionen innerhalb und zwischen Apps und Diensten, um ein Szenario zu erstellen, in dem Ihre Daten automatisch übertragen und transformiert werden. Das Szenario, in dem Sie Watches für Daten in einer App oder einem Dienst erstellen und diese Daten verarbeiten, um das gewünschte Ergebnis zu liefern.

Ein Szenario besteht aus einer Reihe von Modulen, die angeben, wie Daten in einer App umgewandelt oder zwischen Apps und Webdiensten übertragen werden sollen.

So erklären Sie, wie Sie ein Szenario erstellen und Best Practices bei der Verwendung von [!DNL Workfront Fusion], führt Sie dieser Artikel Schritt für Schritt durch den Prozess. Wir erstellen ein Szenario, das einen neuen Datensatz in [!DNL Workfront] für jede Zeile in einer [!DNL Google Sheets] Tabelle.

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>Ein solches Szenario wäre nützlich, wenn Sie eine Tabelle mit Projekten haben, an denen gearbeitet werden muss, indem Sie Projekte in [!DNL Workfront]. Das Szenario könnte das Arbeitsblatt für neue Zeilen &quot;ansehen&quot;und ein neues Projekt in [!DNL Workfront] für jede einzelne.

Das Erstellen eines Szenarios umfasst mehrere Hauptaufgaben:

## Wählen Sie die Apps aus und benennen Sie das Szenario

1. Herunterladen [Tabellenblatt](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx)laden Sie es dann in Ihre [!DNL Google Drive] während dieser Übung verwendet werden.

   Oder

   Erstellen oder Suchen nach einer eigenen einfachen [!DNL Google Sheets] eine ähnliche Tabelle:

   ![](assets/spreadsheet-headers-350x55.png)

1. Melden Sie sich bei Ihrem [!DNL Workfront Fusion] -Konto.
1. Klicken **[!UICONTROL Szenarien]** ![](assets/scenarios-icon.png) im linken Bereich.

   Im linken Bereich, der angezeigt wird, können Sie Ihre Szenarien in Ordnern organisieren.

   Oben im Hauptbereich rechts können Sie **[!UICONTROL Alle]** Szenarien, die Sie erstellt haben, **[!UICONTROL Aktive Szenarien]** und **[!UICONTROL Inaktive Szenarien]** und **[!UICONTROL Konzepte]**, die Szenarien sind, in denen zuvor noch etwas mehr Arbeit erforderlich ist [!DNL Workfront Fusion] kann sie als aktiv oder inaktiv klassifizieren.

   ![](assets/scenarios-left-panel-350x215.png)

1. Klicken Sie im linken Bereich auf die **[!UICONTROL Ordner hinzufügen]** icon ![](assets/add-folder-icon.png)Geben Sie dann einen Namen wie &quot;Practice scenarios&quot;für Ihren ersten Ordner ein.

1. Öffnen Sie den Ordner und klicken Sie auf **[!UICONTROL Neues Szenario erstellen]** in der oberen rechten Ecke der Seite.

   Die angezeigte Landingpage ermöglicht das Vorausfüllen aller Apps, die Sie in dem Szenario verwenden möchten, das Sie erstellen möchten.

1. Suchen Sie für diese Übung nach und wählen Sie die **[!UICONTROL Google Tabellen]** App.
1. Klicken **[!UICONTROL Weiter]** in der oberen rechten Ecke.

   Der Szenario-Editor wird mit einem leeren Modul in der Mitte angezeigt. [!DNL Google Sheets] App, die Sie vorgeladen haben, und einige Optionen in der Symbolleiste am unteren Rand.

   ![](assets/scenario-editor-350x235.png)

   Wenn Sie mit der Erstellung eines neuen Szenarios beginnen, ist es empfehlenswert, einen Namen dafür zu erstellen.

1. Wählen Sie die **[!UICONTROL Neues Szenario]** Platzhaltername in der oberen linken Ecke und geben Sie dann einen Namen wie &quot;Practice scenario 1&quot;ein.
1. Fahren Sie mit [Hinzufügen und Konfigurieren des ersten Moduls](#add-and-configure-the-first-module) unten.

## Hinzufügen und Konfigurieren des ersten Moduls

Das leere Modul mit einem Fragezeichen stellt das Trigger-Modul dar, das Sie hinzufügen müssen. Dieses Modul startet das Szenario bei jeder Ausführung. Das Uhrsymbol auf dem leeren Modul zeigt an, dass es sich um ein geplantes Modul handelt.

![](assets/empty-module.png)

Dieses Modul enthält die Daten, die das Szenario überwachen soll.

1. Klicken Sie auf das leere Modul, um die App auszuwählen, aus der Sie ein Modul auswählen.

   Die zuvor vorab geladene App wird neben dem leeren Modul angezeigt. Sie können alle anderen Apps mit Modulen hinzufügen, indem Sie die [!UICONTROL Suche] ankreuzen.

   ![](assets/pre-loaded-apps-350x139.png)

1. Klicken **[!DNL Google Sheets]**.

   Die Liste ändert sich, sodass alle [!DNL Google Sheets] -Module, die Sie als Trigger-Modul verwenden können.

1. Klicken Sie auf das Trigger-Modul **[!UICONTROL Auf Aufzeichnungen achten]**.

   Nun müssen Sie eine authentifizierte Verbindung zu Ihrem Google-Konto herstellen. Jedes Modul, das Sie einem Szenario hinzufügen, muss eine Verbindung zu seiner App haben.

1. Im **[!DNL Google Sheets]** Feld, unter **[!UICONTROL Verbindung]** klicken **[!UICONTROL Hinzufügen]** Geben Sie dann einen Namen für die Verbindung ein, z. B. &quot;Google-Konto von Olivia&quot;und klicken Sie auf **[!UICONTROL Weiter]**.
1. Authentifizieren Sie die Verbindung im angezeigten Fenster.

   Der Prozess zum Authentifizieren einer Verbindung kann zwischen Apps etwas variieren. Möglicherweise müssen Sie sich bei der App anmelden. Normalerweise müssen Sie auf einen **[!UICONTROL Zulassen]** Schaltfläche. Wenn Sie Hilfe benötigen, lesen Sie [Über die Verbindung [!DNL Adobe Workfront Fusion] an eine App oder einen Dienst](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Konfigurieren des ersten Moduls

Nach der Verbindung [!DNL Workfront Fusion] auf [!DNL Google Sheets] -Konto, können Sie eine [!DNL Google Sheets] Tabelle, auf die Sie Zugriff haben, und die Daten dort, die das erste Modul verarbeiten soll.

1. Klicken Sie auf **[!UICONTROL Tabelle]** und wählen Sie dann die **[!UICONTROL Workfront Fusionspraktiken - Szenario] #1** in der Liste, die angezeigt wird.

   Diese Tabelle enthält 2 Tabellenblätter (Registerkarten). Daher müssen wir angeben, welches Blatt die gewünschten Daten enthält:

1. Im **[!UICONTROL Blatt]** Dropdown-Liste auswählen **[!UICONTROL Projekte]**.

   Unsere Tabelle enthält Kopfzeilen und wir möchten, dass das -Modul sie verwendet, um die Daten zu identifizieren, die wir verarbeiten möchten:

   ![](assets/spreadsheet-headers-350x55.png)

1. Urlaub **[!UICONTROL Ja]** ausgewählt für **[!UICONTROL Tabelle enthält Kopfzeilen]**.

1. Im **[!UICONTROL Zeile mit Kopfzeilen]** können Sie einen Zeilenbereich angeben, den Sie einbeziehen möchten, aber lassen Sie uns für diese Übung die standardmäßige A1:Z1-Zeile dort belassen.
1. Im **[!UICONTROL Limit]** Feld, Typ 1.

   Auf diese Weise verarbeitet das Modul jedes Mal, wenn Sie das Szenario ausführen, nur eine Zeile im Arbeitsblatt. Dies ist nützlich, um Ihre Testläufe während der Erstellung des Szenarios zu vereinfachen.

1. Klicken **[!UICONTROL OK]**.

   Die **[!UICONTROL Festlegen, wo der Start beginnen soll]** fordert Sie auf, anzugeben, wo im Arbeitsblatt das Modul mit der Verarbeitung beginnen soll.

1. Klicken **[!UICONTROL Manuell auswählen]**, wählen Sie die obere Option in der angezeigten Liste aus und klicken Sie auf **[!UICONTROL OK]**.
1. Klicken Sie mit der rechten Maustaste auf das Modul und klicken Sie auf **[!UICONTROL Umbenennen]** Geben Sie dann einen Namen ein, den beschreibt, was das Modul tun soll (z. B. &quot;Projektliste ansehen&quot;), und klicken Sie dann auf **[!UICONTROL OK]**.

   Der Name erscheint direkt unter dem Modul. darunter: [!DNL Workfront Fusion] enthält eine kurze Beschreibung der Art der Aktion, die vom Modul ausgeführt wird.

   ![](assets/module-renamed-350x388.png)

1. Fahren Sie mit [Zweites Modul hinzufügen und konfigurieren](#add-and-configure-the-second-module).

## Zweites Modul hinzufügen und konfigurieren

1. Klicken Sie auf den Teilkreis rechts neben dem des Moduls, um **[!UICONTROL Hinzufügen eines weiteren Moduls]**.

   Dieses zweite Modul muss ein [!DNL Workfront] -Modul, aber wir haben die [!DNL Workfront] App.

1. So suchen Sie die [!DNL Workfront] App, beginnen Sie mit der Eingabe von &quot;[!DNL Workfront]und klicken Sie auf die App, sobald sie angezeigt wird.
1. In der Liste der [!DNL Workfront] angezeigte Module, klicken Sie auf **[!UICONTROL Datensatz erstellen]**.

1. Klicken Sie wie bei der Google Tabellen-App auf **[!UICONTROL Hinzufügen]** im [!DNL Workfront] zum Hinzufügen einer Verbindung zwischen Workfront Fusion und Workfront.

   Jetzt legen wir fest, was wir mit den Daten aus der Tabelle machen möchten.

1. Klicken **[!UICONTROL Record Type]**, wählen Sie **[!UICONTROL Projekt]** weil wir ein Projekt in [!DNL Workfront] Verwendung einer Zeile aus der Tabelle.

   >[!TIP]
   >
   >Sie finden **[!UICONTROL Projekt]** in der Liste, wenn Sie beginnen, das Wort &quot;[!UICONTROL Projekt].&quot;

   Das Feld wird erweitert und zeigt alle verfügbaren [!DNL Workfront] Projektfelder, in denen Sie die vom ersten Modul gefundenen Informationen ablegen können.

   Wir werden die **[!UICONTROL Name]** -Feld: Wir möchten, dass dieses Modul jedes Projekt in [!DNL Workfront] mit dem Text im entsprechenden [!UICONTROL Google Tabellen] Zeile.

1. Suchen und klicken Sie auf **[!UICONTROL Name]** -Feld.

   >[!TIP]
   >
   >Sie können **Befehl+F** ([!DNL Mac] OS) oder **Strg+F**([!DNL Windows] OS), um ein Feld schnell zu finden.

   Dadurch wird die Liste der Variablen geöffnet, die Sie in der Variablen **[!UICONTROL Name]** -Feld, um den Namen für jedes in Workfront erstellte Projekt zu definieren.

   ![](assets/list-of-available-variables-350x261.png)

   Beachten Sie, dass die Variablen oben in der Liste den Spaltenüberschriften im Arbeitsblatt entsprechen.

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. Klicken Sie auf die Variable **[!UICONTROL Mein Projektname (A)]** , um ihn zum **[!UICONTROL Name]** -Feld.

   Sie haben gerade Ihr erstes Datenelement für dieses Szenario zugeordnet.

   Zuordnen eines weiteren Datenelements aus der Tabelle zu [!DNL Workfront]: das Startdatum für jedes Projekt.

1. Suchen und klicken Sie auf **[!UICONTROL Geplantes Startdatum]** und klicken Sie auf das **[!UICONTROL Geplantes Anfangsdatum (E)]** , um Daten aus dieser Spalte in der Tabelle abzurufen.

1. Klicken **[!UICONTROL OK]**.

   Jetzt haben Sie ein funktionierendes Szenario.

1. Geben Sie dem zweiten Modul einen Namen wie &quot;Workfront-Projekt erstellen&quot;und fahren Sie dann mit [Testen des Szenarios](#test-the-scenario).

## Testen des Szenarios

Bevor Sie Ihr Szenario aktivieren, müssen Sie es testen, indem Sie es mindestens einmal ausführen und die Ergebnisse anzeigen. Auf diese Weise können Sie erkennen, wie Daten durch das Szenario fließen und Fehler finden.

Es wurde ausgewählt, dass 1 Zeile aus dem Arbeitsblatt verarbeitet werden soll, um ein Projekt in Workfront zu erstellen. Wenn Sie das Szenario ausführen, sollte dies geschehen.

1. Klicken **[!UICONTROL Einmal ausführen]** in der linken unteren Ecke des Szenario-Editors.
1. Nachdem das Szenario abgeschlossen ist, klicken Sie auf die Blase über dem [!DNL Google Sheets] -Modul.

   ![](assets/click-bubble.png)

   In dem angezeigten Feld können Sie Informationen zum Datenbündel, das das Modul verarbeitet hat, anzeigen, einschließlich der tatsächlichen Daten, die für die Zeile, mit der Sie begonnen haben, aus der Tabelle abgerufen wurden.

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. Klicken Sie auf den Ausführungsinspektor oberhalb der [!DNL Workfront] -Modul, um die Eingabe von Informationen und die Ausgabe zu sehen, was die Kennung des Projekts ist, das jetzt in erstellt wird. [!DNL Workfront]

   ![](assets/execution-inspector-wf-350x384.png)

   Weitere Informationen zum Lesen von Informationen zur Ausführung von Szenarien finden Sie in den folgenden Artikeln:

   * Allgemeine Informationen finden Sie unter [Ausführungsfluss des Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Weitere Informationen zu verarbeiteten Bundles finden Sie unter [Ausführung des Szenarios, Zyklen und Phasen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Navigieren Sie zu [!DNL Workfront] und suchen Sie nach &quot;soho downtown loft&quot;, um das Projekt zu sehen, das das Szenario erstellt hat. Dies war die letzte Zeile im Arbeitsblatt.
1. In [!DNL Workfront Fusion]klicken **[!UICONTROL Speichern]** ![](assets/save-icon.png) in der Nähe der linken unteren Ecke, um den Fortschritt des Szenarios zu speichern.

   >[!IMPORTANT]
   >
   >Speichern Sie oft, während Sie ein Szenario testen.

## Fertigstellen des Szenarios und erneutes Testen

Wir müssen das Szenario weiterhin konfigurieren, um Projekte für alle anderen Zeilen im Arbeitsblatt zu erstellen.

1. Klicken Sie auf **[!UICONTROL Zeilen ansehen]** -Modul, das Sie für Google Tabellen erstellt haben.
1. Ändern Sie die **[!UICONTROL Limit]** auf 100.

   Wenn Sie eine Zahl angeben, die höher ist als die Anzahl der Zeilen, von denen Sie wissen, dass sie sich im Arbeitsblatt befinden, wird sichergestellt, dass alle Zeilen im Szenario erfasst werden.

1. Klicken Sie mit der rechten Maustaste auf die **[!UICONTROL Zeilen ansehen]** Modul, klicken Sie auf **[!UICONTROL Festlegen, wo der Start beginnen soll]** klicken **[!UICONTROL Alle]** Klicken Sie auf **[!UICONTROL OK]**.

1. Klicken **[!UICONTROL Einmal ausführen]** und beobachten, was in den Ausführungsblasen geschieht.

   Die [!DNL Google] Blätter **[!UICONTROL Zeilen ansehen]** -Modul wird einmal ausgeführt, um alle Zeilen zu lesen. Dann die Workfront **[!UICONTROL Datensatz erstellen]** 20-mal ausgeführt, um ein Projekt für jede der 20 verbleibenden Zeilen im Arbeitsblatt zu erstellen.

1. Klicken Sie auf den Ausführungsinspektor für die [!DNL Workfront] -Modul, um alle 20 Vorgänge anzuzeigen, und klicken Sie dann auf einen der Vorgänge, um die Informationen zum erstellten Projekt anzuzeigen.
1. Klicken **[!UICONTROL Speichern]** ![](assets/save-icon.png) in der Nähe der unteren linken Ecke.
1. Navigieren Sie zu [!DNL Workfront] , um die vom Szenario erstellten Projekte anzuzeigen.

>[!TIP]
>
>Wir empfehlen die optionale, aber nützliche Vorgehensweise, Hinweise zu jedem Modul hinzuzufügen.
>
>1. Klicken Sie mit der rechten Maustaste auf die [!DNL Workfront] Modul, und klicken Sie dann auf **[!UICONTROL Notiz hinzufügen]**.
>1. Geben Sie in die angezeigte Notiz eine Übersicht für das Modul ein.

>
>   Dies ist hilfreich, da Sie das Modul nicht ständig öffnen müssen, um zu sehen, was es tut. Sie können beispielsweise &quot;Erstellt ein Projekt mit dem Namen, dem geplanten Startdatum und der aus einer Tabelle zugeordneten Priorität&quot;eingeben.
>
>   Für [!UICONTROL Google Tabellen] -Modul können Sie beispielsweise &quot;Projektliste für neue hinzugefügte Zeilen/Projekte ansehen&quot;eingeben.
>
>   Sie können mehrere Notizen für ein Modul hinzufügen.
>
>1. Schließen Sie die **[!UICONTROL Hinweise]** Bereich.
>
>   Nachdem Sie einem Szenario eine Notiz hinzugefügt haben, wird auf der Seite **[!UICONTROL Hinweise]** icon ![](assets/notes-icon-w-dot.png) unten im Szenario-Editor.
>
>1. Klicken Sie auf **[!UICONTROL Hinweise]** icon ![](assets/notes-icon-w-dot.png) um Ihre Notizen anzuzeigen.

>




## Aktivieren des Szenarios

Wenn dies ein Szenario wäre, das Sie für echte Daten verwenden würden, würden Sie es als Letztes aktivieren. Nachdem Sie ein Szenario aktiviert haben, wird es standardmäßig alle 15 Minuten ausgeführt. Sie können dies ändern, indem Sie festlegen, wann und wie oft die Anwendung ausgeführt werden soll.

Weitere Informationen zum Aktivieren von Szenarien finden Sie unter [Aktivieren oder Deaktivieren eines Szenarios in Adobe Workfront Fusion](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Weitere Informationen zu Zeitplänen finden Sie unter [Planen eines Szenarios in Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md).
