---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Erstellen und Bearbeiten von Plänen im Szenario-Planer
description: Sie können Pläne im Rahmen des Workfront-Szenario-Planers erstellen, wenn Sie die übergeordnete Strategie Ihres Unternehmens priorisieren. Weitere Informationen zu Plänen finden Sie unter Übersicht über Pläne im Szenario-Planer.
author: Alina
feature: Workfront Scenario Planner
exl-id: 15c0e519-0164-449d-84f3-470d0d4eb795
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: tm+mt
source-wordcount: '2402'
ht-degree: 1%

---

# Erstellen und Bearbeiten von Plänen im [!DNL Scenario Planner]

Sie können Pläne erstellen, indem Sie die [!DNL Workfront Scenario Planner], wenn Sie die Strategie Ihres Unternehmens auf höherer Ebene priorisieren. Weitere Informationen zu Plänen finden Sie unter [Übersicht über Pläne im [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: talk about:</p>
<p>- Show people conflicts >> this impacts the conflicts calculation for initiatives>> link to the conflicts article</p>
<p>- explain what hovering over the green upward-pointing arrow does, with screen shot)</p>
</div>
-->

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] Plan*</p> </td> 
   <td>[!UICONTROL Business] oder höher</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>[!UICONTROL Review] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td>Produkt</td> 
   <td> <p>Sie müssen eine zusätzliche Lizenz für die [!DNL Adobe Workfront Scenario Planner] , um auf die in diesem Artikel beschriebene Funktionalität zuzugreifen.</p> <p>Informationen zum Abrufen des [!UICONTROL Workfront Scenario Planner] finden Sie unter <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Zugriff erforderlich für die Verwendung des [!UICONTROL Szenario-Planers]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Konfigurationen auf Zugriffsebene* </td> 
   <td> <p>Zugriff auf [!UICONTROL Bearbeiten] oder höher auf die [!DNL Scenario Planner]</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Für Informationen zur [!DNL Workfront] Administratoren können die Zugriffsebene ändern, siehe <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektberechtigungen </p> </td> 
   <td> <p>[!DNL Manage] Berechtigungen für einen Plan</p> <p>Informationen über die Anforderung eines zusätzlichen Zugangs zu einem Plan finden Sie unter <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Anfordern des Zugriffs auf einen Plan im [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Erstellen und Bearbeiten von Plänen

Sie können einen Plan von Grund auf neu erstellen oder einen existierenden bearbeiten, der für Sie freigegeben wurde.

>[!NOTE]
>
>Nachdem Sie einen Plan erstellt haben, werden Sie als Planersteller und -eigentümer betrachtet. Wenn ein Benutzer deaktiviert wird, hat der Plan keinen Eigentümer und ist für niemanden sichtbar, es sei denn, er wurde zuvor für einen Link freigegeben.

In diesem Artikel wird beschrieben, wie Sie einen Plan von Grund auf neu erstellen oder einen bestehenden Plan bearbeiten können.

Alle Überlegungen zu Plänen, einschließlich der für einen Plan verfügbaren Informationen, finden Sie unter [Übersicht über Pläne im [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

Informationen zum Löschen von Plänen finden Sie unter [Löschen von Plänen in [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

So erstellen oder bearbeiten Sie einen Plan:

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png)Klicken Sie auf [!UICONTROL Szenarien].

   Eine Liste der von Ihnen erstellten Pläne wird im [!DNL Workfront Scenario Planner].

1. (Optional) Klicken Sie auf die **[!UICONTROL Filter]** icon ![](assets/filter-icon-34x37.png)in der oberen rechten Ecke der Planliste aus und wählen Sie eine der folgenden Optionen aus:

   | Filter | Beschreibung |
   |---|---|
   | [!UICONTROL Alle] | Zeigt alle Pläne an, die Sie erstellt haben oder die für Sie freigegeben wurden. |
   | [!UICONTROL Meine Pläne] | Zeigt von Ihnen erstellte Pläne an. |
   | [!UICONTROL Für mich freigegeben] | Zeigt die für Sie freigegebenen Pläne an. |

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Optional) Klicken Sie auf die **[!UICONTROL Suche]** icon ![](assets/search-icon.png) um einen Suchbegriff einzugeben und einen Plan schnell in der Liste zu finden.

1. Klicken Sie auf den Namen eines bestehenden Plans, um ihn zu bearbeiten und mit Schritt 7 fortzufahren.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate) </p>
   -->

   Oder

   Klicken **[!UICONTROL Neuer Plan]** in der linken oberen Ecke, um einen Plan zu erstellen und mit Schritt 5 fortzufahren.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate)</p>
   -->

   ![](assets/new-plan-button.png)

   Die [!UICONTROL Neuer Plan] angezeigt.

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
      <li> <p><span><strong>FTE</strong>. Dies ist die Standardeinstellung </span> </p> 
      <p><b>WICHTIG</b></p>  
      <p>Für alle Berechnungen im [!DNL Scenario Planner], [!DNL Workfront] verwendet den folgenden Wert: 1 VZÄ = 8 Stunden. </p> </li> 
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

1. (Bedingt) Klicken Sie auf **[!UICONTROL Nächste]**.

   Die Zeitleiste des Plans wird als **[!UICONTROL Ursprüngliches Szenario]**.

   Weitere Informationen zum Erstellen zusätzlicher Szenarien finden Sie unter [Erstellen und Vergleichen von Planszenarien in [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Optional) Wählen Sie aus dem Dropdownmenü &quot;Timeline&quot;eine der Optionen in der folgenden Tabelle aus, um die Ansicht der Zeitleiste des Plans zu ändern.

   ![](assets/month-dropdown-with-all-options.png)

   | Dropdown-Menüoption | Beschreibung |
   |---|---|
   | [!UICONTROL Monat] | Zeigt die Timeline nach Monat an. Dies ist die Standardoption und die einzige Option für einen Jahresplan. |
   | [!UICONTROL Quartal] | Zeigt die Timeline vierteljährlich an. Diese Option ist nur verfügbar, wenn die Variable [!UICONTROL Dauer] des Plans beträgt 3 oder 5 Jahre. Dies ist die Standardoption für einen Dreijahresplan. |
   | [!UICONTROL Jahr] | Zeigt die Timeline nach Jahr an. Diese Option ist nur verfügbar, wenn die Variable [!UICONTROL Dauer] des Plans beträgt fünf Jahre. Dies ist die Standardoption für einen Fünfjahresplan. |

1. (Optional) Scrollen Sie von links nach rechts, um die gesamte Dauer des Plans anzuzeigen.
1. (Optional) Klicken Sie auf die **[!UICONTROL Heute]** Indikatorlinie, um zum aktuellen Tag zurückzukehren.

   ![](assets/today-indicator-350x160.png)

1. Klicken Sie auf **[!UICONTROL Vorgangsrollen]** in der Kopfzeile des Plans zum Hinzufügen von Auftragsrollen, die zur Ausführung des Plans verfügbar sein werden.

   Die Einzelheiten der [!UICONTROL Vorgangsrollen] angezeigt.

   >[!TIP]
   >
   >Die Rollenzuweisungseinheit (VZÄ oder Stunden), die [!DNL Workfront] verwendet für diesen Plan wird in Klammern im Titel des Felds angezeigt.

   ![](assets/adding-people-to-plan-350x206.png)

1. Klicken Sie auf **[!UICONTROL Eingabe der Auftragsrolle beginnen]** und wählen Sie eine Rolle aus der Liste aus oder geben Sie den Namen einer aktiven Rolle ein.

   Wenn Sie auf dieses Feld klicken, werden alle aktiven Vorgangsrollen im System aufgelistet.

   Dadurch wird die Auftragsrolle zur Spalte &quot;Auftragsrollen&quot;hinzugefügt.

1. Aktualisieren oder überprüfen Sie die folgenden Informationen für die Auftragsrolle:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max. verfügbar] (für FTE) </p> <p role="rowheader">oder </p> <p role="rowheader"><span>[!UICONTROL Insgesamt verfügbar] (für Stunden)</span> </p> </td> 
      <td> <p><span>Je nachdem, ob Sie sich für die Verwendung von Stunden oder FTE für Ihren Plan entschieden haben, geben Sie</span> die Anzahl der FTE für die berufliche Rolle <span>oder Stunden</span> die zur Ausführung der Planarbeiten in den folgenden Feldern verfügbar sind: </p> 
       <ul> 
        <li> <p style="font-weight: normal;"><strong>[!UICONTROL Insgesamt verfügbar]</strong> (für Stunden): Geben Sie die Gesamtzahl der Stunden für alle Monate während der Dauer des Szenarios an. Standardmäßig [!DNL Workfront] teilt die verfügbare Gesamtanzahl gleichmäßig auf alle Monate während der Dauer des Szenarios. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Wenn Sie für einen Designer 1200 Stunden eingeben, bedeutet dies, dass der Designer während der Laufzeit des Plans für 100 Stunden pro Monat verfügbar ist, wenn die Plandauer [!UICONTROL Dauer] 1 Jahr beträgt. </p> </li> 
        <li> <p><b>[!UICONTROL Max. verfügbar]</b> (für VZÄ): Geben Sie an, wie viele FTE für jeden Monat während der Laufzeit des Plans zur Verfügung stehen. Standardmäßig <strong>Workfront</strong> weist jedem Monat während der Dauer des Szenarios die maximal verfügbare Zahl [!UICONTROL] zu.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Wenn Sie eine FTE für einen Berater eingeben, bedeutet dies, dass der Berater während der Laufzeit des Plans für jeden Monat für eine FTE zur Verfügung steht. </p> <p>Sie können eine Zahl unter 1 FTE eingeben. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Beispiel: </b></span></span>Eine 0,5-Beraterrolle würde bedeuten, dass ein Berater die Hälfte seiner FTE (in der Regel 4 Stunden, wobei 8 Stunden 1 FTE betragen) für die Arbeit an diesem Plan aufwenden würde. Für alle Berechnungen im Szenario-Planer verwendet Workfront den folgenden Wert: 1 VZÄ = 8 Stunden. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max erforderlich] (für FTE)</p> <p role="rowheader">oder </p> <p role="rowheader"><span>[!UICONTROL Gesamt erforderlich] (für Stunden)</span> </p> </td> 
      <td> <p><span>Je nachdem, ob Sie sich für die Verwendung von Stunden oder FTE für Ihren Plan entschieden haben, lesen Sie</span> die Anzahl der FTE für die berufliche Rolle <span>oder Stunden</span> die zum Abschließen der im Szenario vorgesehenen Initiativen erforderlich sind. Überprüfen Sie die folgenden Felder:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Gesamt erforderlich]</strong> (für Stunden): Die Gesamtzahl der Stunden, die während der Laufzeit des Plans für alle Monate erforderlich sind.</p> </li> 
        <li> <p><strong>[!UICONTROL Max. erforderlich]</strong> (für VZÄ): Die maximale Anzahl von VZÄ, die während der Laufzeit des Plans für einen der Monate benötigt werden. </p> </li> 
       </ul> <p>Tipp: Die <span>maximum</span> Anzahl der FTE <span>oder die Gesamtzahl der Stunden</span> für diese Rolle erforderlich ist, wird angezeigt, nachdem Sie mit dem Hinzufügen von Initiativen begonnen haben. Informationen zum Hinzufügen von Initiativen zu einem Plan finden Sie unter <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">Erstellen und Bearbeiten von Initiativen im [!DNL Scenario Planner]</a>.</p> </td> 
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
      <td> <p>Dies ist der [!UICONTROL Kosten-Stunden]-Satz für die Stellenfunktion. Der Stundensatz wird in der Währung Ihres Systems angezeigt. Informationen zum Einrichten von Wechselkursen für Ihr System finden Sie unter <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Wechselkurse einrichten</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Bewegen Sie den Mauszeiger nach der Aktualisierung der Rolleninformationen über den Namen einer Auftragsrolle oder klicken Sie auf die Registerkarte . Klicken Sie dann auf **[!UICONTROL Papierkorbsymbol]** ![](assets/delete.png) , um sie aus dem Plan zu entfernen.
1. Klicken **[!UICONTROL Aufgabenverteilung]**.

   Der Bereich für die Auftragsrollenverteilung wird für alle Monate während der Dauer des Szenarios angezeigt.

   ![](assets/job-role-monthly-distribution-box-fte-350x144.png)

1. Geben Sie den Namen einer Auftragsrolle ein, um sie dem Plan im **[!UICONTROL Eingabe des Aufgabenrollenfelds beginnen]** und klicken Sie dann auf die Schaltfläche Eingabetaste , wenn sie in der Liste angezeigt wird. Dadurch wird die Stellenrolle zum [!UICONTROL Vorgangsrollen] Spalte.
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
      <td role="rowheader"> <p>[!UICONTROL Verfügbar] (max. &lt;number of="" ftes=""&gt;) </p> 
       <div> 
        <p>oder</p> 
        <p>[!UICONTROL Verfügbar] (gesamt &lt;number of="" hours=""&gt;) </p> 
       </div> </td> 
      <td> <p><span>Je nachdem, ob Sie sich für die Verwendung von Stunden oder FTE für Ihren Plan entschieden haben, überprüfen oder aktualisieren Sie</span> die monatliche Anzahl von FTE für die berufliche Rolle <span>oder Stunden</span> für das Szenario in den folgenden Feldern verfügbar:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Verfügbar] (max. &lt;number of="" ftes=""&gt;)</strong>: Die Zahl in Klammern zeigt die maximale Anzahl der Rollen an, die für einen der Monate des Szenarios verfügbar sind. Überprüfen oder aktualisieren Sie die Anzahl der VZÄ für jeden Monat des Szenarios. Durch eine Änderung der monatlichen Zuweisung könnte die Anzahl der VZÄ in den Klammern aktualisiert werden. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Verfügbar] (gesamt &lt;number of="" hours=""&gt;)</strong>: Die Zahl in Klammern zeigt die Gesamtanzahl der Stunden an, die für alle Monate im Szenario verfügbar sind. Überprüfen oder aktualisieren Sie die Anzahl der Stunden für jeden Monat des Szenarios. Durch Änderung der monatlichen Zuordnung wird die Anzahl der Stunden in den Klammern aktualisiert.</span> </p> </li> 
       </ul> <p>Die manuelle Aktualisierung der monatlichen Zuordnung von Aufgaben für Arbeitsplätze ist eine weitere Möglichkeit, um Konflikte zwischen Aufgabenrollen zwischen Initiativen im Szenario zu lösen. </p> <p>Tipp:   <p><span>Um die monatliche Rollenverfügbarkeit für mehrere Monate zu aktualisieren, geben Sie die Anzahl der Stunden oder FTEs in das Feld [!UICONTROL Verfügbar] eines Monats ein und ziehen Sie dann die Ecke des Felds über die angrenzenden Monate, um denselben Wert für jeden Monat zu kopieren. Legen Sie sie ab, um alle Monate zu aktualisieren.</span> </p> <p> <img src="assets/job-role-distribution-draggable-corner-highlighted-350x83.png" style="width: 350;height: 83;"> </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Erforderlich] (max. &lt;number&gt;)</p> 
       <div> 
        <p role="rowheader">oder</p> 
        <p role="rowheader">[!UICONTROL Erforderlich] (insgesamt &lt;number&gt;)</p> 
       </div> </td> 
      <td> <p><span>Je nachdem, ob Sie sich für die Verwendung von Stunden oder FTE für Ihren Plan entschieden haben, lesen Sie</span> die monatliche Anzahl von FTEs für die Rolle als Job, die für das Szenario erforderlich sind, in den folgenden Feldern: </p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Erforderlich] (max. &lt;number of="" ftes=""&gt;)</strong>: Die Zahl in Klammern zeigt die maximale Anzahl von Rollen an, die für einen der Monate des Szenarios erforderlich sind. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Erforderlich] (insgesamt &lt;number of="" hours=""&gt;)</strong>: Die Zahl in Klammern zeigt die Gesamtzahl der Stunden an, die für alle Monate des Szenarios erforderlich sind.</span> </p> </li> 
       </ul> <p>Tipp: Sie können die erforderliche Anzahl von FTEs nicht ändern <span>oder Stunden</span> für die Rolle "Arbeit". Diese Zahl wird für das Szenario angezeigt, nachdem Sie mit dem Hinzufügen von Initiativen und deren Anforderungen an die Rolle in der Arbeitswelt begonnen haben. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Unterschied]</td> 
      <td> 
       <div> 
        <p>Die monatliche Differenz zwischen den erforderlichen und verfügbaren Auftragsrollen für das Szenario. [!DNL Workfront] berechnet den Unterschied für jede Stellenrolle für jeden Monat mithilfe der folgenden Formel:</p> 
        <p><code>Monthly role difference = Monthly required roles - Monthly available roles</code> (in VZÄ oder Stunden) </p> 
        <p>Tipp: Wenn der Unterschied eine negative Zahl anzeigt, erfordert das Szenario mehr Stellenrollen als der Plan verfügbar ist. Ihre Ressourcen sind überzugewiesen. </p> 
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
         <li> <p><b>Grün</b>: Die verfügbare und die erforderliche Anzahl von Auftragsrollen stimmen überein. Die Ressourcen sind vollständig zugewiesen und der Prozentsatz der Verwendung beträgt 100%. </p> </li> 
         <li> <p><b>Rot</b>: Es gibt mehr erforderliche Jobrollen als der Plan verfügbar ist. Die Ressourcen werden überverteilt und der Prozentsatz der Auslastung liegt bei über 100 %.</p> </li> 
         <li> <p><b>Blau</b>: Es stehen mehr Jobrollen zur Verfügung, als erforderlich sind. Die Mittel sind zu niedrig zugewiesen und der Prozentsatz der Auslastung liegt unter 100 %. </p> </li> 
        </ul> 
       </div> <p> <img src="assets/utilization-percent-colors-sp-350x61.png" style="width: 350;height: 61;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **[!UICONTROL Anwenden]** Speichern der monatlichen Aufgabenrollenverteilung

   Oder

   Klicken **[!UICONTROL Abbrechen]** , um die Verteilungsliste für die Auftragsrolle zu schließen und zum Szenario zurückzukehren.

1. Klicken Sie auf **[!UICONTROL Finanzausstattung]** in der Kopfzeile des Plans, um das Budget für diesen Plan hinzuzufügen.

   Die Einzelheiten der [!UICONTROL Finanzausstattung] angezeigt.

   >[!TIP]
   >
   >Die Währung, in der [!DNL Workfront] verwendet für diesen Plan wird in Klammern im Titel des Felds angezeigt.

1. Geben Sie die **[!UICONTROL Jahresbudget]**.

   >[!NOTE]
   >
   >Wenn Ihr Plan mehrere Jahre umfasst, müssen Sie für jedes Jahr einen Budgetbetrag angeben.

1. Drücken Sie die Eingabetaste , um das jährliche Budget zu speichern, und [!UICONTROL Registerkarte] , um zum folgenden Jahr zu wechseln.

   Das jährliche Budget wird automatisch zu gleichen Teilen für jeden Monat des ausgewählten Jahres verteilt.

1. Klicken **[!UICONTROL Erweitert]** um die monatliche Budgetverteilung anzuzeigen. Die jährlichen und monatlichen Budgets sind immer auf Zahlen gerundet. Wenn der Budgetbetrag aufgrund von Dezimalstellen nicht gleichmäßig auf alle Monate innerhalb eines Jahres verteilt werden kann **[!UICONTROL Verbleibend]** wird unter der jährlichen Budgetverteilung angezeigt.

   ![](assets/adanced-and-remaining-links-on-plan-budget-350x507.png)

1. Passen Sie die monatlichen Budgets manuell an, um die überschrittenen Beträge zu eliminieren.

   Wenn die Summe aller monatlichen Budgetbeträge den Jahreshaushalt übersteigt, wird ein **[!UICONTROL mehr]** Warnhinweis wird unter der jährlichen Budgetverteilung angezeigt. Passen Sie die monatlichen Budgetbeträge manuell an, bis sie dem für den Plan verfügbaren Budget entsprechen oder darunter liegen.

   ![](assets/exceeding-budget-warning-on-plan-350x483.png)

1. Deaktivieren Sie die **[!UICONTROL Personenkosten einschließen]** Festlegung, um die mit Stellenangeboten verbundenen Kosten von der Zählung auf die Gesamtkosten des Plans auszuschließen. Feste Kosten werden immer auf die Gesamtkosten des Plans angerechnet. Diese Einstellung ist standardmäßig aktiviert und wirkt sich auf alle Szenarien im Plan aus.
1. Klicken Sie auf eine beliebige Stelle außerhalb von [!UICONTROL Finanzausstattung] zum Schließen. Die eingegebenen Informationen werden automatisch gespeichert.

   Sie können nun mit der Erstellung der Initiativen für den Plan und dem Hinzufügen von Szenarien beginnen.

1. (Empfohlen) Klicken Sie auf **[!UICONTROL Neue Initiative]** um eine neue Initiative hinzuzufügen.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Should this include information on how to create scenarios - see also information about scenarios in Manage Plans?)</p>
   -->

   Informationen zum Hinzufügen von Initiativen finden Sie im Artikel [Erstellen und Bearbeiten von Initiativen im [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. (Optional) Erstellen Sie eine Kopie des vorhandenen Szenarios, um ein neues Szenario desselben Plans zu erstellen. Weitere Informationen zum Erstellen und Verwenden mehrerer Szenarien finden Sie unter [Erstellen und Vergleichen von Planszenarien in [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).
1. Klicken **[!UICONTROL Plan speichern]**.

   Ihr Plan wird erstellt oder aktualisiert.

1. (Optional) Klicken Sie auf die **[!UICONTROL Favoriten-Symbol]** ![](assets/favorites-icon-small.png) rechts neben dem Namen des Plans klicken, um den Plan Ihrer Favoritenliste hinzuzufügen.

1. (Optional) Kopieren Sie die URL des Plans und senden Sie sie an jeden anderen Benutzer, der sie möglicherweise überprüfen oder aktualisieren muss. Sie müssen mindestens [!UICONTROL Ansicht] Zugriff auf die Zugriffsstufe, um den Plan anzeigen zu können. Sie müssen [!UICONTROL Bearbeiten] Zugriff auf die Bearbeitung. Wenn sie die finanziellen Informationen über den Plan, wie Informationen über Budgets, Kosten und Stellenkosten, überprüfen müssen, müssen sie auch Zugang zu [!UICONTROL Finanzdaten] in ihrer Zugriffsebene. Informationen über den für die [!DNL Scenario Planner], siehe [Zugriff erforderlich für die Verwendung der [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).
