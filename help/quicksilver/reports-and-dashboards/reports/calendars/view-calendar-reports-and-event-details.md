---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: View Calendar Reports and Event Details
description: You can view calendar reports and event details that you created or were shared with you in Adobe Workfront.
author: Lisa
feature: Reports and Dashboards
exl-id: db016e91-43e4-400c-ac9d-1639c7f94479
source-git-commit: 3e5fdb157a6ff29daf964b505d3a0bf4f9842e88
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

# Anzeigen von Kalenderberichten und Ereignisdetails

You can view calendar reports and event details that you created or were shared with you in Adobe Workfront.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront plan]</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>New: Contributor</p>
       <p>oder</p>
       <p>Aktuell: Anfrage</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf [!UICONTROL View] oder höher auf [!UICONTROL Reports], [!UICONTROL Dashboards] und [!UICONTROL Calenders]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>[!UICONTROL Ansicht] oder höhere Berechtigungen für den Kalenderbericht</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anzeigen eines Kalenderberichts

<!--{{step1-to-calendars}}-->

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **[!UICONTROL Kalender]**.

   Abhängig von Ihrer Zugriffsebene werden möglicherweise die folgenden Kalender angezeigt:

   * Standardkalender [!DNL Adobe Workfront]

     Workfront creates a calendar for you based on the projects, tasks, and issues that are assigned to you or that are assigned to teams, groups, or roles to which you are assigned.

   * Calendars that you have created

     To learn about creating calendars, see [Calendar reports overview](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

   * Calendars that other users have shared with you

     To learn about sharing calendars, see [[!UICONTROL Share a calendar] report](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

1. (Bedingt) Klicken Sie auf die **[!UICONTROL Ansicht]** und wählen Sie dann die Kalenderdauer aus, die Sie anzeigen möchten.
   ![Calendar duration](assets/view-menu-calendar-report-350x189.png)
You can choose from the following calendar report views:

   * **[!UICONTROL Month]**: Displays four weeks of the calendar
   * **[!UICONTROL Week]**: Displays one week of the calendar
   * **[!UICONTROL Gantt]**: Displays a continuous view of the calendar

     You can see more events in a [!UICONTROL Gantt] view by scrolling down or sideways. A loading symbol appears as data is populated for the view.

   >[!NOTE]
   >
   >In der [!UICONTROL Monat] und [!UICONTROL Woche]-Ansicht haben Ereignisse, die aktuell oder zukünftig sind (einschließlich Ereignisse, die sich über mehrere Tage erstrecken, sofern sie heute oder einen zukünftigen Tag enthalten), eine Schattierung, die der Farbe in dem Projekt oder der Kalendergruppierung entspricht. Vergangene Ereignisse haben eine hellere Schattierung, um anzuzeigen, dass sie nicht mehr aktuell sind. Sie können diese Ereignisse jedoch weiterhin auswählen und anzeigen.

1. (Optional) Wenn Sie den Kalender in der Ansicht [!UICONTROL Monat] oder [!UICONTROL Woche] anzeigen, können Sie Ihre Kalenderansicht mit den folgenden Optionen ändern:

   * Ein- oder Ausschließen von Wochenenden:

      1. Klicken Sie in **[!UICONTROL Kalender]**-Symbolleiste auf **[!UICONTROL Kalenderaktionen]** und wählen Sie dann in der Dropdown-Liste entweder **[!UICONTROL Wochenende anzeigen]** oder **[!UICONTROL Wochenende ausblenden]**.

   * So ändern Sie die angezeigten Daten schnell:

      1. Klicken Sie in **[!UICONTROL Kalender]**-Symbolleiste auf den linken Pfeil der Datumsanzeige, um im Kalender zurückzukehren, oder auf den rechten Pfeil, um fortzufahren.

         ![Auf Pfeil klicken, um Datum zu ändern](assets/click-arrows-to-change-dates-calendar-report.png)\
         Die angezeigten Datumswerte werden durch ein Intervall angepasst, das auf Ihrer aktuellen Kalenderansicht basiert. Wenn Sie z. B. den Kalender in der Ansicht [!UICONTROL Woche] anzeigen, wird der Kalender je nach ausgewähltem Pfeil entweder eine Woche vor oder eine Woche zurück angezeigt.

      1. (Optional) Um zum aktuellen Tag zurückzukehren, klicken Sie auf [!UICONTROL **Heute**].


1. (Optional) Um einen Kalender im Vollbildmodus anzuzeigen, klicken Sie auf die Vollbildpfeile auf der rechten Seite der Symbolleiste **[!UICONTROL Kalender]**.
   ![Click arrow to change date](assets/click-arrows-to-change-dates-calendar-report.png)\
   Press Esc to return to the normal view of the calendar.

1. (Optional) To hide the events for a project or calendar grouping linked to the calendar, clear the project or calendar grouping in the project list.
   ![Hide events](assets/hide-events-for-project-or-cal-grouping.png)
You can make the events visible again by selecting the [!UICONTROL project] or calendar grouping in the project list.

## Kalenderbericht-Ereignisdetails anzeigen

You can see the details of an event in a calendar, for both current and past events.

1. Navigieren Sie zum Ereignis, für das Sie die Details wissen möchten, und klicken Sie dann auf das Ereignis. Die Details werden in einem Bedienfeld auf der rechten Seite geöffnet.
1. (Optional) Klicken Sie auf den Titel des Objekts, um das verknüpfte Projekt, die zugehörige Aufgabe oder das zugehörige Problem zu öffnen.
