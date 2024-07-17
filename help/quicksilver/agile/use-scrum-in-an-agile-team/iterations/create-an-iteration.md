---
product-area: agile-and-teams
navigation-topic: iterations
title: Iteration erstellen
description: Iterationen sind eine Schlüsselkomponente für Scrum-agile-Teams bei der Planung der Arbeitskapazität. [!DNL Adobe Workfront] ermöglicht es Scrum agile Teams, ihre Arbeit zu verwalten, indem mehrere Iterationen erstellt werden, um Teamanforderungen gerecht zu werden.
author: Lisa
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: ddff70b61a2c3b3479e278bb3bb8628ac83f5c97
workflow-type: tm+mt
source-wordcount: '1057'
ht-degree: 0%

---

# Iteration erstellen

Iterationen sind eine Schlüsselkomponente für Scrum-agile-Teams bei der Planung der Arbeitskapazität. Mit [!DNL Adobe Workfront] können Scrum-agile-Teams ihre Arbeit verwalten, indem sie mehrere Iterationen erstellen, um Teamanforderungen gerecht zu werden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Review] oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um herauszufinden, welchen Plan oder welchen Lizenztyp Sie haben.

## Iteration hinzufügen

Verwenden Sie die Funktion [!UICONTROL Iteration hinzufügen] , um schnell eine Iteration zu erstellen und Aufgaben und Probleme später hinzuzufügen.

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Teams]**.![](assets/main-menu-icon.png)

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Klicken Sie auf der Registerkarte **[!UICONTROL Iterationen]** auf **[!UICONTROL Iteration hinzufügen]**.\
   ![](assets/add-iteration-adobe-350x275.png)

1. Geben Sie Folgendes an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Iteration Name]</strong></td> 
      <td>Geben Sie den Namen der Iteration ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Ziel]</strong></td> 
      <td>Fügen Sie Ziele hinzu, die Sie für die Iteration haben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Startdatum]</strong></td> 
      <td>Geben Sie das Datum ein, an dem die Iteration beginnen soll.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Enddatum]</strong></td> 
      <td><p>Geben Sie das Datum ein, an dem die Iteration enden soll. [!DNL Workfront] empfiehlt, ein Enddatum festzulegen, das nicht länger als 4 Wochen ab dem Startdatum ist.</p><p>Tipp: Stellen Sie sicher, dass Sie einen Arbeitstag als Enddatum auswählen. In den Berechnungen verwendet das Diagramm nur Arbeitstage.<br>Standardmäßig verwendet das Diagramm für die Aufschlüsselung den Standardzeitplan zur Definition von Arbeitstagen (wie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Zeitplan erstellen</a> beschrieben). Oder um Team-spezifische, nicht-arbeitstägliche Tage einzubinden, können agile Teams einen alternativen Zeitplan verwenden (wie unter "Definieren eines alternativen Team-Zeitplans für Niederschlagskarten"in <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Erstellen eines agilen Teams</a> beschrieben).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Geben Sie die Kapazität für die Iteration an. Dies ist die Anzahl der Punkte oder Stunden, die Ihr Team bei der Iteration erreichen kann. Die Zahl, die Sie eingeben, muss größer oder gleich der Anzahl der Punkte oder Stunden ab der Summe aller Geschichten in der Iteration sein.<br>[!DNL Workfront] füllt dieses Feld standardmäßig mit einer Kapazität von 50. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>Geben Sie den Fokusprozentsatz des Teams an. Wenn sich alle Mitglieder des Teams vollständig auf diese Iteration konzentrieren würden, wäre der Fokus 100 %.<br>[!DNL Workfront] füllt dieses Feld standardmäßig mit 100 %. </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Senden]**. Nachdem Sie nun eine Iteration erstellt haben, müssen Sie Geschichten hinzufügen. Weitere Informationen finden Sie unter [Meldungen zu einer vorhandenen Iteration hinzufügen](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Planen Sie eine Iteration auf der Registerkarte [!UICONTROL Backlog] .

Verwenden Sie die Funktion [!UICONTROL Iteration planen] , um eine Iteration mithilfe von Aufgaben im Rückstadium zu erstellen.

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Teams]**.![](assets/main-menu-icon.png)

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Team-Symbol wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen Sie im linken Bereich **[!UICONTROL Rückprotokoll]** aus. Klicken Sie dann auf **[!UICONTROL Iteration planen]**.

1. Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Iteration Name]</strong></td> 
      <td>Geben Sie einen Namen für die Iteration an.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Startdatum]</strong></td> 
      <td> Geben Sie das Datum an, an dem die Iteration beginnen soll.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Enddatum]</strong> </td> 
      <td><p>Geben Sie das Datum an, an dem die Iteration enden soll. [!DNL Workfront] empfiehlt, ein Enddatum festzulegen, das nicht länger als 4 Wochen ab dem Startdatum ist.</p><p>Tipp: Stellen Sie sicher, dass Sie einen Arbeitstag als Enddatum auswählen. In den Berechnungen verwendet das Diagramm nur Arbeitstage.<br>Standardmäßig verwendet das Diagramm für die Aufschlüsselung den Standardzeitplan zur Definition von Arbeitstagen (wie unter <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Zeitplan erstellen</a> beschrieben). Oder um Team-spezifische Nicht-Arbeitstage zu integrieren, können agile Teams einen alternativen Zeitplan verwenden (wie unter <a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md" class="MCXref xref">Verwenden eines alternativen Teamzeitplans für die Abbruchdiagramme</a> beschrieben).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>Geben Sie den Fokusprozentsatz des Teams an. Wenn sich alle Mitglieder des Teams vollständig auf diese Iteration konzentrieren würden, wäre der Fokus 100 %.<br>[!DNL Workfront] füllt dieses Feld mit dem Durchschnittswert aus den vergangenen Ausführungen Ihres Teams. Wenn dies die erste Iteration Ihres Teams ist, ist dieser Feldwert standardmäßig 0.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Geben Sie die Kapazität für die Iteration an. Dies ist die Anzahl der Punkte oder Stunden, die Ihr Team bei der Iteration erreichen kann. Die Zahl, die Sie eingeben, muss größer oder gleich der Anzahl der Punkte oder Stunden ab der Summe aller Geschichten in der Iteration sein.<br>[!DNL Workfront] füllt dieses Feld mit dem Durchschnittswert aus den vergangenen Ausführungen Ihres Teams. Wenn dies die erste Iteration Ihres Teams ist, ist dieser Feldwert standardmäßig 0.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Ziel]</strong></td> 
      <td> Geben Sie ein Ziel für die Iteration an. Dieses Feld ist nicht erforderlich.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wählen Sie Meldungen aus, die Sie der Iteration jetzt hinzufügen möchten, oder Sie können diesen Schritt überspringen und einer Iteration zu einem späteren Zeitpunkt Meldungen hinzufügen. Die Geschichten oben im Rückstand haben eine höhere Priorität. Geschichten werden grün hervorgehoben, wenn sie in die Kapazität passen; sie werden rot hervorgehoben, wenn sie dies nicht tun.\
   Sie können sowohl Aufgaben als auch Probleme zu einer einzelnen Iteration hinzufügen:

   * **So fügen Sie der Iteration Aufgaben hinzu:** Stellen Sie auf der Registerkarte **[!UICONTROL Rückprotokoll]** sicher, dass die Registerkarte **[!UICONTROL Meldungen]** ausgewählt ist (diese Registerkarte ist bei Ansicht des Rückstands standardmäßig ausgewählt). Wählen Sie die Meldungen aus, die Sie der Iteration hinzufügen möchten.\

     Wenn Sie einer Iteration Aufgaben hinzufügen, wird das Startdatum der Aufgabe wie in [[!UICONTROL Grundlegendes] darüber berechnet, wie die Aufgabenstartdaten berechnet werden, wenn sie einer Iteration hinzugefügt werden](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration).

   * **Um der Iteration Probleme hinzuzufügen:** Klicken Sie auf der Registerkarte **[!UICONTROL Rückprotokoll]** auf die Registerkarte **[!UICONTROL Probleme]** . Wählen Sie die Probleme aus, die Sie der Iteration hinzufügen möchten.

1. Klicken Sie auf **[!UICONTROL Speichern].**
Die Iteration wird erstellt.

1. (Optional) Informationen zum Hinzufügen von Meldungen zu einer vorhandenen Iteration finden Sie unter [Hinzufügen von Meldungen zu einer vorhandenen Iteration](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Erfahren Sie, wie Aufgabenstartdaten berechnet werden, wenn sie einer Iteration hinzugefügt werden {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

Wenn Sie eine Aufgabe als Geschichte zu einer Iteration hinzufügen, wird für jede Geschichte die Beschränkung [!UICONTROL Must Finish On task] verwendet. In den meisten Fällen wird das geplante Startdatum der Aufgabe anhand der folgenden Formel berechnet:

[!UICONTROL Iteration End Date] minus (-) [!UICONTROL Task Duration] gleich (=) [!UICONTROL Task Scheduled Start Date]

Das [!UICONTROL Projektende-Datum] wird anstelle des   wenn das Projektstartdatum nach dem Iterationsstartdatum liegt und das Projektende-Datum nach dem Iterationsenddatum liegt.

Sie können einzelne Scrum-Teams so konfigurieren, dass die Projektdaten standardmäßig anstelle der Iterationsdaten verwendet werden. Weitere Informationen finden Sie im Abschnitt [Konfigurieren, wie Daten angewendet werden, wenn Arbeitselemente zu einer Iteration hinzugefügt werden](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) im Artikel [Konfigurieren von Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).
