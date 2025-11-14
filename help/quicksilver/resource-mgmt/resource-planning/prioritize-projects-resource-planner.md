---
product-area: resource-management;projects
navigation-topic: resource-planning
title: Priorisieren von Projekten im Ressourcenplaner
description: Projekte werden im Ressourcenplaner nach Priorität geordnet aufgelistet, wobei das wichtigste Projekt ganz oben steht.
author: Lisa
feature: Resource Management
exl-id: fe9c8cf9-f1e0-4cd5-9299-0f04893d71a5
source-git-commit: 8cd6c47acf8de313bab5fe7298125eb63cc10faf
workflow-type: tm+mt
source-wordcount: '1282'
ht-degree: 2%

---

# Priorisieren von Projekten im Ressourcenplaner

Projekte werden im Ressourcenplaner nach Priorität geordnet aufgelistet, wobei das wichtigste Projekt ganz oben steht.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td>
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf das Ressourcenmanagement bearbeiten, der den Zugriff auf die Bearbeitung von Prioritäten und Budgetstunden im Ressourcenplaner beinhaltet</p> <p>Zugriff auf Finanzdaten, Projekte und Benutzer bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td>Objektberechtigungen</td> 
   <td> <p>Verwalten Sie Berechtigungen für die Projekte, für die Sie Informationen budgetieren möchten, mit der Möglichkeit, Finanzen zu verwalten.</p></td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Standardreihenfolge der Projekte im Ressourcenplaner

Standardmäßig werden die Projekte in der Projektansicht des Ressourcenplaners unter Berücksichtigung der folgenden Kriterien aufgelistet.

>[!IMPORTANT]
>
>Projekte werden nur beim ersten Öffnen des Ressourcenplaners nach den drei unten stehenden Kriterien aufgelistet. Diese Standardpriorität wird jedoch automatisch zu Ihrer benutzerdefinierten Priorität und kann nicht bei jeder der folgenden Aktionen auf die ursprüngliche Priorität zurückgesetzt werden:
>
>* Wenn Sie jederzeit auf Speichern klicken.
>* Wenn Sie die Projektplanungspriorität manuell ändern. Informationen zum manuellen Ändern der Projektplanungspriorität finden Sie im Abschnitt [Manuelles Ändern der Projektplanungspriorität](#manually-change-the-project-planning-priority) in diesem Artikel.
>
>Nachdem die Projektpriorität zu Ihrer benutzerdefinierten Priorität geworden ist, wirken sich Änderungen an den Projektinformationen nicht mehr auf die Reihenfolge der Projekte mit diesen Kriterien aus. Danach können Sie Projekte nur noch manuell priorisieren.

Die ursprünglichen Standardkriterien für die Auflistung der Projekte in der Projektansicht sind wie folgt:

1. Nach dem Alignment-Score des Projekts\
   Weitere Informationen zum Ausrichtungswert des Projekts finden Sie unter [Anwenden einer Scorecard auf ein Projekt und Generieren eines Ausrichtungswerts](../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md) .

1. Nach dem geplanten Startdatum des Projekts (wenn das Ausrichtungsfeld null oder für mehrere Projekte identisch ist).
1. Alphabetisch (wenn das Ausrichtungsfeld null oder identisch ist und das geplante Startdatum für mehrere Projekte identisch ist).

Beachten Sie bei der Arbeit mit Projektprioritäten im Ressourcenplaner Folgendes:

* Sie können die Projektpriorität nur manuell anpassen, wenn Sie die Projektansicht anwenden. Dadurch wird auch die Reihenfolge der Projekte im Ressourcenplaner geändert.
* Wenn Sie die Rollen- oder Benutzeransichten im Ressourcenplaner anwenden, werden die Projekte in der gleichen Prioritätsreihenfolge angezeigt, die in der Projektansicht festgelegt wurde.
* Die Reihenfolge der Projekte im Ressourcenplaner ist für Sie eindeutig. Andere Benutzer können dieselben Projekte im Ressourcenplaner anzeigen, jedoch in einer anderen Reihenfolge. Sie können keine Berichte über das Feld Projektplanungspriorität erstellen. Dies ist nur im Ressourcenplaner sichtbar und dient als Markierung für die Priorisierung Ihrer Projekte.

Projekte, die mit einem Portfolio verknüpft sind, können eine Priorität auf Portfolioebene haben. Zusätzlich zur Ressourcenplanerpriorität können Sie die Anzeige der Portfoliopriorität eines Projekts im Ressourcenplaner aktivieren. Sie können die Projekte auch nach ihrer Portfoliopriorität sortieren.

## Manuelles Ändern der Projektplanungspriorität {#manually-change-the-project-planning-priority}

Sie müssen Bearbeitungszugriff auf das Ressourcen-Management und Verwaltungsberechtigungen für Projekte haben, um Projekte im Ressourcenplaner neu anordnen zu können.

Wenn Sie Projekten eine neue Priorität einräumen, können Sie sie nach ihrer Wichtigkeit ordnen.

So bearbeiten Sie die Projektplanungspriorität:

1. Navigieren Sie zum **Ressourcenplaner**.

1. Klicken Sie in das Feld links neben dem Projektnamen, der eine Zahl enthält, und geben Sie eine Zahl ein, um die Planungspriorität zu ändern. Drücken Sie dann die Eingabetaste.\
   ![Planungspriorität ändern](assets/mceclip4.png)\
   Oder\
   Bewegen Sie den Mauszeiger über den Projektnamen, klicken Sie auf die Anzeige links neben dem Projektnamen, ziehen Sie sie und legen Sie sie an der richtigen Stelle ab, um die Priorität zu ändern.

   ![drag_and_drop_projects_RP__1_.png](assets/drag-and-drop-projects-rp--1--350x184.png)

   Bei der Auswahl von Zahlen für die Priorisierung von Projekten sollten Sie niedrigere Zahlen für höhere (wichtigere) Prioritäten und höhere Zahlen für niedrigere (weniger wichtige) Prioritäten auswählen. Wenn Sie die Prioritätsnummer eines Projekts in eine niedrigere Zahl (höhere Priorität) ändern, werden alle anderen Projekte im Ressourcenplaner auf der Liste nach unten verschoben (sie werden weniger wichtig).\
   Wenn Sie die Prioritätsnummer eines Projekts in eine höhere Zahl (niedrigere Priorität) ändern, werden alle anderen Projekte im Ressourcenplaner in der Liste nach oben verschoben (wichtiger).

1. Klicken Sie auf **Speichern**.\
   Die Reihenfolge der Projekte ändert sich entsprechend Ihren Auswahlen. Dies wird zu Ihrer benutzerdefinierten Projektpriorität im Ressourcenplaner. Andere Benutzer können die Prioritätsreihenfolge für die Projekte im Ressourcenplaner nicht sehen, obwohl sie möglicherweise dieselben Projekte in ihren Ressourcenplanern anzeigen können.

## Bestellen von Projekten nach ihrer Portfolio-Priorität im Ressourcenplaner

>[!IMPORTANT]
>
>Ihr Unternehmen muss über ein Prime- oder ein höheres Workfront-Paket verfügen, um Projekte im Portfolio Optimizer zu priorisieren.
>
>Weitere Informationen zu den Workfront-Paketen finden Sie unter [Adobe Workfront-Pakete und Preise](https://business.adobe.com/de/products/workfront/pricing.html).
>
>Informationen zum Priorisieren von Projekten in Portfolio Optimizer finden Sie unter [Priorisieren von Projekten in Portfolio Optimizer](../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md).

1. Öffnen Sie **Ressourcenplaner** in der **Projektansicht**.
1. Klicken Sie auf **Symbol** Einstellungen“.
1. Aktivieren Sie **Einstellung &quot;Portfolio-** anzeigen“, um die Projektprioritäten entsprechend der Portfolio anzuzeigen, der sie zugewiesen sind. Die Priorität der Projekte entsprechend ihren Portfolios wird neben der Ressourcenplaner-Priorität angezeigt. Diese Einstellung ist standardmäßig deaktiviert.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: check screen shot to see if this is accurate still - should say Order, and not Sort:)</p>
   -->

   ![Portfolio-Priorität](assets/rp-portfolio-priority-unordered-edit-350x180.png)

   Die Portfolioprioritäten der Projekte werden nur in der Projektansicht des Ressourcenplaners angezeigt.

1. Klicken Sie **Reihenfolge**, um die Projekte entsprechend den Portfolioprioritäten zu sortieren.

   Wenn Sie Projekte haben, die zu mehr als einem Portfolio gehören, können Sie im Ressourcenplaner mehrere Projekte mit derselben Portfoliopriorität sehen. In diesem Fall werden die Projekte mit derselben Portfoliopriorität nach folgenden Kriterien in der folgenden Reihenfolge aufgelistet:

   1. Ausrichtungsbewertung
   1. Geplantes Startdatum
   1. Projektname

   ![Portfolio-Priorität sortiert](assets/rp-portfolio-priority-ordered-350x198.png)

1. Klicken Sie auf **Speichern**.

## Auswirkungen der Änderung der Projektplanungspriorität auf die verfügbaren Stunden des Benutzers

Die Projektplanungspriorität wirkt sich auf die verfügbaren Stunden von Benutzern aus. Die Benutzerinnen und Benutzer, die mit dem Projekt mit der höchsten Priorität verknüpft sind, zeigen entsprechend ihren Zeitplänen ihre volle Verfügbarkeit für die Spalte Verfügbare Stunden (AVL) für dieses Projekt an.

Dieselben Benutzer, die dem zweiten Projekt in der Reihenfolge ihrer Priorität zugeordnet sind, zeigen den Wert Verfügbare Stunden an, der die Differenz zwischen ihrem vollen Betrag der Verfügbaren Stunden und dem darstellt, was bereits für das erste Projekt in der Spalte Budgetierte Stunden budgetiert wurde, usw. Weitere Informationen zur Budgetierung von Ressourcen im Ressourcenplaner finden Sie unter [Budgetressourcen im Ressourcenplaner mithilfe der Projekt- und Aufgabenansichten](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

Wenn für das erste Projekt (in der Reihenfolge der Priorität) keine Stunden für einen Benutzer budgetiert wurden, für das zweite Projekt jedoch für denselben Benutzer budgetiert wurden, zeigt der Benutzer die volle Anzahl der verfügbaren Stunden für beide Projekte an.

Es wird empfohlen, die Spalte Budgetierte Stunden für die Benutzer in der Reihenfolge der Projekte im Ressourcenplaner zu aktualisieren, um sicherzustellen, dass Sie die verfügbaren Stunden für die Benutzer jederzeit genau sehen können.

>[!NOTE]
>
>Da die Projektplanungspriorität für jeden Ressourcen-Manager eindeutig ist, kann Ihr Projekt zweiter Priorität ein Projekt erster Priorität für eine andere Person sein, die dieselben Projekte in ihrem Ressourcenplaner anzeigt. Wenn ein anderer Ressourcenmanager eine Ressource für sein erstes Projekt budgetiert, verringern sich die verfügbaren Stunden für diese Ressource für Ihr erstes Projekt auf der Grundlage dieser Änderung.
>
>Der Benutzer, der die Stunden budgetiert, ordnet diese Ressource zuerst zu und reduziert die Anzahl der verfügbaren Stunden für diese Ressource im System. Die Anzahl der verfügbaren Stunden sollte für alle Benutzer aktualisiert werden, sobald die budgetierten Stunden für eine Ressource im Ressourcenplaner gespeichert wurden.
>
>Weitere Informationen zu Verfügbare Stunden finden Sie unter [Verfügbarkeit und Zuweisung von Ressourcen](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#availability-and-allocation-of-resources).
