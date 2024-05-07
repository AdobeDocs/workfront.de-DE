---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Basisszenario erstellen in [!DNL Adobe Workfront Fusion]
description: Erfahren Sie, wie Sie mit Adobe Workfront Fusion ein einfaches Automatisierungsszenario erstellen. Automatisierungsszenarien automatisieren Workfront-Prozesse, einschließlich Datenmanipulationen und -umwandlungen. In diesem Beispiel werden Sie durch die Erstellung eines Szenarios geführt, in dem nach einem [!DNL Workfront] in Workfront und konvertiert sie in ein Projekt.
author: Becky
feature: Workfront Fusion
source-git-commit: 91d3dcde8eda416286c6781f6eef85404fd382c2
workflow-type: tm+mt
source-wordcount: '1300'
ht-degree: 0%

---

# Basisszenario erstellen in [!DNL Adobe Workfront Fusion]

Die Rolle [!DNL Adobe Workfront Fusion] ist es, Ihre Prozesse zu automatisieren, sodass Sie sich auf neue Aufgaben konzentrieren können, anstatt dieselben Aufgaben immer wieder zu wiederholen. Es funktioniert durch die Verknüpfung von Aktionen innerhalb und zwischen Apps und Diensten, um ein Szenario zu erstellen, in dem Ihre Daten automatisch übertragen und transformiert werden. Das Szenario, in dem Sie Watches für Daten in einer App oder einem Dienst erstellen und diese Daten verarbeiten, um das gewünschte Ergebnis zu liefern.

In diesem Beispiel werden Sie durch die Erstellung eines Szenarios geführt, in dem nach einem [!DNL Workfront] in Workfront und konvertiert sie in ein Projekt.

<!--# Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>
To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

-->

## Erstellen eines Praxisszenarios

### Erstellen des Szenarios beginnen

1. Im **Szenarien** Bereich, klicken Sie **Neues Szenario erstellen**.

   <!--To locate the Scenarios area, see navigation article-->

   Der Szenario-Editor wird angezeigt, der ein leeres Modul in der Mitte enthält.

   <!--picture?-->

1. Wählen Sie die **[!UICONTROL Neues Szenario]** Platzhalternamen in der linken oberen Ecke und geben Sie einen Namen ein.
1. Fahren Sie mit [Hinzufügen und Konfigurieren des ersten Moduls](#add-and-configure-the-first-module) unten.

### Hinzufügen und Konfigurieren des ersten Moduls

1. Klicken Sie auf das leere Modul, um die App auszuwählen, aus der Sie ein Modul auswählen.

   Rechts neben dem Modul wird eine Liste von Apps angezeigt.

1. Auswählen **[!DNL Adobe Workfront]**. Wenn sie nicht angezeigt wird, klicken Sie auf die Suchleiste am unteren Rand der Liste, geben Sie &quot;Workfront&quot;ein und wählen Sie sie aus, wenn sie in der Liste angezeigt wird.

   Die Liste ändert sich, sodass alle [!DNL Workfront] -Module, die Sie verwenden können.

1. Klicken Sie auf **[!UICONTROL Suche]** -Modul.

   Das Fenster zur Modulkonfiguration wird geöffnet.

1. Im [!UICONTROL Verbindung] Wählen Sie Ihre Workfront-Verbindung aus.

   Wenn Sie keine Workfront-Verbindung haben, lesen Sie [Erstellen Sie eine Verbindung zu [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)
1. Im [!UICONTROL Record Type] auswählen **[!UICONTROL Aufgabe]**. Dadurch wird das Modul so eingestellt, dass nur Aufgaben durchsucht werden.

   Sie finden **[!UICONTROL Aufgabe]** in der Liste, wenn Sie beginnen, das Wort &quot;[!UICONTROL Aufgabe].&quot;

1. Im **[!UICONTROL Ergebnissatz]** auswählen **[!UICONTROL Erster übereinstimmender Datensatz]**.

   Dadurch wird das -Modul so eingestellt, dass nur der erste Datensatz zurückgegeben wird, der nach seiner Auswahl die Kriterien erfüllt.
1. Im **[!UICONTROL Suchkriterien]** -Bereich konfigurieren Sie die Kriterien, um die spezifische Aufgabe zurückzugeben.

   1. Im ersten Feld unter [!UICONTROL Suchkriterien]wählen Sie das Feld aus, das Sie in die Suche einbeziehen möchten. Wählen Sie für dieses Beispiel **[!UICONTROL Name]**.

      Sie finden **[!UICONTROL Name]** in der Liste, wenn Sie beginnen, das Wort &quot;[!UICONTROL name].&quot;
   1. Klicken Sie für den Operator auf den Dropdown-Pfeil neben **Existiert** und ändern Sie sie in [!UICONTROL **Enthält (nicht von Schreibweise abhängig)**].

      Dadurch kann das Modul Projekte mit dem Namen Ihrer ausgewählten Wörter finden, selbst wenn Sie nicht den gesamten Namen eingeben oder den Namen mit der falschen Groß-/Kleinschreibung eingeben (z. B. alle Großbuchstaben).
   1. Im letzten Feld unter [!UICONTROL Suchkriterien], geben Sie ein Wort oder eine Wortgruppe ein, von dem Sie wissen, dass es sich um den Namen der gesuchten Aufgabe handelt.

1. Im **[!UICONTROL Ausgaben]** auswählen, wählen Sie die Felder aus, die das Modul ausgeben soll. Wählen Sie für dieses Beispiel die **[!UICONTROL ID]** und **[!UICONTROL Name]** -Felder.

   >[!TIP]
   >
   >Sie können **Befehl+F** ([!DNL Mac] OS) oder **Strg+F** ([!DNL Windows] OS), um ein Feld schnell zu finden.

1. Klicks **[!UICONTROL OK]** , um die Modulkonfiguration zu speichern.

1. Klicken Sie mit der rechten Maustaste auf das Modul und klicken Sie auf **[!UICONTROL Umbenennen]** Geben Sie einen Namen ein, der beschreibt, was das Modul tun soll (z. B. &quot;Suche nach Aufgabe&quot;), und klicken Sie dann auf **[!UICONTROL OK]**.

   Der Name erscheint direkt unter dem Modul. Darunter: [!DNL Workfront Fusion] enthält eine kurze Beschreibung der Art der Aktion, die vom Modul ausgeführt wird.

   ![](assets/module-renamed-wf.png)

1. Fahren Sie mit [Zweites Modul hinzufügen und konfigurieren](#add-and-configure-the-second-module).

## Zweites Modul hinzufügen und konfigurieren

1. Bewegen Sie den Mauszeiger über den partiellen Kreis rechts neben dem des Moduls und klicken Sie dann auf **[!UICONTROL Hinzufügen eines weiteren Moduls]**.
1. Auswählen [!DNL Adobe Workfront] Wählen Sie aus der Anwendungsliste das Modul aus. **[!UICONTROL Konvertierungsobjekt]**.
1. Im [!UICONTROL Verbindung] Wählen Sie dieselbe Workfront-Verbindung aus, die Sie im vorherigen Modul verwendet haben.
1. Im **[!UICONTROL Record Type]** Feld auswählen **[!UICONTROL Aufgabe]**, da das Modul eine Aufgabe konvertiert.
1. Im **[!UICONTROL Konvertieren in]** Feld auswählen **Projekt**.
1. Klicken Sie neben dem Feld Task ID auf den Umschalter Zuordnung , um es zu aktivieren.

   Der Umschalter wird blau, wenn er aktiviert ist. Auf diese Weise können Sie die Aufgaben-ID aus dem vorherigen Modul zuordnen.

   ![Umschalten zwischen Zuordnungen](assets/map-toggle.png)
1. Klicken Sie auf **[!UICONTROL Task-ID]** -Feld.

   Es wird ein Bedienfeld geöffnet, in dem Sie auswählen können, was als ID der Aufgabe verwendet werden soll, die Sie in ein Projekt konvertieren möchten. Da Sie die Zuordnung aktiviert haben, enthält das Bedienfeld die Ausgabe aus allen vorherigen Modulen. Sie haben die ID als Ausgabe des vorherigen Moduls ausgewählt, sodass sie jetzt im Bedienfeld verfügbar ist.

   Dieses Bedienfeld wird als Zuordnungsbedienfeld bezeichnet. Weitere Informationen zum Zuordnungsbedienfeld finden Sie unter [Informationen zwischen Modulen zuordnen](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. Auswählen **ID** im Zuordnungsbereich.

   Im Feld ID wird ein ID-Block angezeigt. Es zeigt die Anzahl des Moduls, von dem es zugeordnet wird, und das Feld, das zugeordnet wird.

   ![Zuordnungs-ID](assets/map-id.png)

1. Klicken Sie auf **Vorlagen-ID** ein, geben Sie den Namen der Workfront-Vorlage ein, die Sie für dieses Projekt verwenden möchten, und wählen Sie ihn dann aus, wenn er in der Liste angezeigt wird.
1. Klicks **[!UICONTROL OK]** , um die Modulkonfiguration zu speichern.

1. Klicken Sie mit der rechten Maustaste auf das Modul und klicken Sie auf **[!UICONTROL Umbenennen]** Geben Sie einen Namen ein, der beschreibt, was das Modul tun soll (z. B. &quot;In Projekt konvertieren&quot;), und klicken Sie dann auf **[!UICONTROL OK]**.

1. Weiter zu [Testen des Szenarios](#test-the-scenario).

## Testen des Szenarios

Bevor Sie Ihr Szenario aktivieren, müssen Sie es testen, indem Sie es mindestens einmal ausführen und die Ergebnisse anzeigen. Auf diese Weise können Sie erkennen, wie Daten durch das Szenario fließen und Fehler finden.

Für dieses Szenario würde ein erfolgreicher Test dazu führen, dass die neue Aufgabe gefunden und in ein Projekt konvertiert wird.

1. Klicks **[!UICONTROL Einmal ausführen]** in der linken unteren Ecke des Szenario-Editors.
1. Nachdem das Szenario abgeschlossen ist, klicken Sie auf die Blase über dem ersten Modul, um Informationen über das vom Modul verarbeitete Datenbündel anzuzeigen, einschließlich der Daten, die aus der vom Modul zurückgegebenen Aufgabe abgerufen wurden.

1. Klicken Sie auf den Ausführungsinspektor oberhalb des zweiten Moduls, um die Eingabe (die Aufgabe) und die Ausgabe (das konvertierte Projekt) anzuzeigen.

   Weitere Informationen zu den Daten in den Inspektionsblasen finden Sie unter:

   * Allgemeine Informationen finden Sie unter [Ausführungsfluss des Szenarios in [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-flow.md).
   * Weitere Informationen zu verarbeiteten Bundles finden Sie unter [Ausführung des Szenarios, Zyklen und Phasen in [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. In [!DNL Workfront Fusion]klicken **[!UICONTROL Speichern]** in der Nähe der linken unteren Ecke, um den Fortschritt des Szenarios zu speichern.

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

Der letzte Schritt beim Erstellen eines Szenarios besteht darin, es zu aktivieren.

Da in diesem Szenario nach einer bestimmten Aufgabe gesucht wird, muss sie nicht aktiviert werden. Wenn Sie ein Szenario aktivieren, wird es nach einem Zeitplan oder bei einer bestimmten Aktion in einer Anwendung ausgeführt. Nachdem Sie ein Szenario aktiviert haben, wird es standardmäßig alle 15 Minuten ausgeführt. Sie können dies ändern, indem Sie festlegen, wann und wie oft die Anwendung ausgeführt werden soll.

Weitere Informationen zum Aktivieren von Szenarien finden Sie unter [Aktivieren oder deaktivieren Sie ein Szenario in [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Weitere Informationen zu Zeitplänen finden Sie unter [Planen eines Szenarios in [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md).

## Nächste Schritte

* [Trigger-Modul hinzufügen](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/add-trigger-to-simple-scenario.md) , damit das Szenario regelmäßig nach neuen Anforderungen sucht und sie in Projekte konvertiert.
* Fügen Sie einen Webhook hinzu, damit das Szenario jedes Mal ausgeführt werden kann, wenn eine Anforderung eingegeben wird.
* Fügen Sie einen Filter hinzu, um sicherzustellen, dass nur bestimmte Anforderungen in Projekte konvertiert werden.
* Fügen Sie eine Funktion hinzu, mit der der Name des neuen Projekts angepasst wird.
* Fügen Sie die Fehlerbehandlung hinzu, um sicherzustellen, dass das Szenario fehleranfällig ist.

