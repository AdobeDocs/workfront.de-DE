---
navigation-topic: business-case-and-scorecards
title: Anwenden einer Scorecard auf ein Projekt und Generieren einer Alignment-Bewertung
description: Mit einer Scorecard können Sie messen, wie gut ein Projekt mit den zuvor festgelegten Kriterien eines Portfolios übereinstimmt. Eine Scorecard spiegelt häufig die Mission, Werte und strategischen Ziele einer Organisation wider.
author: Alina
feature: Work Management
exl-id: 21cf5493-147d-4b8d-8b16-2891eb7e0491
source-git-commit: 78878fa3578e4f3a33baec3806298282d3909d8d
workflow-type: tm+mt
source-wordcount: '1292'
ht-degree: 0%

---

# Anwenden einer Scorecard auf ein Projekt und Generieren einer Alignment-Bewertung

Mit einer Scorecard können Sie messen, wie gut ein Projekt mit den zuvor festgelegten Kriterien eines Portfolios übereinstimmt. Eine Scorecard spiegelt häufig die Mission, Werte und strategischen Ziele einer Organisation wider.

Weitere Informationen zu Scorecards und dazu, wie Sie eine erstellen können, finden Sie unter [Scorecard erstellen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Unternehmen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p>Zugriff auf Portfolio anzeigen oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für ein Projekt verwalten</p> <p>Anzeigen von oder höheren Berechtigungen für ein Portfolio </p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Projekt-Scorecards {#project-scorecards}

* [Scorecards - Übersicht](#scorecards-overview)
* [Projekt-Scorecards](#project-scorecards)

### Scorecards - Übersicht {#scorecards-overview}

In der Regel füllt ein Projektmanager die Scorecard-Informationen aus, um einen Ausrichtungswert zwischen 0 und 100 für das Projekt zu erzielen. Der erzeugte Wert wird später verwendet, wenn der Portfoliomanager die Projekte im Portfoliooptimierer überprüft, um sie zu vergleichen.

Weitere Informationen zur Portfoliooptimierung finden Sie im Artikel [Übersicht über Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

### Anwenden einer Scorecard auf ein Projekt

Als Benutzer mit einer Planungslizenz und Verwaltungsberechtigungen für ein Projekt können Sie eine Scorecard an das Projekt anhängen.

Weitere Informationen zu Projektberechtigungen finden Sie unter [Freigeben eines Projekts in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

Sie können einem Projekt beim Erstellen des Geschäftsszenarios für das Projekt Scorecards hinzufügen.

Weitere Informationen zum Erstellen eines Geschäftsfalls finden Sie unter [Geschäftsszenario für ein Projekt erstellen](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Ihr Adobe Workfront-Administrator oder Gruppenadministrator muss den Scorecard-Abschnitt im Geschäftsfallbereich Ihrer Projekte aktivieren, bevor Sie über den Geschäftsfall auf Scorecards zugreifen können. Informationen zum Einrichten von Projekteinstellungen und Aktivieren von Bereichen des Geschäftsfalls finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

So wenden Sie eine Scorecard auf ein Projekt an:

1. Gehen Sie zu einem Projekt, auf das Sie eine Scorecard anwenden möchten.
1. Klicken **Geschäftsfall** im linken Bereich.
1. Suchen Sie die **Scorecard** Abschnitt des Geschäftsfalls.\
   Sie müssen eine Scorecard vor der **Scorecard** im Geschäftsfall angezeigt.

   Informationen zum Erstellen einer Scorecard finden Sie unter [Scorecard erstellen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

1. Wählen Sie eine Scorecard aus dem Dropdown-Menü aus.

   ![new_scorecard.png](assets/new-scorecard-350x149.png)

1. Geben Sie eine Antwort für alle Fragen in der Scorecard an.

   Workfront wendet für jede Frage eine Punktzahl an und berechnet anhand des individuellen Punktes jeder Frage einen Gesamtergebnis.

   Weitere Informationen zum Generieren des Gesamtausrichtungswerts des Projekts finden Sie unter [Generieren einer Alignment-Bewertung für ein Projekt](#generate-an-alignment-score-for-a-project).

1. Klicken **Speichern** , um die Scorecard zu speichern und das Projekt zu bewerten.

   Die Scorecard ist jetzt mit dem Projekt verknüpft und das Projekt wird bewertet.

<!--This functionality was removed when we redesigned bulk editing projects with 23.2: 

1. (Conditional) When changes occur in the values of scorecard questions, you must recalculate the scorecard to reflect the new values for the project score. To recaulate the scorecard, do the following: 

   1. Go to a list of projects and select all projects in the list. 
   1. Click the **Edit** icon at the top of the list. 
   1. Click **Settings** in the left panel, then check the **Recalculate Scorecards** option at the end of the Settings area. 
   1. Click Save. This recalculates the score value based on the scorecards attached for all the selected projects.  

      >[!NOTE]
      >
      >   The option to recalculate scorecards has been removed from the Preview environment, when editing projects in bulk. 

-->

## Generieren einer Alignment-Punktzahl

* [Generieren einer Alignment-Bewertung für ein Projekt](#generate-an-alignment-score-for-a-project)
* [Generieren einer Alignment-Bewertung für ein Portfolio](#generate-an-alignment-score-for-a-portfolio)

### Generieren einer Alignment-Bewertung für ein Projekt {#generate-an-alignment-score-for-a-project}

Der Ausrichtungswert ist der Wert, der nach Abschluss der Scorecard erzeugt wird.

Scorecards enthalten Fragen mit Antwortmöglichkeiten, denen numerische Werte zugewiesen wurden, so genannte Ausrichtungspunkte. Anhand dieser Punkte wird bestimmt, wie gut das Projekt an Ihrer Organisation ausgerichtet ist. Die Ausrichtungspunkte für jede Frage enthalten eine Zahl zwischen 0 und 100.

Wenn die Scorecard abgeschlossen ist, berechnet Workfront den Ausrichtungswert des Projekts in Prozent mithilfe der folgenden Formel:

```
Project Alignment Score = The sum of the question points from the scorecard met at a given time/ The sum of the possible points on the scorecard
```

Weitere Informationen finden Sie unter [Scorecard erstellen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

### Generieren einer Alignment-Bewertung für ein Portfolio {#generate-an-alignment-score-for-a-portfolio}

Der Alignment-Wert des Portfolios entspricht dem Durchschnittswert der Alignment-Bewertungen aller Projekte im Portfolio.

Wenn die Scorecards der Projekte abgeschlossen sind, verwendet Workfront diese Werte, um den Alignment-Wert des Portfolios in Prozent zu berechnen, indem es folgende Formel verwendet:

Portfolio Alignment Score = Die Summe der Prozentsätze der Projektausrichtungsbewertungen/ Anzahl der  im Portfolio

>[!NOTE]
>
>Wenn einem Projekt keine Scorecard zugeordnet ist und es daher keine Alignment-Bewertung hat, wird davon ausgegangen, dass es eine 0%ige Ausrichtung im Portfolio hat. Das Projekt wird bei der Anzahl der Projekte im Portfolio berücksichtigt.

## Alignment-Punktzahl anzeigen

Sie können den Ausrichtungswert eines Portfolios auf Projektebene oder im Projektoptimierer anzeigen.

* [Anzeigen der Alignment-Bewertung in einem Projekt](#View%20the)
* [Anzeigen der Alignment-Werte des Projekts und des Portfolios im Portfolio Optimizer](#View%20the2)

### Anzeigen der Alignment-Bewertung in einem Projekt

Wenn Sie über Beitragsrechte für das Projekt verfügen, können Sie den Ausrichtungswert eines Projekts auf Projektebene anzeigen.

1. Wechseln Sie zu dem Projekt, dessen Alignment-Bewertung Sie anzeigen möchten.
1. Klicken **Geschäftsfall** im linken Bereich.
1. Navigieren Sie zu **Zusammenfassung von Geschäftsfällen** auf der rechten Bildschirmseite angezeigt.

   Die Alignment-Bewertung befindet sich in der Zusammenfassung der Geschäftsfälle im **Alignment** -Wert.

   ![align_score_on_a_project.png](assets/alignment-score-on-a-project.png)

### Anzeigen der Alignment-Werte des Projekts und des Portfolios im Portfolio Optimizer

Sie können die Alignment-Bewertung eines Portfolios oder Portfolios im Portfolio-Optimizer anzeigen, wenn Sie Zugriff auf das Portfolio verwalten haben.

Weitere Informationen zu den im Portfolio Optimizer angezeigten Informationen finden Sie unter [Übersicht über Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md).

* [Suchen Sie die Alignment-Bewertung des Portfolios im Projektoptimierer.](#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer)
* [Suchen Sie die Alignment-Bewertung des Portfolios im Portfolio Optimizer](#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer)

   ![](assets/alignment-score-in-portfolio-optimizer-nwe-350x97.png)

#### Suchen Sie die Alignment-Bewertung des Portfolios im Projektoptimierer. {#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer}

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png), dann **Portfolios**.

1. Klicken Sie auf den Namen eines Portfolios.
1. Klicken **Portfolio-Optimierung** im linken Bereich.

   Der Portfolio Optimizer wird angezeigt.

1. Der Ausrichtungswert eines Projekts wird als Prozentsatz im **Ausrichtung** -Spalte des Portfolio Optimizer.

   Dies ist der Ausrichtungswert des Projekts basierend auf der mit dem Projekt verknüpften Scorecard.

#### Suchen Sie die Alignment-Bewertung des Portfolios im Portfolio Optimizer  {#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer}

1. Navigieren Sie zu **Projekte** in der Symbolleiste für globale Navigation.
1. Wählen Sie die **Portfolios** Registerkarte.
1. Klicken Sie auf den Namen eines Portfolios.
1. Wählen Sie die **Portfolio-Optimierung** Registerkarte.
1. Suchen Sie oben im Portfolio Optimizer die **Alignment** sowie der **Ausrichtung** Messung, die den Ausrichtungswert des Portfolios angibt.

   Dies ist der Alignment-Wert des Portfolios.

   Weitere Informationen dazu, wie die Alignment-Bewertung eines Portfolios generiert wird, finden Sie unter [Generieren einer Alignment-Bewertung für ein Portfolio](#generate-an-alignment-score-for-a-portfolio).

## Übersicht über die Portfolio Optimizer-Bewertung

Es gibt einen Unterschied zwischen dem Alignment-Wert und dem Portfolio-Optimierer-Wert eines Projekts.

Der Ausrichtungswert eines Projekts wird anhand der Punkte berechnet, die nach Abschluss der Scorecard ermittelt wurden. Dieser Punktstand wird dann zur Bestimmung des Portfolioausrichtungswerts verwendet. Der Ausrichtungswert wird als Prozentsatz angezeigt.

Der Ausrichtungswert eines Projekts wird im **Ausrichtung** -Spalte des Portfolio Optimizer.

Das Portfolio-Optimierer-Ergebnis ist ein im Portfolio Optimizer automatisch berechnetes Ranking, anhand dessen Projekte priorisiert werden können. Das Portfolio-Optimierungsergebnis wird als Indikatorsymbol mit einer Zahl angezeigt und im **Ergebnis** -Spalte des Portfolio Optimizer. Ein Portfolio-Optimizer-Ergebnis wird nur generiert, wenn alle Abschnitte des Geschäftsszenarios abgeschlossen sind, mit Ausnahme von &quot;Ziele&quot;.

Weitere Informationen zum Erstellen eines Geschäftsszenarios für ein Projekt finden Sie unter [Geschäftsszenario für ein Projekt erstellen](../../../manage-work/projects/define-a-business-case/create-business-case.md).

Weitere Informationen zur Berechnung des Portfolio-Optimierungswerts eines Projekts finden Sie unter [Übersicht über die Portfolio Optimizer-Bewertung](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).
