---
navigation-topic: use-the-gantt-chart
title: Informationen anzeigen im  [!UICONTROL Gantt-Diagramm]
description: Die Aufgabenliste Gantt-Diagramm und die Projektliste Gantt-Diagramm zeigen Informationen zu Projekten und Aufgaben an.
author: Alina
feature: Work Management
exl-id: e6b55699-0831-40d4-a997-6fe3f8828ee1
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: tm+mt
source-wordcount: '930'
ht-degree: 1%

---

# Informationen anzeigen im  [!UICONTROL Gantt-Diagramm]

Aufgabenliste [!UICONTROL Gantt-Diagramm] und Projektliste [!UICONTROL Gantt-Diagramm] Informationen zu Projekten und Aufgaben anzeigen.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel zu befolgen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenzübersicht*</td> 
   <td> <p>[!UICONTROL Review] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>[!UICONTROL Ansicht] oder höherer Zugriff auf Projekte und Aufgaben</p> <p><b>NOTIZ</b>

Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>[!UICONTROL Ansicht] oder höherer Zugriff auf das Projekt</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Suchen Sie die  [!UICONTROL Gantt-Diagramm]

Sie können sowohl das Gantt-Diagramm als auch die Projektliste der Aufgabe finden [!UICONTROL Gantt-Diagramm] aus mehreren Bereichen in Workfront. Weitere Informationen finden Sie unter [Erste Schritte mit [!UICONTROL Gantt-Diagramm]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md).

## Aufgaben in der [!UICONTROL Kritischer Pfad]

In der Projektliste [!UICONTROL Gantt-Diagramm], Aufgaben, die sich nicht im [!UICONTROL Kritischer Pfad] als hellblaue horizontale Linien anzeigen. Aufgaben, die sich auf der [!UICONTROL Kritischer Pfad] eines Projekts werden als rote horizontale Linien angezeigt.

Weitere Informationen zu Aufgaben im [!UICONTROL Kritischer Pfad], siehe [Überblick über das Projekt [!UICONTROL Kritischer Pfad]](../../../manage-work/tasks/manage-tasks/critical-path.md).

## Aufgabeninformationen in der Projektliste anzeigen [!UICONTROL Gantt-Diagramm]

Sie können die Aufgabeninformationen für ein Projekt direkt in der Projektliste anzeigen. Aufgaben werden unter dem Namen jedes Projekts aufgeführt.

>[!NOTE]
>
>Aufgaben können nicht über die Projektliste bearbeitet werden [!UICONTROL Gantt-Diagramm].

Sie können die Aufgabeninformationen für ein Projekt direkt aus einer Liste von Projekten in den folgenden Bereichen anzeigen:

* Im [!UICONTROL Projekte] area
* Innerhalb eines Portfolios
* Innerhalb eines Programms

So zeigen Sie Aufgaben in einem Projekt aus einer Projektliste an:

1. Zu einem der oben genannten Bereiche gehen.

   Beispiel: aus dem [!UICONTROL Hauptmenü]klicken **[!UICONTROL Projekte]**.

   Eine Liste der Projekte wird angezeigt.

1. Klicken Sie auf **[!UICONTROL Gantt-Diagramm]** icon ![](assets/gantt-icon-nwe.png) in der oberen rechten Ecke des Bildschirms.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: images conditioned for classic and nwe) <br></p>
   -->

1. Klicken Sie auf **[!UICONTROL Aufgabenliste anzeigen]** Symbol.

1. Klicken Sie links in der Projektliste auf den Dropdown-Pfeil neben dem Namen des Projekts, um alle Aufgaben unter diesem Projekt anzuzeigen.\
   Dadurch werden Aufgabeninformationen für die  [!UICONTROL Gantt-Diagramm].\
   ![Show_task_list_enabled_project_expand.png](assets/show-task-list-enabled-project-expanded-350x78.png)

1. (Optional) Klicken Sie auf die **[!UICONTROL Drucken]** -Symbol oben rechts, um die [!UICONTROL Gantt-Diagramm].

   >[!NOTE]
   >
   >Die Projektliste [!UICONTROL Gantt-Diagramm] exportiert nur Projekte. Aufgabeninformationen sind nicht enthalten.

## Ändern Sie den Zeitraum, für den Informationen in der Variablen [!UICONTROL Gantt-Diagramm]

Sie können den auf der [!UICONTROL Gantt-Diagramm] , um Informationen auf granularer Ebene anzuzeigen, oder Sie können schnell zu einer Tages-, Wochen-, Monats-, Quartals- oder Jahresansicht navigieren:

* [Zeitraum auf einer granularen Ebene ändern](#change-the-time-period-on-a-granular-level)
* [Anzeigen von Informationen nach Tag, Woche, Monat, Quartal oder Jahr](#view-information-by-day-week-month-quarter-or-year)

### Zeitraum auf einer granularen Ebene ändern {#change-the-time-period-on-a-granular-level}

1. Bewegen Sie den Mauszeiger über die Timeline der  [!UICONTROL Gantt-Diagramm]und ziehen Sie dann den Zoom-Indikator von links nach rechts, um die Timeline zu erweitern oder zu verkleinern.\
   ![zoom_tool_in_gantt.png](assets/zoom-tool-in-gantt-350x180.png)

### Anzeigen von Informationen nach Tag, Woche, Monat, Quartal oder Jahr {#view-information-by-day-week-month-quarter-or-year}

1. Im  [!UICONTROL Gantt-Diagramm]klicken Sie auf das Dropdown-Menü für den Zeitrahmen.

   ![](assets/timeline-options.png)

1. Wählen Sie einen Zeitraum aus den folgenden verfügbaren Optionen aus:

   * **[!UICONTROL Alle anpassen]**: Diese Option zeigt die Zeitleiste des gesamten Projekts an.
   * **[!UICONTROL Alle Projekte]**: Diese Option ist nur im Gantt-Diagramm der Projektliste verfügbar.
   * **[!UICONTROL Jahr]**
   * **[!UICONTROL Quartal]**
   * **[!UICONTROL Monat]**
   * **[!UICONTROL Woche]**
   * **[!UICONTROL Tag]**

1. (Optional) Wählen Sie einen detaillierteren Zeitrahmen aus, z. B. [!UICONTROL Woche] oder [!UICONTROL Tag]und klicken und ziehen Sie die horizontale Bildlaufleiste am unteren Rand des  [!UICONTROL Gantt-Diagramm] , um in der Zeitleiste des Projekts von links nach rechts zu wechseln.\
   Ein Timeline-Schnappschuss der [!UICONTROL Gantt] angezeigt, um das gesamte Projekt anzuzeigen.

   >[!TIP]
   >
   >Der Timeline-Schnappschuss wird erst angezeigt, nachdem Sie auf die horizontale Bildlaufleiste geklickt haben.

   ![gestreckchy_gantt_minimap_with_entwurf__1_.png](assets/stretchy-gantt-minimap-with-outline--1--350x140.png)

1. (Optional) Klicken Sie auf eine beliebige Stelle innerhalb des Zeitleisten-Snapshots, um zu einem bestimmten Punkt im Projektlebenszyklus zu navigieren.\
   Oder\
   Ziehen Sie die Griffe des Snapshot-Viewers, um einen bestimmten Zeitraum für die Anzeige in der Hauptseite auszuwählen [!UICONTROL Gantt].

## Filter, Ansichten und Gruppierungen verwenden

Die [!UICONTROL Gantt-Diagramm] ist eine visuelle Darstellung der Informationen, die derzeit in der Aufgabenliste angezeigt werden. Sie können Filter, Ansichten und Gruppierungen auf die Objekte anwenden, die in beiden [!UICONTROL Gantt-Diagramm]s.

>[!CAUTION]
>
>Sie können bei der Auswahl von [!UICONTROL Manuell] save [!UICONTROL Timeline-Planung] , um Änderungen an Ihrer Aufgabenliste zu speichern. Informationen zum Speichern von Änderungen an Aufgaben in einer Liste finden Sie unter [Aufgaben in einer Liste bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md).

Filter und Gruppierungen, die Sie auf die Liste anwenden, werden sowohl in der Projektliste als auch in der Aufgabenliste angezeigt  [!UICONTROL Gantt-Diagramm]s und sind auch enthalten, wenn die Gantt-Diagramme exportiert werden:

* Filter\
   Sie können einen Filter auf die Liste anwenden, um die in der Variablen [!UICONTROL Gantt-Diagramm].\
   Informationen zum Anwenden eines Filters finden Sie unter  [Filterübersicht in [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Gruppierungen\
   Gruppierungen, die Sie auf die Liste anwenden, werden auf der Seite [!UICONTROL Gantt-Diagramm].\
   Informationen zum Anwenden einer Gruppierung finden Sie unter  [Gruppierungsübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

Ansichten werden nicht auf der [!UICONTROL Gantt-Diagramm]. Wenn Sie jedoch die [!UICONTROL Gantt-Diagramm] (gemäß  [Exportieren Sie die [!UICONTROL Gantt-Diagramm] PDF](../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md)), wird die Aufgabenliste zusätzlich zum [!UICONTROL Gantt-Diagramm], wobei die aktuelle Ansicht auf die Liste angewendet wird.

## Anzeigeoptionen konfigurieren

Sie können auswählen, welcher Informationstyp in beiden [!UICONTROL Gantt-Diagramme]. Weitere Informationen finden Sie unter [Konfigurieren der Anzeige von Informationen auf der [!UICONTROL Gantt-Diagramm]](../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).
