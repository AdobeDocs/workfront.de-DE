---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Erstellen und Bearbeiten von Initiativen im Szenario-Planer
description: Wenn Sie den Adobe Workfront-Szenario-Planer verwenden, können Sie Initiativen in einem von Ihnen erstellten oder für Sie freigegebenen Plan erstellen. Durch die Erstellung von Initiativen können Sie zeigen, wie kleinere Organisationseinheiten zur Fertigstellung des Plans beitragen. Wenn Ihr Unternehmen beispielsweise über einen Plan für die nächsten drei Jahre verfügt, um einen neuen Markt zu erschließen, können Sie innerhalb dieses Plans Initiativen für jede Abteilung erstellen, um abzuschätzen, ob die einzelnen Abteilungen Personen und Budgets benötigen, um diesen Plan durchzuführen.
author: Alina
feature: Workfront Scenario Planner
exl-id: a811bad0-d3c0-4cba-8b78-d9a14ffc8482
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '1626'
ht-degree: 0%

---

# Erstellen und Bearbeiten von Initiativen im [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Bei Verwendung des [!UICONTROL Adobe Workfront-Szenario-Planers] können Sie Initiativen in einem Plan erstellen, den Sie erstellt haben oder der für Sie freigegeben wurde. Durch die Erstellung von Initiativen können Sie zeigen, wie kleinere Organisationseinheiten zur Fertigstellung des Plans beitragen. Wenn Ihr Unternehmen beispielsweise über einen Plan für die nächsten drei Jahre verfügt, um einen neuen Markt zu erschließen, können Sie innerhalb dieses Plans Initiativen für jede Abteilung erstellen, um abzuschätzen, ob die einzelnen Abteilungen Personen und Budgets benötigen, um diesen Plan durchzuführen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>Neu: Ultimate </p></li>
   <p>Der Szenario-Planer ist für die neuen Workfront Select- oder Workfront Prime-Pläne nicht verfügbar. </p>
   <li><p>Aktuell: [!UICONTROL Business] oder höher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>Neu: Licht oder höher</p> 
   <p>Aktuell: [!UICONTROL Review] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td>Produkt* </td> 
   <td> <ul><li><p>Für die neuen Workfront-Pläne:</p><p> Adobe Workfront</li></p>
   <li><p>Für die aktuellen Workfront-Pläne: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront-Szenario-Planer</p></li></ul>

<p>Weitere Informationen finden Sie unter <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Für die Verwendung des [!DNL Scenario Planner]</a> erforderlichen Zugriff. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Zugriffsebene </td> 
   <td> <p>Zugriff auf [!UICONTROL Bearbeiten] [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektberechtigungen </p> </td> 
   <td> <p>[!UICONTROL Berechtigungen für einen Plan verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff auf einen Plan finden Sie unter <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Anfordern des Zugriffs auf einen Plan in der [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen für die Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Sie müssen einen Plan erstellen oder ein anderer Benutzer muss einen Plan für Sie freigeben, bevor Sie eine Initiative in diesem Plan erstellen können. Informationen zum Erstellen von Plänen finden Sie unter [Erstellen und Bearbeiten von Plänen in der [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Weitere Informationen zu Initiativen finden Sie unter [Übersicht über Initiativen in der [!DNL Scenario Planner]](../scenario-planner/initiatives-overview.md).

## Initiativen erstellen

Sie können Initiativen wie folgt erstellen:

* Von Grund auf neu.
* Importieren von Projekten in einen Plan

  Informationen zum Importieren von Projekten als Initiativen in einem Plan finden Sie unter [Importieren von Projekten in Pläne in der  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Durch Kopieren vorhandener Initiativen.

  Informationen zum Kopieren von Initiativen finden Sie unter [Kopieren von Initiativen in der  [!DNL Scenario Planner]](../scenario-planner/copy-initiatives.md).

So erstellen Sie von Grund auf neue Initiativen:

{{step1-to-scenario-planner}}

1. Klicken Sie auf den Namen des Plans, für den Sie eine Initiative erstellen möchten.
1. Klicken Sie auf das Symbol **+** links neben **[!UICONTROL Neue Initiative]** .

   Oder

   Klicken Sie auf das Dropdownmenü **[!UICONTROL Neue Initiative]** und wählen Sie entweder **[!UICONTROL Neue Initiative]** oder **[!UICONTROL Projekte importieren].**

1. Geben Sie im Feld **[!UICONTROL Untitled Initiative]** einen Namen für Ihre Initiative ein und drücken Sie dann die Eingabetaste oder klicken Sie auf eine beliebige Stelle auf der Seite.

   Die Initiative wird auf der Zeitleiste des Plans als blaue Leiste angezeigt. Standardmäßig beträgt die Dauer einer Initiative einen Monat und beginnt immer am ersten Monat des Plans.

1. (Optional) Ziehen Sie die Trennleiste zwischen dem linken Bedienfeld und der Timeline, um die Größe des linken Bedienfelds zu ändern.

1. (Optional) Ziehen Sie das Ende der Initiativleiste in den Arbeitsbereich, um die Dauer auf mehr als einen Monat zu verlängern, und geben Sie sie an die Stelle frei, an der der Endmonat der Initiative liegen soll.
1. (Optional und bedingt) Wenn die Dauer der Initiative kürzer ist als die des Plans, ziehen Sie die Initiativleiste an eine andere Position auf der Zeitleiste des Plans, um sie in einen anderen Zeitrahmen zu verschieben.

   ![](assets/move-initiative-back-and-forth-on-the-timeline-350x71.png)

   >[!IMPORTANT]
   >
   >Sie können nur eine Dauer in Monaten auswählen. Die Dauer einer Initiative, die Sie von Grund auf neu erstellen, kann die Dauer des Plans niemals überschreiten.

1. (Optional) Wählen Sie aus dem Dropdownmenü **[!UICONTROL Monat]** eine der folgenden Optionen aus, um die Zeitleiste des Plans zu ändern:

   | Dropdown-Menüoption | Beschreibung |
   |---|---|
   | [!UICONTROL Monat] | Zeigt die Timeline nach Monat an. Dies ist die Standardoption für einen Einjahresplan. |
   | [!UICONTROL Quartal] | Zeigt die Timeline vierteljährlich an. Diese Option ist nur verfügbar, wenn die [!UICONTROL Laufzeit] des Plans 3 oder 5 Jahre beträgt. Dies ist die Standardoption für einen Dreijahresplan. |
   | [!UICONTROL Year] | Zeigt die Timeline nach Jahr an. Diese Option ist nur verfügbar, wenn die [!UICONTROL Laufzeit] des Plans 5 Jahre beträgt. Dies ist die Standardoption für einen Fünfjahresplan. |


1. (Optional) Scrollen Sie von links nach rechts, um die gesamte Dauer der Initiative anzuzeigen.
1. (Optional) Klicken Sie auf die Indikatorlinie **[!UICONTROL Heute]** , um zum aktuellen Datum zurückzukehren.

   ![](assets/today-indicator-350x160.png)

   >[!TIP]
   >
   >Wenn Ihr Plan in der Zukunft oder in der Vergangenheit liegt und das aktuelle Datum nicht enthält, wird der Indikator Heute nicht angezeigt.

1. Klicken Sie auf die Leiste einer Initiative. Das Bedienfeld für die Details der Initiative wird rechts geöffnet.

   ![](assets/initiative-details-panel-multiple-months-350x626.png)

   Geben Sie die folgenden Informationen an oder überprüfen Sie sie:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Dauer der Initiative</td> 
      <td>Die Dauer der Initiative in Monaten. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Start- und Enddaten</td> 
      <td>Beginn und Ende der Initiative.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Abschnitt "Erforderliche Auftragsrollen" </td> 
      <td> <p>Klicken Sie auf das Feld <strong>[!UICONTROL Eingabe-Auftrag starten]</strong> und wählen Sie eine Rolle aus der Liste aus oder beginnen Sie mit der Eingabe des Namens einer <span>n aktiven</span> Auftragsrolle. </p> <p><span>Je nachdem, ob der Plan für die Verwendung von FTEs oder Stunden eingerichtet ist, fügt </span> die Anzahl der für diese Initiative benötigten Arbeitsplatzrollen in FTE <span><span> oder Stunden</span></span><span> für jeden Monat in der Initiative hinzu</span>. <span>Die ersten drei Monate der Initiative werden standardmäßig angezeigt.</span></p> <p><span>Durch Aktualisieren der Informationen zur Rolle "Job"für die Initiative werden auch die erforderlichen Informationen zur Rolle "Job"für den Plan aktualisiert.</span> </p> <p>Informationen zum Einrichten des Plans zur Verwendung von FTE oder Stunden finden Sie unter <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Erstellen und Bearbeiten von Plänen in der [!DNL Scenario Planner]</a>. </p>
      <p><b>WICHTIG</b></p>  
      <p>Für alle Berechnungen im [!DNL Scenario Planner] verwendet [!DNL Workfront] den folgenden Wert: 1 FTE = 8 Stunden. </p>

   <p><b>TIPP</b></p>

   <ul> 
       <li> <p><span>Verwenden Sie die [!UICONTROL Tab]-Taste, um zum nächsten Monat zu wechseln.</span> </p> </li> 
      <li> <p> Alle <span>aktiven</span> Vorgangsrollen im System werden angezeigt, wenn Sie auf dieses Feld klicken. </p> </li> 
       <li> <p>Zuerst werden die Stellenrollen angezeigt, die den Stellenrollen des Plans bereits hinzugefügt wurden. Informationen zum Hinzufügen der verfügbaren Auftragsrollen zu einem Plan finden Sie unter <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Erstellen und Bearbeiten von Plänen im Szenario-Planer</a>. </p> </li> 
       <li> <p>[!DNL Workfront] ist der Ansicht, dass ein Vollzeitäquivalent von 160 Stunden pro Monat ist. </p> <p>Für alle Berechnungen im Szenario-Planer verwendet Workfront den folgenden Wert: 1 FTE = 8 Stunden. </p></li> 
      </ul> </p> <p>Sie können eine Zahl unter 1 FTE oder Dezimalzahlen für FTE <span>oder </span> <span>Stunden</span> eingeben. Beispielsweise würde eine 0,5-Beraterrolle bedeuten, dass ein Berater die Hälfte seiner FTE (in der Regel 4 Stunden, wobei 8 Stunden 1 FTE betragen) für die Arbeit an dieser Initiative einsetzt. </p>  </td> 
     </tr> 
     <tr> 
      <td rowspan="3" role="rowheader">Kostenbereich</td> 
      <td> <p>Die Gesamtkosten der Initiative werden rechts neben dem Abschnitt [!UICONTROL Kosten] angezeigt. [!DNL Workfront] berechnet die Kosten einer Initiative anhand der folgenden Formel:</p> <p><code>[!UICONTROL Initiative Costs] = [!UICONTROL Fixed Costs] + [!UICONTROL People] Costs</code> </p> </td> 
     </tr> 
     <tr> 
      <td> <p>Geben Sie im Feld <strong>[!UICONTROL Feste Kosten]</strong> manuell einen ungefähren Schätzwert ein, was Ihrer Meinung nach die Durchführung dieser Initiative kosten wird. Dies sollte keine Kosten im Zusammenhang mit den für die Initiative geschätzten Arbeitsplatzrollen umfassen.</p> <p><span>Geben Sie für jeden Monat der Initiative einen Betrag ein, indem Sie bei Verwendung der Tabulatortaste von einem Monat zum nächsten wechseln.</span> </p> </td> 
     </tr> 
     <tr> 
      <td> 
       <div> 
        <p>Je nachdem, ob der Plan für die Verwendung von FTE oder Stunden eingerichtet ist, verwendet [!UICONTROL Workfront] die folgenden Formeln zur Berechnung der [!UICONTROL People Cost]:</p> 
        <ul> 
         <li> <p>Bei Verwendung von FTE: </p> <p><code>[!UICONTROL People Costs] = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, wobei 160 die Gesamtzahl der Arbeitsstunden pro Monat ist. </p> </li> 
         <li> <p style="font-weight: normal;">Bei Verwendung von Stunden: </p> <p style="font-weight: normal;"><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> <p style="font-weight: normal;">Informationen zum Einrichten des Plans zur Verwendung von Stunden oder FTE finden Sie unter <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Erstellen und Bearbeiten von Plänen im Szenario-Planer</a>.</p> </li> 
        </ul> 
        <p>Die Personenkosten werden in der Basiswährung berechnet, die in Ihren Wechselkursvorlieben ausgewählt ist. Informationen zu Wechselkursen finden Sie unter <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Einrichten von Wechselkursen</a>.</p> 
        <p>Durch die Aktualisierung der Kosteninformationen für eine Initiative wird auch der [!UICONTROL Kosten]-Bereich für den Plan aktualisiert. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"> <p style="font-weight: normal;">Nachdem Sie die erforderliche Rolle und Kostenwerte für Ihre Initiative definiert und die Dauer der Initiative geändert haben, kann eines der folgenden Szenarien eintreten:</p> 
       <ul> 
        <li> <p style="font-weight: normal;">Wenn Sie die Initiative verkürzen, entfernt [!DNL Workfront] den erforderlichen Betrag an Ressourcen und die Kosten, die mit der aus dem Plan entfernten Zeit verbunden sind. Die Jobrollen verbleiben im Plan, haben jedoch keine erforderliche FTE oder <span data-mc-edit-date="2021-04-19T13:46:01.5004065-04:00" data-mc-editor="alinawilson" data-mc-comment="drafted, yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-19T13:45:58.7938344-04:00">Stunden</span>. Die verfügbaren Mittel für den Plan und den Haushalt bleiben unverändert.<br>Informationen zum Aktualisieren von Informationen zum Plan finden Sie unter <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Erstellen und Bearbeiten von Plänen im [!DNL Scenario Planner]</a>. </p> </li> 
        <li> <p style="font-weight: normal;">Wenn Sie die Initiative verlängern, müssen Sie die Anzahl der Arbeitsplätze und die Kosten für die neu hinzugefügten Monate auf der Initiative angeben. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Net Value] Abschnitt</td> 
      <td>Geben Sie im Abschnitt <strong>[!DNL Net Value]</strong> manuell einen groben Schätzwert in das Feld <strong>[!UICONTROL Geplanter Nutzen]</strong> ein. Das ist Ihrer Meinung nach der Nutzen, den die Verwirklichung dieser Initiative bringen wird. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Wenn Sie bereits die Anzahl der Arbeitsplätze und das Budget für Ihren Plan sowie die Anzahl der Arbeitsplätze und die Kosten für die Initiative, die Sie bearbeiten, und für alle darüber liegenden Initiativen festgelegt haben und alle die von Ihnen für den Plan angegebenen Beträge überschreiten, kann [!DNL Workfront] feststellen, dass Sie nicht über genügend Ressourcen verfügen, um die Initiative abzuschließen. [!DNL Workfront] markiert dies als Konflikt beim Versuch, diese Initiative zu erreichen, und zeigt sie als roten Balken an. Alle Initiativen, die auf die konfliktbehaftete Initiative folgen, werden rot hinterlegt. Möglicherweise müssen Sie einige Anforderungen Ihrer Initiativen anpassen, beginnend mit der ersten, die über unzureichende Ressourcen verfügt. Informationen zum Anpassen von in Konflikt stehenden Initiativen finden Sie unter [Beheben von Initiativkonflikten im  [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. (Optional) Bewegen Sie den Mauszeiger über den Namen einer Auftragsrolle und klicken Sie dann auf das Symbol **[!UICONTROL Papierkorb]** ![](assets/delete.png) , um sie aus der Initiative zu entfernen.

1. (Bedingt) Wenn Sie Änderungen an der Initiative vorgenommen haben, klicken Sie auf **[!UICONTROL Anwenden]**.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Add more steps here as you can do more in the Initiative box over time)
   </MadCap:conditionalText>
   -->

1. (Bedingt) Wenn Sie keine Änderungen vorgenommen haben, klicken Sie auf das Symbol **X** oben rechts im Detailbereich der Initiative, um es zu schließen.
1. (Optional) Aktualisieren Sie die Priorität Ihrer Initiativen.

   Weitere Informationen zur Priorisierung von Initiativen finden Sie unter [Aktualisieren von Initiativprioritäten im Szenario-Planer](../scenario-planner/prioritize-initiatives.md).

   >[!TIP]
   >
   >Initiativen, die zuerst in der Liste aufgeführt werden, haben eine höhere Priorität und erhalten Ressourcen vor den Initiativen, die unten in der Liste aufgeführt sind.

1. Klicken Sie auf **[!UICONTROL Plan speichern]**.

   Die Initiative ist jetzt in Ihrem Plan enthalten.

   Informationen zum Löschen von Initiativen aus einem Plan finden Sie unter [Löschinitiativen in der Datei [!DNL Scenario Planner]](../scenario-planner/delete-initiatives.md).
