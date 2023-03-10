---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Pläne - Übersicht im Szenario-Planer
description: Als Business Manager können Sie mit dem Adobe Workfront-Szenario-Planer die kurz- und langfristige Zukunftsstrategie Ihres Unternehmens skizzieren, indem Sie seine Ein-, Drei- oder Fünf-Jahres-Pläne skizzieren.
author: Alina
feature: Workfront Scenario Planner
exl-id: df2b895b-8bc1-4a55-b0d7-8a06db420315
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '1290'
ht-degree: 0%

---

# Übersicht über Pläne im [!DNL Scenario Planner]

Die [!DNL Scenario Planner] erfordert zusätzlich zur [!DNL Adobe Workfront] Lizenz. Informationen zum [!DNL Workfront Scenario Planner], siehe [Die [!DNL Scenario Planner] Übersicht](../scenario-planner/scenario-planner-overview.md).

Als Business Manager können Sie die [!DNL Adobe Workfront Scenario Planner] um die Strategie für die kurz- und langfristige Zukunft Ihres Unternehmens zu skizzieren, indem Sie die Ein-, Drei- oder Fünfjahrespläne skizzieren.

## Zugriffsanforderungen

So verwenden Sie die [!DNL Adobe Workfront Scenario Planner] Sie benötigen folgenden Zugriff:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] Plan</a>*</p> </td> 
   <td>[!UICONTROL Business] oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Lizenztyp*</p> </td> 
   <td> <p>[!UICONTROL Review] oder höher. Weitere Informationen finden Sie unter <a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] Lizenzübersicht</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td> <p>Sie müssen eine zusätzliche Lizenz für die [!DNL Adobe Workfront Scenario Planner] , um auf die in diesem Artikel beschriebene Funktionalität zuzugreifen.</p> <p>Informationen zum Abrufen der [!DNL Workfront Scenario Planner], siehe <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Zugriff erforderlich für die Verwendung der [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Zugriffsebene*</td> 
   <td> <p>Zugriff auf die [!UICONTROL Ansicht] oder höher auf die [!DNL Scenario Planner]</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Objektberechtigungen</p> </td> 
   <td> <p>[!UICONTROL Ansichtsberechtigungen oder höher für einen Plan<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (NOTE: this might change if they have permissions for initiatives/ scenarios, etc) 
      </MadCap:conditionalText>
     --></p> <p>Informationen über die Anforderung eines zusätzlichen Zugangs zu einem Plan finden Sie unter <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Anfordern des Zugriffs auf einen Plan im [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Übersicht über Pläne

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add information about utilization percentage for job roles - per this story?? - https://hub.workfront.com/task/5eb0784900083e1f2cabb60d6e0d04d3/overview)</p>
-->

Sie können jedes Ergebnis der Organisation auf hoher Ebene identifizieren und es als Plan zum [!DNL Workfront Scenario Planner]. Ein Plan ist das größte Arbeitselement im [!DNL Scenario Planner]. Um die Erstellung des Plans zu vereinfachen, können Sie ihn in mehrere Initiativen unterteilen, um anzugeben, welche Schritte die einzelnen Organisationseinheiten zur Fertigstellung des Plans unternehmen müssen.

Anschließend können Sie Initiativen mit echten Projekten verbinden, um anzugeben, wie die tatsächlichen Arbeitsfaktoren für die tatsächliche Fertigstellung des Plans sind. Dieser Artikel enthält allgemeine Informationen zu Plänen. Weitere Informationen zu Initiativen finden Sie unter [Übersicht über Initiativen im [!DNL Scenario Planner]](../scenario-planner/initiatives-overview.md).

Sie können die erforderlichen Arbeitskräfte- und Finanzressourcen definieren, um die im Plan festgelegten Arbeiten abzuschließen. Sie können sich auch die für die im Plan vorgesehenen Initiativen erforderlichen Arbeitskräfte- und Finanzressourcen ansehen, damit sie abgeschlossen werden können.

Sie können die folgenden Informationen für jeden Plan schätzen und überprüfen:

* Schätzen Sie den Typ und die Anzahl der für die Ausführung des Plans verfügbaren Auftragsrollen.
* Schätzen Sie das Budget, das Ihr Unternehmen zum Abschluss des Plans benötigt.
* Überprüfen Sie den Prozentsatz der Auslastung jeder Stellenrolle anhand der erforderlichen Stellenrollen, die mit den Initiativen verbunden sind.
* Prüfen Sie den Nutzungsprozentsatz Ihres Planbudgets anhand der mit den Initiativen verbundenen Kosten.
* Überprüfen Sie den Nettowert des Plans zu jedem Zeitpunkt.
* Die Informationen auf Planebene ändern sich, wenn Sie verschiedene Szenarien auswählen. Jedes Szenario verfügt über unterschiedliche Budget- und Personendaten.

Informationen zum Erstellen von Plänen finden Sie im Artikel [Erstellen und Bearbeiten von Plänen im [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Informationen zum Erstellen von Szenarien finden Sie unter [Erstellen und Vergleichen von Planszenarien in [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

## Überlegungen zu Plänen

Beachten Sie beim Erstellen von Plänen Folgendes:

* Sie können Pläne für ein Team, eine ganze Abteilung oder sogar für Ihr gesamtes Unternehmen erstellen. Pläne sind große Planungseinheiten, die die Strategie eines Unternehmens auf hoher Ebene umreißen.
* Der kürzeste Plan kann eine Laufzeit von 1 Jahr haben. Der längste Plan kann eine Laufzeit von 5 Jahren haben.
* Sie können die eigentliche Arbeit an einem Plan nicht erledigen. Sie können grob abschätzen, ob Sie über die Ressourcen und das Budget verfügen, die für die Planung der Arbeit erforderlich sind. Wenn Ihr Unternehmen beispielsweise ein neues Büro an einem neuen Standort erweitern und erwerben möchte, müssen die erforderlichen Schritte ausgeführt werden, die zunächst in einem Plan auf der Ebene der obersten Führungsebene beschrieben werden können.
* Sie können mehrere Szenarien desselben Plans erstellen. Wenn Ihr ursprünglicher Plan zu viele widersprüchliche Initiativen enthält, sollten Sie mehrere Szenarien erstellen, in denen Sie Initiativen oder Budgets und Kosten bearbeiten können, um zu sehen, welche ideale Situation für die Durchführung des Plans besteht. Initiativen können miteinander in Konflikt geraten, wenn sie versuchen, dieselben Ressourcen während desselben Zeitraums zu verwenden. Sie können dann Szenarien vergleichen, um zu sehen, was am sinnvollsten ist und welches von Ihrem Unternehmen übernommen werden sollte, bevor es beginnt, die eigentlichen Arbeiten hinzuzufügen, um dies zu erreichen. Informationen zum Erstellen von Szenarien finden Sie im Artikel [Erstellen und Vergleichen von Planszenarien in [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).
* Sie können einem Plan mehrere Initiativen hinzufügen, um anzugeben, wie kleinere Planungseinheiten zur Fertigstellung des Plans beitragen werden. Wenn Sie beispielsweise planen, sich auf einen bestimmten Markt auszudehnen, können Sie mehrere Initiativen auf Abteilungsebene haben, die letztendlich dazu beitragen, die Expansion auf allen Ebenen der Organisation zu erreichen. Informationen zum Erstellen von Initiativen finden Sie im Artikel [Erstellen und Bearbeiten von Initiativen im [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).
* Wenn Sie einen Plan erstellen, können Sie ihn nur anzeigen. Sie müssen den Plan mit anderen Benutzern abschließen und diese können darauf zugreifen, wenn sie zumindest Zugriff auf die Ansicht haben auf [!DNL Scenario Planner] in ihrer Zugriffsstufe.

## Informationen zu Aufgabenrollen bei Plänen

Sie können allgemeine Informationen zu den Jobrollen für Pläne anzeigen, in denen die Anzahl der für den Plan verfügbaren Rollen sowie die Anzahl der für den Abschluss der Initiativen erforderlichen Arbeitsplatzrollen angegeben sind. Diese Informationen finden Sie im [!UICONTROL Vorgangsrollen] in der Kopfzeile des Plans.

![](assets/job-role-box-on-plan-not-expanded-fte-350x141.png)

Im Feld &quot;Auftragsrolle&quot;können Sie Folgendes anzeigen:

| Informationen | Beschreibung |
|---|---|
| FTE/Stunden-Indikator | Die ([!UICONTROL FTE]) oder ([!UICONTROL Stunden]) neben &quot;[!UICONTROL Auftragsrolle]&quot; title gibt an, ob der Plan zur Verwendung von FTEs oder Stunden bei seiner Erstellung eingerichtet wurde. Der Plan, alle Szenarien und Initiativen verwenden diese Einheit. |
| [!UICONTROL Verfügbar] | Die Anzahl der für das aktuelle Szenario verfügbaren FTEs für die Rolle &quot;Job&quot;oder Stunden. |
| Erforderlich | Die Anzahl der FTEs für die Rolle von Arbeitsplätzen oder Stunden, die von allen Initiativen im aktuellen Szenario benötigt werden, damit sie abgeschlossen werden können. |

Weitere Informationen zum Zugriff auf einen Plan und zum Anzeigen detaillierter Informationen zu Auftragsrollen finden Sie unter [Erstellen und Bearbeiten von Plänen im [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Finanzinformationen zu Plänen

Sie können Finanzinformationen über einen Plan überprüfen, insbesondere dessen Budget, wie dieser verwendet wird und was der Nettowert des Plans ist. Der Nettowert eines Plans basiert auf dem Nettowert seiner Initiativen. Diese Informationen finden Sie im [!UICONTROL Finanzausstattung] und [!UICONTROL Zusammenfassung] in der Kopfzeile des Plans.

![](assets/budget-net-value-boxes-on-plan-not-expanded-350x86.png)

Sie können Folgendes im [!UICONTROL Finanzausstattung] und [!UICONTROL Zusammenfassung] Kisten auf dem Plan:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL Budget] </p> <p role="rowheader"> </p> </td> 
   <td>Dies ist der Geldbetrag, den Ihr Unternehmen für die Ausführung des Plans festlegt. Workfront verteilt das Budget für jeden Monat während der Laufzeit des Plans gleichmäßig. Die Budgets werden in der Regel für ein Jahr festgelegt, können aber auch für einen Zeitraum von 3 oder 5 Jahren festgelegt werden. Die Währung in den Klammern links neben dem Titel der Finanzbox gibt die Währung Ihres Systems an. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Kosten]</td> 
   <td> <p>Dies ist der Gesamtbetrag der Kosten, die aus allen Initiativen im Rahmen des Plans entstehen. Workfront berechnet die Plankosten nach folgender Formel:</p> <p><code>Plan Costs = SUM(Initiative Costs)</code> </p> <p>Informationen zur Berechnung der Kosten einer Initiative finden Sie unter <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">Erstellen und Bearbeiten von Initiativen im [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">UTIL (Prozentsatz der Budgetauslastung)</td> 
   <td> <p>Dies ist ein berechneter Prozentsatz zwischen den Kosten im Zusammenhang mit Initiativen und dem für den Plan festgelegten Budget. </p> <p>[!DNL Workfront] berechnet den Prozentsatz der Budgetnutzung für einen Plan anhand der folgenden Formel: </p> <p><code>Utilization percentage = (Plan Costs* 100))/ Plan Budget</code> </p> <p>Die Kosten werden nach folgender Formel berechnet:</p> <p><code>Plan Costs = SUM(Initiatives People Costs, Initiatives Fixed Costs)</code> </p> <p>Tipp: Der Prozentsatz für die Verwendung wird gerundet und hat eine Dezimalstelle. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Bereich [!UICONTROL Nettowert] <span>im Feld [!UICONTROL Zusammenfassung]</span></p> <p role="rowheader"> </p> </td> 
   <td> <p>Dies ist eine Berechnung aller Nettowerte aller Initiativen im Plan. </p> <p>Workfront berechnet den Nettowert für den Plan anhand der folgenden Formel: </p> <p><code>Plan Net Value = SUM(Initiative Planned Benefit - People Costs)</code> </p> <p>Oder</p> <p><code>Plan Net Value = SUM(Initiative Net Value)</code> </p> <p>Weitere Informationen zu den Netzwerten von Initiativen finden Sie im Artikel <a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">Übersicht über Initiativen im [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Informationen zum Zugriff auf einen Plan und zum Anzeigen detaillierter Finanzinformationen finden Sie unter [Erstellen und Bearbeiten von Plänen im [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).


