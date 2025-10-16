---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Überblick über Initiativen im Szenario-Planer
description: Der Szenario-Planer ist nur in der neuen Adobe Workfront-Version verfügbar und erfordert eine zusätzliche Lizenz. Weitere Informationen zum Workfront-Szenarioplaner finden Sie unter Szenarioplaner - Übersicht .
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
source-git-commit: 86ee649cdf0ac04230035a94a1326c45b67d36d2
workflow-type: tm+mt
source-wordcount: '945'
ht-degree: 0%

---

# Überblick über Initiativen in der [!DNL Scenario Planner]

Als Business Manager können Sie Initiativen für Pläne in der [!DNL Adobe Workfront Scenario Planner] erstellen. Informationen zum Erstellen von Plänen finden Sie im Artikel [Erstellen und Bearbeiten von Plänen in der [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Initiativen - Überblick

Mithilfe der [!DNL Workfront Scenario Planner] können Sie die folgenden Informationen für jede Initiative schätzen und überprüfen:

* Schätzen Sie die Art und Anzahl der Aufgabengebiete, die möglicherweise erforderlich sind, um die Initiative abzuschließen. Dadurch wird die erforderliche Aufgabengebiet-Anzahl für den Plan erhöht und die Personalkosten berechnet, die Sie für eine Initiative überprüfen können.
* Schätzen Sie die Fixkosten im Zusammenhang mit der Arbeit, die zur Fertigstellung der Initiative erforderlich ist.
* Schätzen Sie den geplanten Nutzen für Ihr Unternehmen, der nach Abschluss der Initiative erzielt werden könnte.

Um Informationen zu Ihren Initiativen anzuzeigen, können Sie innerhalb eines Plans auf einzelne Initiativen zugreifen. Informationen zum Erstellen und Bearbeiten von Initiativen finden Sie im Artikel [Erstellen und Bearbeiten von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Überlegungen zu Initiativen

Beachten Sie beim Erstellen von Initiativen Folgendes:

* Sie müssen einen Plan erstellen, bevor Sie eine Initiative erstellen können.
* Sie können Initiativen von Grund auf neu erstellen oder Projekte in einen Plan importieren. Die Projekte werden zu Initiativen innerhalb des Plans.

  Informationen zum Erstellen von Initiativen von Grund auf finden Sie unter [Erstellen und Bearbeiten von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

  Informationen zum Importieren von Projekten in einen Plan zum Erstellen von Initiativen aus Projekten finden Sie [Projekte in Pläne importieren in der [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Initiativen sind kleinere Planungseinheiten als Pläne und werden nur als Teil eines Plans erstellt.
* Die kürzeste Initiative kann eine Dauer von 1 Monat haben. Die längste Initiative kann eine Laufzeit von fünf Jahren haben.
* Eine Initiative kann nicht bearbeitet werden. Auf der Initiativebene können Sie festlegen, welche Ressourcen benötigt werden und welche Kosten für diese Ressourcen anfallen, damit Sie eine der Anforderungen des Plans ausführen können. Wenn beispielsweise Ihr Unternehmen plant, ein neues Büro an einem neuen Standort zu errichten, könnte Ihre Abteilung eine Initiative zur Installation der Netzwerkinfrastruktur für diesen neuen Standort ergreifen.
* Sie können mehrere Initiativen in einem Plan erstellen. Mit jeder Initiative können Sie eine allgemeine Strategie entwerfen, um die Arbeit in Ihrer Abteilung zu erledigen.
* Sie können innerhalb eines Plans Initiativen priorisieren, um sicherzustellen, dass die wichtigste Initiative das meiste Budget und die meisten Ressourcen erhält.
* Wenn Sie Initiativen in einem Plan erstellen, kann jeder, der diesen Plan anzeigt, auch alle Initiativen im Plan anzeigen.
* Sie können Initiativen veröffentlichen, um Projekte zu erstellen oder die mit ihnen verknüpften Projekte zu aktualisieren. Informationen zu Veröffentlichungsinitiativen finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichung von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

## Finanzielle Informationen zu Initiativen

Sie können Finanzinformationen zu einzelnen Initiativen überprüfen, um zu verstehen, wie die Initiativen in den Plan passen. Informationen zum Zugriff auf eine Initiative finden Sie im Artikel [Erstellen und Bearbeiten von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

Sie können die folgenden Finanzindikatoren zu einer Initiative anzeigen, indem Sie in einem Plan darauf zugreifen:

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Gesamtkosten]</td> 
   <td> <p style="font-weight: normal;">Dies ist eine Berechnung der Gesamtkosten einer Initiative. </p> <p style="font-weight: normal;">[!DNL Workfront] Berechnet den Gesamtkostenwert einer Initiative anhand folgender Formel:</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fixkosten]</td> 
   <td> <p><span style="font-weight: normal;">Dies ist ein manueller Eintrag, mit dem Sie <span> monatlichen Fixkosten für jeden Monat der Initiative schätzen können.</span> Dies umfasst nicht die Kosten im Zusammenhang mit den Rollen, die der Initiative hinzugefügt wurden und die im Feld [!UICONTROL Personalkosten] erfasst werden.</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Personalkosten]</td> 
   <td> <p style="font-weight: normal;">Dies ist eine Gesamtberechnung der Kosten, die mit den Aufgabengebieten der Initiative für die Dauer der Initiative verbunden sind. Diese Zahl hängt davon ab, wie viele FTEs oder Stunden Sie für ein Aufgabengebiet für jeden Monat der Initiative schätzen. </p> 
     <p><b>TIPPS</b>  
     <ul> 
      <li> <p>Die Anzahl der monatlichen VZÄ für dasselbe Aufgabengebiet kann von Monat zu Monat unterschiedlich sein.</p> </li> 
      <li> <p>[!DNL Workfront] ist der Ansicht, dass es in einem Monat 160 Arbeitsstunden gibt. </p> </li> 
     </ul> 
     <p>[!DNL Workfront] Berechnet die [!UICONTROL Personalkosten] einer Initiative nach folgender Formel:</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront] berechnet die monatlichen Personalkosten für jeden Monat während der Dauer der Initiative anhand der folgenden Formel:</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>BEISPIEL</b></p>
      <p>Wenn Sie eine Initiative mit einer Dauer von 6 Monaten haben, für die 1 Designer mit einem Stundensatz von 50 USD für 1 FTE pro Monat und ein Web-Designer mit einem Stundensatz von 100 USD für 2 Monate der Initiative erforderlich sind, werden die Personalkosten der Initiative wie folgt berechnet:</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Geplanter Nutzen]</td> 
   <td>Dies ist ein manueller Eintrag, mit dem Sie den Gesamtvorteil schätzen können, den Ihre Abteilung durch den Abschluss dieser Initiative erzielen würde. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nettowertbetrag]</td> 
   <td> <p style="font-weight: normal;">Dies entspricht dem Wert Ihrer Initiative unter Berücksichtigung der Gesamtkosten und des für die Initiative geschätzten geplanten Nutzens. [!DNL Workfront] berechnet den Nettowert einer Initiative anhand der folgenden Formel:</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
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

## Informationen zur Initiative in Berichten

Sie können Initiativinformationen in Berichten anzeigen, wie in der folgenden Tabelle beschrieben. Diese Informationen sind in Ihrer Workfront-Instanz nur verfügbar, wenn Ihr Unternehmen eine Workfront Scenario Planner-Lizenz erworben hat.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Berichtstyp</b></td> 
   <td><b>Informationen zur Initiative</b></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative] </td> 
   <td>Name, Dauer, Start- und Enddatum, eingegeben von, ID, Datum der letzten Veröffentlichung*, Alle Projektfelder einschließlich benutzerdefinierter Felder*</td> 
  </tr> 
  <tr> 
   <td>Aufgabengebiet der [!UICONTROL Initiative]</td> 
   <td>Alle oben aufgeführten Informationen zur Initiative, (Aufgabengebiet)-ID, Projekt*, Projektzuweisung, geplante Stunden*, Aufgabengebiet-Stunden für die Initiative, (Aufgabengebiet)-Anzahl, alle Projektfelder einschließlich benutzerdefinierter Felder*</td> 
  </tr> 
  <tr> 
   <td><p>[!UICONTROL-Projekt]*</p></td> 
   <td> <p>Alle oben aufgeführten Informationen zur Initiative*</p> </td> 
  </tr> 
 </tbody> 
</table>

*Diese Felder werden nur dann mit Informationen aus dem mit der Initiative verknüpften Projekt gefüllt, wenn die Initiative aus einem Projekt erstellt oder mindestens einmal in einem Projekt veröffentlicht wurde. Informationen zu Veröffentlichungsinitiativen finden Sie unter [Aktualisieren oder Erstellen von Projekten durch Veröffentlichung von Initiativen in der [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
