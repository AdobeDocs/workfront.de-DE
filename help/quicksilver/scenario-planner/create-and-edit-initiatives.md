---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Erstellen und Bearbeiten von Initiativen im Szenario-Planer
description: Wenn Sie den Adobe Workfront-Szenarioplaner verwenden, können Sie Initiativen in einem Plan erstellen, den Sie erstellt haben oder der für Sie freigegeben wurde. Durch die Erstellung von Initiativen können Sie zeigen, wie kleinere Organisationseinheiten zur Fertigstellung des Plans beitragen. Wenn Ihr Unternehmen beispielsweise einen Plan für die nächsten drei Jahre hat, um in einen neuen Markt zu expandieren, können Sie in diesem Plan für jede Abteilung Initiativen erstellen, um den Bedarf jeder Abteilung an Mitarbeitern und Budgets zur Umsetzung dieses Plans zu schätzen.
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

Wenn Sie den [!UICONTROL Adobe Workfront-Szenarioplaner] verwenden, können Sie Initiativen in einem Plan erstellen, den Sie erstellt haben oder der für Sie freigegeben wurde. Durch die Erstellung von Initiativen können Sie zeigen, wie kleinere Organisationseinheiten zur Fertigstellung des Plans beitragen. Wenn Ihr Unternehmen beispielsweise einen Plan für die nächsten drei Jahre hat, um in einen neuen Markt zu expandieren, können Sie in diesem Plan für jede Abteilung Initiativen erstellen, um den Bedarf jeder Abteilung an Mitarbeitern und Budgets zur Umsetzung dieses Plans zu schätzen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] Plan*</p> </td> 
   <td> <ul></li>
   <li><p>Neu: Ultimate </p></li>
   <p>Der Szenario-Planer ist für die neuen Workfront Select- oder Workfront Prime-Pläne nicht verfügbar. </p>
   <li><p>Aktuell: [!UICONTROL Business] oder höher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] Lizenz*</p> </td> 
   <td> <p>Neu: Licht oder höher</p> 
   <p>Aktuell: [!UICONTROL Überprüfen] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td>Produkt* </td> 
   <td> <ul><li><p>Für die neuen Workfront-Pläne:</p><p> Adobe Workfront</li></p>
   <li><p>Für die aktuellen Workfront-Pläne: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront-Szenarioplaner</p></li></ul>

<p>Weitere Informationen finden Sie unter <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Zugriff erforderlich, um die [!DNL Scenario Planner]</a> verwenden zu können. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Zugriffsebene </td> 
   <td> <p>[!UICONTROL Bearbeiten] Zugriff auf [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektberechtigungen </p> </td> 
   <td> <p>[!UICONTROL Manage]-Berechtigungen für einen Plan</p> <p>Informationen zum Anfordern zusätzlichen Zugriffs auf einen Plan finden Sie unter <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Anfordern des Zugriffs auf einen Plan im [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Dokumentation zu Zugriffsanforderungen für Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Sie müssen einen Plan erstellen, oder ein anderer Benutzer muss einen Plan mit Ihnen teilen, bevor Sie eine Initiative innerhalb dieses Plans erstellen können. Informationen zum Erstellen von Plänen finden Sie unter [Erstellen und Bearbeiten von Plänen in der [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Weitere Informationen zu Initiativen finden Sie unter [Initiativen - Übersicht in der [!DNL Scenario Planner]](../scenario-planner/initiatives-overview.md).

## Initiativen erstellen

Sie können Initiativen wie folgt erstellen:

* Von Grund auf.
* Durch Importieren von Projekten in einen Plan

  Informationen zum Importieren von Projekten als Initiativen in einen Plan finden Sie unter [Projekte in Pläne importieren in der [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Durch Kopieren bestehender Initiativen.

  Informationen zum Kopieren von Initiativen finden Sie unter [Kopieren von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/copy-initiatives.md).

So erstellen Sie Initiativen von Grund auf:

{{step1-to-scenario-planner}}

1. Klicken Sie auf den Namen des Plans, für den Sie eine Initiative erstellen möchten.
1. Klicken Sie links neben **Initiative** das Symbol **[!UICONTROL +]**

   Oder

   Klicken Sie auf das **[!UICONTROL Neue Initiative]** Dropdown-Menü und wählen Sie entweder **[!UICONTROL Neue Initiative]** oder **[!UICONTROL Projekte importieren].**

1. Geben Sie einen Namen für Ihre Initiative im Feld **[!UICONTROL Nicht benannte Initiative]** ein und drücken Sie dann die Eingabetaste, oder klicken Sie auf eine beliebige andere Stelle auf der Seite.

   Die Initiative wird in der Zeitleiste des Plans in einem blauen Balken angezeigt. Standardmäßig beträgt die Dauer einer Initiative einen Monat und beginnt immer im ersten Monat des Plans.

1. (Optional) Ziehen Sie die Trennleiste zwischen dem linken Bedienfeld und der Zeitleiste, um die Größe des linken Bedienfelds zu ändern.

1. (Optional) Ziehen Sie das Ende der Initiativleiste, um ihre Dauer auf mehr als einen Monat zu verlängern, und geben Sie sie an die Stelle frei, an der der Endmonat der Initiative sein soll.
1. (Optional und bedingt) Wenn die Dauer der Initiative kürzer als die des Plans ist, ziehen Sie die Initiativleiste per Drag-and-Drop an eine andere Position auf der Zeitleiste des Plans, um sie in einen anderen Zeitrahmen zu verschieben.

   ![](assets/move-initiative-back-and-forth-on-the-timeline-350x71.png)

   >[!IMPORTANT]
   >
   >Sie können nur eine Dauer in Monaten auswählen. Die Dauer einer von Ihnen neu erstellten Initiative darf nie die Dauer des Plans überschreiten.

1. (Optional) Wählen Sie aus **[!UICONTROL Dropdown]** Menü „Monat“ eine der folgenden Optionen aus, um die Zeitleiste des Plans zu ändern:

   | Dropdown-Menüoption | Beschreibung |
   |---|---|
   | [!UICONTROL Monat] | Zeigt die Zeitleiste nach Monat an. Dies ist die Standardoption für einen Ein-Jahres-Plan. |
   | [!UICONTROL Quartal] | Zeigt die Zeitleiste nach Quartal an. Diese Option ist nur verfügbar, wenn [!UICONTROL Laufzeit] des Plans 3 oder 5 Jahre beträgt. Dies ist die Standardoption für einen 3-Jahres-Plan. |
   | [!UICONTROL Jahr] | Zeigt die Zeitleiste nach Jahr an. Diese Option ist nur verfügbar, wenn [!UICONTROL Laufzeit] des Plans 5 Jahre beträgt. Dies ist die Standardoption für einen 5-Jahres-Plan. |


1. (Optional) Scrollen Sie von links nach rechts, um die gesamte Dauer der Initiative anzuzeigen.
1. (Optional) Klicken Sie auf die **[!UICONTROL Heute]**, um zum aktuellen Datum zurückzukehren.

   ![](assets/today-indicator-350x160.png)

   >[!TIP]
   >
   >Wenn Ihr Plan in der Zukunft oder in der Vergangenheit liegt und das aktuelle Datum nicht enthält, wird der Indikator Heute nicht angezeigt.

1. Klicken Sie auf den Balken einer Initiative. Das Bedienfeld mit den Details der Initiative wird auf der rechten Seite geöffnet.

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
      <td role="rowheader">Start- und Enddatum</td> 
      <td>Start- und Enddatum der Initiative</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erforderliche Aufgabengebiete </td> 
      <td> <p>Klicken Sie auf das Feld <strong>[!UICONTROL Start typing job role]</strong> und wählen Sie eine Rolle aus der Liste aus oder beginnen Sie mit der Eingabe des Namens <span> aktiven </span>. </p> <p><span>Je nachdem, ob der Plan für die Verwendung von FTEs oder Stunden eingerichtet wurde, </span> die Anzahl der für diese Initiative benötigten Aufgabengebiete für jeden </span></span><span> in FTE <span><span> Stunden pro Monat in die Initiative aufgenommen</span>. <span>Die ersten drei Monate der Initiative werden standardmäßig angezeigt.</span></p> <p><span>Beim Aktualisieren der Aufgabengebiet-Informationen für die Initiative werden auch die erforderlichen Aufgabengebiet-Informationen für den Plan aktualisiert.</span> </p> <p>Informationen zum Einrichten des Plans für die Verwendung von FTE oder Stunden finden Sie unter <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Erstellen und Bearbeiten von Plänen in der [!DNL Scenario Planner]</a>. </p>
      <p><b>WICHTIG</b></p>  
      <p>Für alle Berechnungen in der [!DNL Scenario Planner] verwendet [!DNL Workfront] den folgenden Wert: 1 FTE = 8 Stunden. </p>

   <p><b>TIPP</b></p>

   <ul> 
       <li> <p><span>Verwenden Sie die [!UICONTROL Tab]-Taste, um zum nächsten Monat zu wechseln.</span> </p> </li> 
      <li> <p> Wenn <span> auf dieses Feld klicken, werden alle </span>aktiven) Aufgabengebiete im System aufgelistet. </p> </li> 
       <li> <p>Die Aufgabengebiete, die den verfügbaren Aufgabengebieten des Plans bereits hinzugefügt wurden, werden zuerst angezeigt. Informationen zum Hinzufügen verfügbarer Aufgabengebiete zu einem Plan finden Sie unter <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Erstellen und Bearbeiten von Plänen im Szenario-Planer</a>. </p> </li> 
       <li> <p>[!DNL Workfront] geht davon aus, dass ein Vollzeitäquivalent 160 Stunden für einen Monat beträgt. </p> <p>Für alle Berechnungen im Szenario-Planer verwendet Workfront den folgenden Wert: 1 FTE = 8 Stunden. </p></li> 
      </ul> </p> <p>Sie können eine Zahl eingeben, die kleiner als 1 FTE oder Dezimalzahlen für FTE <span>oder</span> <span>Stunden</span> ist. Ein Aufgabengebiet von 0,5 Consultant würde beispielsweise bedeuten, dass ein Consultant die Hälfte seines FTE (in der Regel 4 Stunden, wobei 8 Stunden 1 FTE sind) für die Arbeit an dieser Initiative aufwenden würde. </p>  </td> 
     </tr> 
     <tr> 
      <td rowspan="3" role="rowheader">Kostenabschnitt</td> 
      <td> <p>Die Gesamtkosten der Initiative werden rechts neben dem Abschnitt [!UICONTROL Kosten] angezeigt. [!DNL Workfront] berechnet die Kosten einer Initiative anhand der folgenden Formel:</p> <p><code>[!UICONTROL Initiative Costs] = [!UICONTROL Fixed Costs] + [!UICONTROL People] Costs</code> </p> </td> 
     </tr> 
     <tr> 
      <td> <p>Geben Sie im Feld <strong>[!UICONTROL Festkosten]</strong> manuell einen groben Schätzwert der Kosten ein, die Ihrer Meinung nach bei dieser Initiative anfallen werden. Darin sollten nicht die Kosten enthalten sein, die mit den für die Initiative veranschlagten Aufgabengebieten verbunden sind.</p> <p><span>Geben Sie einen Betrag für jeden Monat der Initiative ein, indem Sie mit der Tabulatortaste von einem Monat zum nächsten wechseln.</span> </p> </td> 
     </tr> 
     <tr> 
      <td> 
       <div> 
        <p>Je nachdem, ob der Plan für die Verwendung von FTEs oder Stunden eingerichtet ist, verwendet [!UICONTROL Workfront] die folgenden Formeln zur Berechnung der [!UICONTROL Personalkosten]:</p> 
        <ul> 
         <li> <p>Bei Verwendung von FTEs: </p> <p><code>[!UICONTROL People Costs] = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, wobei 160 der Gesamtzahl der Arbeitsstunden in einem Monat entspricht. </p> </li> 
         <li> <p style="font-weight: normal;">Bei Verwendung von Stunden: </p> <p style="font-weight: normal;"><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> <p style="font-weight: normal;">Informationen zum Einrichten des Plans für die Verwendung von Stunden oder FTE finden Sie unter <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Erstellen und Bearbeiten von Plänen im Szenario-Planer</a>.</p> </li> 
        </ul> 
        <p>Die Personalkosten werden in der Basiswährung berechnet, die Sie in Ihren Wechselkurseinstellungen ausgewählt haben. Weitere Informationen zu Wechselkursen finden Sie unter <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Einrichten von Wechselkursen</a>.</p> 
        <p>Durch die Aktualisierung der Kosteninformationen für eine Initiative wird auch der Bereich [!UICONTROL Kosten] für den Plan aktualisiert. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"> <p style="font-weight: normal;">Nachdem Sie das erforderliche Aufgabengebiet und die Kostenwerte für Ihre Initiative definiert haben und die Dauer der Initiative geändert haben, kann eines der folgenden Szenarien eintreten:</p> 
       <ul> 
        <li> <p style="font-weight: normal;">Wenn Sie die Initiative verkürzen, werden [!DNL Workfront] die erforderliche Menge an Ressourcen und die Kosten, die mit der aus dem Plan entfernten Zeit verbunden sind, entfernt. Die Aufgabengebiete bleiben im Plan, verfügen jedoch über keine erforderlichen FTEs oder <span data-mc-edit-date="2021-04-19T13:46:01.5004065-04:00" data-mc-editor="alinawilson" data-mc-comment="drafted, yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-19T13:45:58.7938344-04:00">Stunden</span>. Die für den Plan und den Haushaltsplan verfügbaren Mittel bleiben unverändert.<br>Informationen zum Aktualisieren des Plans finden Sie unter <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Erstellen und Bearbeiten von Plänen im [!DNL Scenario Planner]</a>. </p> </li> 
        <li> <p style="font-weight: normal;">Wenn Sie die Initiative verlängern, müssen Sie die Anzahl der Aufgabengebiete und Kosten für die neu hinzugefügten Monate auf der Initiative angeben. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Net Value] Abschnitt</td> 
      <td>Geben Sie im Abschnitt <strong>[!DNL Net Value]</strong> manuell einen groben Schätzwert in das Feld <strong>[!UICONTROL Geplanter Nutzen]</strong> ein. Das ist es, was Ihrer Meinung nach der Nutzen dieser Initiative sein wird. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Wenn Sie bereits die Anzahl der Aufgabengebiete und das Budget für Ihren Plan sowie die Anzahl der Aufgabengebiete und die Kosten für die Initiative, die Sie bearbeiten, sowie für alle darüber liegenden Initiativen definiert haben und diese die für den Plan angegebenen Beträge überschreiten, haben [!DNL Workfront] möglicherweise nicht genügend Ressourcen, um die Initiative abzuschließen. [!DNL Workfront] kennzeichnet dies als Konflikt beim Versuch, diese Initiative zu erreichen, und zeigt sie als roten Balken an. Alle Initiativen, die auf die konfliktbehaftete Initiative folgen, werden in einem roten Hintergrund angezeigt. Möglicherweise müssen Sie einige Anforderungen Ihrer Initiativen anpassen, beginnend mit der ersten Initiative, die nicht über ausreichende Ressourcen verfügt. Informationen zum Anpassen widersprüchlicher Initiativen finden Sie unter [Beheben von Initiativkonflikten im [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. (Optional) Bewegen Sie den Mauszeiger über den Namen eines Aufgabengebiets und klicken Sie dann auf das **[!UICONTROL Papierkorbsymbol]** ![](assets/delete.png), um es aus der Initiative zu entfernen.

1. (Bedingt) Wenn Sie Änderungen an der Initiative vorgenommen haben, klicken Sie auf **[!UICONTROL Übernehmen]**.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Add more steps here as you can do more in the Initiative box over time)
   </MadCap:conditionalText>
   -->

1. (Bedingt) Wenn Sie keine Änderungen vorgenommen haben, klicken Sie auf das **X**-Symbol oben rechts im Bedienfeld „Initiativdetails“, um es zu schließen.
1. (Optional) Aktualisieren Sie die Priorität Ihrer Initiativen.

   Informationen zur Priorisierung von Initiativen finden Sie [Aktualisieren von Initiativprioritäten im Szenario-Planer](../scenario-planner/prioritize-initiatives.md).

   >[!TIP]
   >
   >Initiativen, die zuerst in der Liste aufgeführt werden, haben eine höhere Priorität und erhalten Ressourcen, bevor die Initiativen, die weiter unten in der Liste aufgeführt werden.

1. Klicken Sie **[!UICONTROL Plan speichern]**.

   Die Initiative ist jetzt in Ihrem Plan enthalten.

   Informationen zum Löschen von Initiativen aus einem Plan finden Sie unter [Löschen von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/delete-initiatives.md).
