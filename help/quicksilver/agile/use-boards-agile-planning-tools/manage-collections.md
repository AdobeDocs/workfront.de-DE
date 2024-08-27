---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Verwalten von Workflows
description: Ein Workstream ist eine konfigurierbare Gruppe von Foren und Karten für die Zusammenarbeit an der Arbeit.
author: Lisa
feature: Agile
exl-id: c46c42e8-e14d-414d-b883-c4d885338e42
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 1%

---

# Workflows verwalten

>[!IMPORTANT]
>
>Workflows stehen nur einer bestimmten Kundengruppe zur Verfügung.

Ein Workstream ist eine konfigurierbare Gruppe von Foren und Karten für die Zusammenarbeit an der Arbeit. Workflows können verschiedene Arten von Foren enthalten, die aus Vorlagen und einer Liste von Arbeitselementen erstellt wurden. In einem Arbeitsablauf können Sie die Arbeit in Iterationen oder Sprints verfolgen.

Weitere Informationen finden Sie unter [Verwenden der Kartenliste](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) und [Erstellen einer Iteration in einem Workstream](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

Workflows werden im Dashboard zusammen mit den einzelnen Foren angezeigt, auf die Sie Zugriff haben und die nicht Teil eines Workflows sind. Weitere Informationen zum Dashboard für Pinnwände finden Sie unter [Verwenden des Dashboards für Pinnwände](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). Sie können auf einen beliebigen Pinnwandnamen im Dashboard klicken, um ihn zu öffnen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> 
   <p>Neu: [!UICONTROL Contributor] oder höher</p> 
   <p>oder</p>
   <p>Aktuell: [!UICONTROL Anforderung] oder höher</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen eines Workflows

{{step1-to-boards}}

1. Klicken Sie im Bereich [!UICONTROL Workflows] des Dashboards auf **[!UICONTROL Workflow hinzufügen]** .
1. Geben Sie einen Namen ein, um **[!UICONTROL Unbenannter Workstream]** zu ersetzen, und drücken Sie die Eingabetaste.

   Sie können dem Workstream Pinnwände hinzufügen oder auf [!UICONTROL **Alle Pinnwände**] klicken, um zum Dashboard zurückzukehren.

## Erstellen einer neuen Pinnwand in einem Workflow

1. Wenn Sie sich noch nicht in einem Workstream befinden, klicken Sie im Dashboard auf [!UICONTROL **Workflow anzeigen**] , um einen vorhandenen Workstream zu öffnen.
1. Klicken Sie auf der Registerkarte [!UICONTROL Pinnwände] des Workflows auf **[!UICONTROL Pinnwand hinzufügen]** .
1. Wählen Sie eine Vorlage für die Pinnwand aus.

| Vorlage | Beschreibung |
|---------|----------|
| Einfache Pinnwand | Auf der Pinnwand werden drei Standardspalten bereitgestellt. Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen. <p>Es werden keine Spaltenrichtlinien angewendet. |
| Kanban-Board | Die folgenden Spalten werden auf der Pinnwand bereitgestellt: &quot;Backlog&quot;, &quot;Neu&quot;, &quot;In Bearbeitung&quot;, &quot;Abgeschlossen&quot;und &quot;Auf Warten&quot;. Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen.<p>Um den Rückstand zu verwenden, müssen Sie Filter für die Ansauspalte einrichten. Weitere Informationen finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Um die Standardrichtlinien für jede Spalte zu überprüfen, klicken Sie auf das Menü [!UICONTROL **Mehr**] in einer Spalte und wählen Sie [!UICONTROL **Bearbeiten**] aus. Sie können diese voreingestellten Richtlinien ändern. Weitere Informationen finden Sie unter [Pinnwandspalten verwalten](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| Retrospektiv-Board | Die folgenden Spalten werden auf der Pinnwand bereitgestellt: Was ist gut gelaufen? Was könnte verbessert werden? Wen sollten wir feiern? Was können wir tun, um schneller zu handeln? Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen. <p>Es werden keine Spaltenrichtlinien angewendet. |
| Iterationsprozess | Dies ist die Pinnwand, mit der eine Iteration definiert und ausgeführt wird. <p>Die folgenden Spalten werden auf der Pinnwand bereitgestellt: &quot;Backlog&quot;, &quot;Neu&quot;, &quot;In Bearbeitung&quot;, &quot;Abgeschlossen&quot;und &quot;Auf Warten&quot;. Sie können der Pinnwand keine Spalten hinzufügen. <p>Um die Standardrichtlinien für jede Spalte zu überprüfen, klicken Sie auf das Menü [!UICONTROL **Mehr**] in einer Spalte und wählen Sie [!UICONTROL **Bearbeiten**] aus. Sie können diese voreingestellten Richtlinien ändern. Weitere Informationen finden Sie unter [Pinnwandspalten verwalten](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

Weitere Informationen zum Einrichten der Pinnwand finden Sie unter [Erstellen oder Bearbeiten einer Pinnwand](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Filtern der Liste der Foren in einem Workstream

Wenn andere Filter als die Standardfilter auf die Pinnwandliste angewendet werden, wird auf dem Filtersymbol ![Angewendeter Filter](assets/boards-filterapplied-30x30.png) ein Indikator angezeigt. Klicken Sie auf [!UICONTROL **Alle löschen**] , um alle Filter zu entfernen, und klicken Sie auf [!UICONTROL **Filter ausblenden**] , um den Filterbereich zu schließen.

{{step1-to-boards}}

1. Klicken Sie im Dashboard auf [!UICONTROL **Workflow-Stream anzeigen**] , um einen Workflow zu öffnen.
1. Klicken Sie auf die Registerkarte [!UICONTROL **Pinnwände**] , falls sie noch nicht angezeigt wird.
1. Klicken Sie auf [!UICONTROL **Filter**].
1. Wählen Sie die Pinnwände aus, die Sie nach Status anzeigen möchten (archivierte Pinnwände, aktive Pinnwände oder alle Pinnwände).
1. Wählen Sie die Pinnwände aus, die nach Vorlage angezeigt werden sollen.

## Hinzufügen von Mitgliedern zu Workflows

Personen und Teams müssen als Mitglieder zum Workstream hinzugefügt werden, bevor sie den Workflow und dessen Inhalt anzeigen können. Ein Workstream-Mitglied kann Mitglieder zum Workstream hinzufügen und daraus entfernen und sehen, welche Pinnwände sich im Workstream befinden.

>[!NOTE]
>
>Workstream-Mitglieder können eine Pinnwand erst dann in einem Workstream öffnen, wenn sie dieser Pinnwand als Mitglied hinzugefügt werden.

{{step1-to-boards}}

1. Klicken Sie im Dashboard auf [!UICONTROL **Workflow-Stream anzeigen**] , um einen Workflow zu öffnen.
1. Klicken Sie auf das Symbol **[!UICONTROL Mitglied hinzufügen]** ![Mitglieder hinzufügen](assets/boards-addmember-spectrum-25x25.png) , um Mitglieder und Teams zum Workstream hinzuzufügen.

   Dies entspricht dem Hinzufügen von Mitgliedern zu einer Pinnwand. Weitere Informationen finden Sie unter [Hinzufügen oder Entfernen von Mitgliedern aus einer Pinnwand](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

## Hinzufügen von Quellen zu Workflows

Eine Quelle bestimmt, woher die Karten im Workstream stammen.

{{step1-to-boards}}

1. Klicken Sie auf das Symbol [!UICONTROL **Quellen**] ![Quellen](assets/sources-icon.png) , um eine Quelle zum Importieren von Karten in den Workstream zu definieren. Derzeit ist die einzige verfügbare Quelle [!DNL Adobe Workfront].
1. Fügen Sie Filter hinzu, um Aufgaben und Probleme aus Workfront als Karten zu importieren.

   Das Hinzufügen von Filtern für Workstream-Quellen entspricht dem Hinzufügen erweiterter Filter für eine Ansaugspalte auf einer Basis-Pinnwand oder Kanban-Pinnwand. Weitere Informationen finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Konfigurieren eines Workflows

{{step1-to-boards}}

1. Klicken Sie im Dashboard auf [!UICONTROL **Workflow-Stream anzeigen**] , um einen Workflow zu öffnen.
1. Klicken Sie auf [!UICONTROL **Konfigurieren**] , um den Bereich [!UICONTROL Konfigurieren von Workstream] zu öffnen.
1. (Optional) Erweitern Sie [!UICONTROL **Workstream**] und geben Sie eine Beschreibung des Workflows ein. Diese Beschreibung wird im Dashboard angezeigt.
1. (Optional) Erweitern Sie [!UICONTROL **Iterationen**] , um einen Iterationsvorgang für diesen Workstream zu definieren.

   Die Gesamtanzahl der Karten, die Anzahl der spitze Karten und die Anzahl der Iterationen werden im Bereich Kartenliste angezeigt. Klicken Sie auf [!UICONTROL **Liste anzeigen**] , um die Liste zu öffnen und Karten hinzuzufügen. Weitere Informationen finden Sie unter [Verwenden der Kartenliste](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   Wenn bereits eine Iteration definiert wurde, werden ihr Startdatum, die Anzahl der Karten und die Anzahl der Punkte angezeigt. Klicken Sie auf [!UICONTROL **Pinnwand anzeigen**] , um die Pinnwand zu öffnen. Weitere Informationen finden Sie unter [Erstellen einer Iteration in einem Workstream](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. (Optional) Erweitern Sie [!UICONTROL **Tags**] , um Tags zum Workstream hinzuzufügen. Suchen Sie nach einem Tag oder geben Sie einen neuen Tag-Namen in das Suchfeld ein und drücken Sie die Eingabetaste , um es zu erstellen.
