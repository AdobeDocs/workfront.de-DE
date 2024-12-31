---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Erstellen Sie ein einfaches Szenario in [!DNL Adobe Workfront Fusion]
description: Erfahren Sie, wie Sie mit Adobe Workfront Fusion ein einfaches Automatisierungsszenario erstellen. Automatisierungsszenarien automatisieren Workfront-Prozesse, einschließlich Datenmanipulationen und -umwandlungen. Dieses Beispiel führt Sie durch den Prozess der Erstellung eines Szenarios, das in Workfront nach einer  [!DNL Workfront]  sucht und sie dann in ein Projekt konvertiert.
author: Becky
feature: Workfront Fusion
exl-id: 06fa7e15-b8dc-4fe1-9703-c160d580ef79
source-git-commit: 1196e2d7a6d6750944a7c6209222f07382abfee7
workflow-type: tm+mt
source-wordcount: '1300'
ht-degree: 0%

---

# Erstellen eines einfachen Szenarios in [!DNL Adobe Workfront Fusion]

Die Rolle von [!DNL Adobe Workfront Fusion] besteht darin, Ihre Prozesse zu automatisieren, damit Sie sich auf neue Aufgaben konzentrieren können, anstatt dieselben Aufgaben immer wieder zu wiederholen. Es funktioniert durch die Verknüpfung von Aktionen innerhalb und zwischen Apps und Services, um ein Szenario zu erstellen, das Ihre Daten automatisch überträgt und transformiert. Das Szenario, in dem Sie Daten in einer App oder einem Service erstellen, überwacht und verarbeitet diese Daten, um das gewünschte Ergebnis zu liefern.

Dieses Beispiel führt Sie durch den Prozess der Erstellung eines Szenarios, das in Workfront nach einer [!DNL Workfront]-Aufgabe sucht und sie dann in ein Projekt konvertiert.

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

## Erstellen eines Übungsszenarios

### Erstellen des Szenarios

1. Klicken Sie **Bereich &quot;**&quot; auf **Neues Szenario erstellen**.

   <!--To locate the Scenarios area, see navigation article-->

   Der Szenario-Editor wird angezeigt, wobei in der Mitte ein leeres Modul enthalten ist.

   <!--picture?-->

1. Wählen Sie **[!UICONTROL Platzhalternamen]** Neues Szenario“ in der linken oberen Ecke aus und geben Sie dann einen Namen ein.
1. Fahren Sie mit [Hinzufügen und konfigurieren Sie das erste Modul](#add-and-configure-the-first-module) unten fort.

### Hinzufügen und Konfigurieren des ersten Moduls

1. Klicken Sie auf das leere Modul, um die App auszuwählen, aus der Sie ein Modul auswählen möchten.

   Rechts neben dem Modul wird eine Liste mit Apps angezeigt.

1. Wählen Sie **[!DNL Adobe Workfront]** aus. Wenn es nicht sichtbar ist, klicken Sie unten in der Liste auf die Suchleiste, geben Sie &quot;Workfront&quot; ein und wählen Sie es aus, wenn es in der Liste angezeigt wird.

   Die Liste ändert sich und zeigt alle [!DNL Workfront] Module an, die Sie verwenden können.

1. Klicken Sie auf das **[!UICONTROL Suche]**-Modul.

   Das Fenster für die Modulkonfiguration wird geöffnet.

1. Wählen [!UICONTROL  im Feld ] Ihre Workfront-Verbindung aus.

   Wenn Sie keine Workfront-Verbindung haben, lesen Sie [Verbindung zu erstellen [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/connections/connect-to-fusion-general.md)
1. Wählen [!UICONTROL  im Feld „Datensatztyp] die Option **[!UICONTROL Aufgabe]** aus. Dadurch wird das Modul so eingestellt, dass nur Aufgaben gesucht werden.

   Sie finden **[!UICONTROL Aufgabe]** in der Liste, wenn Sie mit der Eingabe des Wortes &quot;[!UICONTROL Aufgabe] beginnen.

1. Wählen Sie im **[!UICONTROL Ergebnissatz]** die Option **[!UICONTROL Erster übereinstimmender Datensatz]**.

   Dadurch wird das Modul so eingestellt, dass nur der erste gefundene Datensatz zurückgegeben wird, der die Kriterien erfüllt.
1. Konfigurieren **[!UICONTROL im Bereich &quot;]**&quot; die Kriterien, um die spezifische Aufgabe zurückzugeben.

   1. Wählen Sie im ersten Feld unter [!UICONTROL Suchkriterien] das Feld aus, das Sie in Ihre Suche einbeziehen möchten. Wählen Sie für dieses Beispiel **[!UICONTROL Name]** aus.

      Sie finden **[!UICONTROL Name]** in der Liste, wenn Sie mit der Eingabe des Wortes &quot;[!UICONTROL name] beginnen.
   1. Klicken Sie für den -Operator auf den Dropdown-Pfeil neben **Vorhanden** und ändern Sie ihn in [!UICONTROL **Enthält (ignoriert Groß-/Kleinschreibung)**].

      Auf diese Weise kann das Modul Projekte mit den ausgewählten Wörtern im Namen finden, auch wenn Sie nicht den gesamten Namen oder nur die falsche Groß-/Kleinschreibung (z. B. alle Großbuchstaben) eingeben.
   1. Geben Sie im letzten Feld unter [!UICONTROL Suchkriterien] ein Wort oder eine Phrase ein, von dem Sie wissen, dass es/sie im Namen der Aufgabe ist, nach der Sie suchen.

1. Wählen Sie in **[!UICONTROL Liste]** Ausgaben“ die Felder aus, die vom Modul ausgegeben werden sollen. Wählen Sie für dieses Beispiel die Felder **[!UICONTROL ID]** und **[!UICONTROL Name]** aus.

   >[!TIP]
   >
   >Sie können **Befehlstaste+F** ([!DNL Mac] OS) oder **Strg+F** ([!DNL Windows] OS) verwenden, um ein Feld schnell zu finden.

1. Klicken Sie **[!UICONTROL OK]**, um die Modulkonfiguration zu speichern.

1. Klicken Sie mit der rechten Maustaste auf das Modul **[!UICONTROL Umbenennen]**, geben Sie dann einen Namen ein, der beschreibt, was das Modul tun soll (z. B. „Nach Aufgabe suchen„), und klicken Sie dann auf **[!UICONTROL OK]**.

   Der Name wird direkt unter dem Modul angezeigt. Darunter finden Sie [!DNL Workfront Fusion] kurze Beschreibung der Art der Aktion, die vom Modul ausgeführt wird.

   ![](assets/module-renamed-wf.png)

1. Fahren Sie mit [Hinzufügen und konfigurieren Sie das zweite Modul](#add-and-configure-the-second-module) fort.

## Hinzufügen und Konfigurieren des zweiten Moduls

1. Bewegen Sie den Mauszeiger über den Teilkreis rechts neben dem Modul und klicken Sie dann auf **[!UICONTROL Weitere Module hinzufügen]**.
1. Wählen Sie [!DNL Adobe Workfront] aus der Liste der Programme und dann das Modul **[!UICONTROL Objekt konvertieren]** aus.
1. Wählen [!UICONTROL  im Feld ] die gleiche Workfront-Verbindung aus, die Sie im vorherigen Modul verwendet haben.
1. Wählen Sie im Feld **[!UICONTROL Datensatztyp]** die Option **[!UICONTROL Aufgabe]** aus, da das Modul eine Aufgabe konvertiert.
1. Wählen Sie im **[!UICONTROL Konvertieren in]** die Option **Projekt** aus.
1. Klicken Sie neben dem Feld Aufgaben-ID auf den Umschalter Zuordnung , um es zu aktivieren.

   Der Umschalter wird blau, wenn er aktiviert ist. Auf diese Weise können Sie die Aufgaben-ID aus dem vorherigen Modul zuordnen.

   ![Umschalter für Zuordnung](assets/map-toggle.png)
1. Klicken Sie auf **[!UICONTROL Feld]** Aufgaben-ID“.

   Es öffnet sich ein Bedienfeld, in dem Sie auswählen können, was als ID der Aufgabe verwendet werden soll, die Sie in ein Projekt konvertieren möchten. Da Sie die Zuordnung aktiviert haben, enthält das Bedienfeld Ausgaben aus allen vorherigen Modulen. Sie haben ID als Ausgabe des vorherigen Moduls ausgewählt, sodass es jetzt im Bedienfeld verfügbar ist.

   Dieses Bedienfeld wird als Zuordnungs-Bedienfeld bezeichnet. Weitere Informationen zum Zuordnungsbereich finden Sie unter [Zuordnen von Informationen von einem Modul zu einem anderen](/help/quicksilver/workfront-fusion/mapping/map-information-between-modules.md).
1. Wählen **ID** im Zuordnungsbereich aus.

   Im Feld ID wird ein ID-Block angezeigt. Es zeigt die Nummer des Moduls, dem es zugeordnet ist, und das Feld, das zugeordnet ist.

   ![Map ID](assets/map-id.png)

1. Klicken Sie auf das **Vorlagen** ID), geben Sie den Namen der Workfront-Vorlage ein, die Sie für dieses Projekt verwenden möchten, und wählen Sie sie aus, wenn sie in der Liste angezeigt wird.
1. Klicken Sie **[!UICONTROL OK]**, um die Modulkonfiguration zu speichern.

1. Klicken Sie mit der rechten Maustaste auf das Modul **[!UICONTROL Umbenennen]**, geben Sie dann einen Namen ein, der beschreibt, was das Modul tun soll (z. B. „In Projekt konvertieren„), und klicken Sie dann auf **[!UICONTROL OK]**.

1. Fahren Sie mit [Testen des Szenarios](#test-the-scenario) fort.

## Testen des Szenarios

Bevor Sie Ihr Szenario aktivieren, müssen Sie es testen, indem Sie es mindestens einmal ausführen und die Ergebnisse anzeigen. Auf diese Weise können Sie verstehen, wie Daten durch das Szenario fließen, und Fehler finden.

Bei diesem Szenario würde ein erfolgreicher Test dazu führen, dass die neue Aufgabe gefunden und in ein Projekt konvertiert wird.

1. Klicken Sie **[!UICONTROL Einmal ausführen]** in der linken unteren Ecke des Szenario-Editors.
1. Klicken Sie nach der Ausführung des Szenarios auf den Bubble über dem ersten Modul, um Informationen über das vom Modul verarbeitete Datenpaket anzuzeigen, einschließlich der Daten, die aus der vom Modul zurückgegebenen Aufgabe abgerufen wurden.

1. Klicken Sie auf die Blase „Ausführungs-Inspektor“ über dem zweiten Modul, um die Eingabe (die Aufgabe) und die Ausgabe (das konvertierte Projekt) anzuzeigen.

   Weitere Informationen zu den Daten in den Inspektionsblasen finden Sie unter:

   * Allgemeine Informationen finden Sie unter [Ausführungsfluss von Szenarien in [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-flow.md).
   * Informationen zu verarbeiteten Bundles finden Sie unter [Szenarioausführung, Zyklen und Phasen in [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. Klicken Sie [!DNL Workfront Fusion] auf **[!UICONTROL Speichern]** in der linken unteren Ecke, um den Fortschritt des Szenarios zu speichern.

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

Der letzte Schritt beim Erstellen eines Szenarios besteht darin, es zu aktivieren.

Da dieses Szenario nach einer bestimmten Aufgabe sucht, ist es nicht erforderlich, sie zu aktivieren. Durch die Aktivierung eines Szenarios wird es nach einem Zeitplan ausgeführt oder wenn eine bestimmte Aktion in einem Programm stattfindet. Nachdem Sie ein Szenario aktiviert haben, wird es standardmäßig alle 15 Minuten ausgeführt. Sie können dies ändern, indem Sie festlegen, wann und wie oft die Ausführung erfolgen soll.

Weitere Informationen zum Aktivieren von Szenarien finden Sie unter [Aktivieren oder Deaktivieren eines Szenarios in [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

Weitere Informationen zu Zeitplänen finden Sie unter [Planen eines Szenarios in [!UICONTROL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md).

## Nächste Schritte

* [Ein Trigger-Modul hinzufügen](/help/quicksilver/workfront-fusion/get-started/build-practice-scenarios/add-trigger-to-simple-scenario.md), damit das Szenario regelmäßig nach neuen Anfragen suchen und sie in Projekte konvertieren kann.
* Fügen Sie einen Webhook hinzu, damit das Szenario jedes Mal ausgeführt werden kann, wenn eine Anfrage eingegeben wird.
* Fügen Sie einen Filter hinzu, um sicherzustellen, dass nur bestimmte Anfragen in Projekte konvertiert werden.
* Fügen Sie eine Funktion hinzu, die den Namen des neuen Projekts anpasst.
* Fügen Sie eine Fehlerbehandlung hinzu, um sicherzustellen, dass das Szenario fehlersicher ist.
