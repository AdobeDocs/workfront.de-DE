---
title: Anzeigen der Visualisierung der Projektaktivität in der erweiterten Analyse
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Die Visualisierung der Projektaktivität zeigt eine aggregierte Ansicht der Aktivitäten auf Projektebene - der Aktivitäten jeder dem Projekt zugewiesenen Person -, die während eines bestimmten Zeitraums stattgefunden haben. Sie können den Fokus einschränken, um die Aktivitäten innerhalb eines Projekts zu verstehen, oder Sie können Projektaktivitäten mit anderen Projekten in Adobe Workfront vergleichen.
author: Nolan
feature: Reports and Dashboards
exl-id: 9ef52be8-48d0-4f83-a214-dd32e794c73e
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 8%

---

# Anzeigen der Visualisierung der Projektaktivität in der erweiterten Analyse

<!-- Audited: 12/2023 -->

Die Visualisierung der Projektaktivität zeigt eine aggregierte Ansicht der Aktivitäten auf Projektebene - der Aktivitäten jeder dem Projekt zugewiesenen Person -, die während eines bestimmten Zeitraums stattgefunden haben. Sie können den Fokus einschränken, um die Aktivitäten innerhalb eines Projekts zu verstehen, oder Sie können Projektaktivitäten mit anderen Projekten in Adobe Workfront vergleichen.

>[!NOTE]
>
>Die Visualisierung &quot;Aktivität nach Team&quot;verhält sich ähnlich wie diese Visualisierung, aber die Visualisierung &quot;Aktivität nach Team&quot;zeigt die Aktivität des Startseiten-Teams für alle Projekte an.\
>Informationen zur Visualisierung &quot;Aktivität nach Team&quot;finden Sie unter [Anzeigen der Aktivitäts-Visualisierung nach Team in Enhanced Analytics](../enhanced-analytics/activity-by-team-overview.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfront-Abo</a></td> 
   <td> <p>Unternehmen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a></td> 
   <td>   <p>Neu:</p> 
   <ul><li>Licht oder höher</li></ul>
   <p>Aktuell:</p>
   <ul><li>Überprüfen oder höher</li></ul>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte anzeigen</p> <!--<p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>--> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen</p> <!--<p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p>--> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Voraussetzungen für die Verwendung von Enhanced Analytics finden Sie im Abschnitt &quot;Voraussetzungen&quot;in der [Übersicht über erweiterte Analysen](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualisierung der Projektaktivität

Projektaktivitäten werden in verschiedenen Farben angezeigt, um bestimmte Ereignisse in einem Projekt über einen bestimmten Zeitraum zusammenzufassen:

* **Benutzer, die sich angemeldet haben**: Die lilafarbenen Felder zeigen, dass sich Personen, die dem Projekt zugewiesen sind, an diesem Tag angemeldet haben. Je dunkler der Farbton, umso mehr Personen haben sich angemeldet.

  ![](assets/project-activity-users-logged-in.png)

* **Änderung des Aufgabenstatus**: Rosa Kästchen zeigen an, dass Personen den Status einer Aufgabe für das Projekt an diesem Tag geändert haben. Je dunkler der Farbton, umso mehr Aufgabenstatus haben sich geändert.

  ![](assets/project-activity-task-status-changes.png)

* **Aufgaben abgeschlossen**: blaue Felder zeigen an, dass Personen eine Aufgabe für das Projekt abgeschlossen haben. Je dunkler der Farbton, umso mehr Aufgaben wurden abgeschlossen.

  ![](assets/project-activity-tasks-completed.png)

Wenn Sie den Mauszeiger über ein Feld bewegen, wird angezeigt, wie oft die Aktion an einem bestimmten Tag abgeschlossen wurde. Sie können ein Projekt auswählen, um eine Aufschlüsselung dieser Aktivitäten nach jedem einzelnen Beitragenden am Projekt anzuzeigen.

Anhand dieser Informationen können Sie Folgendes feststellen:

* Die Aktivität für ein bestimmtes Projekt.
* Die Aktivität eines Projekts im Vergleich zu anderen Projekten.
* Welche Benutzende an einem Projekt arbeiten und mit welcher Frequenz.

Informationen zum Abrufen der besten Daten für diese Visualisierung finden Sie unter [Überblick über erweiterte Analysen](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualisierung der Projektaktivität anzeigen

1. Klicken Sie auf das Hauptmenü-Symbol ![](assets/main-menu-icon-16x12.png) und wählen Sie dann **Analytics** aus.
1. (Optional) Wenn Sie einen anderen Datumsbereich verwenden möchten, wählen Sie im Filter für den Datumsbereich die neuen Start- und Enddaten aus.

   ![](assets/filters-select-date-range-350x344.png)

   Informationen zur Verwendung des Datumsbereichfilters finden Sie unter [Anwenden von Filtern in Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

   >[!NOTE]
   >
   >Wenn Sie einen Datumsbereich für einen Zeitraum von mehr als 3 Monaten auswählen, werden in der Visualisierung der Projektaktivität keine Daten angezeigt.

1. (Bedingt) Wenn Sie den Projektdatensatz einschränken müssen, wählen Sie die Filter aus, die Sie verwenden möchten, und wenden Sie sie an.

   Weitere Informationen zum Hinzufügen von Filtern in Enhanced Analytics finden Sie unter [Anwenden von Filtern in Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nach dem Hinzufügen von Filtern werden Daten für bis zu 50 Projekte angezeigt und die Filter bleiben auch dann aktiv, wenn Sie die Seite verlassen oder sich von Workfront abmelden.

1. (Optional) Wenn Sie einen Datumsbereich vergrößern möchten, wählen Sie einen Punkt auf der Visualisierung für den Anfang Ihres Datumsbereichs aus und ziehen Sie ihn an das Ende Ihres Datumsbereichs.

   Alle anderen Visualisierungen werden auf denselben Datumsbereich aktualisiert und es wird ein Zeitrahmen-Filter erstellt.

   ![](assets/timeframe-filter-350x220.png)

1. (Optional) Um die Sortierung der Projekte zu ändern, klicken Sie auf das Menü **Sortieren nach** und wählen Sie dann eine neue Sortieroption aus:

   * **A - Z**
   * **Z - A**
   * **Geplantes Abschlussdatum**
   * **Geplantes Startdatum**

   Alle anderen Visualisierungen auf der Seite werden entsprechend Ihrer Sortierungsauswahl aktualisiert.

1. (Bedingt) Wenn Ihr Datensatz mehr als 50 Projekte enthält, können Sie mit den Pfeilen in der linken unteren Ecke der Visualisierung von einer Gruppe von 50 Projekten zur nächsten navigieren.

   Alle anderen Visualisierungen auf der Seite werden entsprechend Ihrer Seitenauswahl aktualisiert.

   ![](assets/pagination-350x118.png)

1. Klicken Sie in der Visualisierung auf ein Projekt, um weitere Details zum Projekt anzuzeigen.

   Die Liste wird erweitert und zeigt die Aktivitäten der einzelnen Mitwirkenden am Projekt an.

1. Bewegen Sie den Mauszeiger über ein Feld, um das Datum anzuzeigen, an dem Benutzer eine Aktion abgeschlossen haben, sowie die Anzahl der für diesen Tag durchgeführten Aktionen.

   ![](assets/project-activity-activity-pop-up-350x137.png)

1. (Optional) Um die Visualisierungsdaten zu exportieren, klicken Sie oben rechts in der Visualisierung auf das Symbol **Exportieren** ![](assets/export.png) und wählen Sie dann das Exportformat aus:

   * **Diagramm (PNG)**
   * **Datentabelle (XSLX)**

