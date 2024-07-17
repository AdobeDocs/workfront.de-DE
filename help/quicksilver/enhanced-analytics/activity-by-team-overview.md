---
title: Anzeigen der Aktivitätsvisualisierung nach Team in Enhanced Analytics
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Die Visualisierung "Aktivität nach Team"zeigt Aktivitäten an, die während eines bestimmten Zeitraums für ein Heimteam stattfinden, sodass Sie verstehen können, wie verschiedene Teams zu Hause ihre Zeit in Adobe Workfront verbracht haben. Je nachdem, wie Ihr Heimteam in Workfront eingerichtet ist, können Sie mit dieser Visualisierung verschiedene Einblicke erhalten und verschiedene Fragen beantworten.
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 4e928defe9b6271cef64f6554e91af4fc31ddeca
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 7%

---

# Anzeigen der Aktivitätsvisualisierung nach Team in Enhanced Analytics

<!-- Audited: 12/2023 -->

Die Visualisierung &quot;Aktivität nach Team&quot;zeigt Aktivitäten an, die während eines bestimmten Zeitraums für ein Heimteam stattfinden, sodass Sie verstehen können, wie verschiedene Teams zu Hause ihre Zeit in Adobe Workfront verbracht haben. Je nachdem, wie Ihr Heimteam in Workfront eingerichtet ist, können Sie mit dieser Visualisierung verschiedene Einblicke erhalten und verschiedene Fragen beantworten.

>[!NOTE]
>
>Die Visualisierung der Projektaktivität ähnelt dieser Visualisierung, zeigt jedoch Aktivitäten basierend auf Personen an, die Projekten zugewiesen sind, anstatt auf Personen, die einem Startseiten-Team zugewiesen sind.\
>Informationen zur Visualisierung der Projektaktivität finden Sie unter [Anzeigen der Visualisierung der Projektaktivität in Enhanced Analytics](../enhanced-analytics/project-activity-overview.md).

![](assets/activity-by-team-350x113.png){width="700"}

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
   <td>
      <p>Neu:</p> 
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

## Erläuterung der Visualisierung &quot;Aktivität nach Team&quot;

Die verschiedenen Aktivitäten werden in verschiedenen Farben angezeigt, um bestimmte Ereignisse über den gefilterten Zeitraum zusammenzufassen:

* **Benutzer, die sich angemeldet haben**: Die lilafarbenen Felder zeigen, dass sich Personen des Startseiten-Teams an diesem Tag angemeldet haben. Je dunkler der Farbton, umso mehr Personen haben sich angemeldet.

  ![](assets/project-activity-users-logged-in.png)

* **Änderung des Aufgabenstatus**: Rosa Kästchen zeigen an, dass Personen im Startteam den Status einer Aufgabe an diesem Tag geändert haben. Je dunkler der Farbton, umso mehr Aufgabenstatus haben sich geändert.

  ![](assets/project-activity-task-status-changes.png)

* **Aufgaben abgeschlossen**: blaue Kästchen zeigen an, dass Personen im Startseiten-Team eine Aufgabe an diesem Tag abgeschlossen haben. Je dunkler der Farbton, umso mehr Aufgaben wurden abgeschlossen.

  ![](assets/project-activity-tasks-completed.png)

Wenn Sie den Mauszeiger über ein Feld bewegen, wird angezeigt, wie oft die Aktion an einem bestimmten Tag abgeschlossen wurde. Sie können ein Team auswählen, um eine Aufschlüsselung dieser Aktivitäten nach den einzelnen Personen im Startseiten-Team anzuzeigen.

Anhand dieser Informationen können Sie Folgendes feststellen:

* Welche Aktivitäten werden in einem Home-Team durchgeführt und wie hoch ist der Anteil?
* Welche Home-Teams überarbeitet werden oder das System verwenden mehr.
* ob die Arbeitsteilung für das Stamm-Team angemessen ist.

Informationen zum Abrufen der besten Daten für diese Visualisierung finden Sie unter [Überblick über erweiterte Analysen](../enhanced-analytics/enhanced-analytics-overview.md).

## Ansicht der Aktivität nach Teamvisualisierung

1. Klicken Sie auf das Hauptmenü-Symbol ![](assets/main-menu-icon-16x12.png) und wählen Sie dann **Analytics** aus.
1. Wählen Sie im linken Bereich **Personen** aus.

   ![](assets/people-area-cropped-qs-350x276.png)

1. (Optional) Wenn Sie einen anderen Datumsbereich verwenden möchten, wählen Sie im Filter für den Datumsbereich die neuen Start- und Enddaten aus.

   ![](assets/filters-select-date-range-350x344.png)

   Informationen zur Verwendung des Datumsbereichfilters finden Sie unter [Anwenden von Filtern in Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Bedingt) Wenn Sie Ihren Team-Filter nicht festgelegt haben, fügen Sie den Team-Filter hinzu und wählen Sie die Teams aus, für die Sie Daten anzeigen möchten.

   Weitere Informationen zum Hinzufügen von Filtern in Enhanced Analytics finden Sie unter [Anwenden von Filtern in Enhanced Analytics](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nach dem Hinzufügen von Filtern werden Daten für bis zu 50 Projekte angezeigt und die Filter bleiben auch dann aktiv, wenn Sie die Seite verlassen oder sich von Workfront abmelden.

1. (Optional) Wenn Sie einen Datumsbereich vergrößern möchten, wählen Sie einen Punkt auf der Visualisierung für den Anfang Ihres Datumsbereichs aus und ziehen Sie ihn an das Ende Ihres Datumsbereichs.

   Alle anderen Visualisierungen werden auf denselben Datumsbereich aktualisiert und es wird ein Zeitrahmen-Filter erstellt.

   ![](assets/timeframe-filter-350x220.png)

1. Auf Teamnamen klicken

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   or role
   </MadCap:conditionalText>
   -->

   um weitere Details zu den vom Startseiten-Team abgeschlossenen Aktivitäten anzuzeigen.

   Die Liste wird erweitert und zeigt die Aktivitäten jeder dem Startseiten-Team zugewiesenen Person an.

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Role not available</span>
   -->

1. Bewegen Sie den Mauszeiger über ein farbiges Feld, um das Datum anzuzeigen, an dem die Benutzer eine Aktion abgeschlossen haben, sowie die Anzahl der Fertigstellungen der Aktion an diesem Tag.

   Dunklere Farben zeigen eine höhere Aktivität an.

   ![](assets/activity-by-team-activity-pop-up-350x155.png)

1. (Optional) Um die Visualisierungsdaten zu exportieren, klicken Sie in der oberen rechten Ecke der Visualisierung auf das Symbol Exportieren ![](assets/export.png) und wählen Sie dann das Exportformat aus:

   * **Diagramm (PNG)**
   * **Datentabelle (XSLX)**

