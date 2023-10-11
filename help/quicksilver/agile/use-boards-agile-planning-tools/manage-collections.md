---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Workflows verwalten
description: Ein Workstream ist eine konfigurierbare Gruppe von Foren und Karten für die Zusammenarbeit an der Arbeit.
author: Lisa
feature: Agile
exl-id: c46c42e8-e14d-414d-b883-c4d885338e42
source-git-commit: 4e5bff5ad62dce8766072e04e3a2b89371a90f03
workflow-type: tm+mt
source-wordcount: '915'
ht-degree: 2%

---

# Workflows verwalten

>[!IMPORTANT]
>
>Workflows stehen nur einer bestimmten Kundengruppe zur Verfügung.

Ein Workstream ist eine konfigurierbare Gruppe von Foren und Karten für die Zusammenarbeit an der Arbeit. Workflows können verschiedene Arten von Foren enthalten, die aus Vorlagen und einer Liste von Arbeitselementen erstellt wurden. In einem Arbeitsablauf können Sie die Arbeit in Iterationen oder Sprints verfolgen.

Weitere Informationen finden Sie unter [Kartenliste verwenden](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) und [Erstellen einer Iteration in einem Workstream](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

Workflows werden im Dashboard zusammen mit den einzelnen Foren angezeigt, auf die Sie Zugriff haben und die nicht Teil eines Workflows sind. Weitere Informationen zum Dashboard für Pinnwände finden Sie unter [Verwenden des Dashboards-Dashboards](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). Sie können auf einen beliebigen Pinnwandnamen im Dashboard klicken, um ihn zu öffnen.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan*</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Anforderung] oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

## Erstellen eines Workflows

{{step1-to-boards}}

1. Klicks **[!UICONTROL Workflow hinzufügen]** im [!UICONTROL Workflows] Bereich des Dashboards.
1. Geben Sie einen Namen ein, der **[!UICONTROL Unbenannter Workstream]** und drücken Sie die Eingabetaste.

   Sie können dem Workstream Pinnwände hinzufügen oder auf [!UICONTROL **Alle Pinnwände**] zum Dashboard zurückkehren.

## Erstellen einer neuen Pinnwand in einem Workflow

1. Wenn Sie sich noch nicht in einem Workstream befinden, klicken Sie auf [!UICONTROL **Arbeitsablauf anzeigen**] auf dem Dashboard, um einen vorhandenen Workstream zu öffnen.
1. Klicks **[!UICONTROL Pinnwand hinzufügen]** auf [!UICONTROL Pinnwände] -Registerkarte des Workflows.
1. Wählen Sie eine Vorlage für die Pinnwand aus.

| Vorlage | Beschreibung |
|---------|----------|
| Einfache Pinnwand | Auf der Pinnwand werden drei Standardspalten bereitgestellt. Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen. <p>Es werden keine Spaltenrichtlinien angewendet. |
| Kanban-Board | Die folgenden Spalten werden auf der Pinnwand bereitgestellt: &quot;Backlog&quot;, &quot;Neu&quot;, &quot;In Bearbeitung&quot;, &quot;Abgeschlossen&quot;und &quot;Auf Warten&quot;. Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen.<p>Um den Rückstand zu verwenden, müssen Sie Filter für die Ansauspalte einrichten. Weitere Informationen finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Um die Standardrichtlinien für jede Spalte zu überprüfen, klicken Sie auf die [!UICONTROL **Mehr** Menü] in einer Spalte auswählen [!UICONTROL **Bearbeiten**]. Sie können diese voreingestellten Richtlinien ändern. Weitere Informationen finden Sie unter [Pinnwandspalten verwalten](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| Retrospektiv-Board | Die folgenden Spalten werden auf der Pinnwand bereitgestellt: Was ist gut gelaufen? Was könnte verbessert werden? Wer soll gefeiert werden? Wie können wir unsere Verfahren beschleunigen? Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen. <p>Es werden keine Spaltenrichtlinien angewendet. |
| Iterationsprozess | Dies ist die Pinnwand, mit der eine Iteration definiert und ausgeführt wird. <p>Die folgenden Spalten werden auf der Pinnwand bereitgestellt: &quot;Backlog&quot;, &quot;Neu&quot;, &quot;In Bearbeitung&quot;, &quot;Abgeschlossen&quot;und &quot;Auf Warten&quot;. Sie können der Pinnwand keine Spalten hinzufügen. <p>Um die Standardrichtlinien für jede Spalte zu überprüfen, klicken Sie auf die [!UICONTROL **Mehr**] in einer Spalte auswählen [!UICONTROL **Bearbeiten**]. Sie können diese voreingestellten Richtlinien ändern. Weitere Informationen finden Sie unter [Pinnwandspalten verwalten](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

Weitere Informationen zum Einrichten der Pinnwand finden Sie unter [Pinnwand erstellen oder bearbeiten](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Filtern der Liste der Foren in einem Workstream

Wenn auf die Pinnwand andere Filter als die Standardfilter angewendet werden, wird auf dem Filtersymbol ein Indikator angezeigt ![Filter angewendet](assets/boards-filterapplied-30x30.png). Klicks [!UICONTROL **Alle löschen**] , um alle Filter zu entfernen, und klicken Sie auf [!UICONTROL **Filter ausblenden**] , um den Filterbereich zu schließen.

{{step1-to-boards}}

1. Klicken Sie im Dashboard auf [!UICONTROL **Arbeitsablauf anzeigen**] , um einen Workflow zu öffnen.
1. Klicken Sie auf [!UICONTROL **Pinnwände**] hinzufügen, wenn sie noch nicht angezeigt wurde.
1. Klicks [!UICONTROL **Filter**].
1. Wählen Sie die Pinnwände aus, die Sie nach Status anzeigen möchten (archivierte Pinnwände, aktive Pinnwände oder alle Pinnwände).
1. Wählen Sie die Pinnwände aus, die nach Vorlage angezeigt werden sollen.

## Hinzufügen von Mitgliedern zu Workflows

Personen und Teams müssen als Mitglieder zum Workstream hinzugefügt werden, bevor sie den Workflow und dessen Inhalt anzeigen können. Ein Workstream-Mitglied kann Mitglieder zum Workstream hinzufügen und daraus entfernen und sehen, welche Pinnwände sich im Workstream befinden.

>[!NOTE]
>
>Workstream-Mitglieder können eine Pinnwand erst dann in einem Workstream öffnen, wenn sie dieser Pinnwand als Mitglied hinzugefügt werden.

{{step1-to-boards}}

1. Klicken Sie im Dashboard auf [!UICONTROL **Arbeitsablauf anzeigen**] , um einen Workflow zu öffnen.
1. Klicken Sie auf **[!UICONTROL Mitglied hinzufügen]** icon ![Mitglieder hinzufügen](assets/boards-addmember-spectrum-25x25.png) , um Mitglieder und Teams zum Workflow hinzuzufügen.

   Dies entspricht dem Hinzufügen von Mitgliedern zu einer Pinnwand. Weitere Informationen finden Sie unter [Hinzufügen oder Entfernen von Mitgliedern aus einer Pinnwand](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

## Hinzufügen von Quellen zu Workflows

Eine Quelle bestimmt, woher die Karten im Workstream stammen.

{{step1-to-boards}}

1. Klicken Sie auf [!UICONTROL **Quellen**] icon ![Quellen-Symbol](assets/sources-icon.png) , um eine Quelle zum Importieren von Karten in den Workflow zu definieren. Derzeit ist die einzige verfügbare Quelle [!DNL Adobe Workfront].
1. Fügen Sie Filter hinzu, um Aufgaben und Probleme aus Workfront als Karten zu importieren.

   Das Hinzufügen von Filtern für Workstream-Quellen entspricht dem Hinzufügen erweiterter Filter für eine Ansaugspalte auf einer Basis-Pinnwand oder Kanban-Pinnwand. Weitere Informationen finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Konfigurieren eines Workflows

{{step1-to-boards}}

1. Klicken Sie im Dashboard auf [!UICONTROL **Arbeitsablauf anzeigen**] , um einen Workflow zu öffnen.
1. Klicks [!UICONTROL **Konfigurieren**] , um die [!UICONTROL Konfigurieren von Workstream] Bedienfeld.
1. (Optional) Erweitern [!UICONTROL **Workstream**] und geben Sie eine Beschreibung des Workflows ein. Diese Beschreibung wird im Dashboard angezeigt.
1. (Optional) Erweitern [!UICONTROL **Iterationen**] , um einen Iterationsvorgang für diesen Workstream zu definieren.

   Die Gesamtanzahl der Karten, die Anzahl der spitze Karten und die Anzahl der Iterationen werden im Bereich Kartenliste angezeigt. Klicks [!UICONTROL **Liste anzeigen**] , um die Liste zu öffnen und Karten hinzuzufügen. Weitere Informationen finden Sie unter [Kartenliste verwenden](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   Wenn bereits eine Iteration definiert wurde, werden ihr Startdatum, die Anzahl der Karten und die Anzahl der Punkte angezeigt. Klicks [!UICONTROL **Pinnwand anzeigen**] , um die Iterationskarte zu öffnen. Weitere Informationen finden Sie unter [Erstellen einer Iteration in einem Workstream](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. (Optional) Erweitern [!UICONTROL **Tags**] , um Tags zum Workflow hinzuzufügen. Suchen Sie nach einem Tag oder geben Sie einen neuen Tag-Namen in das Suchfeld ein und drücken Sie die Eingabetaste , um es zu erstellen.
