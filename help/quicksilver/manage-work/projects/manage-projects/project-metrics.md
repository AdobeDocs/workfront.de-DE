---
content-type: overview;how-to-procedural
product-area: projects
keywords: Analytics,Metriken,Projekt,Aufgaben,Verantwortlicher,Abgeschlossen,Status,Überfällig,Bevorstehende
navigation-topic: manage-projects
title: Verstehen von Projektmetriken
description: Projektmetriken bieten Ihnen eine Visualisierung der Vorgänge in einem Projekt, sodass Sie die Anforderungen und den Status eines Projekts schnell bewerten können. Erfahren Sie, wie der Bereich „Metriken“ im linken Bereich eines Projekts interpretiert wird.
author: Alina
feature: Work Management
exl-id: 54c2a59d-9f6b-4126-9526-5169aeda8517
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/ebZ7z4dnpQUN0i0zbEuyqx0tZBbDfTJWgqw743E2a2U
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: be65ef36-43e4-48e1-a062-caa3778e15be
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 1221
ht-degree: 3%

---

# Grundlegendes zu Projektmetriken

Projektmetriken bieten eine allgemeine Ansicht der Leistung eines Projekts im Diagrammformat.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Licht oder höher</p>
   <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte anzeigen</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von Berechtigungen für ein Projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workfront license*</td> 
   <td> <p>New: Light or higher </p>
   <p>Current: Review or higher </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration</td> 
   <td> <p>View access to Projects</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a project</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Voraussetzungen

Um über das linke Bedienfeld eines Projekts auf den Bereich Metriken zuzugreifen, ist Folgendes erforderlich:

* Lassen Sie die Option Metriken im linken Bedienfeld im Bereich Projekte Ihrer Layout-Vorlage aktivieren.

  Informationen dazu, wie Workfront-Admins oder Gruppenadmins den linken Bereich mit einer Layout-Vorlage anpassen können, finden Sie unter [Anpassen des linken Bereichs mithilfe einer Layout-Vorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

## Übersicht über den Bereich Projektmetriken

Projektmetriken bieten Ihnen eine Visualisierung der Vorgänge in einem Projekt, sodass Sie die Anforderungen und den Status eines Projekts schnell bewerten können.

![Projektmetriken](assets/project-metrics-full-screen-350x238.png)

Im Bereich Metriken können Sie den Gesamtzustand eines Projekts sowie Folgendes anzeigen:

* Wo Arbeit aktiv oder gestoppt ist
* Wer hat offene Arbeitselemente zugewiesen
* Details zu Aufgaben oder Problemen, die überfällig sind oder kurz vor dem geplanten Abschlussdatum liegen

Sie können auch ein Drilldown in jedes Diagramm durchführen, um Aufgaben oder Probleme in einer bestimmten Kategorie genauer zu untersuchen.

Weitere Informationen zum Untersuchen dieser Aufgaben oder Probleme finden Sie unter [Metrikdetails anzeigen](#view-metrics-details).

<!--
this was deprecated: 
>[!TIP]
>
>To see metrics at a higher level for a group of projects within a program, portfolio, etc., navigate to the Enhanced analytics area.  
>To learn more about Enhanced analytics, see [Enhanced analytics overview](../../../enhanced-analytics/enhanced-analytics-overview.md).
-->

## Projektkennzahlen

Die wichtigsten Leistungsindikatoren (KPIs) werden oben im Bereich „Metriken“ angezeigt.

![Projektmetriken](assets/project-metrics-kpis-350x52.png)

Diese KPIs sind in die folgenden Kategorien unterteilt:

| Abgeschlossene Aufgaben | **Abgeschlossene Aufgaben** zeigt die Anzahl der Aufgaben mit dem Status Abgeschlossen an. Diese Zahl umfasst auch Aufgaben mit einem benutzerdefinierten Status, der „Abgeschlossen“ entspricht. |
|---|---|
| Unvollständige Aufgaben | **Nicht abgeschlossene Aufgaben** zeigt die Anzahl der Aufgaben an, die sich nicht im Status Abgeschlossen oder Geschlossen bzw. einem Status befinden, der Abgeschlossen entspricht. |
| Überfällige Aufgaben | **Überfällige Aufgaben** zeigt die Anzahl der Aufgaben an, die hinter dem geplanten Abschlussdatum liegen und sich nicht im Status Abgeschlossen oder Geschlossen oder in einem Status befinden, der Abgeschlossen oder Geschlossen entspricht. |
| Aufgaben insgesamt | **Aufgaben insgesamt** zeigt die Gesamtzahl der Aufgaben im Projekt an. |

>[!TIP]
>
>Um eine Liste der Arbeitselemente für einen bestimmten KPI anzuzeigen, klicken Sie auf diesen KPI. In dieser Liste können Sie auf ein bestimmtes Arbeitselement klicken, um weitere Details auf einer neuen Registerkarte anzuzeigen.\
>![Abgeschlossene Aufgaben](assets/completed-tasks-dialog-350x75.png)\
>Weitere Informationen finden Sie unter [Metrikdetails anzeigen](#view-metrics-details).

## Balkendiagramm für Aufgaben oder Probleme

In dem Balkendiagramm, das unter den Projekt-KPIs angezeigt wird, können Sie den Status oder die Priorität der Arbeitselemente im Projekt anzeigen. Die Aufgabenansicht ist standardmäßig ausgewählt.

Wenn der Status in diesem Diagramm ausgewählt ist, können Sie alle Status von Aufgaben oder Problemen in einem Projekt anzeigen. Jeder Status wird in einem Balken im Diagramm gruppiert. Alle Standardsystemstatus und benutzerdefinierten Status werden in diesem Diagramm angezeigt.

![Aufgabenproblem nach Status](assets/project-metrics-task-issue-by-status-350x120.png)

Wenn in diesem Diagramm Priorität ausgewählt ist, können Sie alle Prioritäten von Aufgaben oder Problemen in einem Projekt anzeigen.

![Aufgaben und Probleme nach Priorität](assets/project-metrics-task-issue-by-priority-350x121.png)

>[!TIP]
>
>Um eine Liste von Arbeitselementen mit einem bestimmten Status oder einer bestimmten Priorität anzuzeigen, klicken Sie auf einen Balken im Diagramm. In dieser Liste können Sie auf ein bestimmtes Arbeitselement klicken, um weitere Details auf einer neuen Registerkarte anzuzeigen.\
>![Feld „Abgeschlossene Aufgaben“](assets/completed-tasks-dialog-350x75.png)\
>Weitere Informationen finden Sie unter [Metrikdetails anzeigen](#view-metrics-details).

## Ringdiagramm

Das Ringdiagramm, das sich unter den Projekt-KPIs befindet, ermöglicht es Ihnen, das Verhältnis zwischen abgeschlossenen Arbeitselementen und unvollständigen Arbeitselementen in einem Projekt anzuzeigen.

![Aufgaben oder Probleme nach abgeschlossenem Status](assets/tasks-issues-by-complete-status-350x250.png)

Im Dropdown-Menü über dem Diagramm können Sie Folgendes auswählen:

| Alle Aufgaben | Wenn Sie **Aufgaben** auswählen, werden die Gesamtzahl der Aufgaben im Projekt sowie das Verhältnis zwischen abgeschlossenen und unvollständigen Aufgaben angezeigt. |
|---|---|
| Alle Probleme | Wenn Sie **Probleme** auswählen, werden die Gesamtzahl der Probleme im Projekt sowie das Verhältnis zwischen abgeschlossenen und unvollständigen Problemen angezeigt. |

>[!TIP]
>
>Um eine Liste der abgeschlossenen oder unvollständigen Arbeitselemente anzuzeigen, klicken Sie auf diesen Abschnitt im Ringdiagramm. In dieser Liste können Sie auf ein bestimmtes Arbeitselement klicken, um weitere Details auf einer neuen Registerkarte anzuzeigen.\
>![Feld „Abgeschlossene Aufgaben“](assets/completed-tasks-dialog-350x75.png)\
>Weitere Informationen finden Sie unter [Metrikdetails anzeigen](#view-metrics-details).

## Balkendiagramm für Zugewiesene

Das Balkendiagramm Zugewiesene Person zeigt die Anzahl der Aufgaben an, die den einzelnen Personen im Projekt zugewiesen wurden. Diese Zahl variiert je nach der Kategorie, die Sie aus dem Dropdown-Menü auswählen.

![Aufgabe und Probleme nach zugewiesener Person](assets/tasks-issues-by-assignee-350x104.png)

Sie können Aufgabenzuweisungen für ein Projekt in den folgenden Kategorien anzeigen:

| Abgeschlossen | Wenn Sie **Abschließen** auswählen, wird die Anzahl der Aufgaben angezeigt, die den einzelnen abgeschlossenen Benutzern zugewiesen wurden. |
|---|---|
| Unvollständig | Wenn Sie **Unvollständig** auswählen, wird die Anzahl der den einzelnen Benutzenden zugewiesenen Aufgaben angezeigt, die noch nicht abgeschlossen wurden. |
| Bevorstehend | Wenn Sie **Kommend** auswählen, wird die Anzahl der Aufgaben angezeigt, die jedem Benutzer zugewiesen wurden und das geplante Startdatum noch nicht erreicht haben. |
| Überfällig | Wenn Sie **Überfällig** auswählen, wird die Anzahl der Aufgaben angezeigt, die jedem Benutzer zugewiesen wurden und das geplante Abschlussdatum überschreiten und noch nicht abgeschlossen sind. |

>[!TIP]
>
>Um eine Liste der Arbeitselemente in der ausgewählten Kategorie anzuzeigen, die einem bestimmten Benutzer zugewiesen sind, klicken Sie auf den Balken neben dem Namen des Benutzers im Diagramm. In dieser Liste können Sie auf ein bestimmtes Arbeitselement klicken, um weitere Details auf einer neuen Registerkarte anzuzeigen.\
>![Feld „Abgeschlossene Aufgaben“](assets/completed-tasks-dialog-350x75.png)\
>Weitere Informationen finden Sie unter [Metrikdetails anzeigen](#view-metrics-details).

## Anzeigen von Metrikdetails {#view-metrics-details}

Sie können mit den Diagrammen im Bereich Metriken interagieren, um verschiedene Aspekte eines Diagramms anzuzeigen oder die Aufgaben und Probleme innerhalb eines Diagramms genauer zu betrachten.

1. Navigieren Sie zu dem Projekt, für das Sie Metriken anzeigen möchten.
1. Klicken Sie im linken Bedienfeld auf **Metriken**.\
   Die Diagramme im Bereich Metriken zeigen standardmäßig Informationen zu Aufgaben an.\
   ![Abschnitt Metriken](assets/metrics-section-350x298.png)

1. (Bedingt) Wenn in einem Diagramm ein Dropdown-Pfeil angezeigt wird, klicken Sie auf das Symbol **Dropdown-Pfeil** ![Dropdown-Pfeil](assets/dropdown-arrow.png) im Diagramm und wählen Sie die gewünschte Option aus dem Menü aus.\
   Informationen zu den Optionen, die in den Menüs der einzelnen Diagramme angezeigt werden, finden Sie im entsprechenden Abschnitt oben.

1. (Optional) Gehen Sie wie folgt vor, um Aufgaben oder Probleme für eine Metrik auf der Seite genauer zu untersuchen:

   1. Klicken Sie auf das Element, für das Sie Details anzeigen möchten, z. B. Aufgaben, die einem bestimmten Benutzer zugewiesen sind, Probleme mit hoher Priorität oder alle überfälligen Aufgaben.

      Eine Liste mit Aufgaben oder Problemen wird angezeigt.

      ![Feld „Abgeschlossene Aufgaben“](assets/completed-tasks-dialog-350x75.png)

   1. Verwenden Sie die Pfeile unten in der Liste, um die Aufgabe oder das Problem zu finden, die bzw. das Sie überprüfen möchten.

      ODER

      Wählen Sie eine bestimmte Zahl aus, um Aufgaben oder Probleme auf einer bestimmten Seite anzuzeigen.

      ![Paginierung](assets/pagination-300x152.png)

   1. Wählen Sie eine Aufgabe oder ein Problem aus, um weitere Details anzuzeigen.

      Die Aufgabe oder das Problem wird in einer neuen Registerkarte geöffnet.

1. (Optional) Um das Dashboard für Projektmetriken in eine .png-Datei zu exportieren, klicken Sie auf das **Export**-Symbol ![Export-Symbol](assets/export.png) und wählen Sie dann **Als PNG exportieren** aus dem Dropdown-Menü aus.

   >[!TIP]
   >
   >Wenn Sie das Dashboard exportieren, enthält die exportierte Datei nur das, was derzeit in Ihrem Viewport angezeigt wird. Um bestimmte Elemente in die exportierte Datei aufzunehmen, müssen Sie möglicherweise auf der Seite nach oben oder unten scrollen oder die Zoom-Einstellungen Ihres Browsers anpassen.
