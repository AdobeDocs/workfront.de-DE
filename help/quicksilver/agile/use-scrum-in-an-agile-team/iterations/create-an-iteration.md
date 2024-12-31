---
product-area: agile-and-teams
navigation-topic: iterations
title: Erstellen einer Iteration
description: Iterationen sind eine Schlüsselkomponente für agile Scrum-Teams bei der Planung der Arbeitskapazität. [!DNL Adobe Workfront] Scrum ermöglicht es agilen Teams, ihre Arbeit zu verwalten, indem sie mehrere Iterationen erstellen, um Team-Anforderungen zu erfüllen.
author: Lisa
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: d660707dd69fab78095eed1414092a7c909ba174
workflow-type: tm+mt
source-wordcount: '1051'
ht-degree: 0%

---

# Erstellen einer Iteration

Iterationen sind eine Schlüsselkomponente für agile Scrum-Teams bei der Planung der Arbeitskapazität. [!DNL Adobe Workfront] ermöglicht es agilen Scrum-Teams, ihre Arbeit zu verwalten, indem sie mehrere Iterationen erstellen, um Team-Anforderungen zu erfüllen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> <p>Neu: [!UICONTROL light] oder höher</p> 
   oder
   <p>Aktuell: [!UICONTROL Überprüfen] oder höher</p> </td> 
  </tr>
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Iteration hinzufügen

Verwenden Sie die Funktion [!UICONTROL Wiederholung hinzufügen], um schnell eine Iteration zu erstellen und später Aufgaben und Probleme hinzuzufügen.

{{step1-to-team}}

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Symbol Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Scrum-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Klicken Sie auf **[!UICONTROL Registerkarte]** Wiederholungen **[!UICONTROL auf „Wiederholung hinzufügen]**.
   ![](assets/add-iteration-adobe-350x275.png)

1. Geben Sie Folgendes an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Iterationsname]</strong></td> 
      <td>Geben Sie den Namen der Iteration ein.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Ziel]</strong></td> 
      <td>Fügen Sie alle Ziele hinzu, die Sie für die Iteration haben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Startdatum]</strong></td> 
      <td>Geben Sie das Datum ein, an dem die Iteration beginnen soll.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Enddatum]</strong></td> 
      <td><p>Geben Sie das Datum ein, an dem die Iteration enden soll. [!DNL Workfront] empfiehlt, ein Enddatum festzulegen, das nicht länger als 4 Wochen ab dem Startdatum liegt.</p><p>Tipp: Achten Sie darauf, einen Arbeitstag als Enddatum auszuwählen. Das Burndown-Diagramm verwendet bei seinen Berechnungen nur Arbeitstage.<br>Standardmäßig verwendet das Burndown-Diagramm den Standardzeitplan zum Definieren von Arbeitstagen (wie in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Zeitplan erstellen) </a>. Oder um teamspezifische arbeitsfreie Tage einzubinden, können Agile-Teams einen alternativen Zeitplan verwenden (wie unter „Definieren eines alternativen Team-Zeitplans für Burndown-Diagramme“ in <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">Erstellen eines agilen Teams</a> beschrieben).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Kapazität]</strong></td> 
      <td> Geben Sie die Kapazität für die Iteration an. Dies ist die Anzahl der Punkte oder Stunden, die Ihr Team in der Iteration erreichen kann. Die eingegebene Zahl muss größer oder gleich der Anzahl der Punkte oder Stunden ab der Summe aller Storys in der Iteration sein.<br>[!DNL Workfront] füllt dieses Feld standardmäßig mit 50 Kapazitäten aus. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL focus]</strong></td> 
      <td>Geben Sie den Fokusprozentsatz des Teams an. Wenn sich alle Mitglieder des Teams vollständig auf diese Iteration konzentrieren, würde der Fokus auf 100 % liegen.<br>[!DNL Workfront] füllt dieses Feld standardmäßig mit 100 % aus. </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **[!UICONTROL Senden]**. Nachdem Sie eine Iteration erstellt haben, müssen Sie Storys hinzufügen. Weitere Informationen finden Sie unter [Hinzufügen von Storys zu einer vorhandenen Iteration](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Planen einer Iteration auf der Registerkarte [!UICONTROL Auftragsbestand]

Verwenden Sie die Funktion [!UICONTROL Wiederholung planen], um eine Iteration mithilfe von Aufgaben in Ihrem Rückstand zu erstellen.

{{step1-to-team}}

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Team wechseln]** ![Symbol Team wechseln](assets/switch-team-icon.png) und wählen Sie dann entweder ein neues Scrum-Team aus dem Dropdown-Menü aus oder suchen Sie in der Suchleiste nach einem Team.

1. Wählen **[!UICONTROL im]** Bedienfeld „Auftragsbestand“ aus. Klicken Sie dann auf **[!UICONTROL Wiederholung planen]**.

1. Geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Iterationsname]</strong></td> 
      <td>Geben Sie einen Namen für die Iteration an.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Startdatum]</strong></td> 
      <td> Geben Sie das Datum an, an dem die Iteration beginnen soll.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Enddatum]</strong> </td> 
      <td><p>Geben Sie das Datum an, an dem die Iteration enden soll. [!DNL Workfront] empfiehlt, ein Enddatum festzulegen, das nicht länger als 4 Wochen ab dem Startdatum liegt.</p><p>Tipp: Achten Sie darauf, einen Arbeitstag als Enddatum auszuwählen. Das Burndown-Diagramm verwendet bei seinen Berechnungen nur Arbeitstage.<br>Standardmäßig verwendet das Burndown-Diagramm den Standardzeitplan zum Definieren von Arbeitstagen (wie in <a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">Zeitplan erstellen) </a>. Um teamspezifische arbeitsfreie Tage einzubinden, können agile Teams auch einen alternativen Zeitplan verwenden (siehe <a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md" class="MCXref xref">Verwenden eines alternativen Teamplans für Burndown-Diagramme</a>).</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL focus]</strong></td> 
      <td>Geben Sie den Fokusprozentsatz des Teams an. Wenn sich alle Mitglieder des Teams vollständig auf diese Iteration konzentrieren, würde der Fokus auf 100 % liegen.<br>[!DNL Workfront] füllt dieses Feld vorab mit dem Durchschnittswert aus den vorherigen Iterationen Ihres Teams. Wenn dies die erste Iteration Ihres Teams ist, ist dieser Feldwert standardmäßig 0.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Kapazität]</strong></td> 
      <td> Geben Sie die Kapazität für die Iteration an. Dies ist die Anzahl der Punkte oder Stunden, die Ihr Team in der Iteration erreichen kann. Die eingegebene Zahl muss größer oder gleich der Anzahl der Punkte oder Stunden ab der Summe aller Storys in der Iteration sein.<br>[!DNL Workfront] füllt dieses Feld vorab mit dem Durchschnittswert aus den vorherigen Iterationen Ihres Teams. Wenn dies die erste Iteration Ihres Teams ist, ist dieser Feldwert standardmäßig 0.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Ziel]</strong></td> 
      <td> Geben Sie ein Ziel für die Iteration an. Dieses Feld ist nicht erforderlich.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Wählen Sie Storys aus, um sie der Iteration jetzt hinzuzufügen. Alternativ können Sie diesen Schritt überspringen und einer Iteration zu einem späteren Zeitpunkt Storys hinzufügen. Die Geschichten am Anfang des Rückstands haben eine höhere Priorität. Geschichten werden grün hervorgehoben, wenn sie die gewünschte Kapazität haben. Wenn dies nicht der Fall ist, werden sie rot hervorgehoben.
Sie können einer einzigen Iteration sowohl Aufgaben als auch Probleme hinzufügen:

   * **Aufgaben zur Iteration hinzufügen:** Stellen Sie sicher, dass auf der Registerkarte **[!UICONTROL Backlog]** die Registerkarte **[!UICONTROL Storys]** ausgewählt ist (diese Registerkarte ist standardmäßig ausgewählt, wenn der Backlog angezeigt wird). Wählen Sie die Storys aus, die Sie der Iteration hinzufügen möchten.

     Wenn Sie Aufgaben zu einer Iteration hinzufügen, wird das Startdatum der Aufgabe wie unter [[!UICONTROL Erfahren Sie, wie ] Startdaten einer Aufgabe berechnet werden, wenn sie zu einer Iteration hinzugefügt werden](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration) beschrieben berechnet.

   * **So fügen Sie Probleme zur Iteration hinzu** Klicken Sie auf der Registerkarte **[!UICONTROL Auftragsbestand]** auf die Registerkarte **[!UICONTROL Probleme]**. Wählen Sie die Probleme aus, die Sie der Iteration hinzufügen möchten.

1. Klicken Sie auf **[!UICONTROL Speichern].**
Die Iteration wird erstellt.

1. (Optional) Informationen zum Hinzufügen von Storys zu einer vorhandenen Iteration finden Sie unter [Hinzufügen von Storys zu einer vorhandenen Iteration](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Verstehen, wie Aufgabenstarttermine berechnet werden, wenn sie zu einer Iteration hinzugefügt werden {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

Wenn Sie einer Iteration eine Aufgabe als Story hinzufügen, wird für jede Story die [!UICONTROL Muss abgeschlossen sein]-Einschränkung verwendet. In den meisten Fällen wird das geplante Startdatum der Aufgabe anhand der folgenden Formel berechnet:

[!UICONTROL Enddatum der Iteration] minus (-) [!UICONTROL Aufgabendauer] ist gleich (=) [!UICONTROL Geplantes Startdatum der Aufgabe]

Das [!UICONTROL Enddatum des Projekts] wird anstelle des   Wenn das Startdatum des Projekts nach dem Startdatum der Iteration liegt und das Enddatum des Projekts nach dem Enddatum der Iteration liegt.

Sie können einzelne Scrum-Teams so konfigurieren, dass sie standardmäßig die Projektdaten und nicht die Iterationsdaten verwenden. Weitere Informationen finden Sie im Abschnitt [Konfigurieren der Anwendung von Datumsangaben beim Hinzufügen von Arbeitselementen zu einer Iteration](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) im Artikel [Konfigurieren von Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).
