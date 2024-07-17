---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Erstellen eines Szenarios für die Automatisierung von Verfahren in  [!DNL Adobe Workfront Fusion]
description: In diesem Artikel wird beschrieben, wie Sie mit Adobe Workfront Fusion ein Automatisierungsszenario erstellen. Automatisierungsszenarien automatisieren Workfront-Prozesse, einschließlich Datenmanipulationen und -umwandlungen. Dieses Beispiel führt Sie durch die Erstellung eines Szenarios, in dem nach einem Projekt gesucht wird, und gibt dann alle mit diesem Projekt verknüpften Aufgaben zurück.
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 8769ed5844e340e007f844370791e93393696819
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 0%

---

# Erstellen eines Automatisierungsszenarios für Vorgehensweisen in [!DNL Adobe Workfront Fusion]

Automatisierungsszenarien automatisieren Workfront-Prozesse, einschließlich Datenmanipulationen und -umwandlungen. Dieser Artikel führt Sie durch den Prozess der Erstellung eines Szenarios, in dem nach einem Projekt gesucht wird, und gibt dann alle mit diesem Projekt verknüpften Aufgaben zurück.

<!-- not sure why these are here?
For instructions on building an integration scenario that connects separate apps, see [Create a practice integration scenario in Adobe Workfront Fusion](../../workfront-fusion/get-started/create-a-practice-scenario.md).

For more information on functionality available with each Workfront Fusion license, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>Adobe Workfront-Abo</td>  
      <td>Alle</td>  
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
        Aktuell: Keine Workfront Fusion-Lizenzanforderungen.<br>
        Oder<br>
        Veraltet: Beliebig
      </td>  
    </tr>  
    <tr>  
      <td>Produkt</td>  
      <td> 
        Neu: Wählen Sie den Workfront-Plan aus oder führen Sie ihn aus: Ihr Unternehmen muss Adobe Workfront Fusion erwerben.<br>
        Ultimate Workfront Plan: Workfront Fusion ist im Lieferumfang enthalten.<br>
        Oder<br>
        Aktuell: Ihr Unternehmen muss Adobe Workfront Fusion erwerben.
      </td>  
    </tr> 
  </tbody>  
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Erstellen eines Automatisierungspraktiken-Szenarios

[!DNL Adobe Workfront Fusion] hilft Ihnen, sich auf wichtige Aufgaben zu konzentrieren, indem Sie sich wiederholende Aufgaben automatisieren. Es werden Szenarien erstellt, in denen Ihre Daten automatisch über verschiedene Apps und Dienste hinweg verwaltet werden.

Jedes Szenario besteht aus Modulen, die die Verarbeitung von Daten in einer App oder die Übertragung zwischen verschiedenen Apps und Diensten steuern. Sie können beispielsweise ein Szenario in Fusion erstellen, um automatisch ein [!DNL Workfront] -Projekt zu finden und dessen Aufgaben aufzulisten. Auf diese Weise spart Fusion Ihnen Zeit und Mühe, indem Sie Routineaufgaben erledigen.

Dieses Szenario führt Sie durch die Erstellung eines Szenarios, in dem nach einem [!DNL Workfront] -Projekt gesucht wird und das die Aufgaben im Projekt zurückgibt.

![](assets/create-practice-scenario-wf-only-350x157.png)

### Bevor Sie beginnen

Erstellen Sie ein Projekt mit Aufgaben an der Arbeitsfläche, die Sie für diese Übung verwenden können. Sie müssen keine zusätzliche Konfiguration vornehmen, außer Aufgaben zum Projekt hinzuzufügen.

Weitere Informationen zum Erstellen eines Projekts in Workspace finden Sie unter xxx.

### 1. Erstellen und Benennen des Szenarios

1. Melden Sie sich bei Ihrem [!DNL Workfront Fusion] -Konto an.
1. Klicken Sie im linken Bereich auf **[!UICONTROL Szenarios]** ![](assets/scenarios-icon.png) .

   >[!NOTE]
   >
   >Wenn das linke Navigationsfenster oder dessen Symbole nicht angezeigt werden, klicken Sie auf das Menü-Symbol ![Menü](assets/main-menu-icon-left-nav.png) .

1. Klicken Sie im Bedienfeld [!UICONTROL **Ordner**] auf das Symbol **[!UICONTROL Ordner hinzufügen]** ![](assets/add-folder-icon.png) und geben Sie dann einen Namen wie &quot;Practice scenarios&quot;für Ihren ersten Ordner ein.

1. Öffnen Sie den Ordner und klicken Sie dann oben rechts auf der Seite auf **[!UICONTROL Neues Szenario erstellen]** .

1. Wählen Sie für diese Übung die **[!DNL Adobe Workfront]** -App aus und klicken Sie unten auf **Suchen** .


1. Wählen Sie oben links den Platzhalternamen **[!UICONTROL Neues Szenario]** aus und geben Sie dann einen Namen wie &quot;Praxisszenario 1&quot;ein.

   ![](assets/name-the-scenario.png)

1. Fahren Sie mit [Verbinden Sie das erste Modul](#2-connect-the-first-module) weiter unten.

### 2. Verbinden Sie das erste Modul

Nun müssen Sie eine authentifizierte Verbindung zu Ihrem [!DNL Workfront]-Konto herstellen. Jedes Modul, das Sie einem Szenario hinzufügen, muss eine Verbindung zu seiner App haben.

1. Klicken Sie im Feld &quot;**[!DNL Workfront]**&quot;unter &quot;**[!UICONTROL Verbindung]**&quot;auf &quot;**[!UICONTROL Hinzufügen]**&quot;, geben Sie einen Namen für die Verbindung ein, z. B. &quot;Olivas Workfront-Konto&quot;und klicken Sie dann auf &quot;**[!UICONTROL Weiter]**&quot;.
1. Authentifizieren Sie die Verbindung im angezeigten Fenster.

   Der Prozess zum Authentifizieren einer Verbindung kann zwischen Apps etwas variieren. Der folgende Prozess ist spezifisch für [!DNL Workfront], der Prozess ähnelt jedoch vielen Apps:

   1. Geben Sie Ihre Domäne [!DNL Workfront] ein und klicken Sie dann auf **[!UICONTROL Weiter]**.
   1. Melden Sie sich bei [!DNL Workfront] an.
   1. Überprüfen Sie den Zugriff, den [!DNL Workfront Fusion] anfordert, und klicken Sie dann auf **[!UICONTROL Zugriff zulassen]**.

   Wenn Sie Hilfe benötigen, finden Sie weitere Informationen unter [Übersicht über Verbindungen](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

### 3. Konfigurieren des ersten Moduls

Nachdem Sie [!DNL Workfront Fusion] mit Ihrem [!DNL Workfront] -Konto verbunden haben, können Sie ein [!DNL Workfront] -Projekt angeben, auf das Sie Zugriff haben, sowie die Daten, auf die das erste Modul verarbeitet werden soll.

1. Wählen Sie im Feld [!UICONTROL Record Type] die Option **[!UICONTROL Project]**. Dadurch wird das Modul so eingestellt, dass nur Projekte durchsucht werden.

   >[!TIP]
   >
   >Sie können **[!UICONTROL Projekt]** in der Liste finden, wenn Sie mit der Eingabe des Wortes &quot;[!UICONTROL Projekt]&quot;beginnen.

1. Wählen Sie im Feld **[!UICONTROL Ergebnissatz]** die Option **[!UICONTROL Erster übereinstimmender Datensatz]** aus. Dadurch wird das -Modul so eingestellt, dass nur der erste Datensatz zurückgegeben wird, der nach seiner Auswahl die Kriterien erfüllt. Für dieses Beispiel benötigen wir nur einen Datensatz.
1. Im Bereich **[!UICONTROL Suchkriterien]** werden wir einen Filter einrichten, um das spezifische Projekt zurückzugeben:

   | Feld | Aktion |
   |--------|-------------|
   | Suchkriterienfelder | Wählen Sie das Feld aus, nach dem Sie die Werte durchsuchen möchten. Wählen Sie für dieses Beispiel **[!UICONTROL Name]** aus. |
   | Suchkriterien | Wählen Sie im ersten Dropdown-Menü **[!UICONTROL Name]** aus. |
   | Grundlegende Operatoren | Wählen Sie in der zweiten Dropdown-Liste [!UICONTROL Enthält (Groß-/Kleinschreibung nicht beachten)] aus. Dadurch kann das Modul Projekte mit dem Namen Ihrer ausgewählten Wörter finden, selbst wenn Sie nicht den gesamten Namen eingeben oder den Namen mit der falschen Groß-/Kleinschreibung eingeben (z. B. alle Großbuchstaben). |
   | Textfeld | Geben Sie ein Wort oder eine Wortgruppe ein, von dem Sie wissen, dass es sich im Namen des Projekts befindet, nach dem Sie suchen. |

+++ Erweitern Sie , um ein Beispiel auf dem Bildschirm anzuzeigen.
   ![](assets/search-name.png)
+++

1. Wählen Sie in der Liste **[!UICONTROL Ausgaben]** die Felder aus, die das Modul ausgeben soll. Wählen Sie für dieses Beispiel die Felder **[!UICONTROL ID]** und **[!UICONTROL Name]** aus.

   >[!TIP]
   >
   >Sie können **Befehl+F** ([!DNL Mac] BS) oder **Strg+F** ([!DNL Windows] OS) verwenden, um ein Feld schnell zu finden.

1. Klicken Sie auf **[!UICONTROL OK]**.

   >[!NOTE]
   >
   >Da es sich nicht um ein Trigger-Modul handelt, wählen Sie nicht, wo es gestartet werden soll. Bei Verwendung eines Trigger-Moduls würden Sie jetzt auswählen, wo es gestartet werden soll.
   >
   >
   >Weitere Informationen finden Sie unter [Auswählen, wo ein Trigger-Modul in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md) beginnt.

1. Klicken Sie mit der rechten Maustaste auf das Modul, klicken Sie auf **[!UICONTROL Umbenennen]**, geben Sie einen Namen ein, der beschreibt, was das Modul tun soll (z. B. &quot;Suche nach Projekt&quot;), und klicken Sie dann auf **[!UICONTROL OK]**.

   Der Name erscheint direkt unter dem Modul. Darunter enthält [!DNL Workfront Fusion] eine kurze Beschreibung der Art der Aktion, die vom Modul ausgeführt wird.

   ![](assets/module-renamed-wf.png)

1. Fahren Sie mit [Hinzufügen und Konfigurieren des zweiten Moduls](#add-and-configure-the-second-module) fort.

### 4. Das zweite Modul hinzufügen und konfigurieren

1. Klicken Sie auf den Teilkreis rechts neben dem Modul, um **[!UICONTROL ein weiteres Modul hinzufügen]** hinzuzufügen.
1. Wählen Sie [!DNL Workfront] aus der Liste der Anwendungen und dann das Suchmodul **[!UICONTROL Verwandte Datensätze lesen]**.
1. Wählen Sie im Feld **[!UICONTROL Verbindung]** die Verbindung aus, die Sie für das vorherige Modul erstellt haben. Sie müssen sicherstellen, dass dieses Modul dieselbe Verbindung wie das vorherige Modul verwendet.
1. Klicken Sie auf **[!UICONTROL Record type]** und wählen Sie dann **[!UICONTROL Project]** aus, da wir Datensätze lesen möchten, die sich auf ein Projekt beziehen.

   >[!TIP]
   >
   >Sie finden **[!UICONTROL Projekt]** in der Liste, wenn Sie mit der Eingabe des Wortes &quot;Projekt&quot;beginnen.

1. Klicken Sie auf das Feld **[!UICONTROL Übergeordnete Datensatz-ID]** . Für dieses Feld ist die Workfront ID des Projekts erforderlich, aus dem Sie Aufgaben zurückgeben möchten.

   Durch Klicken auf das Feld wird die Liste der Variablen geöffnet, die Sie im Feld **[!UICONTROL Übergeordnete Datensatz-ID]** verwenden können, um das Projekt in Workfront zu identifizieren.

   ![](assets/list-of-available-variables-wf-350x368.png)

1. Klicken Sie auf die Variable **[!UICONTROL ID]** , um sie dem Feld **[!UICONTROL Übergeordnete Datensatz-ID]** hinzuzufügen. Dadurch kann die vom ersten Modul zurückgegebene ID als Kennung für das Projekt verwendet werden, mit dem Sie im zweiten Modul arbeiten möchten. Dadurch wird sichergestellt, dass die zurückgegebenen Aufgaben zu diesem Projekt gehören.
1. Wählen Sie im Feld **[!UICONTROL Sammlungen]** die Option **[!UICONTROL Aufgaben]** aus. Dies bedeutet, dass das Modul Aufgaben zurückgibt, die mit dem ausgewählten Projekt verknüpft sind.
1. Wählen Sie im Feld **[!UICONTROL Ausgaben]** die Optionen **[!UICONTROL ID]** und **[!UICONTROL Name]** aus.
1. Klicken Sie auf **[!UICONTROL OK]**

   Jetzt haben Sie ein funktionierendes Szenario.

1. Geben Sie dem zweiten Modul einen Namen wie &quot;Aufgaben zurückgeben, die mit dem Projekt verknüpft sind&quot;und fahren Sie dann mit [Szenario testen](#test-the-scenario) fort.

## Testen des Szenarios

Bevor Sie Ihr Szenario aktivieren, müssen Sie es testen, indem Sie es mindestens einmal ausführen und die Ergebnisse anzeigen. Auf diese Weise können Sie erkennen, wie Daten durch das Szenario fließen und Fehler finden.

Wir haben ausgewählt, dass 1 Projekt zurückgegeben werden soll und die mit diesem Projekt verbundenen Aufgaben. Wenn Sie das Szenario ausführen, sollte dies geschehen.

1. Klicken Sie in der linken unteren Ecke des Szenario-Editors auf **[!UICONTROL Einmal ausführen]** .
1. Nachdem das Szenario abgeschlossen ist, klicken Sie auf die Blase über dem ersten Modul.

   ![](assets/click-bubble.png)

   In dem angezeigten Feld können Sie Informationen zum Datenbündel, das das Modul verarbeitet hat, anzeigen, einschließlich der tatsächlichen Daten, die aus dem vom Modul zurückgegebenen Projekt abgerufen wurden.

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. Klicken Sie auf die Blase über dem zweiten Modul, um die Eingabe der Informationen und die Ausgabe anzuzeigen, bei der es sich um eine Sammlung von Aufgaben im Projekt handelt.

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   Weitere Informationen zum Lesen von Informationen zur Ausführung von Szenarien finden Sie in den folgenden Artikeln:

   * Allgemeine Informationen finden Sie unter [Ausführungsfluss eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * Informationen zu verarbeiteten Bundles finden Sie unter [Ausführung, Zyklen und Phasen eines Szenarios in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Klicken Sie in [!DNL Workfront Fusion] unten links auf **[!UICONTROL Speichern]** ![](assets/save-icon.png) , um den Fortschritt des Szenarios zu speichern.

   >[!IMPORTANT]
   >
   >Speichern Sie oft, während Sie ein Szenario testen.

>[!TIP]
>
>Wir empfehlen die optionale, aber nützliche Vorgehensweise, Hinweise zu jedem Modul hinzuzufügen.
>
>1. Klicken Sie mit der rechten Maustaste auf ein [!DNL Workfront]-Modul und klicken Sie dann auf **[!UICONTROL Notiz hinzufügen]**.
>1. Geben Sie in die angezeigte Notiz eine Übersicht für das Modul ein.
>
>    Sie können mehrere Notizen für ein Modul hinzufügen.
>
>1. Schließen Sie den Bereich **[!UICONTROL Notizen]** .
>
>     Nachdem Sie einem Szenario eine Notiz hinzugefügt haben, wird am unteren Rand des Szenario-Editors auf dem Symbol **[!UICONTROL Notizen]** ![](assets/notes-icon-w-dot.png) ein orangefarbener Punkt angezeigt.
>
>1. Klicken Sie auf das Symbol **[!UICONTROL Notizen]** ![](assets/notes-icon-w-dot.png), um Ihre Notizen anzuzeigen.
>

## Aktivieren des Szenarios

In diesem Beispielszenario gibt es kein Trigger-Modul. Wenn dies ein Szenario wäre, das Sie für echte Daten verwenden würden, würde es mit einem Trigger-Modul beginnen und das Letzte, was Sie tun würden, ist es zu aktivieren. Nachdem Sie ein Szenario aktiviert haben, wird es standardmäßig alle 15 Minuten ausgeführt. Sie können dies ändern, indem Sie festlegen, wann und wie oft die Anwendung ausgeführt werden soll.

Weitere Informationen zum Aktivieren von Szenarien finden Sie unter [Aktivieren oder Deaktivieren eines Szenarios in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Informationen zu Zeitplänen finden Sie unter [Planen eines Szenarios in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).
