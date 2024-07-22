---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Erstellen und Bearbeiten von Plänen im Szenario-Planer
description: Sie können Pläne im Rahmen des Workfront-Szenario-Planers erstellen, wenn Sie die übergeordnete Strategie Ihres Unternehmens priorisieren. Weitere Informationen zu Plänen finden Sie unter Übersicht über Pläne im Szenario-Planer.
author: Alina
feature: Workfront Scenario Planner
exl-id: 15c0e519-0164-449d-84f3-470d0d4eb795
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '2389'
ht-degree: 0%

---

# Erstellen und Bearbeiten von Plänen im [!DNL Scenario Planner]

Sie können Pläne im Rahmen der Verwendung von [!DNL Workfront Scenario Planner] erstellen, wenn Sie die übergeordnete Strategie Ihres Unternehmens priorisieren. Weitere Informationen zu Plänen finden Sie unter [Übersicht über Pläne in der [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: talk about:</p>
<p>- Show people conflicts >> this impacts the conflicts calculation for initiatives>> link to the conflicts article</p>
<p>- explain what hovering over the green upward-pointing arrow does, with screen shot)</p>
</div>
-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <p>Aktuell: [!UICONTROL Business] oder höher</p>
   <p>Neu: Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>Neu: Licht oder höher</p> 
   <p>Aktuell: [!UICONTROL Review] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td>Produkt* </td> 
   <td> 
   <p>Für die aktuellen Workfront-Pläne: </p>
   <p>Sie müssen eine zusätzliche Lizenz für die [!DNL Adobe Workfront Scenario Planner] erwerben, um auf die in diesem Artikel beschriebene Funktion zugreifen zu können.</p> <p>Informationen zu Zugriff und Berechtigungen für den [!DNL Workfront Scenario Planner] finden Sie unter <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Für die Verwendung des [!DNL Scenario Planner]</a> benötigten Zugriff. </p> </td> 
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

## Erstellen und Bearbeiten von Plänen

Sie können einen Plan von Grund auf neu erstellen oder einen existierenden bearbeiten, der für Sie freigegeben wurde.

>[!NOTE]
>
>Nachdem Sie einen Plan erstellt haben, werden Sie als Planersteller und -eigentümer betrachtet. Wenn ein Benutzer deaktiviert wird, hat der Plan keinen Eigentümer und ist für niemanden sichtbar, es sei denn, er wurde zuvor für einen Link freigegeben.

In diesem Artikel wird beschrieben, wie Sie einen Plan von Grund auf neu erstellen oder einen bestehenden Plan bearbeiten können.

Alle Überlegungen zu Plänen, einschließlich der für einen Plan verfügbaren Informationen, finden Sie unter [Übersicht über Pläne in der [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

Weitere Informationen zum Löschen von Plänen finden Sie unter [Pläne löschen in der  [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

So erstellen oder bearbeiten Sie einen Plan:

{{step1-to-scenario-planner}}

Eine Liste der vorhandenen Pläne, die Sie erstellt haben, wird im [!DNL Workfront Scenario Planner] angezeigt.

1. (Optional) Klicken Sie oben rechts in der Planliste auf das Symbol **[!UICONTROL Filter]** ![](assets/filter-icon-34x37.png) und wählen Sie eine der folgenden Optionen aus:

   | Filter | Beschreibung |
   |---|---|
   | [!UICONTROL Alle] | Zeigt alle Pläne an, die Sie erstellt haben oder die für Sie freigegeben wurden. |
   | [!UICONTROL Meine Pläne] | Zeigt die von Ihnen erstellten Pläne an. |
   | [!UICONTROL Für mich freigegeben] | Zeigt die für Sie freigegebenen Pläne an. |

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Suchen]** ![](assets/search-icon.png), um einen Suchbegriff einzugeben und einen Plan schnell in der Liste zu finden.

1. Klicken Sie auf den Namen eines bestehenden Plans, um ihn zu bearbeiten und mit Schritt 7 fortzufahren.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate) </p>
   -->

   Oder

   Klicken Sie oben links auf **[!UICONTROL Neuer Plan]** , um einen Plan zu erstellen und mit Schritt 5 fortzufahren.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate)</p>
   -->

   ![](assets/new-plan-button.png)

   Das Feld [!UICONTROL Neuer Plan] wird angezeigt.

   ![](assets/new-plan-ui-adding-a-new-plan-350x306.png)

1. (Bedingt) Wenn Sie einen neuen Plan erstellen, geben Sie die folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Geben Sie einen Namen für den Plan ein. Dies ist ein Pflichtfeld.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p>Wichtig: <span style="font-weight: normal;">Sie können die folgenden Auswahlen nach dem Erstellen und Speichern des Plans nicht mehr ändern.</span> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>FTE ([!UICONTROL Vollzeitäquivalent]) oder [!UICONTROL Stunden]</span> </td> 
      <td> <p><span>Wählen Sie eine der folgenden Optionen aus, um anzugeben, wie Sie die Informationen zur Rolle des Auftrags für diesen Plan schätzen möchten:</span> </p> 
       <ul> 
      <li> <p><span><strong>FTE</strong>. Dies ist der Standardwert </span> </p> 
      <p><b>WICHTIG</b></p>  
      <p>Für alle Berechnungen im [!DNL Scenario Planner] verwendet [!DNL Workfront] den folgenden Wert: 1 FTE = 8 Stunden. </p> </li> 
      <li> <p><strong>[!UICONTROL Hours]</strong> </p> </li> 
       </ul> <p><b>WICHTIG</b></p>

   Die hier ausgewählte Option bestimmt, wie Informationen zur Rolle des Auftrags für den Plan, die Szenarien des Plans und Initiativen angezeigt werden.</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Startdatum]</td> 
      <td> <p>Wählen Sie den Monat und das Jahr aus, in dem der Plan beginnen soll. Sie können nur Monate in diesem Feld auswählen. [!DNL Workfront] geht davon aus, dass das Startdatum des Plans der erste Tag des ausgewählten Monats ist und das Enddatum der letzte Tag des Monatsendes in seiner Dauer ist. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Dauer]</td> 
      <td> <p>Wählen Sie aus dem Dropdown-Menü aus den folgenden Dauern aus:</p> 
       <ul> 
        <li>1 Jahr. Dies ist die Standarddauer. </li> 
        <li>3 Jahre</li> 
        <li> <p>5 Jahre</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--for table above - how FTE is calcualted: NOTE: snippet below: this is per Ani; it does NOT look at the system FTE.) </p>-->

1. (Bedingt) Klicken Sie auf **[!UICONTROL Weiter]**.

   Die Zeitleiste des Plans wird als **[!UICONTROL Anfangsszenario]** angezeigt.

   Informationen zum Erstellen zusätzlicher Szenarien finden Sie unter [Erstellen und Vergleichen von Planszenarien in der  [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Optional) Wählen Sie aus dem Dropdownmenü &quot;Timeline&quot;eine der Optionen in der folgenden Tabelle aus, um die Ansicht der Zeitleiste des Plans zu ändern.

   ![](assets/month-dropdown-with-all-options.png)

   | Dropdown-Menüoption | Beschreibung |
   |---|---|
   | [!UICONTROL Monat] | Zeigt die Timeline nach Monat an. Dies ist die Standardoption und die einzige Option für einen Jahresplan. |
   | [!UICONTROL Quartal] | Zeigt die Timeline vierteljährlich an. Diese Option ist nur verfügbar, wenn die [!UICONTROL Laufzeit] des Plans 3 oder 5 Jahre beträgt. Dies ist die Standardoption für einen Dreijahresplan. |
   | [!UICONTROL Year] | Zeigt die Timeline nach Jahr an. Diese Option ist nur verfügbar, wenn die [!UICONTROL Laufzeit] des Plans 5 Jahre beträgt. Dies ist die Standardoption für einen Fünfjahresplan. |

1. (Optional) Scrollen Sie von links nach rechts, um die gesamte Dauer des Plans anzuzeigen.
1. (Optional) Klicken Sie auf die Indikatorlinie **[!UICONTROL Today]** , um zum aktuellen Tag zurückzukehren.

   ![](assets/today-indicator-350x160.png)

1. Klicken Sie in der Kopfzeile des Plans auf das Feld **[!UICONTROL Vorgangsrollen]** , um Auftragsrollen hinzuzufügen, die für die Ausführung des Plans verfügbar sein werden.

   Die Details des Felds [!UICONTROL Auftragsrollen] werden angezeigt.

   >[!TIP]
   >
   >Die Rollenzuordnungseinheit (VZÄ oder Stunden), die [!DNL Workfront] für diesen Plan verwendet, wird im Titel des Feldes in Klammern angezeigt.

   ![](assets/adding-people-to-plan-350x206.png)

1. Klicken Sie auf das Feld **[!UICONTROL Eingeben der Auftragsrolle beginnen]** und wählen Sie eine Rolle aus der Liste aus oder geben Sie den Namen einer aktiven Auftragsrolle ein.

   Wenn Sie auf dieses Feld klicken, werden alle aktiven Vorgangsrollen im System aufgelistet.

   Dadurch wird die Auftragsrolle zur Spalte &quot;Auftragsrollen&quot;hinzugefügt.

1. Aktualisieren oder überprüfen Sie die folgenden Informationen für die Auftragsrolle:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max. verfügbar] (für FTE) </p> <p role="rowheader">oder </p> <p role="rowheader"><span>[!UICONTROL Insgesamt verfügbar] (für Stunden)</span> </p> </td> 
      <td> <p><span>Je nachdem, ob Sie die Verwendung von Stunden oder FTE für Ihren Plan ausgewählt haben, geben Sie </span> die Anzahl der FTEs für die Auftragsrolle <span>oder Stunden</span> ein, die für die Ausführung der Planarbeiten verfügbar sind, und zwar in den folgenden Feldern: </p> 
       <ul> 
        <li> <p style="font-weight: normal;"><strong>[!UICONTROL Gesamt verfügbar]</strong> (für Stunden): Geben Sie die Gesamtanzahl der Stunden für alle Monate während der Dauer des Szenarios an. Standardmäßig teilt [!DNL Workfront] die verfügbare Gesamtanzahl gleichmäßig auf alle Monate während der Dauer des Szenarios. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Wenn Sie für eine Designer 1200 Stunden eingeben, bedeutet dies, dass die Designer während der Laufzeit des Plans für jeden Monat 100 Stunden zur Verfügung steht, wenn die Plandauer [!UICONTROL Dauer] 1 Jahr beträgt. </p> </li> 
        <li> <p><b>[!UICONTROL Max. verfügbar]</b> (für FTE): Geben Sie die Anzahl der FTEs an, für die während der Laufzeit des Plans die Jobrolle für jeden Monat verfügbar ist. Standardmäßig weist <strong>Workfront</strong> jedem Monat während der Laufzeit des Szenarios die Zahl [!UICONTROL Max. verfügbare] Zahl zu.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Wenn Sie eine FTE für einen Berater eingeben, bedeutet dies, dass der Berater während der Laufzeit des Plans für jeden Monat für eine FTE zur Verfügung steht. </p> <p>Sie können eine Zahl unter 1 FTE eingeben. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Eine 0,5-Beraterrolle würde bedeuten, dass ein Berater die Hälfte seiner VZÄ (normalerweise 4 Stunden, wobei 8 Stunden 1 VZÄ betragen) für die Arbeit an diesem Plan aufwendet. Für alle Berechnungen im Szenario-Planer verwendet Workfront den folgenden Wert: 1 FTE = 8 Stunden. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max erforderlich] (für FTE)</p> <p role="rowheader">oder </p> <p role="rowheader"><span>[!UICONTROL Gesamt erforderlich] (für Stunden)</span> </p> </td> 
      <td> <p><span>Je nachdem, ob Sie sich für die Verwendung von Stunden oder FTE für Ihren Plan entschieden haben, überprüfen Sie die Anzahl der FTEs für die Rolle als Job <span> oder Stunden</span>, die zum Abschließen der Initiativen im Szenario erforderlich sind. </span> Überprüfen Sie die folgenden Felder:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Gesamt erforderlich]</strong> (für Stunden): Die Gesamtanzahl der Stunden, die für alle Monate während der Dauer des Plans erforderlich sind.</p> </li> 
        <li> <p><strong>[!UICONTROL Max erforderlich]</strong> (für VZÄ): Die maximale Anzahl von VZÄ, die während der Laufzeit des Plans für einen der Monate erforderlich sind. </p> </li> 
       </ul> <p>Tipp: Nach dem Hinzufügen von Initiativen wird die <span>maximale </span> Anzahl von FTEs <span> oder die Gesamtzahl der Stunden</span> angezeigt, die für diese Auftragsrolle erforderlich sind. Informationen zum Hinzufügen von Initiativen zu einem Plan finden Sie unter <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">Erstellen und Bearbeiten von Initiativen im [!DNL Scenario Planner]</a>.</p> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">[!UICONTROL Avg utilization]</td> 
       <td> <p>(NOTE: this field was removed in 21.2 - May 2021) </p> <p>[!DNL Workfront] calculates the average utilization for each job role using the job role FTEs associated with initiatives (required) and the job role FTEs associated with the plan (available). </p> <p> [!DNL Workfront] calculates the job role utilization percentage for a plan using the following formula: </p> <p><code>Job role utilization percentage = Sum [(Required job roles for each month of the plan *100)/ (Available job roles for each month of the plan)] / Number of months in the Duration of the plan</code> </p> 
        <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Example: </b></span></span> 
         <p>For example, if you have a plan with a duration of 12 months and an initiative with the duration of 2 months, where you use 1 Designer for your initiative (required job role) and there are 2 Designers available on the plan (available), the Utilization percentage for the Designer job role is calculated as follows:</p> 
         <p><code>Designer utilization percentage = [(1/2 + 1/2) * 100] / 12 = 100 / 12 = 8.3%</code> </p> 
        </div> <p>As you add job roles to the plan and indicate the Available amount for each one, the [!UICONTROL Utilization] value for each role also updates and [!DNL Workfront] calculates a utilization percentage for the plan. For information about how [!DNL Workfront] calculates the Job Role Utilization for a plan, see <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Plans overview in the [!DNL Scenario Planner]</a>. </p> <p>Tip: The Utilization percentage is rounded and has one decimal. </p> </td> 
      </tr>
     --> 
     <tr> 
      <td role="rowheader">[!UICONTROL Stündliche Rate]</td> 
      <td> <p>Dies ist der [!UICONTROL Kosten-Stunden]-Satz für die Stellenfunktion. Der Stundensatz wird in der Währung Ihres Systems angezeigt. Informationen zum Einrichten von Wechselkursen für Ihr System finden Sie unter <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Einrichten von Wechselkursen</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Bewegen Sie den Mauszeiger über den Namen einer Auftragsrolle oder klicken Sie auf die Registerkarte , nachdem Sie die Rolleninformationen aktualisiert haben, und klicken Sie dann auf das Papierkorbsymbol ]**![](assets/delete.png) , um sie aus dem Plan zu entfernen.**[!UICONTROL 
1. Klicken Sie auf **[!UICONTROL Verteilung der Auftragsrolle]**.

   Der Bereich für die Auftragsrollenverteilung wird für alle Monate während der Dauer des Szenarios angezeigt.

   ![](assets/job-role-monthly-distribution-box-fte-350x144.png)

1. Geben Sie den Namen einer Auftragsrolle ein, die zum Plan hinzugefügt werden soll, im Feld **[!UICONTROL Aufgabenrolle beim Eingeben des Auftrags beginnen]** und klicken Sie dann auf &quot;Enter&quot;, wenn sie in der Liste angezeigt wird. Dadurch wird die Auftragsrolle zur Spalte [!UICONTROL Vorgangsrollen] hinzugefügt.
1. Aktualisieren oder überprüfen Sie die folgenden Informationen für jeden Monat des Szenarios:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Job Roles] (FTE oder Stunden)</td> 
      <td>Sowohl die für das Szenario verfügbare Rolle als auch die für die Initiativen im Szenario erforderlichen Aufgaben werden im Bereich "Verteilung der Rolle der Arbeitsplätze"angezeigt. Es gibt einen Hinweis darauf, ob die Schätzungen für die Rolle des Auftrags in FTEs oder Stunden in der Spaltenüberschrift enthalten sind. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Verfügbar] (max. &lt;Anzahl der VZÄ&gt;) </p> 
       <div> 
        <p>oder</p> 
        <p>[!UICONTROL Verfügbar] (insgesamt &lt;Anzahl der Stunden&gt;) </p> 
       </div> </td> 
      <td> <p><span>Je nachdem, ob Sie die Verwendung von Stunden oder FTE für Ihren Plan ausgewählt haben, überprüfen oder aktualisieren Sie</span> die monatliche Anzahl von FTEs für die Rolle "Auftrag"<span>oder Stunden</span>, die für das Szenario in den folgenden Feldern verfügbar sind:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Verfügbar] (max &lt;Anzahl der FTE&gt;)</strong>: Die Anzahl in Klammern zeigt die maximale Anzahl der Rollen an, die für einen der Monate des Szenarios verfügbar sind. Überprüfen oder aktualisieren Sie die Anzahl der VZÄ für jeden Monat des Szenarios. Durch eine Änderung der monatlichen Zuweisung könnte die Anzahl der VZÄ in den Klammern aktualisiert werden. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Verfügbar] (gesamt &lt;Anzahl der Stunden&gt;)</strong>: Die Zahl in Klammern zeigt die Gesamtanzahl der Stunden an, die für alle Monate im Szenario verfügbar sind. Überprüfen oder aktualisieren Sie die Anzahl der Stunden für jeden Monat des Szenarios. Durch Änderung der monatlichen Zuordnung wird die Anzahl der Stunden in den Klammern aktualisiert.</span> </p> </li> 
       </ul> <p>Die manuelle Aktualisierung der monatlichen Zuordnung von Aufgaben für Arbeitsplätze ist eine weitere Möglichkeit, um Konflikte zwischen Aufgabenrollen zwischen Initiativen im Szenario zu lösen. </p> <p>Tipp:   <p><span>Um die monatliche Rollenverfügbarkeit für mehrere Monate zu aktualisieren, geben Sie die Anzahl der Stunden oder FTEs in das Feld [!UICONTROL Verfügbar] eines Monats ein und ziehen Sie dann die Ecke des Felds über die angrenzenden Monate, um denselben Wert für jeden Monat zu kopieren. Legen Sie sie ab, um alle Monate zu aktualisieren.</span> </p> <p> <img src="assets/job-role-distribution-draggable-corner-highlighted-350x83.png" style="width: 350;height: 83;"> </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Erforderlich] (max &lt;Zahl&gt;)</p> 
       <div> 
        <p role="rowheader">oder</p> 
        <p role="rowheader">[!UICONTROL Erforderlich] (insgesamt &lt;Zahl&gt;)</p> 
       </div> </td> 
      <td> <p><span>Je nachdem, ob Sie die Verwendung von Stunden oder FTE für Ihren Plan ausgewählt haben, überprüfen Sie die monatliche Anzahl von FTEs für die Rolle als Job in den folgenden Feldern:</span> Die für das Szenario erforderliche Anzahl von FTEs für die Rolle als Job. </p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Erforderlich] (max &lt;Anzahl der FTE&gt;)</strong>: Die Anzahl in Klammern zeigt die maximale Anzahl der Rollen an, die für einen der Monate des Szenarios erforderlich sind. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Erforderlich] (total &lt;Anzahl der Stunden&gt;)</strong>: Die Anzahl in Klammern zeigt die Gesamtanzahl der Stunden an, die für alle Monate im Szenario erforderlich sind.</span> </p> </li> 
       </ul> <p>Tipp: Sie können die erforderliche Anzahl von FTEs <span>oder Stunden</span> für die Auftragsrolle nicht ändern. Diese Zahl wird für das Szenario angezeigt, nachdem Sie mit dem Hinzufügen von Initiativen und deren Anforderungen an die Rolle in der Arbeitswelt begonnen haben. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Unterschied]</td> 
      <td> 
       <div> 
        <p>Die monatliche Differenz zwischen den erforderlichen und verfügbaren Auftragsrollen für das Szenario. [!DNL Workfront] berechnet die Differenz für jede Auftragsrolle für jeden Monat mithilfe der folgenden Formel:</p> 
        <p><code>Monthly role difference = Monthly required roles - Monthly available roles</code> (in VZÄ oder Stunden) </p> 
        <p>Tipp: Wenn der Unterschied eine negative Zahl anzeigt, erfordert das Szenario mehr Auftragsrollen als der Plan verfügbar ist. Ihre Ressourcen sind überzugewiesen. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nutzung] %</td> 
      <td> 
       <div> 
        <p>Der Prozentsatz der Nutzung zeigt an, wie viele der verfügbaren Arbeitsplatzrollen tatsächlich für die Initiativen im Szenario verwendet (oder benötigt werden) werden. </p> 
        <p>[!DNL Workfront] berechnet die Nutzung pro Stellenausschreibung und Monat anhand der folgenden Formel: </p> 
        <p><code>Monthly role utilization % = Monthly required roles / Monthly available roles * 100</code> </p> 
        <p>Der Prozentsatz der Auslastung kann je nach Zuordnung Ihrer Ressourcen in den folgenden Farben angezeigt werden:</p> 
        <ul> 
         <li> <p><b>Grün</b>: Die verfügbare und die erforderliche Anzahl von Vorgangsrollen stimmen überein. Die Ressourcen sind vollständig zugewiesen und der Prozentsatz der Verwendung beträgt 100%. </p> </li> 
         <li> <p><b>Rot</b>: Es gibt mehr erforderliche Vorgangsrollen, als der Plan verfügbar ist. Die Ressourcen werden überverteilt und der Prozentsatz der Auslastung liegt bei über 100 %.</p> </li> 
         <li> <p><b>Blau</b>: Es gibt mehr verfügbare Auftragsrollen, als erforderlich sind. Die Mittel sind zu niedrig zugewiesen und der Prozentsatz der Auslastung liegt unter 100 %. </p> </li> 
        </ul> 
       </div> <p> <img src="assets/utilization-percent-colors-sp-350x61.png" style="width: 350;height: 61;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **[!UICONTROL Anwenden]** , um die monatliche Aufgabenrollenverteilung zu speichern.

   Oder

   Klicken Sie auf **[!UICONTROL Abbrechen]** , um die Aufgabenrollenverteilungsliste zu schließen und zum Szenario zurückzukehren.

1. Klicken Sie in der Kopfzeile des Plans auf das Feld **[!UICONTROL Finanzen]** , um das Budget für diesen Plan hinzuzufügen.

   Die Details des Feldes [!UICONTROL Financial] werden angezeigt.

   >[!TIP]
   >
   >Die Währung, die [!DNL Workfront] für diesen Plan verwendet, wird im Titel des Felds in Klammern angezeigt.

1. Geben Sie das **[!UICONTROL jährliche Budget]** an.

   >[!NOTE]
   >
   >Wenn Ihr Plan mehrere Jahre umfasst, müssen Sie für jedes Jahr einen Budgetbetrag angeben.

1. Drücken Sie die Eingabetaste , um das jährliche Budget zu speichern, und dann [!UICONTROL Tab] , um zum folgenden Jahr zu wechseln.

   Das jährliche Budget wird automatisch zu gleichen Teilen für jeden Monat des ausgewählten Jahres verteilt.

1. Klicken Sie auf **[!UICONTROL Erweitert]** , um die monatliche Budgetverteilung anzuzeigen. Die jährlichen und monatlichen Budgets sind immer auf Zahlen gerundet. Wenn der Budgetbetrag aufgrund von Dezimalstellen nicht gleichmäßig auf alle Monate innerhalb eines Jahres verteilt werden kann, wird unter der jährlichen Budgetverteilung ein Indikator **[!UICONTROL Verbleibend]** angezeigt.

   ![](assets/adanced-and-remaining-links-on-plan-budget-350x507.png)

1. Passen Sie die monatlichen Budgets manuell an, um die überschrittenen Beträge zu eliminieren.

   Wenn die Summe aller monatlichen Budgetbeträge größer ist als das jährliche Budget, wird unter der jährlichen Budgetverteilung ein Warnhinweis mit dem Wert **[!UICONTROL Überschreiten]** angezeigt. Passen Sie die monatlichen Budgetbeträge manuell an, bis sie dem für den Plan verfügbaren Budget entsprechen oder darunter liegen.

   ![](assets/exceeding-budget-warning-on-plan-350x483.png)

1. Deaktivieren Sie die Einstellung **[!UICONTROL Personenkosten einschließen]** , um die Kosten im Zusammenhang mit Stellenrollen von der Zählung auf die Gesamtkosten des Plans auszuschließen. Feste Kosten werden immer auf die Gesamtkosten des Plans angerechnet. Diese Einstellung ist standardmäßig aktiviert und wirkt sich auf alle Szenarien im Plan aus.
1. Klicken Sie auf eine beliebige Stelle außerhalb des Felds [!UICONTROL Financial] , um es zu schließen. Die eingegebenen Informationen werden automatisch gespeichert.

   Sie können nun mit der Erstellung der Initiativen für den Plan und dem Hinzufügen von Szenarien beginnen.

1. (Empfohlen) Klicken Sie auf **[!UICONTROL Neue Initiative]** , um eine neue Initiative hinzuzufügen.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Should this include information on how to create scenarios - see also information about scenarios in Manage Plans?)</p>
   -->

   Weitere Informationen zum Hinzufügen von Initiativen finden Sie im Artikel [Erstellen und Bearbeiten von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. (Optional) Erstellen Sie eine Kopie des vorhandenen Szenarios, um ein neues Szenario desselben Plans zu erstellen. Weitere Informationen zum Erstellen und Arbeiten mit mehreren Szenarien finden Sie unter [Erstellen und Vergleichen von Planszenarien in der  [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).
1. Klicken Sie auf **[!UICONTROL Plan speichern]**.

   Ihr Plan wird erstellt oder aktualisiert.

1. (Optional) Klicken Sie auf das Symbol **[!UICONTROL Favoriten]** ![](assets/favorites-icon-small.png) rechts neben dem Namen des Plans, um den Plan Ihrer Favoritenliste hinzuzufügen.

1. (Optional) Kopieren Sie die URL des Plans und senden Sie sie an jeden anderen Benutzer, der sie möglicherweise überprüfen oder aktualisieren muss. Sie müssen mindestens über den Zugriff auf die Zugriffsebene verfügen, um den Plan anzeigen zu können.  Sie müssen über den Zugriff [!UICONTROL Bearbeiten] verfügen, um sie zu bearbeiten. Wenn sie finanzielle Informationen zum Plan, wie Informationen zu Budgets, Kosten und Stellenraten, überprüfen müssen, müssen sie auch Zugriff auf [!UICONTROL Finanzdaten] in ihrer Zugriffsebene haben. Informationen über den für [!DNL Scenario Planner] benötigten Zugriff finden Sie unter [Für die Verwendung des  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md) benötigten Zugriff.
