---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: Projekt in der Agile-Ansicht verwalten
description: Erforderliche Pläne, Lizenztypen und Zugriffe auf das Adobe Workfront Planungsteam, Pro, Business oder Enterprise Workfront-Lizenztyp Prüfen, Arbeiten oder Planen von Berechtigungen im Zugriffsmodell Zugriff bearbeiten und Möglichkeit, Berichte, Dashboards und Kalender zu erstellen
author: Alina
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1311'
ht-degree: 0%

---

# Projekt in der Agile-Ansicht verwalten

Erforderliche Pläne, Lizenztypen und Zugriffsrechte

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront-Plan</a> </p> </td> 
   <td> <p>Team, Pro, Business oder Enterprise </p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="https://one.workfront.com/s/article/Understanding-License-Types-906212506?language=en_US&amp;r=16&amp;ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&amp;ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&amp;ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&amp;ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&amp;ui-self-service-components-controller.ArticleTopicList.getTopics=1&amp;ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank">Workfront-Lizenztyp</a> </p> </td> 
   <td> <p>Überprüfen, Arbeiten oder Planen </p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> <p>Permissions in the access model</p> </td> 
    <td> <li>Edit access and ability to create reports, dashboards, and calendars</li> </td> 
   </tr>
  --> 
 </tbody> 
</table>

Sie können die agile Funktionalität für Ihr Projekt nutzen

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(such as story boards and burndown charts)
</MadCap:conditionalText>
-->

 ohne die administrativen Herausforderungen, die normalerweise mit agilen Vorgehensweisen einhergehen (z. B. Verwaltung eines Team-Rückstands oder Erstellen von Iterationen).

Wenn Sie in einer agilen Umgebung arbeiten möchten, die einen Team-Backlog verwendet und es Ihnen ermöglicht, Iterationen aus Aufgaben im Backlog zu erstellen, folgen Sie den Anweisungen unter [Arbeiten in einer agilen Umgebung](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Bearbeiten Sie den Zugriff auf die folgenden Bereiche:</p> 
    <ul> 
     <li> <p>Projekte</p> </li> 
     <li> <p>Berichte, Dashboards, Kalender</p> </li> 
     <li> <p>Filter, Ansichten, Gruppierungen</p> </li> 
    </ul> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Projekt anzeigen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Grundlegendes zu Agile-Projekten

* [Agile Funktionalität in einem Projekt](#agile-functionality-in-a-project)
* [Unterschiede bei der Verwendung der Agile-Ansicht für ein Projekt im Vergleich zu einer Iteration](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### Agile Funktionalität in einem Projekt {#agile-functionality-in-a-project}

Die folgende agile Funktion ist verfügbar, wenn ein Projekt in einer agilen Ansicht verwaltet wird:

* Fertigstellungsstatus\
   Weitere Informationen zum Fertigstellungsstatus finden Sie unter [Übersicht über den Iterationsabschluss](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md).

* Story Board\
   Weitere Informationen zum Storyboard finden Sie im Abschnitt [Pinnwand](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md) Abschnitt.

Es gibt einige Unterschiede bei der Verwendung von agilen Ansichten für ein Projekt im Vergleich zur Arbeit in einer reinen agilen Umgebung (mit Rückständen und Iterationen). Weitere Informationen finden Sie unter [Unterschiede bei der Verwendung der Agile-Ansicht für ein Projekt im Vergleich zu einer Iteration](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) in diesem Artikel.

### Unterschiede bei der Verwendung der Agile-Ansicht für ein Projekt im Vergleich zu einer Iteration {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [Aufgaben und Unteraufgaben folgen unterschiedlichen Anzeigeregeln auf dem Meldungsboard](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [Rücklogs und Iterationen werden nicht verwendet](#backlogs-and-iterations-are-not-used)
* [Die Aufgabenreihenfolge wird in der Agile-Ansicht beibehalten und kann nicht neu angeordnet werden](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [Aufgaben werden nur in geplanten Stunden gemessen](#tasks-are-measured-only-in-planned-hours)
* [Das Agile-Team wird nicht verwendet](#the-agile-team-is-not-used)
* [Jeder Benutzer im Projekt kann das Projekt in einer anderen Agile-Ansicht anzeigen](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### Aufgaben und Unteraufgaben folgen unterschiedlichen Anzeigeregeln auf dem Meldungsboard {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* Aufgaben, die weder über eine übergeordnete Aufgabe noch über eine Unteraufgabe verfügen, werden immer als eine einzige Storykarte auf dem Storyboard angezeigt.\
   Diese Aufgaben werden beispielsweise in der Listenansicht des Projekts wie folgt angezeigt:

   ![Agile Projektliste - Aufgaben ohne übergeordnete Aufgaben oder Unteraufgaben](assets/agile-project-single-list-nwe.png) Diese Aufgaben werden in der agilen Projektansicht wie folgt angezeigt:

   ![Projektansicht - Aufgaben ohne übergeordnete Aufgaben oder Unteraufgaben](assets/agile-project-singlecard-nwe.png)

* Übergeordnete Aufgaben mit Unteraufgaben werden immer im **Meldungen** Spalte des Storyboards. Unteraufgaben werden in der Swimlane der übergeordneten Aufgabe angezeigt.\
   Diese Aufgaben werden beispielsweise in der Listenansicht des Projekts wie folgt angezeigt:

   ![Agile Projektliste - Aufgaben mit übergeordneten Elementen und Unteraufgaben](assets/agile-project-parent-list-nwe.png)\
   Diese Aufgaben werden in der agilen Projektansicht wie folgt angezeigt:

   ![Agile Projektansicht - Aufgaben mit übergeordneten Elementen und Unteraufgaben](assets/agile-project-parent-nwe.png)

* Unteraufgaben der zweiten Ebene (Unteraufgaben von Unteraufgaben) werden als hängende graue Karte der unmittelbar übergeordneten Aufgabe angezeigt.
* Unteraufgaben der dritten Ebene (Unteraufgaben von Unteraufgaben von Unteraufgaben) werden nie auf dem Storyboard angezeigt.

#### Rücklogs und Iterationen werden nicht verwendet {#backlogs-and-iterations-are-not-used}

Beim Anzeigen eines Projekts in einer agilen Ansicht werden die folgenden agilen Komponenten nicht verwendet:

* **Rückprotokoll:** Es wird kein Rückstau verwendet, da Aufgaben im Projekt automatisch als Meldungen angezeigt werden.
* **Iterationen:** Statt Iterationen zu erstellen, um die Daten zu definieren, zu denen die Arbeit abgeschlossen sein wird, werden die derzeit in der Projekt-Timeline festgelegten Tage zu Arbeitstagen.

#### Die Aufgabenreihenfolge wird in der Agile-Ansicht beibehalten und kann nicht neu angeordnet werden {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

Die Reihenfolge, in der Aufgaben in einem Projekt angezeigt werden, wird beibehalten, wenn Sie das Projekt in einem agilen Storyboard anzeigen.

Sie können Aufgaben im Projekt nicht neu anordnen, wenn Sie das Projekt in einer agilen Ansicht anzeigen. Da sich eine Änderung der Aufgabenreihenfolge auf andere Aufgaben auswirken kann, die möglicherweise Abhängigkeiten aufweisen, müssen Sie das Projekt in einer Standardansicht anzeigen, um die Aufgabenreihenfolge zu ändern.

#### Aufgaben werden nur in geplanten Stunden gemessen {#tasks-are-measured-only-in-planned-hours}

Aufgaben an einem Projekt werden immer in geplanten Stunden gemessen.

Bei einer Iteration können Aufgaben (Geschichten) in Stunden oder Punkten gemessen werden.

#### Das Agile-Team wird nicht verwendet {#the-agile-team-is-not-used}

Da agile Teams die Arbeit mit den ihnen zugewiesenen Iterationen abschließen, werden agile Teams nicht verwendet, wenn ein Projekt in einer agilen Ansicht angezeigt wird.

Stattdessen werden alle Benutzer im Projekt im Wesentlichen zum agilen Team für dieses Projekt.

#### Jeder Benutzer im Projekt kann das Projekt in einer anderen Agile-Ansicht anzeigen {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

Im Gegensatz zu einer agilen Iteration können Benutzer eines Projekts die agile Ansicht für sich selbst anpassen, während andere Benutzer eine andere agile Ansicht verwenden.

Bei einer agilen Iteration werden die auf der agilen Story-Pinnwand verfügbaren Informationen (z. B. verfügbare Statusspalten) auf Teamebene bestimmt.

Informationen zum Anpassen einer agilen Ansicht finden Sie unter  [Erstellen oder Anpassen einer Agile-Ansicht](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in  [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 

## Anzeigen eines Projekts in der Agile-Ansicht

1. Wechseln Sie zu dem Projekt, das Sie in einer agilen Ansicht anzeigen möchten.
1. Klicken Sie auf **Agile** Symbol.\
   ![Symbol &quot;Agil&quot;](assets/agile-icon-nwe.png)\
   Das Projekt wird in der standardmäßigen agilen Ansicht angezeigt.\
   Wenn Sie das Projekt zuvor in einer benutzerdefinierten agilen Ansicht angezeigt haben, wird das Projekt in dieser Ansicht und nicht in der standardmäßigen agilen Ansicht angezeigt.

1. (Optional) Wenn Sie eine benutzerdefinierte agile Ansicht erstellt haben oder wenn ein anderer Benutzer eine benutzerdefinierte agile Ansicht erstellt und für Sie freigegeben hat, können Sie sie anstelle der standardmäßigen agilen Ansicht anzeigen.\
   Klicken Sie auf **Ansicht** Dropdown-Menü und klicken Sie dann auf die gewünschte benutzerdefinierte Ansicht.

   Die benutzerdefinierte Ansicht &quot;agile&quot;wird verwendet, wenn Sie das nächste Mal auf die **Agile** Symbol.\
   Informationen zum Erstellen einer neuen agilen Ansicht finden Sie unter [Erstellen und Anpassen von Agile-Ansichten](#create-and-customize-agile-views).\
   Das Projekt wird in der benutzerdefinierten agile Ansicht angezeigt.

1. (Bedingt) Wenn Aufgaben in Ihrem Projekt andere Status als &quot;Neu&quot;, &quot;In Bearbeitung&quot;oder &quot;Abgeschlossen&quot;(die Standardstatus für die Agile-Ansicht) verwenden, müssen Sie die zusätzlichen Status zur agilen Ansicht hinzufügen, damit alle Aufgaben in diesen Status angezeigt werden.\
   Wenn Aufgaben sich in einem Status befinden, der nicht auf der agilen Story-Pinnwand angezeigt wird, wird die Aufgabe selbst nicht auf der agilen Story-Pinnwand angezeigt (der prozentuale Abschluss dieser Aufgaben trägt jedoch weiterhin zum Percent Complete der übergeordneten Aufgaben und zum Percent Complete des übergeordneten Projekts bei).\
   Um der agilen Ansicht Status hinzuzufügen, erstellen Sie entweder eine neue agile Ansicht oder passen Sie eine vorhandene agile Ansicht an, wie im Abschnitt &quot;Erstellen oder Anpassen einer Agile-Ansicht&quot;im Artikel beschrieben. [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. (Optional) Um zur Listenansicht zurückzukehren, klicken Sie auf die **Liste** Symbol.\
   ![](assets/list-icon.png)

## Erstellen und Anpassen von Agile-Ansichten {#create-and-customize-agile-views}

Wie bei standardmäßigen Ansichten in Workfront können Sie vorhandene agile Ansichten anpassen oder neue agile Ansichten von Grund auf neu erstellen. Im Gegensatz zu Standardansichten können Sie keine neuen agilen Ansichten basierend auf vorhandenen agilen Ansichten erstellen.

Weitere Informationen zum Erstellen und Anpassen agiler Ansichten finden Sie im Abschnitt &quot;Erstellen oder Anpassen einer Agile-Ansicht&quot;im Artikel [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 

## Vorhandene Agile-Ansicht freigeben

Informationen zum Freigeben einer agilen Ansicht finden Sie unter [Filter, Ansichten oder Gruppierungen freigeben](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

## Vorhandene Agile-Ansicht entfernen

Informationen zum Löschen einer Ansicht finden Sie im Abschnitt &quot;Ansicht entfernen&quot;im Artikel [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md). 
