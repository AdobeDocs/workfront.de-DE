---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Übersicht über Initiativen im Szenario-Planer
description: Der Szenario-Planer ist nur im neuen Adobe Workfront-Erlebnis verfügbar und erfordert eine zusätzliche Lizenz. Weitere Informationen zum Workfront-Szenario-Planer finden Sie unter Übersicht über den Szenario-Planer .
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 0%

---

# Übersicht über Initiativen im [!DNL Scenario Planner]

Die [!DNL Scenario Planner] ist nur in der neuen [!DNL Adobe Workfront] Erfahrung und erfordert eine zusätzliche Lizenz. Informationen zum [!DNL Workfront Scenario Planner], siehe [Die [!DNL Scenario Planner] Übersicht](../scenario-planner/scenario-planner-overview.md).
Als Business Manager können Sie im [!DNL Adobe Workfront Scenario Planner]. Informationen zum Erstellen von Plänen finden Sie im Artikel [Erstellen und Bearbeiten von Plänen im [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Übersicht über Initiativen

Verwenden der [!DNL Workfront Scenario Planner]können Sie für jede Initiative die folgenden Informationen schätzen und überprüfen:

* Schätzen Sie die Art und Anzahl der Rollen, die zum Abschluss der Initiative erforderlich sein könnten. Dies erhöht die erforderliche Anzahl von Arbeitsplätzen für den Plan und berechnet die Personenkosten, die Sie für eine Initiative überprüfen können.
* Schätzen Sie die Fixkosten, die mit der für den Abschluss der Initiative erforderlichen Arbeit verbunden sind.
* Schätzen Sie den geplanten Nutzen, den Ihr Unternehmen nach Abschluss der Initiative erzielen könnte.

Um Informationen über Ihre Initiativen anzuzeigen, können Sie innerhalb eines Plans auf einzelne Initiativen zugreifen. Informationen zum Erstellen und Aufrufen von Initiativen finden Sie im Artikel [Erstellen und Bearbeiten von Initiativen im [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Überlegungen zu Initiativen

Beachten Sie beim Erstellen von Initiativen Folgendes:

* Sie müssen einen Plan erstellen, bevor Sie eine Initiative erstellen können.
* Sie können Initiativen von Grund auf neu erstellen oder Projekte in einen Plan importieren. Die Projekte werden zu Initiativen im Rahmen des Plans.

   Weitere Informationen zum Erstellen einer Initiative von Grund auf finden Sie unter [Erstellen und Bearbeiten von Initiativen im [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   Informationen zum Importieren von Projekten in einen Plan zur Erstellung von Initiativen aus Projekten finden Sie unter [Importieren von Projekten in Pläne in [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Initiativen sind kleiner als Pläne und werden nur im Rahmen eines Plans erstellt.
* Die kürzeste Initiative kann eine Dauer von 1 Monat haben. Die längste Initiative kann eine Laufzeit von fünf Jahren haben.
* Sie können keine tatsächliche Arbeit an einer Initiative leisten. Auf der Ebene der Initiative können Sie festlegen, welche Ressourcen benötigt werden und welche Kosten diese Ressourcen verursachen, damit Sie eine der Anforderungen des Plans erfüllen können. Wenn Ihr Unternehmen beispielsweise plant, ein neues Büro an einem neuen Standort zu erweitern und zu erwerben, könnte Ihre Abteilung eine Initiative zur Installation der Netzwerkinfrastruktur für diesen neuen Standort haben.
* Sie können mehrere Initiativen in einem Plan erstellen. Mit jeder Initiative können Sie eine allgemeine Strategie für die Arbeit in Ihrer Abteilung entwerfen.
* Sie können Initiativen innerhalb eines Plans priorisieren, um sicherzustellen, dass die wichtigste Initiative das meiste Budget und die meisten Mittel erhält.
* Wenn Sie Initiativen innerhalb eines Plans erstellen, können alle, die diesen Plan betrachten, auch alle Initiativen innerhalb des Plans anzeigen.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change when we add to the access levels granularity)</p>
  -->

* Sie können Initiativen veröffentlichen, um Projekte zu erstellen oder die ihnen zugeordneten Projekte zu aktualisieren. Informationen zu Veröffentlichungsinitiativen finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen im [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

## Finanzinformationen zu Initiativen

Sie können finanzielle Informationen über einzelne Initiativen einsehen, um zu verstehen, wie die Initiativen in den Plan passen. Informationen zum Zugriff auf eine Initiative finden Sie im Artikel [Erstellen und Bearbeiten von Initiativen im [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

Sie können die folgenden Finanzindikatoren zu einer Initiative anzeigen, indem Sie innerhalb eines Plans darauf zugreifen:

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Gesamtkosten]</td> 
   <td> <p style="font-weight: normal;">Dies ist eine Berechnung der Gesamtkosten einer Initiative. </p> <p style="font-weight: normal;">[!DNL Workfront] berechnet anhand dieser Formel den Gesamtkostenwert einer Initiative:</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Festkosten]</td> 
   <td> <p><span style="font-weight: normal;">Dies ist ein manueller Eintrag, in dem Sie Folgendes schätzen können: <span>monatliche Festbeträge für jeden Monat der Initiative.</span> Dies umfasst nicht die Kosten im Zusammenhang mit den Rollen, die der Initiative hinzugefügt und im Feld [!UICONTROL People Cost] erfasst werden.</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Personalkosten]</td> 
   <td> <p style="font-weight: normal;">Dies ist eine Gesamtberechnung der Kosten, die im Zusammenhang mit den Aufgaben im Rahmen der Initiative für die Dauer der Initiative anfallen. Diese Zahl hängt davon ab, wie viele FTEs oder Stunden Sie für die jeweilige Rolle in einem Monat der Initiative schätzen. </p> 
     <p><b>TIPP</b>  
     <ul> 
      <li> <p>Die Anzahl der monatlichen VZÄ für dieselbe Rolle kann von Monat zu Monat variieren.</p> </li> 
      <li> <p>[!DNL Workfront] ist der Auffassung, dass es in einem Monat 160 Arbeitsstunden gibt. </p> </li> 
     </ul> 
     <p>[!DNL Workfront] berechnet die [!UICONTROL People Costs] einer Initiative nach folgender Formel:</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront] berechnet die monatlichen Personalkosten für jeden Monat während der Dauer der Initiative anhand der folgenden Formel:</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>BEISPIEL</b></p>
      <p>Wenn Sie eine Initiative mit einer Dauer von 6 Monaten haben, für die 1 Designer mit einem Stundensatz von 50 USD pro Monat und einem Web-Designer mit einem Stundensatz von 100 USD für 2 Monate der Initiative erforderlich ist, werden die Kosten für Personen der Initiative wie folgt berechnet:</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Geplanter Vorteil]</td> 
   <td>Dies ist ein manueller Eintrag, bei dem Sie den Gesamtvorteil schätzen können, den Ihre Abteilung durch diese Initiative erzielen würde. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nettowert]</td> 
   <td> <p style="font-weight: normal;">Dies stellt den Wert Ihrer Initiative dar, wenn Sie die Gesamtkosten und den für die Initiative geschätzten geplanten Nutzen berücksichtigen. [!DNL Workfront] berechnet den Nettowert einer Initiative anhand der folgenden Formel:</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

<!--drafted content from People Costs:
(NOTE: drafted below)</p> 
       <p>Depending on whether the plan is set up to use FTEs or hours, Workfront uses the following formulas to calculate People Cost:</p> 
       <ul> 
        <li> <p>When using FTEs: </p> <p><code>People Costs = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, where 160 is the total number of working hours in a month. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span style="font-weight: normal;"> When estimating resources using FTEs,(NOTE: drafted and yellow and fix the rest of the sentence)
      <p>When using hours:</p> 
      <p><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> 
      <p>For information about setting up the plan to use hours or FTE, see <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Scenario Planner</a>.</p>-->

## Initiativinformationen in Berichten

Sie können Initiativinformationen in Berichten anzeigen, wie in der folgenden Tabelle beschrieben. Diese Informationen sind nur dann in Ihrer Workfront-Instanz verfügbar, wenn Ihr Unternehmen eine Workfront Scenario Planer-Lizenz erworben hat.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Berichtstyp</b></td> 
   <td><b>Initiativinformationen</b></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative] </td> 
   <td>Name, Dauer, Start- und Enddatum, eingegeben von, ID, Datum der letzten Veröffentlichung*, Alle Projektfelder einschließlich benutzerdefinierter Felder*</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role]</td> 
   <td>Alle oben aufgeführten Initiativinformationen, (Auftrags-Rolle)-ID, Projekt*, Projektzuweisung geplant für Stunden*, Anzahl der Aufgaben für Initiativaufträge, (Auftragsrolle), Alle Projektfelder, einschließlich benutzerdefinierter Felder*</td> 
  </tr> 
  <tr> 
   <td><p>[!UICONTROL Projekt]*</p></td> 
   <td> <p>Alle oben aufgelisteten Informationen zur Initiative*</p> </td> 
  </tr> 
 </tbody> 
</table>

*Diese Felder enthalten Informationen aus dem Projekt, das mit der Initiative verknüpft ist, nur, wenn die Initiative aus einem Projekt erstellt oder mindestens einmal in einem Projekt veröffentlicht wurde. Informationen zu Veröffentlichungsinitiativen finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichen von Initiativen im [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
