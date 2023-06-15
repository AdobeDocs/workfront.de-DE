---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Erstellen Sie ein Automatisierungsszenario für Vorgehensweisen in [!DNL Adobe Workfront Fusion]
description: In diesem Artikel wird beschrieben, wie Sie mit Adobe Workfront Fusion ein Automatisierungsszenario erstellen. Automatisierungsszenarien automatisieren Workfront-Prozesse, einschließlich Datenmanipulationen und -umwandlungen. Dieses Beispiel führt Sie durch die Erstellung eines Szenarios, in dem nach einem Projekt gesucht wird, und gibt dann alle mit diesem Projekt verknüpften Aufgaben zurück.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 99a8ad82c5fb2fb3f6adce9ff037086523be9b02
workflow-type: tm+mt
source-wordcount: '1800'
ht-degree: 0%

---

# Erstellen Sie ein Automatisierungsszenario für Vorgehensweisen in [!DNL Adobe Workfront Fusion]

In diesem Artikel wird beschrieben, wie Sie mit Adobe Workfront Fusion ein Automatisierungsszenario erstellen. Automatisierungsszenarien automatisieren Workfront-Prozesse, einschließlich Datenmanipulationen und -umwandlungen. Dieses Beispiel führt Sie durch die Erstellung eines Szenarios, in dem nach einem Projekt gesucht wird, und gibt dann alle mit diesem Projekt verknüpften Aufgaben zurück.

Anweisungen zum Erstellen eines Integrationsszenarios, das separate Apps verbindet, finden Sie unter [Erstellen eines Szenarios für die Integration von Verfahren in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

Weitere Informationen zu den für jede Workfront Fusion-Lizenz verfügbaren Funktionen finden Sie unter [Adobe Workfront Fusion-Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>  </td> 
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
In diesem Beispiel werden Sie durch die Erstellung eines Szenarios geführt, in dem nach einem [!DNL Workfront] und gibt die Aufgaben im Projekt zurück.

![](assets/create-practice-scenario-wf-only-350x157.png)

Das Erstellen eines Szenarios umfasst mehrere Hauptaufgaben:

## Wählen Sie die Apps aus und benennen Sie das Szenario

1. Melden Sie sich bei Ihrem [!DNL Workfront Fusion] -Konto.
1. Klicken **[!UICONTROL Szenarien]** ![](assets/scenarios-icon.png) im linken Bereich.

   >[!NOTE]
   >
   >Wenn das linke Navigationsfenster oder dessen Symbole nicht angezeigt werden, klicken Sie auf das Menü ![Menü](assets/main-menu-icon-left-nav.png) Symbol.

   In grau [!UICONTROL Ordner] angezeigt werden, können Sie Ihre Szenarien in Ordnern organisieren.

   Oben im Hauptbereich rechts können Sie **[!UICONTROL Alle]** Szenarien, die Sie erstellt haben, **[!UICONTROL Aktive Szenarien]**, **[!UICONTROL Inaktive Szenarien]** und **[!UICONTROL Konzepte]**. Konzepte sind Szenarien, in denen zuvor noch etwas mehr Arbeit benötigt wird [!DNL Workfront Fusion] kann sie als aktiv oder inaktiv klassifizieren.

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. Im [!UICONTROL Ordner] auf **[!UICONTROL Ordner hinzufügen]** icon ![](assets/add-folder-icon.png)Geben Sie dann einen Namen wie &quot;Practice scenarios&quot;für Ihren ersten Ordner ein.

1. Öffnen Sie den Ordner und klicken Sie auf **[!UICONTROL Neues Szenario erstellen]** in der oberen rechten Ecke der Seite.

   Die angezeigte Landingpage ermöglicht das Vorausfüllen aller Apps, die Sie in dem Szenario verwenden möchten, das Sie erstellen möchten.

1. Suchen Sie für diese Übung nach und wählen Sie die **[!DNL Workfront]** App.
1. Klicken **[!UICONTROL Weiter]** in der oberen rechten Ecke.

   Der Szenario-Editor wird mit einem leeren Modul in der Mitte angezeigt. [!DNL Workfront] App, die Sie vorgeladen haben, und einige Optionen in der Symbolleiste am unteren Rand.

<!--
   ![](assets/scenario-editor-350x235.png)
-->

Wenn Sie mit der Erstellung eines neuen Szenarios beginnen, ist es empfehlenswert, einen Namen dafür zu erstellen.

1. Wählen Sie die **[!UICONTROL Neues Szenario]** Platzhaltername in der oberen linken Ecke und geben Sie dann einen Namen wie &quot;Practice scenario 1&quot;ein.
1. Fahren Sie mit [Hinzufügen und Konfigurieren des ersten Moduls](#add-and-configure-the-first-module) unten.

## Hinzufügen und Konfigurieren des ersten Moduls

Das leere Modul mit einem Fragezeichen stellt das Trigger-Modul dar, das Sie hinzufügen müssen. Dieses Modul startet das Szenario bei jeder Ausführung. Das Uhrsymbol auf dem leeren Modul zeigt an, dass es sich um ein geplantes Modul handelt.

![](assets/empty-module.png)

Dieses Modul enthält die Daten, die das Szenario überwachen soll.

Für dieses Beispiel verwenden wir kein Trigger-Modul. Stattdessen beginnt dieses Szenario mit einer Suche.

1. Klicken Sie auf das leere Modul, um die App auszuwählen, aus der Sie ein Modul auswählen.

   Die zuvor vorab geladene App wird neben dem leeren Modul angezeigt. Sie können alle anderen Apps mit Modulen hinzufügen, indem Sie die [!UICONTROL Suche] ankreuzen.

   ![](assets/pre-loaded-app-wf-350x172.png)

1. Klicken **[!DNL Workfront]**.

   Die Liste ändert sich, sodass alle [!DNL Workfront] -Module, die Sie als Trigger-Modul verwenden können.

1. Klicken Sie auf das Suchmodul **[!UICONTROL Suche]**.

   Jetzt müssen Sie eine authentifizierte Verbindung zu Ihrem [!DNL Workfront] -Konto. Jedes Modul, das Sie einem Szenario hinzufügen, muss eine Verbindung zu seiner App haben.

1. Im **[!DNL Workfront]** Feld, unter **[!UICONTROL Verbindung]** klicken **[!UICONTROL Hinzufügen]** Geben Sie dann einen Namen für die Verbindung ein, z. B. &quot;Workfront-Konto von Olivia&quot;und klicken Sie auf **[!UICONTROL Weiter]**.
1. Authentifizieren Sie die Verbindung im angezeigten Fenster.

   Der Prozess zum Authentifizieren einer Verbindung kann zwischen Apps etwas variieren. Der folgende Prozess ist spezifisch für [!DNL Workfront], aber der Prozess ähnelt vielen Apps.

   1. Geben Sie Ihre [!DNL Workfront] Domäne und klicken Sie auf **[!UICONTROL Weiter]**.
   1. Anmelden [!DNL Workfront].
   1. Untersuchen Sie den Zugriff, der [!DNL Workfront Fusion] fordert an und klicken Sie dann auf **[!UICONTROL Zugriff erlauben]**.

   Wenn Sie Hilfe benötigen, lesen Sie [Über die Verbindung [!DNL Adobe Workfront Fusion] an eine App oder einen Dienst](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## Konfigurieren des ersten Moduls

Nach der Verbindung [!DNL Workfront Fusion] auf [!DNL Workfront] -Konto, können Sie eine [!DNL Workfront] Anforderungswarteschlange, auf die Sie Zugriff haben, und die Daten dort, die das erste Modul verarbeiten soll.

1. Im [!UICONTROL Record Type] auswählen **[!UICONTROL Projekt]**. Dadurch wird das Modul so eingestellt, dass nur Projekte durchsucht werden.

   >[!TIP]
   >
   >Sie finden **[!UICONTROL Projekt]** in der Liste, wenn Sie beginnen, das Wort &quot;[!UICONTROL Projekt].&quot;

1. Im **[!UICONTROL Ergebnissatz]** auswählen **[!UICONTROL Erster übereinstimmender Datensatz]**. Dadurch wird das -Modul so eingestellt, dass nur der erste Datensatz zurückgegeben wird, der nach seiner Auswahl die Kriterien erfüllt. Für dieses Beispiel benötigen wir nur einen Datensatz.
1. Im **[!UICONTROL Suchkriterien]** -Bereich, richten wir einen Filter ein, um das spezifische Projekt zurückzugeben.

   1. Im ersten Feld unter [!UICONTROL Suchkriterien]wählen Sie das Feld aus, nach dem Sie die Werte suchen möchten. Wählen Sie für dieses Beispiel **[!UICONTROL Name]**.
   1. Wählen Sie für den Operator [!UICONTROL Enthält (nicht von Schreibweise abhängig)]. Dadurch kann das Modul Projekte mit dem Namen Ihrer ausgewählten Wörter finden, selbst wenn Sie nicht den gesamten Namen eingeben oder den Namen mit der falschen Groß-/Kleinschreibung eingeben (z. B. alle Großbuchstaben).
   1. Im letzten Feld unter [!UICONTROL Suchkriterien]ein Wort oder einen Satz eingeben, von dem Sie wissen, dass es sich um einen Begriff im Namen des Projekts handelt, nach dem Sie suchen.

1. Im **[!UICONTROL Ausgaben]** Liste die Felder aus, die das Problem ausgeben soll. Wählen Sie für dieses Beispiel die **[!UICONTROL ID]** und **[!UICONTROL Name]** -Felder.

   >[!TIP]
   >
   >Sie können **Befehl+F** ([!DNL Mac] OS) oder **Strg+F** ([!DNL Windows] OS), um ein Feld schnell zu finden.

1. Klicken **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >(Nur Informationen) Da es sich nicht um ein Trigger-Modul handelt, wählen Sie nicht, wo es gestartet werden soll. Bei Verwendung eines Trigger-Moduls würden Sie jetzt auswählen, wo es gestartet werden soll.
   >
   >
   >Weitere Informationen finden Sie unter [Festlegen, wo ein Trigger-Modul beginnt [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. Klicken Sie mit der rechten Maustaste auf das Modul und klicken Sie auf **[!UICONTROL Umbenennen]** Geben Sie einen Namen ein, der beschreibt, was das Modul tun soll (z. B. &quot;Suche nach Projekt&quot;), und klicken Sie dann auf **[!UICONTROL OK]**.

   Der Name erscheint direkt unter dem Modul. darunter: [!DNL Workfront Fusion] enthält eine kurze Beschreibung der Art der Aktion, die vom Modul ausgeführt wird.

   ![](assets/module-renamed-wf.png)

1. Fahren Sie mit [Zweites Modul hinzufügen und konfigurieren](#add-and-configure-the-second-module).

## Zweites Modul hinzufügen und konfigurieren

1. Klicken Sie auf den Teilkreis rechts neben dem des Moduls, um **[!UICONTROL Hinzufügen eines weiteren Moduls]**.
1. Auswählen [!DNL Workfront] Wählen Sie aus der Liste der Anwendungen das Suchmodul aus. **[!UICONTROL Verwandte Aufzeichnungen lesen]**.
1. Sie haben bereits eine Verbindung zu [!DNL Workfront] für das vorherige Modul. Sie müssen es hier nicht erneut erstellen, aber Sie müssen sicherstellen, dass dieses Modul dieselbe Verbindung wie das vorherige Modul verwendet.\
   Im **[!UICONTROL Verbindung]** auswählen, wählen Sie die Verbindung aus, die Sie für das vorherige Modul erstellt haben.
1. Klicken **[!UICONTROL Record Type]**, wählen Sie **[!UICONTROL Projekt]**, da wir Datensätze lesen möchten, die sich auf ein Projekt beziehen.

   >[!TIP]
   >
   >Sie finden **[!UICONTROL Projekt]** in der Liste, wenn Sie beginnen, das Wort &quot;Projekt&quot;einzugeben.

1. Klicken Sie auf **[!UICONTROL Übergeordnete Datensatz-ID]** -Feld. Für dieses Feld ist die Workfront ID des Projekts erforderlich, aus dem Sie Aufgaben zurückgeben möchten.

   Durch Klicken auf das Feld wird die Liste der Variablen geöffnet, die Sie im **[!UICONTROL Übergeordnete Datensatz-ID]** -Feld, um das Projekt in Workfront zu identifizieren.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Klicken Sie auf die Variable **[!UICONTROL ID]** , um ihn zum **[!UICONTROL Übergeordnete Datensatz-ID]** -Feld. Dadurch kann die vom ersten Modul zurückgegebene ID als Kennung für das Projekt verwendet werden, mit dem Sie im zweiten Modul arbeiten möchten. Dadurch wird sichergestellt, dass die zurückgegebenen Aufgaben zu diesem Projekt gehören.
1. Im **[!UICONTROL Sammlungen]** Feld, wählen Sie **[!UICONTROL Aufgaben]**. Dies bedeutet, dass das Modul Aufgaben zurückgibt, die mit dem ausgewählten Projekt verknüpft sind.
1. Klicken **[!UICONTROL OK]**

   Jetzt haben Sie ein funktionierendes Szenario.

1. Geben Sie dem zweiten Modul einen Namen wie &quot;Aufgaben zurückgeben, die mit dem Projekt verknüpft sind&quot;und fahren Sie dann mit [Testen des Szenarios](#test-the-scenario).

## Testen des Szenarios

Bevor Sie Ihr Szenario aktivieren, müssen Sie es testen, indem Sie es mindestens einmal ausführen und die Ergebnisse anzeigen. Auf diese Weise können Sie erkennen, wie Daten durch das Szenario fließen und Fehler finden.

Wir haben ausgewählt, dass 1 Projekt zurückgegeben werden soll und die mit diesem Projekt verbundenen Aufgaben. Wenn Sie das Szenario ausführen, sollte dies geschehen.

1. Klicken **[!UICONTROL Einmal ausführen]** in der linken unteren Ecke des Szenario-Editors.
1. Nachdem das Szenario abgeschlossen ist, klicken Sie auf die Blase über dem ersten Modul.

   ![](assets/click-bubble.png)

   In dem angezeigten Feld können Sie Informationen zum Datenbündel, das das Modul verarbeitet hat, anzeigen, einschließlich der tatsächlichen Daten, die aus dem vom Modul zurückgegebenen Projekt abgerufen wurden.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. Klicken Sie auf die Blase über dem zweiten Modul, um die Eingabe der Informationen und die Ausgabe anzuzeigen, bei der es sich um eine Sammlung von Aufgaben im Projekt handelt.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   Weitere Informationen zum Lesen von Informationen zur Ausführung von Szenarien finden Sie in den folgenden Artikeln:

   * Allgemeine Informationen finden Sie unter [Ausführungsfluss des Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Weitere Informationen zu verarbeiteten Bundles finden Sie unter [Ausführung des Szenarios, Zyklen und Phasen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. In [!DNL Workfront Fusion]klicken **[!UICONTROL Speichern]** ![](assets/save-icon.png) in der Nähe der linken unteren Ecke, um den Fortschritt des Szenarios zu speichern.

   >[!IMPORTANT]
   >
   >Speichern Sie oft, während Sie ein Szenario testen.

>[!TIP]
>
>Wir empfehlen die optionale, aber nützliche Vorgehensweise, Hinweise zu jedem Modul hinzuzufügen.
>
>1. Rechtsklick auf einen [!DNL Workfront] Modul, und klicken Sie dann auf **[!UICONTROL Notiz hinzufügen]**.
>1. Geben Sie in die angezeigte Notiz eine Übersicht für das Modul ein.
>
>    Sie können mehrere Notizen für ein Modul hinzufügen.
>
>1. Schließen Sie die **[!UICONTROL Hinweise]** Bereich.
>
>     Nachdem Sie einem Szenario eine Notiz hinzugefügt haben, wird auf der Seite **[!UICONTROL Hinweise]** icon ![](assets/notes-icon-w-dot.png) unten im Szenario-Editor.
>
>1. Klicken Sie auf **[!UICONTROL Hinweise]** icon ![](assets/notes-icon-w-dot.png) um Ihre Notizen anzuzeigen.
>



## Aktivieren des Szenarios

In diesem Beispielszenario gibt es kein Trigger-Modul. Wenn dies ein Szenario wäre, das Sie für echte Daten verwenden würden, würde es mit einem Trigger-Modul beginnen und das Letzte, was Sie tun würden, ist es zu aktivieren. Nachdem Sie ein Szenario aktiviert haben, wird es standardmäßig alle 15 Minuten ausgeführt. Sie können dies ändern, indem Sie festlegen, wann und wie oft die Anwendung ausgeführt werden soll.

Weitere Informationen zum Aktivieren von Szenarien finden Sie unter [Aktivieren oder deaktivieren Sie ein Szenario in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Weitere Informationen zu Zeitplänen finden Sie unter [Planen eines Szenarios in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
