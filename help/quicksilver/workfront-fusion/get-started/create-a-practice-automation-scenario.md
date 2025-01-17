---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Erstellen Sie ein Automatisierungsszenario in [!DNL Adobe Workfront Fusion]
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1562'
ht-degree: 0%

---

# Erstellen eines Praxisautomatisierungsszenarios in [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Workflow zum Erstellen eines Szenarios](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/plan-a-scenario/create-a-scenario-workflow.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

Automatisierungsszenarien automatisieren Workfront-Prozesse, einschließlich Datenmanipulationen und -umwandlungen. Dieser Artikel führt Sie durch den Prozess der Erstellung eines Szenarios, das nach einem Projekt sucht und dann alle mit diesem Projekt verbundenen Aufgaben zurückgibt.

<!-- not sure why these are here?
For instructions on building an integration scenario that connects separate apps, see [Create a practice integration scenario in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

For more information on functionality available with each Workfront Fusion license, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

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

## Erstellen eines Automatisierungsszenarios

[!DNL Adobe Workfront Fusion] können Sie sich auf wichtige Aufgaben konzentrieren, indem Sie sich wiederholende Aufgaben automatisieren. Es werden Szenarien erstellt, in denen Ihre Daten automatisch über verschiedene Apps und Services hinweg verwaltet werden.

Jedes Szenario besteht aus Modulen, die steuern, wie Daten innerhalb einer App verarbeitet oder zwischen verschiedenen Apps und Services übertragen werden. Sie können beispielsweise ein Szenario in Fusion erstellen, um automatisch ein [!DNL Workfront] Projekt zu finden und dessen Aufgaben aufzulisten. Auf diese Weise spart Fusion Ihnen Zeit und Mühe bei der Durchführung von Routineaufgaben.

Dieses Übungsszenario führt Sie durch den Prozess der Erstellung eines Szenarios, das nach einem [!DNL Workfront] Projekt sucht und die Aufgaben im Projekt zurückgibt.

![](assets/create-practice-scenario-wf-only-350x157.png)

### Bevor Sie beginnen

Erstellen Sie ein Projekt mit Aufgaben in Workfront, die Sie für diese Übung verwenden können. Außer dem Hinzufügen von Aufgaben zum Projekt müssen Sie keine weiteren Konfigurationen vornehmen.

Informationen zum Erstellen eines Projekts in Workfront finden Sie unter xxx.

### 1. Szenario erstellen und benennen

1. Melden Sie sich bei Ihrem [!DNL Workfront Fusion] Konto an.
1. Klicken Sie **[!UICONTROL linken Bedienfeld]** Szenarios![](assets/scenarios-icon.png).

   >[!NOTE]
   >
   >Wenn der linke Navigationsbereich oder dessen Symbole nicht angezeigt werden, klicken Sie auf das Symbol Menü ![Menü](assets/main-menu-icon-left-nav.png) .

1. Klicken Sie im [!UICONTROL **Ordner**]-Bedienfeld auf das Symbol **[!UICONTROL Ordner hinzufügen]** ![](assets/add-folder-icon.png) und geben Sie dann einen Namen wie „Übungsszenarien“ für Ihren ersten Ordner ein.

1. Öffnen Sie den Ordner und klicken Sie **[!UICONTROL oben]** auf der Seite auf „Neues Szenario erstellen“.

1. Wählen Sie für diese Übung die **[!DNL Adobe Workfront]** App aus und klicken Sie dann unten **Suchen**.


1. Wählen Sie **[!UICONTROL Platzhalternamen]** Neues Szenario“ in der oberen linken Ecke aus und geben Sie dann einen Namen ein, z. B. „Übungsszenario 1“.

   ![](assets/name-the-scenario.png)

1. Fahren Sie mit [Verbinden des ersten Moduls](#2-connect-the-first-module) unten fort.

### 2. Erstes Modul anschließen

Jetzt müssen Sie eine authentifizierte Verbindung zu Ihrem [!DNL Workfront]-Konto herstellen. Jedes Modul, das Sie einem Szenario hinzufügen, muss über eine Verbindung zu seiner App verfügen.

1. Klicken Sie im **[!DNL Workfront]** unter **[!UICONTROL Verbindung]** auf **[!UICONTROL Hinzufügen]**, geben Sie dann einen Namen für die Verbindung ein, z. B. „Olivias Workfront-Konto“, und klicken Sie dann auf **[!UICONTROL Weiter]**.
1. Authentifizieren Sie die Verbindung im angezeigten Fenster.

   Der Prozess zum Authentifizieren einer Verbindung kann zwischen Apps etwas variieren. Der folgende Prozess ist spezifisch für [!DNL Workfront], ähnelt jedoch vielen anderen Apps:

   1. Geben Sie Ihre [!DNL Workfront] Domain ein und klicken Sie dann auf **[!UICONTROL Weiter]**.
   1. Anmelden bei [!DNL Workfront].
   1. Überprüfen Sie den von [!DNL Workfront Fusion] angeforderten Zugriff und klicken Sie dann auf **[!UICONTROL Zugriff zulassen]**.

   Wenn Sie Hilfe benötigen, lesen Sie [Verbindungen - Übersicht](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

### 3. Konfigurieren des ersten Moduls

Nachdem Sie [!DNL Workfront Fusion] mit Ihrem [!DNL Workfront]-Konto verbunden haben, können Sie ein [!DNL Workfront]-Projekt, auf das Sie Zugriff haben, und die Daten angeben, die das erste Modul verarbeiten soll.

1. Wählen [!UICONTROL  im Feld „Datensatztyp] die Option **[!UICONTROL Projekt]** aus. Dadurch wird das Modul so eingerichtet, dass nur Projekte gesucht werden.

   >[!TIP]
   >
   >Sie finden **[!UICONTROL Projekt]** in der Liste, wenn Sie mit der Eingabe des Wortes &quot;[!UICONTROL Projekt] beginnen.

1. Wählen Sie im **[!UICONTROL Ergebnissatz]** die Option **[!UICONTROL Erster übereinstimmender Datensatz]**. Dadurch wird das Modul so eingestellt, dass nur der erste gefundene Datensatz zurückgegeben wird, der die Kriterien erfüllt. Für dieses Beispiel benötigen wir nur einen zurückgegebenen Datensatz.
1. Im Bereich **[!UICONTROL Suchkriterien]** richten wir einen Filter ein, um das spezifische Projekt zurückzugeben:

   | Feld | Aktion |
   |--------|-------------|
   | Felder für Suchkriterien | Wählen Sie das Feld aus, nach dem Sie die Werte durchsuchen möchten. Wählen Sie für dieses Beispiel **[!UICONTROL Name]** aus. |
   | Suchkriterien | Wählen Sie im ersten Dropdown-Menü &quot;**[!UICONTROL &quot;]**. |
   | Standardoperatoren | Wählen Sie im zweiten Dropdown-Menü [!UICONTROL Enthält (Groß-/Kleinschreibung wird nicht beachtet)]. Auf diese Weise kann das Modul Projekte mit den ausgewählten Wörtern im Namen finden, auch wenn Sie nicht den gesamten Namen oder nur die falsche Groß-/Kleinschreibung (z. B. alle Großbuchstaben) eingeben. |
   | Textfeld | Geben Sie ein Wort oder eine Phrase ein, von dem bzw. der Sie wissen, dass es/sie im Namen des gesuchten Projekts ist. |

+++ Erweitern Sie , um ein Beispiel auf dem Bildschirm anzuzeigen.
   ![](assets/search-name.png)
+++

1. Wählen Sie in **[!UICONTROL Liste]** Ausgaben“ die Felder aus, die vom Modul ausgegeben werden sollen. Wählen Sie für dieses Beispiel die Felder **[!UICONTROL ID]** und **[!UICONTROL Name]** aus.

   >[!TIP]
   >
   >Sie können **Befehlstaste+F** ([!DNL Mac] OS) oder **Strg+F** ([!DNL Windows] OS) verwenden, um ein Feld schnell zu finden.

1. Klicken Sie **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >Da es sich hierbei nicht um ein Trigger-Modul handelt, kann nicht ausgewählt werden, wo es gestartet werden soll. Bei Verwendung eines Trigger-Moduls würden Sie jetzt auswählen, wo Sie es starten möchten.
   >
   >
   >Weitere Informationen finden Sie unter [Auswählen, wo ein Trigger beginnt [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

1. Klicken Sie mit der rechten Maustaste auf das Modul **[!UICONTROL Umbenennen]**, geben Sie dann einen Namen ein, der beschreibt, was das Modul tun soll (z. B. „Nach Projekt suchen„), und klicken Sie dann auf **[!UICONTROL OK]**.

   Der Name wird direkt unter dem Modul angezeigt. Darunter finden Sie [!DNL Workfront Fusion] kurze Beschreibung der Art der Aktion, die vom Modul ausgeführt wird.

   ![](assets/module-renamed-wf.png)

1. Fahren Sie mit [Hinzufügen und konfigurieren Sie das zweite Modul](#add-and-configure-the-second-module) fort.

### 4. Hinzufügen und Konfigurieren des zweiten Moduls

1. Klicken Sie auf den Teilkreis rechts neben dem Modul, um **[!UICONTROL Weitere Module hinzufügen]**.
1. Wählen Sie [!DNL Workfront] aus der Liste der Programme und dann das Suchmodul (**[!UICONTROL Datensätze lesen]** aus.
1. Wählen **[!UICONTROL im Feld]** die Verbindung aus, die Sie für das vorherige Modul erstellt haben. Sie müssen sicherstellen, dass dieses Modul dieselbe Verbindung wie das vorherige Modul verwendet.
1. Klicken Sie **[!UICONTROL Datensatztyp]** und wählen Sie **[!UICONTROL Projekt]** aus, da wir Datensätze im Zusammenhang mit einem Projekt lesen möchten.

   >[!TIP]
   >
   >Sie finden **[!UICONTROL Projekt]** in der Liste, wenn Sie mit der Eingabe des Wortes „Projekt“ beginnen.

1. Klicken Sie auf das Feld **[!UICONTROL ID des übergeordneten Datensatzes]**. Dieses Feld erfordert die Workfront-ID des Projekts, von dem Sie Aufgaben zurückgeben möchten.

   Wenn Sie auf das Feld klicken, wird die Liste der Variablen geöffnet, die Sie im Feld **[!UICONTROL ID des übergeordneten Datensatzes]** zur Identifizierung des Projekts in Workfront verwenden können.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Klicken Sie auf die Variable **[!UICONTROL ID]**, um sie zum Feld **[!UICONTROL ID des übergeordneten Datensatzes“]**. Dadurch kann die vom ersten Modul zurückgegebene ID als Kennung für das Projekt verwendet werden, mit dem Sie im zweiten Modul arbeiten möchten. Dadurch wird sichergestellt, dass die zurückgegebenen Aufgaben zu diesem Projekt gehören.
1. Wählen Sie im **[!UICONTROL Sammlungen]** die Option **[!UICONTROL Aufgaben]** aus. Dies zeigt an, dass das Modul Aufgaben zurückgeben soll, die mit dem ausgewählten Projekt verknüpft sind.
1. Wählen Sie im Feld **[!UICONTROL Ausgaben]** die Optionen **[!UICONTROL ID]** und **[!UICONTROL Name]** aus.
1. Klicken Sie auf **[!UICONTROL OK]**

   Jetzt haben Sie ein funktionierendes Szenario.

1. Geben Sie dem zweiten Modul einen Namen, z. B. „Aufgaben zurückgeben, die mit dem Projekt verknüpft sind“, und fahren Sie dann mit [Szenario testen](#test-the-scenario) fort.

## Testen des Szenarios

Bevor Sie Ihr Szenario aktivieren, müssen Sie es testen, indem Sie es mindestens einmal ausführen und die Ergebnisse anzeigen. Auf diese Weise können Sie verstehen, wie Daten durch das Szenario fließen, und Fehler finden.

Wir haben ausgewählt, dass 1 Projekt sowie die mit diesem Projekt verbundenen Aufgaben zurückgegeben werden. Wenn Sie das Szenario ausführen, sollte dies passieren.

1. Klicken Sie **[!UICONTROL Einmal ausführen]** in der linken unteren Ecke des Szenario-Editors.
1. Klicken Sie nach der Ausführung des Szenarios auf die Blase oberhalb des ersten Moduls.

   ![](assets/click-bubble.png)

   Im angezeigten Feld können Sie Informationen zum Datenpaket anzeigen, das vom Modul verarbeitet wurde, einschließlich der tatsächlichen Daten, die aus dem Projekt abgerufen wurden, das das Modul zurückgegeben hat.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. Klicken Sie auf die Blase „Ausführungs-Inspektor“ über dem zweiten Modul, um die Eingabe von Informationen und die Ausgabe anzuzeigen, bei der es sich um eine Sammlung von Aufgaben handelt, die im Projekt enthalten sind.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   Weitere Informationen zum Lesen von Informationen zur Szenario-Ausführung finden Sie in den folgenden Artikeln:

   * Allgemeine Informationen finden Sie unter [Ausführungsfluss von Szenarien in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Informationen zu verarbeiteten Bundles finden Sie unter [Szenarioausführung, Zyklen und Phasen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Klicken Sie [!DNL Workfront Fusion] auf **[!UICONTROL Speichern]** ![](assets/save-icon.png) unten links, um Ihren Fortschritt im Szenario zu speichern.

   >[!IMPORTANT]
   >
   >Speichern Sie häufig, während Sie ein Szenario verfeinern und testen.

>[!TIP]
>
>Wir empfehlen die optionale, aber nützliche Vorgehensweise, Hinweise zu jedem Modul hinzuzufügen.
>
>1. Klicken Sie mit der rechten Maustaste auf ein [!DNL Workfront] und dann auf **[!UICONTROL Notiz hinzufügen]**.
>1. Geben Sie in der angezeigten Anmerkung eine Übersicht für das Modul ein.
>
>    Sie können mehrere Notizen für ein Modul hinzufügen.
>
>1. Schließen Sie den **[!UICONTROL Anmerkungen]**.
>
>     Nachdem Sie einem Szenario eine Anmerkung hinzugefügt haben, wird auf dem Symbol **[!UICONTROL Anmerkungen]** unten im Szenario-Editor ein orangefarbener Punkt ![](assets/notes-icon-w-dot.png).
>
>1. Klicken Sie auf das **[!UICONTROL Notizen]**-Symbol ![](assets/notes-icon-w-dot.png), um Ihre Notizen anzuzeigen.
>

## Aktivieren des Szenarios

Dieses Beispielszenario hat kein Trigger-Modul. Wenn dies ein Szenario wäre, das Sie für echte Daten verwenden würden, würde es mit einem Trigger-Modul beginnen, und das letzte, was Sie tun würden, wäre, es zu aktivieren. Nachdem Sie ein Szenario aktiviert haben, wird es standardmäßig alle 15 Minuten ausgeführt. Sie können dies ändern, indem Sie festlegen, wann und wie oft die Ausführung erfolgen soll.

Weitere Informationen zum Aktivieren von Szenarien finden Sie unter [Aktivieren oder Deaktivieren eines Szenarios in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Weitere Informationen zu Zeitplänen finden Sie unter [Planen eines Szenarios in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
