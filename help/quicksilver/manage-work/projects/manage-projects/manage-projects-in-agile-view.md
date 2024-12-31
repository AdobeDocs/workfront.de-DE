---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: Verwalten eines Projekts in der Agile-Ansicht
description: Sie können die Agile-Funktionen für Ihr Projekt nutzen, ohne die administrativen Herausforderungen zu bewältigen, die mit Agile-Praktiken verbunden sind (z. B. die Verwaltung eines Team-Rückstands oder die Erstellung von Iterationen).
author: Alina and Lisa
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '1423'
ht-degree: 0%

---

# Verwalten eines Projekts in der Agile-Ansicht

<!-- Audited: 2/2024 -->

Sie können die Agile-Funktionen für Ihr Projekt nutzen, ohne die administrativen Herausforderungen zu bewältigen, die mit Agile-Praktiken verbunden sind (z. B. die Verwaltung eines Team-Rückstands oder die Erstellung von Iterationen).

Wenn Sie in einer agilen Umgebung arbeiten möchten, die einen Rückstand im Team aufweist und es Ihnen ermöglicht, Iterationen aus Aufgaben im Rückstand zu erstellen, befolgen Sie die Anweisungen unter [Arbeiten in einer agilen Umgebung](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Aktuell: Überprüfung oder höher</p> 
   <p>Neu: Mitwirkender oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>Bearbeiten Sie den Zugriff auf die folgenden Bereiche:</p> 
    <ul> 
     <li> <p>Projekte</p> </li> 
     <li> <p>Berichte, Dashboards, Kalender</p> </li> 
     <li> <p>Filter, Ansichten, Gruppierungen</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen der Berechtigungen für das Projekt</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Agile-Projekte

>[!NOTE]
>
>Dieser Abschnitt gilt nur für die veraltete Agile-Ansicht, nicht für die Board-Ansicht eines Projekts.

* [Agile-Funktionalität in einem Projekt](#agile-functionality-in-a-project)
* [Unterschiede zwischen der Verwendung der Agile-Ansicht eines Projekts und einer Iteration](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration)

### Agile-Funktionalität in einem Projekt {#agile-functionality-in-a-project}

Die folgenden Agile-Funktionen sind beim Verwalten eines Projekts in einer Agile-Ansicht verfügbar:

* Fertigstellungsstatus\
  Weitere Informationen zum Abschlussstatus finden Sie unter [Übersicht über den Iterationsabschlussstatus](../../../agile/use-scrum-in-an-agile-team/burndown/iteration-completion-status-overview.md).

* Storyboard\
  Weitere Informationen zum Story Board finden Sie im Abschnitt [Scrum-Board](../../../agile/use-scrum-in-an-agile-team/scrum-board/scrum-board.md) .

Es gibt einige Unterschiede zwischen der Verwendung agiler Ansichten für ein Projekt und der Arbeit in einer reinen agilen Umgebung (mit Rückständen und Iterationen). Weitere Informationen finden Sie unter [ bei der Verwendung der Agile-Ansicht bei einem Projekt im Vergleich zu einer Iteration ](#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration) diesem Artikel.

### Unterschiede zwischen der Verwendung der Agile-Ansicht eines Projekts und einer Iteration {#differences-when-using-the-agile-view-on-a-project-versus-on-an-iteration}

* [Aufgaben und Teilaufgaben folgen unterschiedlichen Anzeigeregeln in einer Agile-Projektansicht und im Story Board einer Iteration](#tasks-and-subtasks-follow-different-display-rules-on-the-story-board)
* [Rückstände und Iterationen werden in der Agile-Ansicht nicht verwendet](#backlogs-and-iterations-are-not-used)
* [Die Aufgabenreihenfolge wird in der Agile-Ansicht beibehalten und kann nicht neu angeordnet werden](#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered)
* [Aufgaben werden in einer Projektliste nur in geplanten Stunden gemessen](#tasks-are-measured-only-in-planned-hours)
* [Das Agile-Team wird in einer Agile-Ansicht nicht verwendet](#the-agile-team-is-not-used)
* [Jeder Benutzer im Projekt kann das Projekt in einer anderen Agile-Ansicht anzeigen.](#each-user-on-the-project-can-view-the-project-in-a-different-agile-view)

#### Aufgaben und Teilaufgaben folgen unterschiedlichen Anzeigeregeln in einer Agile-Projektansicht und im Story Board einer Iteration {#tasks-and-subtasks-follow-different-display-rules-on-the-story-board}

* Aufgaben, die weder eine übergeordnete Aufgabe noch eine Unteraufgabe haben, werden immer als eine einzige Story-Karte im Story Board der Agile-Ansicht angezeigt.\
  Diese Aufgaben werden beispielsweise in der Projektlistenansicht wie folgt angezeigt:

  ![Agile-Projektliste - Aufgaben ohne übergeordnete oder untergeordnete Aufgaben](assets/agile-project-single-list-nwe.png)

  Diese Aufgaben werden in der agilen Ansicht des Projekts wie folgt angezeigt:

  ![Agile Projektansicht - Aufgaben ohne übergeordnete oder Teilaufgaben](assets/agile-project-singlecard-nwe.png)

* Übergeordnete Aufgaben mit Teilaufgaben werden immer in der Spalte **Storys** des Storyboards der Agile-Ansicht angezeigt. Teilaufgaben werden in der Navigationsleiste der übergeordneten Aufgabe angezeigt.\
  Diese Aufgaben werden beispielsweise in der Projektlistenansicht wie folgt angezeigt:

  ![Agile-Projektliste - Aufgaben mit übergeordneten und untergeordneten Aufgaben](assets/agile-project-parent-list-nwe.png)\
  Diese Aufgaben werden in der agilen Ansicht des Projekts wie folgt angezeigt:

  ![Agile-Projektansicht - Aufgaben mit übergeordneten und untergeordneten Aufgaben](assets/agile-project-parent-nwe.png)

* Unteraufgaben der zweiten Ebene (Unteraufgaben von Unteraufgaben) werden als hängende graue Karte der unmittelbar übergeordneten Aufgabe angezeigt.
* Unteraufgaben der dritten Ebene (Unteraufgaben von Unteraufgaben von Unteraufgaben) werden niemals in der Agile-Ansicht angezeigt.

#### Rückstände und Iterationen werden in der Agile-Ansicht nicht verwendet {#backlogs-and-iterations-are-not-used}

Beim Anzeigen eines Projekts in einer Agile-Ansicht werden die folgenden Agile-Komponenten nicht verwendet:

* **Rückstand:** wird kein Rückstand verwendet, da alle Aufgaben im Projekt automatisch als Storys angezeigt werden.
* **Iterationen:** Anstatt Iterationen zu erstellen, um die Daten zu definieren, an denen die Arbeit abgeschlossen wird, werden die aktuell in der Projektzeitleiste festgelegten Tage zu Arbeitstagen.

#### Die Aufgabenreihenfolge wird in der Agile-Ansicht beibehalten und kann nicht neu angeordnet werden {#task-order-is-maintained-in-the-agile-view-and-cannot-be-reordered}

Die Reihenfolge, in der Aufgaben in einem Projekt angezeigt werden, wird beibehalten, wenn Sie das Projekt in einem Agile-Story-Board anzeigen.

Sie können Aufgaben im Projekt nicht neu anordnen, wenn Sie das Projekt in einer Agile-Ansicht anzeigen. Da sich die Änderung der Aufgabenreihenfolge auf andere Aufgaben auswirken kann, die möglicherweise Abhängigkeiten aufweisen, müssen Sie das Projekt in einer Standardansicht anzeigen, um die Aufgabenreihenfolge ändern zu können.

#### Aufgaben werden in einer Projektliste nur in geplanten Stunden gemessen {#tasks-are-measured-only-in-planned-hours}

Aufgaben in einem Projekt werden immer in „Geplante Stunden“ gemessen.

In einer Iteration können Aufgaben (Storys) in Stunden oder Punkten gemessen werden.

#### Das agile Team wird in einer Agile-Ansicht nicht verwendet {#the-agile-team-is-not-used}

Da agile Teams die ihnen zugewiesenen Iterationen abschließen, werden agile Teams nicht verwendet, wenn ein Projekt in einer agilen Ansicht angezeigt wird.

Stattdessen werden alle Benutzer im Projekt im Wesentlichen zum agilen Team für dieses Projekt.

#### Jeder Benutzer im Projekt kann das Projekt in einer anderen Agile-Ansicht anzeigen. {#each-user-on-the-project-can-view-the-project-in-a-different-agile-view}

Im Gegensatz zu einer agilen Iteration können Benutzende eines Projekts die Agile-Ansicht für sich selbst anpassen, während andere Benutzende eine andere Agile-Ansicht verwenden.

Bei einer agilen Iteration werden die Informationen, die auf dem Agile-Story-Board verfügbar sind (z. B. verfügbare Statusspalten), auf Team-Ebene bestimmt.

Informationen zum Anpassen einer Agile-Ansicht finden Sie unter [Erstellen oder Anpassen einer Agile](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) in [Erstellen oder Bearbeiten von Ansichten in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Anzeigen eines Projekts in der Agile-Ansicht

1. Wechseln Sie zu dem Projekt, das Sie in einer Agile-Ansicht anzeigen möchten, entweder in der Aufgabenliste oder in der Problemliste.
1. Klicken Sie auf **Symbol** Pinnwand-Ansicht![ (](assets/board-icon-for-agile-view.png).

   Die Pinnwand-Ansicht des Projekts wird standardmäßig angezeigt.

   ![Board-Ansicht des Projekts](assets/project-agile-board-view.png)

   <!--(Legacy agile view only) If you previously viewed the project in a custom agile view, the project is displayed in that view rather than in the default agile view.-->

1. (Optional) Klicken Sie auf **Konfigurieren**, um Optionen für die Spalten und Karten festzulegen.

   Weitere Informationen finden Sie unter [Verwalten von ](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md) und [Anpassen, welche Felder auf einer Karte angezeigt werden](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md). Beachten Sie, dass Sie keine Spaltenrichtlinien in der Pinnwand-Ansicht eines Projekts definieren können.

1. (Optional) Klicken Sie auf **Veraltete Agile verwenden**, um die veraltete Agile-Ansicht anstelle der Board-Ansicht zu verwenden.

1. (Optional - Nur veraltete Agile-Ansicht) Wenn Sie eine benutzerdefinierte Agile-Ansicht erstellt haben oder wenn ein anderer Benutzer eine benutzerdefinierte Agile-Ansicht erstellt und für Sie freigegeben hat, können Sie sie anstelle der standardmäßigen Agile-Ansicht anzeigen.

   Klicken Sie auf **Dropdown** Menü „Ansicht“ und dann auf die benutzerdefinierte agile Ansicht, die Sie anzeigen möchten.

   Die benutzerdefinierte Agile-Ansicht wird verwendet, wenn Sie das nächste Mal auf das Symbol **Agile** klicken.

   Weitere Informationen zum Erstellen einer neuen Agile-Ansicht finden Sie [Erstellen und Anpassen von Agile-Ansichten](#create-and-customize-agile-views) unten.

   Das Projekt wird in der benutzerdefinierten agilen Ansicht angezeigt.

1. (Bedingt - nur veraltete Agile-Ansicht) Wenn Aufgaben in Ihrem Projekt andere Status als „Neu“, „In Bearbeitung“ oder „Abgeschlossen“ verwenden (die Standardstatus für die Agile-Ansicht), müssen Sie die zusätzlichen Status zur Agile-Ansicht hinzufügen, damit alle Aufgaben in diesen Status angezeigt werden.

   Wenn Aufgaben in einem Status sind, der nicht im Agile-Story-Board angezeigt wird, wird die Aufgabe selbst nicht im Agile-Story-Board angezeigt (die Prozentangabe „Prozent abgeschlossen“ dieser Aufgaben trägt jedoch weiterhin zum Prozentwert der Fertigstellung übergeordneter Aufgaben und zum Prozentwert der Fertigstellung des gesamten Projekts bei).

   Um Status zur Agile-Ansicht hinzuzufügen, erstellen Sie entweder eine neue Agile-Ansicht oder passen Sie eine vorhandene Agile-Ansicht an, wie [ unten unter „Erstellen und Anpassen ](#create-and-customize-agile-views) Agile-Ansichten“ beschrieben.

1. (Optional) Um zur Listenansicht zurückzukehren, klicken Sie auf das Symbol **Liste**.

## Erstellen und Anpassen von Agile-Ansichten {#create-and-customize-agile-views}

>[!NOTE]
>
>Dieser Abschnitt gilt nur für die veraltete Agile-Ansicht, nicht für die Board-Ansicht eines Projekts.

Wie bei Standardansichten in Workfront können Sie vorhandene Agile-Ansichten anpassen oder neue Agile-Ansichten von Grund auf neu erstellen. Im Gegensatz zu Standardansichten können Sie keine neuen Agile-Ansichten erstellen, die auf vorhandenen Agile-Ansichten basieren.

Weitere Informationen zum Erstellen und Anpassen von Agile-Ansichten finden Sie [ Abschnitt „Erstellen oder Anpassen einer Agile](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) im Artikel [Erstellen oder Bearbeiten von Ansichten in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Freigeben einer vorhandenen Agile-Ansicht

>[!NOTE]
>
>Dieser Abschnitt gilt nur für die veraltete Agile-Ansicht, nicht für die Board-Ansicht eines Projekts.

Sie können eine Agile-Ansicht, die Sie erstellt haben, freigeben oder über Berechtigungen zum Freigeben verfügen, genauso wie Sie eine andere Ansicht, einen Filter oder eine Gruppierung freigeben.

Weitere Informationen finden Sie unter [Freigeben von Filtern, Ansichten oder Gruppierungen](../../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

## Entfernen einer vorhandenen Agile-Ansicht

>[!NOTE]
>
>Dieser Abschnitt gilt nur für die veraltete Agile-Ansicht, nicht für die Board-Ansicht eines Projekts.

Sie können eine Agile-Ansicht auf die gleiche Weise entfernen wie jede andere Ansicht, jeden Filter oder jede Gruppierung.

Weitere Informationen finden Sie unter [Filter, Ansichten und Gruppierungen entfernen](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/remove-filters-views-groupings.md).
