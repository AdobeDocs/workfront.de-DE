---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: Arbeitsabläufe verwalten
description: Ein Arbeitsablauf ist eine konfigurierbare Gruppe von Pinnwänden und Karten für die Zusammenarbeit bei der Arbeit.
author: Lisa
feature: Agile
exl-id: c46c42e8-e14d-414d-b883-c4d885338e42
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '947'
ht-degree: 1%

---

# Arbeitsabläufe verwalten

>[!IMPORTANT]
>
>Arbeitsabläufe stehen nur einer bestimmten Kundengruppe zur Verfügung.

Ein Arbeitsablauf ist eine konfigurierbare Gruppe von Pinnwänden und Karten für die Zusammenarbeit bei der Arbeit. Arbeitsabläufe können verschiedene Arten von Pinnwänden enthalten, die aus Vorlagen und einer Liste von Arbeitsaufgaben erstellt wurden. In einem Arbeitsablauf können Sie Arbeiten in Iterationen oder Sprints verfolgen.

Weitere Informationen finden Sie unter [Verwenden der Kartenliste](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) und [Erstellen einer Iteration in einem Arbeitsablauf](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

Im Dashboard werden Arbeitsabläufe zusammen mit einzelnen Boards angezeigt, auf die Sie Zugriff haben und die nicht Teil eines Arbeitsablaufs sind. Weitere Informationen zum Dashboard „Pinnwände“ finden Sie unter [Verwenden des Dashboards](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). Sie können auf einen beliebigen Pinnwand-Namen im Dashboard klicken, um ihn zu öffnen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td> 
   <p>Neu: [!UICONTROL Contributor] oder höher</p> 
   <p>oder</p>
   <p>Aktuell: [!UICONTROL-Anfrage] oder höher</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen eines Arbeitsablaufs

{{step1-to-boards}}

1. Klicken Sie **** Dashboard im Bereich [!UICONTROL Arbeitsabläufe] auf „Arbeitsablauf hinzufügen“.
1. Geben Sie einen Namen ein, der ersetzt werden soll **[!UICONTROL Nicht benannter Arbeitsablauf]** und drücken Sie die Eingabetaste.

   Sie können dem Arbeitsablauf Pinnwände hinzufügen oder auf &quot;[!UICONTROL **Pinnwände“**], um zum Dashboard zurückzukehren.

## Erstellen einer neuen Pinnwand in einem Arbeitsablauf

1. Wenn Sie sich noch nicht in einem Arbeitsablauf befinden, klicken Sie auf [!UICONTROL **Arbeitsablauf anzeigen**], um einen vorhandenen Arbeitsablauf zu öffnen.
1. Klicken **[!UICONTROL auf]** Registerkarte [!UICONTROL Pinnwände] des Arbeitsablaufs.
1. Wählen Sie eine Vorlage für die Pinnwand aus.

| Vorlage | Beschreibung |
|---------|----------|
| Einfache Pinnwand | Auf der Pinnwand werden drei Standardspalten bereitgestellt. Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen. <p>Es werden keine Spaltenrichtlinien angewendet. |
| Kanban-Board | Auf der Pinnwand werden die folgenden Spalten bereitgestellt: Auftragsbestand, Neu, In Bearbeitung, Abgeschlossen und Halten. Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen.<p>Um den Rückstand zu verwenden, müssen Sie Filter für die Aufnahmespalte einrichten. Weitere Informationen finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>Um die Standardrichtlinien für jede Spalte zu überprüfen, klicken Sie auf das Menü [!UICONTROL **Mehr** ] in einer Spalte und wählen Sie [!UICONTROL **Bearbeiten**] aus. Sie können jede dieser voreingestellten Richtlinien ändern. Weitere Informationen finden Sie unter [Pinnwand-Spalten verwalten](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| Retrospektiv-Board | Die folgenden Spalten sind auf der Pinnwand vorhanden: Was ist gut gelaufen? Was könnte verbessert werden? Wen sollen wir feiern? Was können wir tun, um schneller voranzukommen? Sie können neue Spalten hinzufügen und die Standardspalten umbenennen oder löschen. <p>Es werden keine Spaltenrichtlinien angewendet. |
| Iterationsprozess | Dies ist die Pinnwand zum Definieren und Ausführen einer Iteration. <p>Auf der Pinnwand werden die folgenden Spalten bereitgestellt: Auftragsbestand, Neu, In Bearbeitung, Abgeschlossen und Halten. Sie können der Pinnwand keine Spalten hinzufügen. <p>Um die Standardrichtlinien für jede Spalte zu überprüfen, klicken Sie auf das Menü [!UICONTROL **Mehr**] in einer Spalte und wählen Sie [!UICONTROL **Bearbeiten**] aus. Sie können jede dieser voreingestellten Richtlinien ändern. Weitere Informationen finden Sie unter [Pinnwand-Spalten verwalten](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

Weitere Informationen zum Einrichten der Pinnwand finden Sie unter [Erstellen oder Bearbeiten einer Pinnwand](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## Filtern der Liste von Pinnwänden in einem Arbeitsablauf

Wenn andere Filter als die Standardwerte auf der Pinnwand-Liste angewendet werden, wird eine Anzeige auf dem Filtersymbol ![Filter angewendet](assets/boards-filterapplied-30x30.png) angezeigt. Klicken Sie auf [!UICONTROL **Alle löschen**], um alle Filter zu entfernen, und klicken Sie auf [!UICONTROL **Filter ausblenden**], um das Filterbedienfeld zu schließen.

{{step1-to-boards}}

1. Klicken Sie im Dashboard auf [!UICONTROL **Arbeitsablauf anzeigen**], um einen Arbeitsablauf zu öffnen.
1. Klicken Sie auf [!UICONTROL **Registerkarte**] Boards“, falls diese noch nicht angezeigt wird.
1. Klicken Sie [!UICONTROL **Filter**].
1. Wählen Sie die Pinnwände aus, die nach Status angezeigt werden sollen (archivierte Pinnwände, aktive Pinnwände oder alle Pinnwände).
1. Wählen Sie die Pinnwände aus, die nach Vorlage angezeigt werden sollen.

## Mitglieder zu einem Arbeitsablauf hinzufügen

Personen und Teams müssen dem Arbeitsablauf als Mitglieder hinzugefügt werden, bevor sie den Arbeitsablauf und seine Inhalte anzeigen können. Ein Mitglied eines Arbeitsablaufs kann Mitglieder zum Arbeitsablauf hinzufügen und daraus entfernen und sehen, welche Boards sich im Arbeitsablauf befinden.

>[!NOTE]
>
>Ein Mitglied eines Arbeitsablaufs kann eine Pinnwand in einem Arbeitsablauf erst öffnen, wenn es dieser Pinnwand als Mitglied hinzugefügt wird.

{{step1-to-boards}}

1. Klicken Sie im Dashboard auf [!UICONTROL **Arbeitsablauf anzeigen**], um einen Arbeitsablauf zu öffnen.
1. Klicken Sie auf das **[!UICONTROL Mitglied hinzufügen]**-Symbol ![Mitglieder hinzufügen](assets/boards-addmember-spectrum-25x25.png), um Mitglieder und Teams zum Arbeitsablauf hinzuzufügen.

   Dies ist der gleiche Prozess wie das Hinzufügen von Mitgliedern zu einer Pinnwand. Weitere Informationen finden Sie unter [Mitglieder zu einer Pinnwand hinzufügen oder daraus entfernen](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

## Hinzufügen von Quellen zu einem Arbeitsablauf

Eine Quelle bestimmt, woher die Karten im Arbeitsablauf kommen.

{{step1-to-boards}}

1. Klicken Sie auf das [!UICONTROL **Quellen**]-Symbol ![Quellen-Symbol](assets/sources-icon.png), um eine Quelle zum Importieren von Karten in den Arbeitsablauf zu definieren. Derzeit ist nur eine Quelle [!DNL Adobe Workfront].
1. Fügen Sie Filter hinzu, um Aufgaben und Probleme aus Workfront als Karten zu importieren.

   Das Hinzufügen von Filtern für Workstream-Quellen entspricht dem Hinzufügen erweiterter Filter für eine Aufnahmespalte auf einer Basis-Pinnwand oder Kanban-Pinnwand. Weitere Informationen finden Sie unter [Hinzufügen einer Aufnahmespalte zu einer Pinnwand](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Konfigurieren eines Arbeitsablaufs

{{step1-to-boards}}

1. Klicken Sie im Dashboard auf [!UICONTROL **Arbeitsablauf anzeigen**], um einen Arbeitsablauf zu öffnen.
1. Klicken Sie auf [!UICONTROL **Konfigurieren**], um das Bedienfeld [!UICONTROL Arbeitsablauf konfigurieren] zu öffnen.
1. (Optional) Erweitern Sie [!UICONTROL **Arbeitsablauf**] und geben Sie eine Beschreibung des Arbeitsablaufs ein. Diese Beschreibung wird im Dashboard angezeigt.
1. (Optional) Erweitern Sie [!UICONTROL **Iterationen**], um einen Iterationsprozess für diesen Arbeitsablauf zu definieren.

   Die Gesamtanzahl der Karten, die Anzahl der spitzen Karten und die Anzahl der Iterationen werden im Abschnitt Kartenliste angezeigt. Klicken Sie [!UICONTROL **Liste anzeigen**], um die Liste zu öffnen und Karten hinzuzufügen. Weitere Informationen finden Sie unter [Verwenden der Kartenliste](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   Wenn eine Iteration bereits definiert wurde, werden ihr Startdatum, die Anzahl der Karten und die Anzahl der Punkte angezeigt. Klicken Sie auf [!UICONTROL **Pinnwand anzeigen**], um die Iterationsplatine zu öffnen. Weitere Informationen finden Sie unter [Erstellen einer Iteration in einem Arbeitsablauf](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. (Optional) Erweitern Sie [!UICONTROL **Tags**], um dem Arbeitsablauf Tags hinzuzufügen. Suchen Sie nach einem Tag oder geben Sie einen neuen Tag-Namen in das Suchfeld ein und drücken Sie die Eingabetaste , um es zu erstellen.
