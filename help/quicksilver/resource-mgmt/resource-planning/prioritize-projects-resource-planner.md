---
product-area: resource-management;projects
navigation-topic: resource-planning
title: Priorisieren von Projekten im Ressourcenplaner
description: Die Projekte werden in der Reihenfolge ihrer Priorität im Ressourcenplaner aufgelistet, wobei das wichtigste Projekt ganz oben aufgeführt ist.
author: Alina
feature: Resource Management
exl-id: fe9c8cf9-f1e0-4cd5-9299-0f04893d71a5
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '1330'
ht-degree: 1%

---

# Priorisieren von Projekten im Ressourcenplaner

Die Projekte werden in der Reihenfolge ihrer Priorität im Ressourcenplaner aufgelistet, wobei das wichtigste Projekt ganz oben aufgeführt ist.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Pro und höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Bearbeiten Sie den Zugriff auf das Ressourcen-Management, das Zugriff auf die Option "Prioritäten bearbeiten"und die Budgetzeiten im Ressourcenplaner enthält.</p> <p>Zugriff auf Finanzdaten, Projekte und Benutzer bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für die Projekte, für die Informationen zum Budget bereitgestellt werden sollen, mit der Möglichkeit, die Finanzen zu verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Standardreihenfolge von Projekten im Ressourcenplaner

Standardmäßig werden die Projekte unter Berücksichtigung der unten stehenden Kriterien in der Projektansicht des Ressourcen-Planers aufgelistet.

>[!IMPORTANT]
>
>Projekte werden nur beim ersten Öffnen des Ressourcenplaners nach den drei folgenden Kriterien aufgelistet. Diese Standardpriorität wird jedoch automatisch zu Ihrer benutzerdefinierten Priorität und kann nicht jedes Mal, wenn Sie einen der folgenden Schritte ausführen, zur ursprünglichen Priorität zurückgesetzt werden:
>
>* Wenn Sie jederzeit auf Speichern klicken.
>* Wenn Sie die Priorität der Projektplanung manuell ändern. Informationen zum manuellen Ändern der Projektplanungspriorität finden Sie im Abschnitt [Manuelles Ändern der Priorität für die Projektplanung](#manually-change-the-project-planning-priority) in diesem Artikel.
>
>Nachdem die Projektpriorität zu Ihrer benutzerdefinierten Priorität wird, wirken sich Änderungen an den Projektinformationen nicht mehr auf die Reihenfolge der Projekte aus, die diese Kriterien verwenden. Danach können Sie Projekte nur manuell priorisieren.

Die ursprünglichen Standardkriterien für die Auflistung der Projekte in der Projektansicht lauten wie folgt:

1. Nach der Alignment-Bewertung im Projekt.\
   Weitere Informationen zur Alignment-Bewertung des Projekts finden Sie unter [Anwenden einer Scorecard auf ein Projekt und Generieren einer Alignment-Bewertung](../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md) .

1. Nach dem geplanten Startdatum des Projekts (wenn das Feld Ausrichtung null oder für mehrere Projekte identisch ist).
1. Alphabetisch (wenn das Feld Ausrichtung null oder gleich ist und das geplante Startdatum für mehrere Projekte dasselbe ist).

Beachten Sie beim Arbeiten mit Projektprioritäten im Ressourcenplaner Folgendes:

* Sie können die Projektpriorität nur manuell anpassen, wenn Sie die Projektansicht anwenden. Dadurch wird auch die Reihenfolge der Projekte im Ressourcenplaner geändert.
* Wenn Sie die Rollen- oder Benutzeransichten im Ressourcenplaner anwenden, werden die Projekte in der in der Projektansicht festgelegten Reihenfolge mit der Priorität angezeigt.
* Die Reihenfolge der Projekte im Ressourcenplaner ist für Sie eindeutig. Andere Benutzer können dieselben Projekte im Ressourcenplaner anzeigen, aber in einer anderen Reihenfolge. Sie können keinen Bericht zum Feld Projektplanungspriorität erstellen. Dies ist direkt im Ressourcen-Planer sichtbar und dient als Flag zur Priorisierung Ihrer Projekte.

Projekte, die mit einem Portfolio verknüpft sind, haben möglicherweise eine Priorität auf Portfolioebene. Sie können die Anzeige der Portfoliopriorität eines Projekts im Ressourcenplaner zusätzlich zur Priorität &quot;Ressourcenplaner&quot;aktivieren. Sie können die Projekte auch nach ihrer Portfoliopriorität bestellen.

## Manuelles Ändern der Priorität für die Projektplanung {#manually-change-the-project-planning-priority}

Sie müssen Zugriff auf Ressourcenverwaltung bearbeiten und Berechtigungen für Projekte verwalten haben, um Projekte im Ressourcenplaner neu anzuordnen.

Wenn Sie Projekten eine neue Priorität einräumen, können Sie sie nach Wichtigkeit ordnen.

So bearbeiten Sie die Priorität der Projektplanung:

1. Navigieren Sie zu **Ressourcenplaner**.

1. Klicken Sie in das Feld links neben dem Projektnamen, der eine Nummer enthält, geben Sie eine Nummer ein, um die Planungspriorität zu ändern, und drücken Sie die Eingabetaste.\
   ![](assets/mceclip4.png)\
   Oder\
   Bewegen Sie den Mauszeiger über den Namen des Projekts und klicken Sie auf den Indikator links neben dem Projektnamen. Ziehen Sie ihn per Drag-and-Drop an die richtige Stelle, um die Priorität zu ändern.

   ![drag_and_drop_projects_RP__1_.png](assets/drag-and-drop-projects-rp--1--350x184.png)

   Wenn Sie Zahlen zur Priorisierung von Projekten auswählen, wählen Sie niedrigere Zahlen für höhere (wichtigere) Prioritäten und höhere Zahlen für niedrigere (weniger wichtige) Prioritäten. Wenn Sie die Prioritätsnummer eines Projekts in eine niedrigere Zahl (höhere Priorität) ändern, werden alle anderen Projekte im Ressourcenplaner auf die Liste verschoben (weniger wichtig).\
   Wenn Sie die Prioritätsnummer eines Projekts in eine höhere Zahl (niedrigere Priorität) ändern, werden alle anderen Projekte im Ressourcenplaner auf der Liste nach oben verschoben (wichtiger).

1. Klicken Sie auf **Speichern**.\
   Die Reihenfolge der Projekte ändert sich entsprechend Ihrer Auswahl. Dies wird zu Ihrer benutzerdefinierten Projektpriorität im Ressourcenplaner. Andere Benutzer können Ihre Prioritätsreihenfolge für die Projekte im Ressourcenplaner nicht sehen, obwohl sie möglicherweise dieselben Projekte in ihrem Ressourcenplaner anzeigen können.

## Bestellen von Projekten nach ihrer Portfolio-Priorität im Ressourcen-Planer

>[!IMPORTANT]
>
>Ihr Unternehmen muss über einen Business- oder höher-Workfront-Plan verfügen, um Portfolio Optimizer-Projekte zu priorisieren.
>
>Weitere Informationen zu den Workfront-Plänen finden Sie unter [Unsere Pläne](https://www.workfront.com/plans).
>
>Informationen zur Priorisierung von Projekten in Portfolio Optimizer finden Sie unter [Priorisieren von Projekten in Portfolio Optimizer](../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md).

1. Öffnen Sie die **Ressourcenplaner** im **Projektansicht**.
1. Klicken Sie auf **Einstellungen** Symbol.
1. Aktivieren Sie die **Anzeigen von Portfolio-Prioritäten** Einstellung, um die Projektprioritäten entsprechend dem Portfolio anzuzeigen, dem sie zugewiesen sind. Die Priorität der Projekte entsprechend ihren Portfolios wird neben der Priorität des Ressourcenplaners angezeigt. Diese Einstellung ist standardmäßig deaktiviert.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: check screen shot to see if this is accurate still - should say Order, and not Sort:)</p>
   -->

   ![](assets/rp-portfolio-priority-unordered-edit-350x180.png)

   Die Portfolioprioritäten der Projekte werden nur in der Projektansicht des Ressourcenplaners angezeigt.

1. Klicken **Bestellung** die Projekte nach den Portfolioprioritäten zu ordnen.

   Wenn Sie über Projekte verfügen, die zu mehr als einem Portfolio gehören, können Sie im Ressourcenplaner mehrere Projekte mit derselben Portfoliopriorität sehen. In diesem Fall werden die Projekte mit derselben Portfoliopriorität nach folgenden Kriterien aufgelistet:

   1. Ausrichtungsbewertung
   1. Geplantes Startdatum
   1. Projektname

   ![](assets/rp-portfolio-priority-ordered-350x198.png)

1. Klicken Sie auf **Speichern**.

## Auswirkungen der Änderung der Priorität für die Projektplanung auf die verfügbaren Stunden der Benutzer

Die Priorität der Projektplanung wirkt sich auf die verfügbaren Stunden von Benutzern aus. Die mit dem Projekt verknüpften Benutzer mit der höchsten Priorität zeigen gemäß ihren Zeitplänen, dass sie für die Spalte Verfügbare Stunden (AVL) für dieses Projekt vollständig verfügbar sind.

Dieselben Benutzer, die in der Reihenfolge ihrer Priorität mit dem zweiten Projekt verbunden sind, zeigen den Wert Verfügbare Stunden an, der den Unterschied zwischen der vollen Anzahl verfügbarer Stunden und dem darstellt, was bereits für das erste Projekt in der Spalte &quot;Geplante Stunden&quot;in den Haushaltsplan eingestellt wurde usw. Informationen zu den im Ressourcenplaner verfügbaren Haushaltsmitteln finden Sie unter [Budgetressourcen im Ressourcenplaner mithilfe der Projekt- und Rollenansicht](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

Wenn für das erste Projekt keine Stunden (in der Reihenfolge der Priorität) für einen Benutzer in den Haushalt aufgenommen wurden, für das zweite Projekt jedoch Stunden für denselben Benutzer vorgesehen wurden, zeigt der Benutzer die volle Anzahl der verfügbaren Stunden für beide Projekte an.

Es wird empfohlen, die Spalte &quot;Budgetierte Stunden&quot;für Ihre Benutzer in der Reihenfolge der Projekte im Ressourcenplaner zu aktualisieren, um sicherzustellen, dass Sie die verfügbaren Stunden für den Benutzer jederzeit genau sehen können.

>[!NOTE]
>
>Da die Priorität für die Projektplanung für jeden Ressourcen-Manager eindeutig ist, kann Ihr Projekt mit der zweiten Priorität für einen anderen Benutzer, der dieselben Projekte in seinem Ressourcenplaner ansieht, ein Projekt mit der ersten Priorität sein. Wenn ein anderer Ressourcen-Manager eine Ressource für das erste Projekt einplant, werden die Verfügbaren Stunden für diese Ressource für das erste Projekt aufgrund dieser Änderung reduziert.
>
>Der Benutzer, der die Stunden einplant, ordnet diese Ressource zuerst zu und reduziert die Anzahl der verfügbaren Stunden für diese Ressource im gesamten System. Die Anzahl der verfügbaren Stunden sollte für alle Benutzer aktualisiert werden, sobald die budgetierten Stunden für eine Ressource im Ressourcenplaner gespeichert wurden.
>
>Weitere Informationen zu verfügbaren Stunden finden Sie unter [Verfügbarkeit und Zuordnung von Ressourcen](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md#availability-and-allocation-of-resources).
