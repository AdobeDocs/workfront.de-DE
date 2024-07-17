---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Überblick über die Bereiche des Geschäftsfalls
description: In diesem Artikel werden die Bereiche des Geschäftsfalls eines Projekts beschrieben.
author: Alina
feature: Work Management
exl-id: 0646e4f0-e8fb-48f2-b533-358229543081
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1605'
ht-degree: 2%

---

# Überblick über die Bereiche des Geschäftsfalls

In diesem Artikel werden die Bereiche des Geschäftsfalls eines Projekts beschrieben.

Informationen zum Erstellen eines Geschäftsfeldes für ein Projekt finden Sie unter [Erstellen eines Geschäftsfeldes für ein Projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Ihr Adobe Workfront-Administrator oder Gruppenadministrator muss alle Abschnitte im Geschäftsfall aktivieren, bevor sie im Projekt sichtbar sind, mit Ausnahme des Bereichs Projektinformationen . Der Bereich Projektinfo ist standardmäßig aktiviert.

Weitere Informationen zur Aktivierung der Bereiche des Geschäftsfalls finden Sie im Abschnitt &quot;Geschäftsfälle&quot;unter  [Systemweite Projektanvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Im Folgenden werden die Bereiche im Geschäftsfall eines Projekts beschrieben:

* Projektinfo
* Ziele
* Ausgaben
* Ressourcenbudgetierung
* Risiken
* Scorecard
* Benutzerdefinierte Formulare
* Business Case-Zusammenfassung

## Projektinfo

Der Bereich **Projektinfo** im Geschäftsfall kann vom Workfront-Administrator nicht konfiguriert werden. Alle Projekte haben einen Bereich Projektinfo im Business Case. 

Der Abschnitt &quot;Projektinfo&quot;im Geschäftsfall enthält die grundlegenden Informationen eines Projekts, bevor das Projekt tatsächlich gestartet wurde.

Bearbeiten Sie die folgenden Felder:

* **Beschreibung**: Geben Sie eine Beschreibung für Ihr Projekt an.
* **Projektbesitzer**

  Standardmäßig ist der Benutzer, der das Projekt erstellt, auch der Projekteigentümer. Sie können dieses Feld bearbeiten und einen anderen aktiven Benutzer als Eigentümer des Projekts angeben.

* **Projektsponsor**

  Erwägen Sie, neben dem Projekteigentümer auch eine andere Person als den Sponsor des Projekts hinzuzufügen. Der Sponsor erhält die Genehmigung des Geschäftsfalls. 

* **Portfolio**: Geben Sie ein Portfolio für das Projekt an. Sie müssen das Portfolio erstellen und in den Status **Aktiv** setzen, bevor es in diesem Dropdownmenü ausgewählt werden kann.

  Weitere Informationen zu Portfolios finden Sie unter [Übersicht über Portfolio in Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

  Weitere Informationen zum Erstellen von Portfolios finden Sie unter [Erstellen eines Portfolios](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

* **Geplanter Nutzen**: Schätzen Sie, welcher finanzielle Nutzen für Ihre Organisation geplant ist, wenn dieses Projekt abgeschlossen ist. Es kann sich um einen beliebigen Währungsbetrag handeln, und es muss sich um einen positiven Wert handeln. Beispiel: 10.000 $.
* **Status**: Standardmäßig ist der Status für eine Projektanforderung auf **Idee** festgelegt.

  Wenn Sie den Status auf einen anderen Wert als &quot;Idee&quot;oder &quot;Planung&quot;ändern, verschwindet die Schaltfläche &quot;**Senden**&quot;aus dem Bereich &quot;Zusammenfassung der Geschäftsfälle&quot;und Sie können den Geschäftsfall nicht mehr zur Genehmigung einreichen. 

* **Festes Startdatum**: Geben Sie ein Datum an, an dem das Projekt beginnen soll.
* **Festes Enddatum**: Geben Sie ein Datum an, an dem das Projekt enden soll.

  >[!NOTE]
  >
  >Das feste Start- und Enddatum im Geschäftsfall hat keine Auswirkungen auf die geplanten Start- und Abschlussdaten des Projekts. Diese stellen die Daten dar, die der Projektersteller zum Zeitpunkt der idealen Entwicklung des Projekts anfordert. Stattdessen zeigen die geplanten Start- und Abschlussdaten des Projekts den geplanten Zeitplan für das Projekt an, der auf den Aufgaben des Projekts basiert.

## Ziele

Ziele definieren die Ziele für das Projekt. Dieser Bereich ist standardmäßig im Geschäftsfall aktiviert, aber der Workfront-Administrator kann ihn möglicherweise nicht anzeigen lassen. In diesem Feld werden die Ziele in der Reihenfolge ihrer Priorität angezeigt.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
>
>Sie können strategische Ziele für Ihre Organisation erstellen, die nicht mit dem individuellen Geschäftsszenario eines Projekts verbunden sind. Sie müssen Zugriff auf Adobe Workfront-Ziele haben, um strategische Ziele erreichen zu können. Sie können sie dann mit Projekten außerhalb ihrer Geschäftsfälle verbinden. Informationen zum Erstellen von Zielen mit Workfront-Zielen finden Sie unter [Übersicht über Adobe Workfront-Ziele](../../../workfront-goals/goal-management/wf-goals-overview.md).

Die Definition der Ziele ist optional, damit das Portfolio im Projektoptimierer eine Punktzahl erhält. Dieser Abschnitt ist der einzige optionale Abschnitt im Geschäftsfall. Alle anderen Abschnitte des Geschäftsszenarios müssen ausgefüllt werden, bevor das Projekt in Portfolio Optimizer bewertet wird. Sie können beim Erstellen des Ziels eine Prioritätsstufe für ein Ziel angeben.

Weitere Informationen zu Zielen finden Sie unter  [Erstellen Sie Geschäftsfallziele](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

## Ausgaben

Ausgaben stellen die Nichtarbeitskosten dar, die während der Laufzeit eines Projekts anfallen könnten. Dieser Bereich ist standardmäßig im Geschäftsfall aktiviert, aber der Workfront-Administrator kann ihn möglicherweise nicht anzeigen lassen. 

Alle Ausgaben, die Sie im Geschäftsfall eingeben, werden auch auf dem Tab Ausgaben des Projekts als &quot;Geplante Ausgaben&quot;angegeben.

Ausgaben wirken sich auf die folgenden Felder des Projekts aus:

* Budgetierte Kosten
* Nettowert

Weitere Informationen zu den budgetierten Kosten und Nettowerten finden Sie unter [Übersicht über die Finanzfelder für Geschäftsfälle](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Weitere Informationen zu Ausgaben finden Sie unter  [Verwalten der Projektausgaben](../../../manage-work/projects/project-finances/manage-project-expenses.md) .

Ihr Workfront-Administrator kann benutzerdefinierte Ausgabentypen einrichten.

Weitere Informationen zum Erstellen benutzerdefinierter Ausgabentypen finden Sie unter [Erstellen benutzerdefinierter Ausgabentypen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md). 

## Ressourcenbudgetierung

Sie können die folgenden Aktionen im Bereich Ressourcenbudgetierung des Geschäftsfalls durchführen:

* Verknüpfen Sie Ressourcenpools mit dem Projekt.
* Budget Ihrer Ressourcen auf Projektebene.

Die für die Ressourcen im Projekt veranschlagten Stunden werden im Bereich Ressourcenbudgetierung des Business Case angezeigt, wodurch die budgetierten Arbeitskosten des Projekts generiert werden. Dieser Bereich des Geschäftsfalls ist standardmäßig aktiviert.

Weitere Informationen zu Budgetierungsressourcen für das Projekt im Geschäftsfall finden Sie unter [Budgetressourcen im Geschäftsfall](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

![](assets/business-case-sp-selected-with-choose-button-350x121.png)

Beachten Sie Folgendes bei der Anzeige des Bereichs Ressourcenbudgetierung im Geschäftsfall:

* Sie können Ressourceninformationen hier mit den folgenden Tools einplanen:

   * Der Ressourcen-Planer

     Weitere Informationen finden Sie unter [Budgetressourcen im Geschäftsfall mit dem Resource Planer](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md).

   * Der Szenario-Planer , wenn Ihr Unternehmen eine zusätzliche Lizenz für den Adobe-Szenario-Planer erworben hat

     Weitere Informationen finden Sie unter [Budgetressourcen im Geschäftsfall mit dem Szenario-Planer](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

     Der Szenario-Planer ist nur im neuen Adobe Workfront-Erlebnis verfügbar und erfordert eine zusätzliche Lizenz. Weitere Informationen zum Workfront-Szenario-Planer finden Sie unter [Überblick über den Szenario-Planer](../../../scenario-planner/scenario-planner-overview.md).

* Die hier angezeigten Informationen werden auch im Ressourcenplaner auf Systemebene oder im Szenario-Planer angezeigt. 

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the "or" stays in&nbsp;NWE&nbsp;only)<br></p>
  -->

* Nach der Budgetierung Ihrer Ressourcen werden die budgetierten Arbeitskosten des Projekts im Bereich Ressourcenbudgetierung angezeigt, wenn die Rollen mit den Kosten pro Stunde verknüpft sind. Die budgetierten Arbeitskosten werden in der Währung des Projekts angezeigt.

  >[!IMPORTANT]
  >
  >Die budgetierten Arbeitskosten sind die Kosten, die mit den Rollen im Projekt und nicht mit den Benutzern verbunden sind. Die Summe aller budgetierten Arbeitskosten für die Benutzer kann oder nicht den budgetierten Arbeitskosten der mit den Nutzern verbundenen Stellenfunktion entsprechen. 

  Weitere Informationen zu den budgetierten Arbeitskosten finden Sie unter [Übersicht über die Finanzfelder für Geschäftsfälle](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

  Weitere Informationen zum Erstellen von Auftragsrollen und zum Zuordnen von Kosten pro Stunde-Raten zu diesen finden Sie unter [Erstellen und Verwalten von Auftragsrollen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## Risiken

Risiken sind Faktoren, die verhindern können, dass ein Projekt rechtzeitig oder zu einem Budget abgeschlossen wird. Die Definition dieser Faktoren ist wichtig, damit der Portfolio-Manager oder der Projektsponsor eine fundierte Entscheidung über die Projektgenehmigung treffen kann. Dieser Bereich ist standardmäßig im Geschäftsfall aktiviert, aber der Workfront-Administrator kann ihn möglicherweise nicht anzeigen lassen.

Sie können potenzielle Kosten mit den Risiken verknüpfen, die Sie für den Fall definieren, dass sie auftreten sollten. Die Kosten der Risiken eines Projekts beeinflussen den Nettowert des Projekts. 

Weitere Informationen zum Projekt-Nettowert finden Sie unter [Übersicht über die Finanzfelder für Geschäftsfälle](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Weitere Informationen zur Risikoerstellung finden Sie unter  [Erstellen und Bearbeiten von Risiken für Projekte](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

Ihr Workfront-Administrator kann benutzerdefinierte Risikotypen einrichten.

Weitere Informationen zum Erstellen und Bearbeiten benutzerdefinierter Risikotypen finden Sie unter [Bearbeiten und Erstellen von Risikotypen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

## Scorecard

Scorecards messen die Ausrichtung des Projekts. Dieser Bereich ist standardmäßig im Geschäftsfall aktiviert, aber der Workfront-Administrator kann ihn möglicherweise nicht anzeigen lassen.

Weitere Informationen zum Anwenden einer Scorecard auf ein Projekt und Generieren eines Ausrichtungswerts finden Sie unter [Anwenden einer Scorecard auf ein Projekt und Generieren einer Ausrichtungsbewertung](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Um eine Scorecard anzuwenden, muss Ihr Workfront-Administrator eine erstellen. Der Bereich **Scorecard** im Geschäftsfall wird nur angezeigt, wenn eine Scorecard erstellt wurde.

Weitere Informationen zum Erstellen einer Scorecard finden Sie unter  [Erstellen Sie eine Scorecard](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Benutzerdefinierte Formulare

Sie können bei der Definition eines Geschäftsszenarios benutzerdefinierte Forms an ein Projekt anhängen. Dieser Bereich ist im Geschäftsfall nicht standardmäßig aktiviert. Der Workfront-Administrator muss es aktivieren, damit es im Geschäftsfall angezeigt werden kann.

Weitere Informationen zum Aktivieren der Bereiche des Geschäftsfalls finden Sie unter [Systemweite Projektanvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Um ein benutzerdefiniertes Formular anzuwenden, muss Ihr Workfront-Administrator zunächst ein benutzerdefiniertes Formular erstellen.

Weitere Informationen zum Erstellen eines benutzerdefinierten Formulars finden Sie unter [Erstellen oder Bearbeiten eines benutzerdefinierten Formulars](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) .

Sie können benutzerdefinierte Formulare verwenden, um zusätzliche Informationen zu erfassen, die nicht in den anderen Feldern des Geschäftsfalls angezeigt werden.

Weitere Informationen zum Anwenden eines benutzerdefinierten Formulars finden Sie unter [Anhängen eines benutzerdefinierten Formulars an einen Geschäftsszenario](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md).

## Business Case-Zusammenfassung

* [Überblick über die Geschäftsfallzusammenfassung](#overview-of-the-business-case-summary)
* [Geschäftsfall exportieren](#export-the-business-case)

### Überblick über die Zusammenfassung der Geschäftsszenarios {#overview-of-the-business-case-summary}

Eine Zusammenfassung der wichtigsten Projektfinanzierungen sowie Informationen dazu, ob ein Projekt mit einer Scorecard in der Zusammenfassung der Geschäftsfälle in der oberen rechten Ecke des Geschäftsfalls ausgerichtet ist, finden Sie in der Zusammenfassung der Geschäftsfälle .

Sie können die Zusammenfassung der Geschäftsfälle nicht bearbeiten. Dies ist nur ein kurzer Überblick über den Stand des Projekts in Bezug auf die Finanzbereiche und die Scorecard. \
 

Die folgenden Felder werden in der Zusammenfassung der Geschäftsfälle angezeigt:

* Der Netzwert des Projekts
* Die im Projekt veranschlagten Kosten
* Die potenziellen Risikokosten
* Der geplante Vorteil
* Die Punktzahl der Ausrichtung

Weitere Informationen zu diesen Feldern finden Sie unter [Übersicht über die Finanzfelder für Geschäftsfälle](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

### Geschäftsfall exportieren {#export-the-business-case}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: made this into a standalone article, linked in the first paragraph of this section)</p>
-->

Sie können den Geschäftsfall in eine PDF-Datei exportieren, falls Sie ihn drucken oder an eine E-Mail anhängen müssen. 

Weitere Informationen finden Sie unter [Geschäftsszenario eines Projekts exportieren](../../../manage-work/projects/define-a-business-case/export-business-case.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>To export a Business Case:</p>
<ol>
<li value="1">Go to the <strong>Business Case</strong> area of a project. </li>
<li value="2"> <p>In the<strong>Business Case Summary</strong> area, click <strong>Export</strong>.<br>A PDF file is downloaded to your computer. The file contains all areas of the Business Case in an easy to read format.</p> <p> <img src="assets/bc-summary-exported-350x160.png" alt="BC_Summary_exported.png" style="width: 350;height: 160;"> </p> </li>
<li value="3">(Optional) You can attach the PDF file to an email, or print it.&nbsp;</li>
</ol>
</div>
-->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>You can export the Business Case to a PDF file, in case you need to print it or attach it to an email in a more condensed format.&nbsp; The file contains all areas of the Business Case in an easy to read format.</p>
<p>For information about how to export the Business Case, see <a href="../../../manage-work/projects/define-a-business-case/export-business-case.md" class="MCXref xref">Export the Business Case of a project </a></p> <!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted and will replace the info above, when the standalone arrticle is live >> Becky!)</p>
-->
</div>
--&gt;
