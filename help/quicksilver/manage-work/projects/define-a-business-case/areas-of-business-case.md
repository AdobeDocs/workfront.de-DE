---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Überblick über die Bereiche des Business Case
description: In diesem Artikel werden die Bereiche des Business Case eines Projekts beschrieben.
author: Alina
feature: Work Management
exl-id: 0646e4f0-e8fb-48f2-b533-358229543081
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1603'
ht-degree: 2%

---

# Überblick über die Bereiche des Business Case

In diesem Artikel werden die Bereiche des Business Case eines Projekts beschrieben.

Informationen zum Erstellen eines Business Case für ein Projekt finden Sie unter [Erstellen eines Business Case für ein Projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Ihr Adobe Workfront-Administrator oder Gruppenadministrator muss alle Abschnitte des Business Case aktivieren, bevor sie im Projekt sichtbar sind, mit Ausnahme des Abschnitts Projektinformationen . Der Abschnitt Projektinformationen ist standardmäßig aktiviert.

Weitere Informationen zur Aktivierung von Bereichen des Business-Case finden Sie im Abschnitt „Business-Cases“ in  [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Im Business Case eines Projekts werden die folgenden Bereiche beschrieben:

* Projektinfo
* Ziele
* Ausgaben
* Ressourcenbudgetierung
* Risiken
* Scorecard
* Benutzerdefinierte Formulare
* Business Case-Zusammenfassung

## Projektinfo

Der **Projektinfo** des Business Case kann vom Workfront-Administrator nicht konfiguriert werden. Alle Projekte verfügen im Business Case über einen Bereich mit Projektinformationen . 

Der Abschnitt Projektinformationen des Business Case enthält die grundlegenden Informationen zu einem Projekt, bevor das Projekt tatsächlich gestartet wurde.

Erwägen Sie, die folgenden Felder zu bearbeiten:

* **Beschreibung**: Geben Sie eine Beschreibung für Ihr Projekt an.
* **Projektbesitzer**

  Standardmäßig ist der Benutzer, der das Projekt erstellt, auch der Projektbesitzer. Sie können dieses Feld bearbeiten und einen anderen aktiven Benutzer als Eigentümer des Projekts angeben.

* **Projektsponsor**

  Erwägen Sie, eine andere Person als den Projektbesitzer als Sponsor des Projekts hinzuzufügen. Der Sponsor erhält die Genehmigung des Business Case. 

* **Portfolio**: Geben Sie ein Portfolio für das Projekt an. Sie müssen das Portfolio erstellen und den Status **Aktiv** annehmen, bevor es in diesem Dropdown-Menü ausgewählt werden kann.

  Weitere Informationen zu Portfolios finden Sie unter Übersicht über das [Portfolio in Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

  Weitere Informationen zum Erstellen von Portfolios finden Sie unter [Erstellen eines Portfolios](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

* **Geplanter Gewinn**: Schätzen Sie, wie hoch der finanzielle Gewinn für Ihr Unternehmen nach Abschluss dieses Projekts sein soll. Es kann eine beliebige Währung sein, und es muss ein positiver Wert sein. Beispiel: 10.000 $.
* **Status**: Standardmäßig ist der Status für eine Projektanfrage auf &quot;**&quot;**.

  Wenn Sie den Status in etwas Anderes als „Idee“ oder „Planung“ ändern **wird die Schaltfläche „Senden** im Bereich „Zusammenfassung des Business-Case“ ausgeblendet, und Sie können den Business-Case nicht mehr zur Genehmigung senden. 

* **Festes Startdatum**: Geben Sie ein Datum an, an dem das Projekt beginnen soll.
* **Festes Enddatum**: Geben Sie ein Datum an, an dem das Projekt enden soll.

  >[!NOTE]
  >
  >Die festen Start- und Enddaten im Business Case wirken sich nicht auf die geplanten Start- und Abschlussdaten des Projekts aus. Diese stellen die vom Projektersteller angeforderten Daten dar, zu denen das Projekt idealerweise entwickelt werden sollte. Stattdessen werden der geplante Start und das geplante Abschlussdatum des Projekts als geplante Zeitleiste für das Projekt angezeigt, die auf den Aufgaben im Projekt basiert.

## Ziele

Ziele definieren die Ziele für das Projekt. Dieser Bereich ist im Business-Case standardmäßig aktiviert, der Workfront-Administrator kann jedoch festlegen, dass er nicht angezeigt wird. Dieses Feld zeigt die Ziele in der Reihenfolge ihrer Priorität an.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
>
>Sie können strategische Ziele für Ihr Unternehmen erstellen, die nicht mit dem individuellen Business Case eines Projekts verbunden sind. Sie müssen Zugriff auf Adobe Workfront-Ziele haben, um strategische Ziele erstellen zu können. Sie können sie dann mit Projekten außerhalb ihrer Business Cases verbinden. Informationen zum Erstellen von Zielen mithilfe von Workfront-Zielen finden Sie unter [Adobe Workfront-Ziele - Übersicht](../../../workfront-goals/goal-management/wf-goals-overview.md).

Die Definition der Ziele ist optional, damit das Projekt ein Score in Portfolio Optimizer erhalten kann. Dieser Abschnitt ist der einzige optionale Abschnitt im Business Case. Alle anderen Abschnitte des Business Case müssen abgeschlossen sein, bevor das Projekt in Portfolio Optimizer bewertet wird. Sie können bei der Erstellung des Ziels eine Prioritätsstufe für ein Ziel angeben.

Weitere Informationen zu Zielen finden Sie unter  [Erstellen von Business Case-Zielen](../../../manage-work/projects/define-a-business-case/create-business-case-goals.md).

## Ausgaben

Aufwendungen stellen die sonstigen Kosten dar, die während der Laufzeit eines Projekts anfallen können. Dieser Bereich ist im Business-Case standardmäßig aktiviert, der Workfront-Administrator kann jedoch festlegen, dass er nicht angezeigt wird. 

Alle Ausgaben, die Sie im Business-Case eingeben, werden auch auf der Registerkarte „Ausgaben“ des Projekts als geplante Ausgaben eingegeben.

Kosten wirken sich auf die folgenden Felder des Projekts aus:

* Budgetierte Kosten
* Nettowert

Weitere Informationen zu den budgetierten Kosten und Nettowerten finden Sie unter [Übersicht über die Finanzfelder des Business Case](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Weitere Informationen zu Ausgaben unter  [Projektausgaben verwalten](../../../manage-work/projects/project-finances/manage-project-expenses.md) .

Ihr Workfront-Administrator kann benutzerdefinierte Ausgabentypen einrichten.

Weitere Informationen zum Erstellen benutzerdefinierter Ausgabentypen finden Sie unter [Erstellen benutzerdefinierter Ausgabentypen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-custom-expense-types.md). 

## Ressourcenbudgetierung

Im Bereich Ressourcenbudgetierung des Business-Case können Sie die folgenden Aktionen ausführen:

* Verknüpfen Sie Ressourcenpools mit dem Projekt.
* Budgetieren Sie Ihre Ressourcen auf Projektebene.

Die budgetierten Stunden für die Ressourcen im Projekt werden im Bereich Ressourcenbudgetierung des Business Case angezeigt und erzeugen die budgetierten Lohnkosten des Projekts. Dieser Bereich des Business Case ist standardmäßig aktiviert.

Weitere Informationen zur Budgetierung von Ressourcen für das Projekt im Business Case finden Sie [Budgetressourcen im Business Case](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

![](assets/business-case-sp-selected-with-choose-button-350x121.png)

Beachten Sie beim Anzeigen des Abschnitts „Ressourcenbudgetierung“ des Business Case Folgendes:

* Hier können Sie Ressourceninformationen mit den folgenden Tools budgetieren:

   * Der Ressourcenplaner

     Weitere Informationen finden Sie [Budgetressourcen im Business Case mit dem Ressourcenplaner](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-resource-planner.md).

   * Der Szenario-Planer , wenn Ihr Unternehmen eine zusätzliche Lizenz für das Adobe des Szenario-Planers erworben hat

     Weitere Informationen finden Sie unter [Budgetressourcen im Business Case mit dem Szenario-Planer](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

     Der Szenario-Planer ist nur in der neuen Adobe Workfront-Version verfügbar und erfordert eine zusätzliche Lizenz. Weitere Informationen zum Workfront-Szenarioplaner finden Sie unter [Szenarioplaner - Übersicht](../../../scenario-planner/scenario-planner-overview.md).

* Die hier angezeigten Informationen werden auch im Ressourcenplaner auf Systemebene oder im Szenario-Planer angezeigt. 

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the "or" stays in&nbsp;NWE&nbsp;only)<br></p>
  -->

* Nachdem Sie Ihre Ressourcen budgetiert haben, werden die budgetierten Lohnkosten des Projekts im Bereich Ressourcenbudgetierung angezeigt, wenn die Funktionen mit den Sätzen Kosten pro Stunde verknüpft sind. Die budgetierten Lohnkosten werden in der Währung des Projekts angezeigt.

  >[!IMPORTANT]
  >
  >Die budgetierten Lohnkosten entsprechen den Kosten, die den Funktionen des Projekts und nicht den Benutzern zugeordnet sind. Die Summe aller budgetierten Lohnkosten für die Benutzer kann den budgetierten Lohnkosten des Aufgabengebiets, das den Benutzern zugeordnet ist, entsprechen oder nicht. 

  Weitere Informationen zu budgetierten Lohnkosten finden Sie unter [Übersicht über die Finanzfelder des Business Case](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

  Weitere Informationen zum Erstellen von Aufgabengebieten und zum Verknüpfen der Stundensätze mit ihnen finden Sie unter [Erstellen und Verwalten von Aufgabengebieten](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

## Risiken

Risiken sind Faktoren, die verhindern können, dass ein Projekt termingerecht oder im Rahmen des Budgets abgeschlossen wird. Die Definition dieser Faktoren ist wichtig, damit der Portfolio-Manager oder Projektsponsor eine fundierte Entscheidung über die Genehmigung des Projekts treffen kann. Dieser Bereich ist im Business-Case standardmäßig aktiviert, der Workfront-Administrator kann jedoch festlegen, dass er nicht angezeigt wird.

Sie können den Risiken, die Sie für den Fall definieren, dass sie eintreten, potenzielle Kosten zuordnen. Die Kosten der Risiken eines Projekts beeinflussen den Nettowert des Projekts. 

Weitere Informationen zum Nettowert des Projekts finden Sie unter [Übersicht über Business Case-Finanzfelder](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

Weitere Informationen zum Erstellen von Risiken finden Sie unter  [Risiken in Projekten erstellen und bearbeiten](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).

Ihr Workfront-Administrator kann benutzerdefinierte Risikotypen einrichten.

Weitere Informationen zum Erstellen und Bearbeiten benutzerdefinierter Risikotypen finden Sie unter [Risikotypen bearbeiten und erstellen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

## Scorecard

Scorecards messen die Ausrichtung des Projekts. Dieser Bereich ist im Business-Case standardmäßig aktiviert, der Workfront-Administrator kann jedoch festlegen, dass er nicht angezeigt wird.

Weitere Informationen zum Anwenden einer Scorecard auf ein Projekt und zum Generieren eines Ausrichtungswerts finden Sie unter [Anwenden einer Scorecard auf ein Projekt und Generieren eines Ausrichtungswerts](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Um eine Scorecard anzuwenden, muss Ihr Workfront-Administrator eine erstellen. Der **Scorecard** des Business Case wird nur angezeigt, wenn eine Scorecard erstellt wird.

Weitere Informationen zum Erstellen einer Scorecard finden Sie unter  [Erstellen einer Scorecard](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Benutzerdefinierte Formulare

Sie können beim Definieren eines Business Case eine benutzerdefinierte Forms an ein Projekt anhängen. Dieser Bereich ist im Business Case nicht standardmäßig aktiviert. Der Workfront-Administrator muss sie aktivieren, um sie im Business Case anzuzeigen.

Weitere Informationen zur Aktivierung verschiedener Bereiche des Business Case finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Um ein benutzerdefiniertes Formular anzuwenden, muss Ihr Workfront-Administrator zunächst ein benutzerdefiniertes Formular erstellen.

Weitere Informationen zum Erstellen eines benutzerdefinierten Formulars finden Sie unter [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Sie können benutzerdefinierte Formulare verwenden, um zusätzliche Informationen zu erfassen, die nicht in den anderen Feldern des Business Case angezeigt werden.

Weitere Informationen zum Anwenden eines benutzerdefinierten Formulars finden Sie unter [Anhängen eines benutzerdefinierten Formulars an einen Business-Case](../../../manage-work/projects/define-a-business-case/attach-custom-form-to-business-case.md).

## Business Case-Zusammenfassung

* [Überblick über die Business Case-Zusammenfassung](#overview-of-the-business-case-summary)
* [Business Case exportieren](#export-the-business-case)

### Überblick über die Zusammenfassung eines Business-Case {#overview-of-the-business-case-summary}

Eine Zusammenfassung der wichtigsten Projektfinanzen und dazu, ob ein Projekt mit einer Scorecard abgestimmt ist oder nicht, finden Sie im Bedienfeld Zusammenfassung eines Business-Case in der oberen rechten Ecke des Business-Case .

Sie können die Zusammenfassung eines Business-Case nicht bearbeiten. Dies ist nur ein kurzer Überblick über den Status des Projekts in Bezug auf Finanzfelder und die Scorecard. \
 

Die folgenden Felder werden in der Zusammenfassung eines Business-Case angezeigt:

* Der Nettowert des Projekts
* Die budgetierten Projektkosten
* Die potenziellen Risikokosten
* Der geplante Nutzen
* Ausrichtungsbewertung

Weitere Informationen zu diesen Feldern finden Sie unter [Übersicht über Business Case-Finanzfelder](../../../manage-work/projects/define-a-business-case/business-case-finances.md).

### Business Case exportieren {#export-the-business-case}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: made this into a standalone article, linked in the first paragraph of this section)</p>
-->

Sie können den Business Case in eine PDF-Datei exportieren, falls Sie ihn drucken müssen oder in einem kürzeren Format an eine E-Mail anhängen. 

Weitere Informationen finden [ unter „Business Case eines Projekts exportieren](../../../manage-work/projects/define-a-business-case/export-business-case.md).

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
