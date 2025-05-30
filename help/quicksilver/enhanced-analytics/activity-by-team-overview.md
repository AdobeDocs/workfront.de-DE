---
title: Visualisierung „Aktivität nach Team“ in Enhanced Analytics anzeigen
content-type: overview
product-area: enhanced-analytics
navigation-topic: enhanced-analytics-navigation-topic
description: Die Visualisierung „Aktivität nach Team“ zeigt Aktivitäten an, die während eines bestimmten Zeitraums für ein Heim-Team stattfinden, sodass Sie verstehen können, wie verschiedene Heim-Teams ihre Zeit in Adobe Workfront verbracht haben. Je nachdem, wie Ihr Home-Team in Workfront eingerichtet ist, kann Ihnen diese Visualisierung verschiedene Einblicke geben und verschiedene Fragen beantworten.
author: Nolan
feature: Reports and Dashboards
exl-id: c4f9886c-ce76-43a8-bd43-cb64fff27e79
source-git-commit: 2a6e767036ae702f6c19dc71cdb11dae8e9e37ea
workflow-type: tm+mt
source-wordcount: '766'
ht-degree: 6%

---

# Visualisierung „Aktivität nach Team“ in Enhanced Analytics anzeigen

>[!IMPORTANT]
>
>Enhanced Analytics wurde am 27. Mai aus Workfront entfernt. Workfront Data Connect ist eine neue, alternative Lösung und kann verwendet werden, um alle derzeit verwendeten Visualisierungen von Enhanced Analytics zu replizieren. <br>Weitere Informationen finden Sie im Handbuch [Erweiterte Analytics](/help/quicksilver/product-announcements/announcements/enhanced-analytics-deprecation.md)Einstellung“.



<!-- Audited: 12/2023 -->

Die Visualisierung „Aktivität nach Team“ zeigt Aktivitäten an, die während eines bestimmten Zeitraums für ein Heim-Team stattfinden, sodass Sie verstehen können, wie verschiedene Heim-Teams ihre Zeit in Adobe Workfront verbracht haben. Je nachdem, wie Ihr Home-Team in Workfront eingerichtet ist, kann Ihnen diese Visualisierung verschiedene Einblicke geben und verschiedene Fragen beantworten.

>[!NOTE]
>
>Die Projektaktivitätsvisualisierung ähnelt dieser Visualisierung, sie zeigt jedoch Aktivitäten basierend auf Personen an, die Projekten zugewiesen sind, und nicht auf Personen, die einem Heim-Team zugewiesen sind.\
>Weitere Informationen zur Visualisierung der Projektaktivität finden Sie unter [Anzeigen der Visualisierung der Projektaktivität in Enhanced Analytics](../enhanced-analytics/project-activity-overview.md).

![Aktivität nach Team](assets/activity-by-team-350x113.png){width="700"}

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://business.adobe.com/products/workfront/pricing.html" target="_blank">Workfront-Plan</a></td> 
   <td> <p>Unternehmen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a></td> 
   <td>
      <p>Neu:</p> 
         <ul><li>Leicht oder höher</li></ul>
      <p>Aktuell:</p>
         <ul><li>Überprüfen oder höher</li></ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte anzeigen</p> <!--<p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level.<br>For information on how a Workfront administrator can change your access level, see <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p>--> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen</p> <!--<p>For information on requesting additional access, see <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p>--> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Voraussetzungen für die Verwendung der erweiterten Analyse finden Sie im Abschnitt „Voraussetzungen“ in [Übersicht über die erweiterte Analyse](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualisierung „Aktivität nach Team“

Die verschiedenen Aktivitäten werden in verschiedenen Farben angezeigt, um bestimmte Ereignisse über den gefilterten Zeitraum zusammenzufassen:

* **Benutzer angemeldet**: Violette Kästchen zeigen an, dass sich Personen im Home-Team an diesem Tag angemeldet haben. Je dunkler der Farbton, umso mehr Personen haben sich angemeldet.

  ![Angemeldete Benutzer](assets/project-activity-users-logged-in.png)

* **Änderung des Aufgabenstatus**: Pinkfarbene Kästchen zeigen an, dass Personen im Home-Team den Status einer Aufgabe an diesem Tag geändert haben. Je dunkler der Farbton, umso mehr Aufgabenstatus haben sich geändert.

  ![Änderungen des Aufgabenstatus](assets/project-activity-task-status-changes.png)

* **Aufgaben abgeschlossen**: Blaue Kästchen zeigen an, dass Personen im Home-Team eine Aufgabe an diesem Tag abgeschlossen haben. Je dunkler der Farbton, umso mehr Aufgaben wurden abgeschlossen.

  ![Aufgaben abgeschlossen](assets/project-activity-tasks-completed.png)

Wenn Sie den Mauszeiger über ein Feld bewegen, wird angezeigt, wie oft die Aktion an einem bestimmten Tag genau abgeschlossen wurde. Sie können ein Team auswählen, um eine Aufschlüsselung dieser Aktivitäten nach den einzelnen Personen im Home-Team anzuzeigen.

Anhand dieser Informationen können Sie Folgendes feststellen:

* Welche Aktivitäten in einem Heim-Team stattfinden und mit welcher Geschwindigkeit.
* Welche Heim-Teams werden überarbeitet oder verwenden das System öfter?
* ob die Arbeitsteilung für das Stamm-Team angemessen ist.

Informationen zum Abrufen der besten Daten für diese Visualisierung finden Sie unter [Erweiterte Analyse - Übersicht](../enhanced-analytics/enhanced-analytics-overview.md).

## Visualisierung „Aktivität nach Team“ anzeigen

1. Klicken Sie auf das Hauptmenüsymbol ![Hauptmenüsymbol](assets/main-menu-icon-16x12.png) und wählen Sie dann **Analytics**.
1. Wählen Sie im linken Bedienfeld die Option **Personen** aus.

   ![Bereich Personen](assets/people-area-cropped-qs-350x276.png)

1. (Optional) Um einen anderen Datumsbereich zu verwenden, wählen Sie im Datumsbereichsfilter Neues Start- und Enddatum aus.

   ![Datumsbereich auswählen](assets/filters-select-date-range-350x344.png)

   Informationen zur Verwendung des Filters für den Datumsbereich finden Sie unter [Anwenden von Filtern in der erweiterten Analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

1. (Bedingt) Wenn Sie Ihren Team-Filter nicht festgelegt haben, fügen Sie den Team-Filter hinzu und wählen Sie jedes Team aus, für das Sie Daten anzeigen möchten.

   Weitere Informationen zum Hinzufügen von Filtern in der erweiterten Analyse finden Sie unter [Anwenden von Filtern in der erweiterten Analyse](../enhanced-analytics/use-enhanced-analytics-filters.md).

   Nachdem Sie Filter hinzugefügt haben, werden Daten für bis zu 50 Projekte angezeigt und die Filter bleiben auch dann aktiv, wenn Sie die Seite verlassen oder sich von Workfront abmelden.

1. (Optional) Um einen Datumsbereich heranzuzoomen, wählen Sie einen Punkt auf der Visualisierung für den Beginn Ihres Datumsbereichs und ziehen Sie ihn an das Ende Ihres Datumsbereichs.

   Alle anderen Visualisierungen werden auf denselben Datumsbereich aktualisiert und ein Zeitrahmenfilter wird erstellt.

   ![Zeitrahmen-Filter](assets/timeframe-filter-350x220.png)

1. Auf einen Teamnamen klicken

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   or role
   </MadCap:conditionalText>
   -->

   , um weitere Details zu den vom Home-Team abgeschlossenen Aktivitäten anzuzeigen.

   Die Liste wird erweitert, um die Aktivitäten jeder Person anzuzeigen, die dem Home-Team zugewiesen ist.

   <!--
   <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode"> Role not available</span>
   -->

1. Bewegen Sie den Mauszeiger über ein farbiges Feld, um das Datum anzuzeigen, an dem die Benutzer eine Aktion abgeschlossen haben, sowie die Anzahl der Abschlüsse der Aktion an diesem Tag.

   Dunklere Farben zeigen eine höhere Aktivität an.

   ![Aktivität nach Team](assets/activity-by-team-activity-pop-up-350x155.png)

1. (Optional) Um die Visualisierungsdaten zu exportieren, klicken Sie auf das Symbol „Exportieren![ &quot;](assets/export.png)&quot; oben rechts in der Visualisierung und wählen Sie dann das Exportformat aus:

   * **Diagramm (PNG)**
   * **Datentabelle (XSLX)**

