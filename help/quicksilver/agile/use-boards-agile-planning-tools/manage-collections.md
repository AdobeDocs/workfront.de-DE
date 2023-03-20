---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Workflows verwalten
description: Ein Workstream ist eine konfigurierbare Gruppe von Foren und Karten für die Zusammenarbeit an der Arbeit.
author: Lisa
feature: Agile
source-git-commit: 16e96d55932116cb475eecbe8b6ebfd4661eb494
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 2%

---

# Workflows verwalten

{{highlighted-preview}}

>[!NOTE]
>
>Workflows sind in der Vorschau-Umgebung und in der Produktion über die frühe Funktion verfügbar, für die [!UICONTROL [!DNL Workfront] Pinnwände]. Weitere Informationen finden Sie unter [Vorabauswahl für Funktionen für Adobe Workfront-Pinnwände](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

Ein Workstream ist eine konfigurierbare Gruppe von Foren und Karten für die Zusammenarbeit an der Arbeit. Workflows können verschiedene Arten von Pinnwänden enthalten, die aus Vorlagen erstellt werden. <span class="preview">und eine Kartenliste mit Arbeitselementen. In einem Arbeitsablauf können Sie die Arbeit in Iterationen oder Sprints verfolgen.</span>

<span class="preview">Weitere Informationen finden Sie unter [Kartenliste verwenden](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) und [Iteration erstellen](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md).</span>

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

1. Klicken **[!UICONTROL Workflow hinzufügen]** im [!UICONTROL Workflows] Bereich des Dashboards.
1. Geben Sie einen Namen ein, der ersetzt werden soll **[!UICONTROL Unbenannter Workstream]** und drücken Sie die Eingabetaste.

   Sie können dem Workstream Pinnwände hinzufügen oder auf [!UICONTROL **Alle Pinnwände**] , um zum Dashboard zurückzukehren.

## Erstellen einer neuen Pinnwand in einem Workflow

1. Wenn Sie sich noch nicht in einem Workstream befinden, klicken Sie auf [!UICONTROL **Workflow anzeigen**] auf dem Dashboard, um einen vorhandenen Workstream zu öffnen.
1. Klicken **[!UICONTROL Pinnwand hinzufügen]** auf [!UICONTROL Pinnwände] -Registerkarte des Workflows.
1. Wählen Sie eine Vorlage für die Pinnwand aus.

| Vorlage | Beschreibung |
|---------|----------|
| Einfache Pinnwand | Auf der Pinnwand werden drei Standardspalten bereitgestellt. Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen. <p>Es werden keine Spaltenrichtlinien angewendet. |
| Kanban-Board | Die folgenden Spalten werden auf der Pinnwand bereitgestellt: Rückstau, Neu, In Bearbeitung, Abgeschlossen und Auf Warten. Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen.<p>Um den Rückstand zu verwenden, müssen Sie Filter für die Ansauspalte einrichten. Weitere Informationen finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Um die Standardrichtlinien für jede Spalte zu überprüfen, klicken Sie auf die [!UICONTROL **Mehr** Menü] in einer Spalte und wählen Sie [!UICONTROL **Bearbeiten**]. Sie können diese voreingestellten Richtlinien ändern. Weitere Informationen finden Sie unter [Pinnwandspalten verwalten](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| Rückblickende Pinnwand | Die folgenden Spalten werden auf der Pinnwand bereitgestellt: Was ist gut gelaufen? Was könnte verbessert werden? Wer soll gefeiert werden? Wie können wir unsere Verfahren beschleunigen? Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen. <p>Es werden keine Spaltenrichtlinien angewendet. |
| <span class="preview">Iteration</span> | <span class="preview">Dies ist die Pinnwand, mit der eine Iteration definiert und ausgeführt wird. <p>Die folgenden Spalten werden auf der Pinnwand bereitgestellt: Rückstau, Neu, In Bearbeitung, Abgeschlossen und Auf Warten. Sie können der Pinnwand keine Spalten hinzufügen. <p>Um die Standardrichtlinien für jede Spalte zu überprüfen, klicken Sie auf die [!UICONTROL **Mehr**] in einer Spalte auswählen [!UICONTROL **Bearbeiten**]. Sie können diese voreingestellten Richtlinien ändern. Weitere Informationen finden Sie unter [Pinnwandspalten verwalten](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).</span> |

Weitere Informationen zum Einrichten der Pinnwand finden Sie unter [Pinnwand erstellen oder bearbeiten](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Filtern der Liste der Foren in einem Workstream

Wenn auf die Pinnwand andere Filter als die Standardfilter angewendet werden, wird auf dem Filtersymbol ein Indikator angezeigt ![Filter angewendet](assets/boards-filterapplied-30x30.png). Klicken [!UICONTROL **Alle löschen**] , um alle Filter zu entfernen, und klicken Sie auf [!UICONTROL **Filter ausblenden**] , um den Filterbereich zu schließen.

{{step1-to-boards}}

1. Klicken Sie im Dashboard auf [!UICONTROL **Workflow anzeigen**] , um einen Workflow zu öffnen.
1. Klicken Sie auf [!UICONTROL **Pinnwände**] hinzufügen, wenn sie noch nicht angezeigt wurde.
1. Klicken [!UICONTROL **Filter**].
1. Wählen Sie die Pinnwände aus, die Sie nach Status anzeigen möchten (archivierte Pinnwände, aktive Pinnwände oder alle Pinnwände).
1. Wählen Sie die Pinnwände aus, die nach Vorlage angezeigt werden sollen.

## Hinzufügen von Mitgliedern zu Workflows

Personen und Teams müssen als Mitglieder zum Workstream hinzugefügt werden, bevor sie den Workflow und dessen Inhalt anzeigen können. Ein Workstream-Mitglied kann Mitglieder zum Workstream hinzufügen und daraus entfernen und sehen, welche Pinnwände sich im Workstream befinden.

>[!NOTE]
>
>Workstream-Mitglieder können eine Pinnwand erst dann in einem Workstream öffnen, wenn sie dieser Pinnwand als Mitglied hinzugefügt werden.

{{step1-to-boards}}

1. Klicken Sie im Dashboard auf [!UICONTROL **Workflow anzeigen**] , um einen Workflow zu öffnen.
1. Klicken Sie auf **[!UICONTROL Mitglied hinzufügen]** icon ![Mitglieder hinzufügen](assets/boards-addmember-spectrum-25x25.png) , um Mitglieder und Teams zum Workflow hinzuzufügen.

   Dies entspricht dem Hinzufügen von Mitgliedern zu einer Pinnwand. Weitere Informationen finden Sie unter [Hinzufügen oder Entfernen von Mitgliedern aus einer Pinnwand](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

<div class="preview">

## Konfigurieren eines Workflows

{{step1-to-boards}}

1. Klicken Sie im Dashboard auf [!UICONTROL **Workflow anzeigen**] , um einen Workflow zu öffnen.
1. Klicken [!UICONTROL **Konfigurieren**] , um [!UICONTROL Workstream konfigurieren] Bereich.
1. (Optional) Geben Sie eine Beschreibung des Workflows ein. Diese Beschreibung wird im Dashboard angezeigt.

   Die Gesamtanzahl der Karten, die Anzahl der spitze Karten und die Anzahl der Iterationen werden im Bereich Kartenliste angezeigt. Klicken [!UICONTROL **Liste anzeigen**] , um die Liste zu öffnen und Karten hinzuzufügen. Weitere Informationen finden Sie unter [Kartenliste verwenden](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   Wenn eine Iteration definiert wurde, werden ihr Startdatum, die Anzahl der Karten und die Anzahl der Punkte angezeigt. Klicken [!UICONTROL **Iterationskarte anzeigen**] , um die Pinnwand zu öffnen. Weitere Informationen finden Sie unter [Iteration erstellen](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration.md).

1. Klicken [!UICONTROL **Quelle hinzufügen**] , um eine Quelle zum Importieren von Karten in den Workflow zu definieren. Derzeit ist die einzige verfügbare Quelle [!DNL Adobe Workfront].
1. Fügen Sie Filter hinzu, um Aufgaben und Probleme aus Workfront als Karten zu importieren.

   Das Hinzufügen von Filtern für Workstream-Quellen entspricht dem Hinzufügen von Filtern für eine Ansaugspalte auf einer Basis-Pinnwand oder Kanban-Pinnwand. Weitere Informationen finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

</div>
