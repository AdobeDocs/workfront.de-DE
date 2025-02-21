---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Lösen von Initiativkonflikten im Szenario-Planer
description: Wenn Initiativen miteinander in Konflikt stehen, konkurrieren sie um dieselben Ressourcen. Die für ein Szenario verfügbaren Ressourcen reichen nicht aus, um alle für alle Initiativen im Szenario erforderlichen Ressourcen abzudecken.
author: Alina
feature: Workfront Scenario Planner
exl-id: d3a3e177-bece-4e03-89d7-9cee6127bc55
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '2220'
ht-degree: 0%

---

# Lösen von Initiativkonflikten im [!DNL Scenario Planner]

Wenn Initiativen miteinander in Konflikt stehen, konkurrieren sie um dieselben Ressourcen. Die für ein Szenario verfügbaren Ressourcen reichen nicht aus, um alle für alle Initiativen im Szenario erforderlichen Ressourcen abzudecken.

Dies kann in jedem der folgenden Fälle eintreten:

* Die Anzahl der für die Initiative erforderlichen Aufgabengebiete ist größer als die Anzahl der für den Plan budgetierten Aufgabengebiete.
* Die Kosten der Initiative übersteigen die für den Plan verfügbaren Haushaltsmittel.

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

## Konflikte lösen - Übersicht

* Ein Konflikt wird auch als eine Überallokation der Aufgabengebiete oder des Budgets eines Szenarios verstanden.
* Wenn [!DNL Workfront] einen Konflikt erkennt, wird der Balken, der dem Monat entspricht, in dem der Konflikt während der Dauer der Initiative besteht, rot angezeigt. Dies kann in jedem der folgenden Fälle eintreten:

   * Die Anzahl der monatlich für eine Initiative erforderlichen Aufgabengebiete ist größer als die Anzahl der für den Plan budgetierten Aufgabengebiete, nachdem alle vorherigen Initiativen die für den Plan budgetierten Ressourcen verwendet haben.
   * Die monatlichen Kosten der Initiative sind höher als das für den Plan verfügbare Budget, nachdem alle vorherigen Initiativen das Budget des Plans zur Deckung ihrer Kosten genutzt haben.

>[!TIP]
>
>Standardmäßig geht der [!DNL Scenario Planner] davon aus, dass Sie für ein Szenario 0 Aufgabengebiete und 0 Dollar oder das Äquivalent von 0 Dollar in der Systemwährung budgetiert haben, sofern Sie nichts anderes angegeben haben. Die Anzahl der Aufgabengebiete gibt die Anzahl der FTEs (Vollzeitäquivalente) oder Stunden an, die für das Aufgabengebiet budgetiert wurden.
>
>Für alle Berechnungen im Szenario-Planer verwendet Workfront den folgenden Wert: 1 FTE = 8 Stunden.
>
>Informationen zum Aktualisieren der verfügbaren Rollen für einen Plan und ein Budget finden Sie unter [Erstellen und Bearbeiten von Plänen in der [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

* Sie können einen Konflikt wie folgt lösen:

   * Automatisches Hinzufügen der fehlenden erforderlichen Ressourcen von den Initiativen im Szenario. In diesem Artikel wird beschrieben, wie Sie Konflikte mit dieser Option lösen können.
   * Aufgabengebiet und Budgetressourcen für das Szenario durch Bearbeiten des Plans anpassen. Weitere Informationen finden Sie unter [Erstellen und Bearbeiten von Plänen in der [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Konflikte zwischen Initiativen lösen

1. Wechseln Sie zu einem Plan, für den Sie Konflikte lösen möchten.

   Informationen zum Erstellen von Plänen finden Sie unter [Erstellen und Bearbeiten von Plänen in der [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   Informationen zum Erstellen von Initiativen finden Sie unter [Erstellen und Bearbeiten von Initiativen im [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. (Optional) Wählen Sie aus dem Dropdown-Menü **[!DNL Initial scenario]** das Szenario aus, das Sie überprüfen möchten.

   >[!TIP]
   >
   >Ein Plan kann mehrere Szenarien aufweisen. Bei der Betrachtung der Konflikte im Plan bezieht [!DNL Workfront] sich auf die derzeit für das ausgewählte Szenario verfügbaren Ressourcen und die für die Initiativen in diesem Szenario erforderlichen Ressourcen. Weitere Informationen zu Szenarien finden Sie unter [Planszenarien erstellen und vergleichen in der [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. Stellen Sie sicher **[!UICONTROL dass „Konflikte anzeigen]** aktiviert ist. Sie ist standardmäßig aktiviert.

   ![Umschalter „Szenarien anzeigen“](assets/show-scenarios-toggle-on.png)

   Die erste Initiative mit Konflikten zeigt die Monate mit Konflikten in rot an. Neben dem Namen der Initiative wird ein Warnsymbol angezeigt.

   Der Hintergrund aller Initiativen, beginnend mit der ersten, die im Konflikt stehen, wird im Plan rot dargestellt.

   Wenn bei einer Initiative ein Konflikt auftritt, bedeutet dies, dass die Anzahl der Aufgabengebiete für mindestens eine bestimmte Funktion, die entstandenen Kosten oder beide die Anzahl der Aufgabengebiete bzw. das Budget überschreiten, die für den Plan für einen bestimmten Monat definiert wurden.

   ![Initiativen für Plan mit Konflikt](assets/initiatives-on-plan-with-conflicts-350x126.png)

1. Führen Sie einen der folgenden Schritte aus, um mehr über die möglichen Konflikte zu erfahren:

   * Bewegen Sie den Mauszeiger über das Warnsymbol neben dem Namen der Initiative, um zu verstehen, ob Sie ein Aufgabengebiet oder einen Budgetkonflikt haben.

     ![Budget-Aufgabengebiet-Konflikt](assets/budget-job-role-conflict-tooltip-on-warning-icon-350x109.png)

     Je nachdem, ob Sie Aufgabengebiete überlastet oder die Kosten für Ihre Initiative überschätzt haben, sehen Sie beim Bewegen des Mauszeigers über das Warnsymbol möglicherweise eine der folgenden Optionen:

      * Aufgabengebiet-Konfliktdetails anzeigen
      * Budget-Konfliktdetails anzeigen
      * Aufgabengebiet- und Budgetdetails anzeigen

   * Wenn Sie den Plan nach Monat anzeigen, bewegen Sie den Mauszeiger über einen Monat in der Zeitleiste des Plans, um die erforderlichen Ressourcen für diesen Monat anzuzeigen und zu sehen, ob die Konflikte für den Monat Personen oder kostenbezogen sind.

     ![Details zu Konflikten in der monatlichen Zeitleiste](assets/details-of-conflicts-on-monthly-plan-timeline-pop-up-350x178.png)

     Überprüfen Sie die folgenden monatlichen Informationen auf Planebene:

      * Die Anzahl der verfügbaren, erforderlichen und überlasteten Aufgabengebiete für den Monat für alle für diesen Monat geplanten Initiativen
      * Die verfügbaren, erforderlichen und überlasteten Kosten für den Monat für alle für diesen Monat geplanten Initiativen

        >[!TIP]
        >
        >Die [!UICONTROL Verfügbare] Kosten sind das Budget des Szenarios für diesen Monat.

   * Bewegen Sie den Mauszeiger einen Monat über den roten Balken einer Initiative, um das Feld mit zusätzlichen Informationen über den in diesem Monat auftretenden Konflikt anzuzeigen.

     ![Details zu Konflikten in der Zeitleiste der Initiative](assets/details-of-conflicts-on-initiative-timeline-pop-up-350x113.png)

     Überprüfen Sie die folgenden Felder im Feld Zusätzliche Informationen auf der Ebene der Initiative:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Monat, in dem der Konflikt auftritt</td> 
        <td>Wird im Titel des Felds Zusätzliche Informationen angezeigt.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Der Name der Initiative</td> 
        <td>Wird im Titel des Felds Zusätzliche Informationen angezeigt.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">[!UICONTROL Aufgabengebiete]</td> 
        <td> <p>Die mit dieser Initiative verknüpften Aufgabengebiete, die für den ausgewählten Monat überlastet sind. In den folgenden Spalten werden Informationen zu den einzelnen Aufgabengebieten angezeigt, die für den ausgewählten Monat erforderlich sind und die mit der Anzahl der für diesen Monat verfügbaren Aufgabengebiete kollidieren:</p> 
         <ul> 
          <li> <p><strong>[!UICONTROL Available]</strong>: Die Anzahl der einzelnen Aufgabengebiete, die im Szenario für den ausgewählten Monat verfügbar sind.</p> </li> 
          <li> <p><strong>[!UICONTROL Erforderlich]</strong>: Die Anzahl der einzelnen Aufgabengebiete, die für die Initiative im ausgewählten Monat erforderlich sind.</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL Überlastet]:</strong> Die Differenz zwischen der für die Initiative erforderlichen Zahl und der aus dem Szenario verfügbaren Zahl. </p> </li> 
         </ul> <p>Tipp: Manchmal stimmt die Anzahl der [!UICONTROL Available]-Rollen mit der Anzahl der [!UICONTROL Required]-Rollen überein oder ist höher, aber die [!DNL Scenario Planner] zeigt weiterhin eine übermäßige Zuordnung an. Dies bedeutet, dass es höherrangige Initiativen gibt, die bereits die im Plan für denselben Monat verfügbaren Aufgabengebiete verwendet haben. </p> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Kosten</td> 
        <td> <p>Die Kosten der Initiative für den ausgewählten Monat. In den folgenden Spalten werden Informationen zu den für den ausgewählten Monat erforderlichen Kosten und dem verfügbaren Budget angezeigt:</p> 
         <ul> 
          <li> <p><strong>[!UICONTROL Available]</strong>: Das Budget, das für den ausgewählten Monat aus dem Plan verfügbar ist.</p> </li> 
          <li> <p><strong>[!UICONTROL Erforderlich]</strong>: Die mit dieser Initiative verbundenen Kosten für den ausgewählten Monat.</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL Überlastet]:</strong> Die Differenz zwischen den Kosten der Initiative und dem verfügbaren Budget des Plans. </p> </li> 
         </ul> <p>Tipp: Manchmal stimmen die [!UICONTROL Available] Kosten mit den [!UICONTROL Required] Kosten der Initiative für den ausgewählten Monat überein oder sind höher als diese, und die [!DNL Scenario Planner] zeigt weiterhin eine Überallokation der Kosten an. Dies bedeutet, dass es höherrangige Initiativen gibt, die bereits das verfügbare Budget für den Plan für denselben Monat verwenden. </p> </td> 
       </tr> 
      </tbody> 
     </table>

1. Führen Sie einen der folgenden Schritte aus, um das Bedienfeld Details der Initiative zu öffnen und weitere Informationen zum Auftreten und zur Lösung von Konflikten anzuzeigen:

   * Klicken Sie auf das Warnsymbol neben dem Namen der Initiative.
   * Klicken Sie auf den Balken einer Initiative.
   * Klicken Sie auf das **[!UICONTROL Mehr]**-Symbol ![Mehr](assets/more-icon.png) rechts neben dem Namen der Initiative und dann auf **[!UICONTROL Bearbeiten]**.

     Das Bedienfeld mit den Initiativdetails wird auf der rechten Seite angezeigt.

     Wenn nicht genügend Personen oder Budget für Ihre Initiative zur Verfügung stehen, wird neben den folgenden Abschnitten ein rotes Warnsymbol angezeigt:

   * [!UICONTROL Erforderliche Aufgabengebiete]
   * [!UICONTROL Kosten]

1. (Bedingt) Für Initiativen mit Aufgabengebiet-Konflikten gehen Sie zum Abschnitt **[!UICONTROL Erforderliche Aufgabengebiete]**, um alle für Ihre Initiative erforderlichen Aufgabengebiete anzuzeigen. Identifizieren Sie, welche Aufgabengebiete möglicherweise überlastet sind. Überprüfen Sie die Anzahl der VZÄ oder Stunden, die für jedes Aufgabengebiet für jeden Monat der Initiative benötigt werden. Das Feld mit der FTE- oder Stunden-Nummer für Monate mit Überallokationen wird in einem roten Umriss angezeigt.

   ![Überlastete Rollen](assets/details-panel-overallocated-roles-350x275.png)

1. (Optional) Klicken Sie auf den Pfeil nach rechts neben den Monaten in der Zeitleiste der Initiative, um anzuzeigen, in welchen zusätzlichen Monaten Aufgabengebiet-Konflikte angezeigt werden.

   ![Rechter Fehler im Detailfeld](assets/right-arrow-initiative-months-inside-details-box-highlighted-350x145.png)

1. (Optional) Klicken Sie unter **[!UICONTROL Aufgabengebiet, das einen Konflikt anzeigt, auf Details anzeigen]**, um zu sehen, wo die Konflikte auftreten, und um die konfliktbehafteten Monate im Diagrammbereich des Plans hervorzuheben. Für jedes Aufgabengebiet werden zusätzliche Informationen angezeigt.

   Für jedes Aufgabengebiet werden die folgenden Felder angezeigt:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Available]</td> 
      <td> <p>Die Anzahl der im Plan für jeden Monat verfügbaren Aufgabengebiete. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL zuvor zugewiesen]</td> 
      <td>Die Anzahl der Aufgabengebiete, die bereits aus dem Budget des Plans für höherrangige Initiativen für einen bestimmten Monat zugewiesen wurden. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL überlastet]</td> 
      <td> <p>Der Unterschied zwischen der Anzahl der erforderlichen Aufgabengebiete auf der Initiative und der Anzahl der verfügbaren Stellen im Plan nach höherrangigen Initiativen verwendete auch einige der Rollen. Workfront berechnet die Anzahl der [!UICONTROL Überlastet]-Aufgabengebiete anhand der folgenden Formel:</p> <p><code>Overallocated roles = (Roles Previously Allocated to higher initiatives + Required roles for current initiative) - Monthly available roles from the plan</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Im Diagramm des Plans werden die Monate, in denen die Aufgabengebiete zugewiesen sind, mit dem Namen und der Anzahl der erforderlichen Aufgabengebiete für jede Initiative angezeigt, in der sie benötigt werden. Sie müssen die Ansicht [!UICONTROL Monat] auswählen, um den Namen der Aufgabengebiete anzuzeigen

   ![Widersprüchliche Aufgabengebiete](assets/conflicting-job-role-months-on-plan-after-clicking-show-details-350x158.png)

1. Führen Sie einen der folgenden Schritte aus, um Konflikte mit Aufgabengebieten zu lösen:

   * Passen Sie die Anzahl der Aufgabengebiete für jeden Monat der Initiative manuell auf eine niedrigere Zahl an.
   * Bewegen Sie den Mauszeiger über den Namen des Aufgabengebiets und klicken Sie auf das Symbol **[!UICONTROL Löschen]**![ Löschen](assets/delete.png), um das Aufgabengebiet aus der Initiative zu entfernen.
   * Wählen Sie **[!UICONTROL Rollen zu den verfügbaren Ressourcen des Szenarios hinzufügen]** und klicken Sie dann auf **[!UICONTROL Anwenden]**.

     Dadurch wird die fehlende Anzahl von Aufgabengebiets-VZÄ oder Stunden zum Feld „Verfügbar[!UICONTROL  des ] hinzugefügt.

     >[!NOTE]
     >
     >Mit den Rollen, die Sie zum Beheben der Konflikte hinzufügen, [!UICONTROL  die Aufgabengebiete ]Verfügbar“ für das ausgewählte Szenario und nicht für alle Szenarien im Plan geändert.

     Ein grüner Aufwärtspfeil (![ grüner Aufwärtspfeil) ](assets/upward-green-arrow.png) den Monat in der Zeitleiste des Plans an, um anzugeben, dass dem Plan in diesem Monat weitere Ressourcen hinzugefügt wurden. Sie müssen die Ansicht [!UICONTROL Monat] auswählen, um diesen Indikator anzuzeigen.

   * (Bedingt) Schließen Sie das Bedienfeld Details und geben Sie der Initiative eine höhere Priorität, um Budgetressourcen vom Plan nach Möglichkeit zuerst zu erhalten. Informationen zum Aktualisieren der Priorität der Initiative finden [ unter „Aktualisieren der Prioritäten der Initiative im ](../scenario-planner/prioritize-initiatives.md)&quot;.

1. (Optional) Klicken Sie auf **[!UICONTROL Details ausblenden]**, um das zusätzliche Detailfeld zu schließen, und klicken Sie dann auf **[!UICONTROL Übernehmen]**, um die Änderungen zu speichern, die Sie an den Aufgabengebieten vornehmen.

1. (Bedingt) Initiativen mit Kostenkonflikten können die Kosten für jeden Monat der Dauer der Initiative im Bereich **[!UICONTROL Kosten]** im Bedienfeld „Details der Initiative“ überprüfen. Stellen Sie fest, in welchen Monaten möglicherweise nicht genügend Geld im Budget des Plans vorhanden ist, um die Kosten für die ausgewählte Initiative zu decken. Das Feld mit dem nicht ausreichenden verfügbaren Budget wird in roter Umrandung angezeigt.
1. (Optional) Klicken Sie auf den Pfeil nach rechts neben den Monaten in der Zeitleiste der Initiative, um zusätzliche Monate anzuzeigen, deren Budget nicht ausreicht, um die Kosten zu decken.

   ![Pfeil für unzureichende Kosten](assets/details-panel-insufficient-costs-350x239.png)

1. (Optional) Klicken Sie **[!UICONTROL Details anzeigen]** unter den Kosteninformationen, um zu sehen, wo der Konflikt auftritt, und um die konfliktbehafteten Monate im Diagramm des Plans hervorzuheben. Die folgenden zusätzlichen Felder werden für jeden Kostentyp angezeigt:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Available]</td> 
      <td> <p>Die aus dem Budget des Plans für jeden Monat verfügbaren Kosten. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL zuvor zugewiesen]</td> 
      <td>Der Betrag, der bereits aus dem Budget des Plans für höherrangige Initiativen zugewiesen wurde. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL überlastet]</td> 
      <td> <p>Die monatliche Differenz zwischen den für die Initiative benötigten Kosten und den aus dem Haushalt des Plans verfügbaren Mitteln nach höherrangigen Initiativen verwendete ebenfalls einen Teil der verfügbaren Mittel. [!DNL Workfront] berechnet die Anzahl der überlasteten Kosten anhand der folgenden Formel:</p> <p><code>Overallocated costs = (Costs Previously Allocated to higher initiatives + Required costs for the current initiative) - Monthly available budget from the plan</code> </p> <p>[!DNL Workfront] Berechnet die erforderlichen Kosten für die aktuelle Initiative für jeden Monat nach folgender Formel:</p> <p><code>Required initiative costs = Initiative Fixed Costs + Initiative People Costs</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Im Diagramm des Plans werden in den Monaten, in denen die Kosten nicht ausreichen, der Name und die Anzahl der für die Initiative noch benötigten Aufgabengebiete angezeigt. Sie müssen die Monatsansicht auswählen, um die Kostenbeträge anzuzeigen.

   ![Widersprüchliche Kosten](assets/conflicting-costs-months-on-plan-after-clicking-show-details-350x139.png)

   >[!NOTE]
   >
   >Wenn Sie die Einstellung [!UICONTROL Personalkosten einbeziehen] für das Feld [!UICONTROL Budget] beim Erstellen des Plans deaktiviert haben, wird die Zeile [!UICONTROL Personalkosten] für keine Initiative in einem Szenario angezeigt. In diesem Fall nimmt Workfront keine Personalkosten in Berechnungen auf, um Kostenkonflikte zu ermitteln. Informationen zum Erstellen eines Plans finden Sie unter [Erstellen und Bearbeiten von Plänen in der [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

1. Führen Sie einen der folgenden Schritte aus, um Kostenkonflikte zu lösen:

   * Passen Sie die Anzahl [!UICONTROL Fixkosten] für jeden Monat der Initiative manuell auf eine niedrigere Zahl an.
   * Passen **[!UICONTROL im Abschnitt „Erforderliche]**&quot; nach Möglichkeit manuell die Anzahl der Aufgabengebiete für den Monat mit einem Personalkostenbudget an. Dies reduziert die Personalkosten.

     >[!TIP]
     >
     >Personalkosten können nicht manuell angepasst werden.

   * Wählen Sie **[!UICONTROL Betrag zum Budget des Szenarios hinzufügen]** und klicken Sie dann auf **[!UICONTROL Anwenden]**.

     Dadurch wird das Budget des Szenarios für die Monate, in denen es fehlte, nicht ausreichend belastet, wodurch auch das Gesamtbudget des Szenarios aktualisiert wird.

     >[!NOTE]
     >
     >Der Betrag, den Sie zur Lösung der Kostenkonflikte hinzufügen, ändert das Budget für das ausgewählte Szenario und nicht für alle Szenarien im Plan.

   * (Bedingt) Schließen Sie das Bedienfeld Details und geben Sie der Initiative eine höhere Priorität, um Budgetressourcen vom Plan nach Möglichkeit zuerst zu erhalten. Informationen zur Aktualisierung der Priorität für die Initiative finden Sie [Aktualisieren der Prioritäten für die Initiative im [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Klicken Sie **[!UICONTROL Anwenden]** wenn Sie Änderungen am Abschnitt „Kosten“ vornehmen.
1. Klicken Sie **[!UICONTROL Plan speichern]** um Ihre Änderungen zu speichern.


