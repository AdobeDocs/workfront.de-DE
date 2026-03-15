---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Workflows verwalten
description: Ein Arbeitsablauf ist eine konfigurierbare Gruppe von Boards und Karten für die Zusammenarbeit an der Arbeit.
author: Courtney
feature: Agile
exl-id: c46c42e8-e14d-414d-b883-c4d885338e42
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 5%

---

# Verwalten von Arbeitsabläufen

>[!IMPORTANT]
>
>Arbeitsabläufe stehen nur einer bestimmten Kundengruppe zur Verfügung.

Ein Arbeitsablauf ist eine konfigurierbare Gruppe von Pinnwänden und Karten für die Zusammenarbeit bei der Arbeit. Workflows können verschiedene Arten von Boards enthalten, die aus Vorlagen und einer Kartenliste von Arbeitsaufgaben erstellt wurden. In einem Workstream können Sie die Arbeit in Iterationen oder Sprints nachverfolgen.

Weitere Informationen finden Sie unter [Verwenden der Kartenliste](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) und [Erstellen einer Iteration in einem Workstream](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

Workflows werden im Dashboard zusammen mit einzelnen Boards angezeigt, auf die Sie Zugriff haben und die nicht Teil eines Workflows sind. Weitere Informationen zum Dashboard für Dashboards finden Sie unter [Dashboard für Dashboards verwenden](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). Sie können auf einen beliebigen Boardnamen im Dashboard klicken, um es zu öffnen.

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
   <td> 
   <p>Mitwirkende oder höher</p> 
   <p>Anfragende oder höher</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen eines Arbeitsablaufs

{{step1-to-boards}}

1. Klicken Sie **** Dashboard im Bereich [!UICONTROL Arbeitsabläufe] auf „Arbeitsablauf hinzufügen“.
1. Geben Sie einen Namen ein, um **[!UICONTROL Unbenannter Workstream]** zu ersetzen, und drücken Sie die Eingabetaste.

   Sie können Boards zum Arbeitsablauf hinzufügen oder auf [!UICONTROL **Alle Boards**] klicken, um zum Dashboard zurückzukehren.

## Erstellen eines neuen Boards in einem Workstream

1. Wenn Sie sich noch nicht in einem Workstream befinden, klicken Sie im Dashboard auf [!UICONTROL **Workstream anzeigen**], um einen vorhandenen Workstream zu öffnen.
1. Klicken Sie auf der Registerkarte **[!UICONTROL Boards]** des Workflows auf [!UICONTROL Board hinzufügen].
1. Wählen Sie eine Vorlage für die Pinnwand aus.

| Vorlage | Beschreibung |
|---------|----------|
| Einfache Pinnwand | Auf der Platine sind drei Standardspalten vorhanden. Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen. <p>Es werden keine Spaltenrichtlinien angewendet. |
| Kanban-Board | Die folgenden Spalten werden auf dem Board bereitgestellt: Rückstand, Neu, In Bearbeitung, Vollständig und Gesperrt. Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen.<p>Um den Rückstand zu nutzen, müssen Sie Filter für die Ansaugspalte einrichten. Weitere Informationen finden Sie unter [Hinzufügen einer Einzugsspalte zu einem Board](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Um die Standardrichtlinien für jede Spalte zu überprüfen, klicken Sie in einer Spalte auf das Menü [!UICONTROL **Mehr**] und wählen Sie [!UICONTROL **Bearbeiten**] aus. Sie können diese voreingestellten Richtlinien ändern. Weitere Informationen finden Sie unter [Mainboard-Spalten verwalten](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| Retrospektiv-Board | Die folgenden Spalten sind auf der Pinnwand vorhanden: Was ist gut gelaufen? Was könnte verbessert werden? Wen sollen wir feiern? Was können wir tun, um uns schneller zu bewegen? Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen. <p>Es werden keine Spaltenrichtlinien angewendet. |
| Iterationsprozess | Dies ist das Board, das zum Definieren und Ausführen einer Iteration verwendet wird. <p>Die folgenden Spalten werden auf dem Board bereitgestellt: Rückstand, Neu, In Bearbeitung, Vollständig und Gesperrt. Sie können der Pinnwand keine Spalten hinzufügen. <p>Um die Standardrichtlinien für jede Spalte zu überprüfen, klicken Sie auf das Menü [!UICONTROL **Mehr**] in einer Spalte und wählen Sie [!UICONTROL **Bearbeiten**] aus. Sie können jede dieser voreingestellten Richtlinien ändern. Weitere Informationen finden Sie unter [Pinnwand-Spalten verwalten](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

Weitere Informationen zum Einrichten der Pinnwand finden Sie unter [Erstellen oder Bearbeiten einer Pinnwand](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Filtern der Liste von Pinnwänden in einem Arbeitsablauf

Wenn in der Board-Liste andere Filter als die Standardfilter angewendet werden, wird ein Indikator auf dem Filtersymbol ![Filter angewendet](assets/boards-filterapplied-30x30.png) angezeigt. Klicken Sie auf [!UICONTROL **Alle löschen**], um alle Filter zu entfernen, und klicken Sie auf [!UICONTROL **Filter ausblenden**], um das Filterfenster zu schließen.

{{step1-to-boards}}

1. Klicken Sie im Dashboard auf [!UICONTROL **Workstream anzeigen**], um einen Workstream zu öffnen.
1. Klicken Sie auf die Registerkarte [!UICONTROL **Boards**], wenn sie noch nicht angezeigt wird.
1. Klicken Sie auf [!UICONTROL **Filter**].
1. Wählen Sie die Boards aus, die nach Status angezeigt werden sollen (archivierte Boards, aktive Boards oder alle Boards).
1. Wählen Sie die Pinnwände aus, die nach Vorlage angezeigt werden sollen.

## Mitglieder zu einem Arbeitsablauf hinzufügen

Personen und Teams müssen dem Arbeitsablauf als Mitglieder hinzugefügt werden, bevor sie den Arbeitsablauf und seine Inhalte anzeigen können. Ein Workstream-Mitglied kann Mitglieder zum Workstream hinzufügen und entfernen und sehen, welche Boards sich im Workstream befinden.

>[!NOTE]
>
>Ein Workstream-Mitglied kann ein Board in einem Workstream erst öffnen, wenn es dem betreffenden Board als Mitglied hinzugefügt wurde.

{{step1-to-boards}}

1. Klicken Sie im Dashboard auf [!UICONTROL **Workstream anzeigen**], um einen Workstream zu öffnen.
1. Klicken Sie auf das Symbol **[!UICONTROL Mitglied hinzufügen]** ![Mitglieder hinzufügen](assets/boards-addmember-spectrum-25x25.png), um dem Arbeitsablauf Mitglieder und Teams hinzuzufügen.

   Dies ist der gleiche Vorgang wie das Hinzufügen von Mitgliedern zu einem Board. Weitere Informationen finden Sie unter [Mitglieder zu einem Board hinzufügen oder daraus entfernen](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

## Hinzufügen von Quellen zu einem Arbeitsablauf

Eine Quelle bestimmt, woher die Karten im Arbeitsablauf kommen.

{{step1-to-boards}}

1. Klicken Sie auf das [!UICONTROL **Quellen**]-Symbol ![Quellen-Symbol](assets/sources-icon.png), um eine Quelle zum Importieren von Karten in den Arbeitsablauf zu definieren. Zu diesem Zeitpunkt ist die einzige verfügbare Quelle [!DNL Adobe Workfront].
1. Fügen Sie Filter hinzu, um Aufgaben und Probleme aus Workfront als Karten zu importieren.

   Das Hinzufügen von Filtern für Workstream-Quellen entspricht dem Hinzufügen von erweiterten Filtern für eine Aufnahmesäule auf einem Basis-Board oder Kanban-Board. Weitere Informationen finden Sie unter [Hinzufügen einer Einzugsspalte zu einem Board](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Konfigurieren eines Workflows

{{step1-to-boards}}

1. Klicken Sie im Dashboard auf [!UICONTROL **Workstream anzeigen**], um einen Workstream zu öffnen.
1. Klicken Sie auf [!UICONTROL **Konfigurieren**], um den Bereich [!UICONTROL Workstream konfigurieren] zu öffnen.
1. (Optional) Erweitern Sie [!UICONTROL **Workstream**] und geben Sie eine Beschreibung des Workflows ein. Diese Beschreibung wird im Dashboard angezeigt.
1. (Optional) Erweitern Sie [!UICONTROL **Iterationen**], um einen Iterationsprozess für diesen Workstream zu definieren.

   Die Gesamtanzahl der Karten, die Anzahl der Karten, auf die verwiesen wird, und die Anzahl der Iterationen werden im Abschnitt &quot;Kartenliste&quot; angezeigt. Klicken Sie auf [!UICONTROL **Liste anzeigen**], um die Liste zu öffnen und Karten hinzuzufügen. Weitere Informationen finden Sie unter [Kartenliste verwenden](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   Wenn eine Iteration bereits definiert wurde, werden ihr Startdatum, die Anzahl der Karten und die Anzahl der Punkte angezeigt. Klicken Sie auf [!UICONTROL **Pinnwand anzeigen**], um die Iterationsplatine zu öffnen. Weitere Informationen finden Sie unter [Erstellen einer Iteration in einem Arbeitsablauf](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. (Optional) Erweitern Sie [!UICONTROL **Tags**], um dem Arbeitsablauf Tags hinzuzufügen. Suchen Sie nach einem Tag oder geben Sie einen neuen Tag-Namen in das Suchfeld ein und drücken Sie die Eingabetaste , um es zu erstellen.
