---
product-area: agile-and-teams
navigation-topic: iterations
title: Iteration erstellen
description: Iterationen sind eine Schlüsselkomponente für Scrum-agile-Teams bei der Planung der Arbeitskapazität. [!DNL Adobe Workfront] ermöglicht es Scrum agile Teams, ihre Arbeit zu verwalten, indem mehrere Iterationen erstellt werden, um die Anforderungen des Teams zu erfüllen.
author: Lisa
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: 6f817ca39c7489b85673ff601faf440fe51ab72c
workflow-type: tm+mt
source-wordcount: '1049'
ht-degree: 0%

---

# Iteration erstellen

Iterationen sind eine Schlüsselkomponente für Scrum-agile-Teams bei der Planung der Arbeitskapazität. [!DNL Adobe Workfront] ermöglicht es Scrum agile Teams, ihre Arbeit zu verwalten, indem mehrere Iterationen erstellt werden, um die Anforderungen des Teams zu erfüllen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Review] oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Iteration hinzufügen

Verwenden Sie die [!UICONTROL Iteration hinzufügen] , um schnell eine Iteration zu erstellen und Aufgaben und Probleme später hinzuzufügen.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Teams]**.

1. (Optional) Klicken Sie auf die **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Im **[!UICONTROL Iterationen]** Registerkarte, klicken Sie auf **[!UICONTROL Iteration hinzufügen]**.\
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
      <td><p>Geben Sie das Datum ein, an dem die Iteration enden soll. [!DNL Workfront] empfiehlt, ein Enddatum festzulegen, das nicht länger als 4 Wochen ab dem Startdatum ist.</p><p>Tipp: Stellen Sie sicher, dass Sie einen Arbeitstag als Enddatum auswählen. In den Berechnungen verwendet das Diagramm nur Arbeitstage.<br>Standardmäßig verwendet das Aufschlüsselungsdiagramm den Standardzeitplan zur Definition von Arbeitstagen (wie beschrieben in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Zeitplan erstellen</a>). Oder um Team-spezifische, nicht-arbeitstägliche Tage zu integrieren, können agile Teams einen alternativen Zeitplan verwenden (wie unter "Definieren eines alternativen Team-Zeitplans für Niederschlagskarten"in <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Erstellen eines agilen Teams</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Capacity]</strong></td> 
      <td> Geben Sie die Kapazität für die Iteration an. Dies ist die Anzahl der Punkte oder Stunden, die Ihr Team bei der Iteration erreichen kann. Die Zahl, die Sie eingeben, muss größer oder gleich der Anzahl der Punkte oder Stunden ab der Summe aller Geschichten in der Iteration sein.<br>[!DNL Workfront] füllt dieses Feld standardmäßig mit 50 Kapazität auf. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>Geben Sie den Fokusprozentsatz des Teams an. Wenn sich alle Mitglieder des Teams vollständig auf diese Iteration konzentrieren würden, wäre der Fokus 100 %.<br>[!DNL Workfront] Fügt dieses Feld standardmäßig mit 100 % vorab ein. </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **[!UICONTROL Einsenden]**. Nachdem Sie nun eine Iteration erstellt haben, müssen Sie Geschichten hinzufügen. Weitere Informationen finden Sie unter [Hinzufügen von Meldungen zu einer vorhandenen Iteration](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Planen Sie eine Iteration auf der [!UICONTROL Rückstand] tab

Verwenden Sie die [!UICONTROL Iteration planen] , um eine Iteration mithilfe von Aufgaben im Rückstand zu erstellen.

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Teams]**.

1. (Optional) Klicken Sie auf die **[!UICONTROL Switch Team]** icon ![Symbol &quot;Team wechseln&quot;](assets/switch-team-icon.png), wählen Sie entweder ein neues Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Auswählen **[!UICONTROL Rückstand]** im linken Bereich. Klicken Sie anschließend auf **[!UICONTROL Iteration planen]**.

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
      <td><p>Geben Sie das Datum an, an dem die Iteration enden soll. [!DNL Workfront] empfiehlt, ein Enddatum festzulegen, das nicht länger als 4 Wochen ab dem Startdatum ist.</p><p>Tipp: Stellen Sie sicher, dass Sie einen Arbeitstag als Enddatum auswählen. In den Berechnungen verwendet das Diagramm nur Arbeitstage.<br>Standardmäßig verwendet das Aufschlüsselungsdiagramm den Standardzeitplan zur Definition von Arbeitstagen (wie beschrieben in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Zeitplan erstellen</a>). Oder um Team-spezifische Nicht-Arbeitstage einzubinden, können agile Teams einen alternativen Zeitplan verwenden (wie unter <a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt--team-schedule-burndown-charts.md" class="MCXref xref">Verwenden eines alternativen Teamzeitplans für Startdiagramme</a>).</p></td> 
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

1. (Optional) Wählen Sie Meldungen aus, die Sie der Iteration jetzt hinzufügen möchten, oder Sie können diesen Schritt überspringen und einer Iteration zu einem späteren Zeitpunkt Meldungen hinzufügen. Die Geschichten oben im Rückstand haben eine höhere Priorität. Geschichten werden grün hervorgehoben, wenn sie in die Kapazität passen. sie sind rot hervorgehoben, wenn sie dies nicht tun.\
   Sie können sowohl Aufgaben als auch Probleme zu einer einzelnen Iteration hinzufügen:

   * **So fügen Sie der Iteration Aufgaben hinzu:** Im **[!UICONTROL Rückstand]** auf, stellen Sie sicher, dass die **[!UICONTROL Meldungen]** ausgewählt ist (diese Registerkarte ist bei Ansicht des Rückstands standardmäßig ausgewählt). Wählen Sie die Meldungen aus, die Sie der Iteration hinzufügen möchten.\

      Wenn Sie einer Iteration Aufgaben hinzufügen, wird das Startdatum der Aufgabe wie in [[!UICONTROL Grundlegendes] Berechnung der Aufgabenstartdaten beim Hinzufügen zu einer Iteration](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration).

   * **So fügen Sie der Iteration Probleme hinzu:** Im **[!UICONTROL Rückstand]** klicken Sie auf die **[!UICONTROL Probleme]** Registerkarte. Wählen Sie die Probleme aus, die Sie der Iteration hinzufügen möchten.

1. Klicken Sie auf **[!UICONTROL Speichern].**
Die Iteration wird erstellt.

1. (Optional) Informationen zum Hinzufügen von Meldungen zu einer vorhandenen Iteration finden Sie unter [Hinzufügen von Meldungen zu einer vorhandenen Iteration](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Erfahren Sie, wie Aufgabenstartdaten berechnet werden, wenn sie einer Iteration hinzugefügt werden {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

Wenn Sie einer Iteration eine Aufgabe als Geschichte hinzufügen, wird die [!UICONTROL Muss bei Aufgabe abgeschlossen sein] -Beschränkung wird für jede Geschichte verwendet. In den meisten Fällen wird das geplante Startdatum der Aufgabe anhand der folgenden Formel berechnet:

[!UICONTROL Iteration End Date] minus (-) [!UICONTROL Aufgabendauer] gleich (=) [!UICONTROL Geplantes Startdatum der Aufgabe]

Die [!UICONTROL Projektende] wird anstelle von verwendet, wenn das Projektstartdatum nach dem Iterationsstartdatum liegt und das Projektende-Datum nach dem Iterationsenddatum liegt.

Sie können einzelne Scrum-Teams so konfigurieren, dass die Projektdaten standardmäßig anstelle der Iterationsdaten verwendet werden. Weitere Informationen finden Sie im Abschnitt . [Konfigurieren der Anwendung von Datumsangaben beim Hinzufügen von Arbeitselementen zu einer Iteration](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) im Artikel [Konfigurieren von Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).
