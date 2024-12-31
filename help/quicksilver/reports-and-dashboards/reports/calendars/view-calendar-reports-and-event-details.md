---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Anzeigen von Kalenderberichten und Ereignisdetails
description: Sie können Kalenderberichte und Ereignisdetails anzeigen, die Sie in Adobe Workfront erstellt haben oder die für Sie freigegeben wurden.
author: Lisa
feature: Reports and Dashboards
exl-id: db016e91-43e4-400c-ac9d-1639c7f94479
source-git-commit: 1723609ce790566c072d071f9ac627dba7dc5350
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---

# Anzeigen von Kalenderberichten und Ereignisdetails

Sie können Kalenderberichte und Ereignisdetails anzeigen, die Sie in Adobe Workfront erstellt haben oder die für Sie freigegeben wurden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Lizenz*</strong></td> 
   <td> <p>[!UICONTROL-Anfrage] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen der Zugriffsebene*</strong></td> 
   <td> <p>Zugriff auf [!UICONTROL View] oder höher auf [!UICONTROL Reports], [!UICONTROL Dashboards] und [!UICONTROL Calenders]</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront], ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie [!DNL Workfront]-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Ansicht] oder höhere Berechtigungen für den Kalenderbericht</p> <p>Weitere Informationen zum Anfordern von Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriff auf Objekte</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Anzeigen eines Kalenderberichts

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** Symbol ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront] und klicken Sie dann auf **[!UICONTROL Kalender]**.

   Abhängig von Ihrer Zugriffsebene werden möglicherweise die folgenden Kalender angezeigt:

   * Standardkalender [!DNL Adobe Workfront]

     Workfront erstellt einen Kalender für Sie basierend auf den Projekten, Aufgaben und Problemen, die Ihnen zugewiesen sind oder die Teams, Gruppen oder Rollen zugewiesen sind, denen Sie zugewiesen sind.
   * Von Ihnen erstellte Kalender

     Informationen zum Erstellen von Kalendern finden Sie unter [Übersicht über Kalenderberichte](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

   * Kalender, die andere Benutzer für Sie freigegeben haben

     Weitere Informationen zum Freigeben von Kalendern finden Sie unter [[!UICONTROL Freigeben ] Kalenders](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

1. (Bedingt) Klicken Sie auf die **[!UICONTROL Ansicht]** und wählen Sie dann die Kalenderdauer aus, die Sie anzeigen möchten.\
   ![Kalenderdauer](assets/view-menu-calendar-report-350x189.png)\
   Sie können aus den folgenden Kalenderberichtsansichten wählen:

   * **[!UICONTROL Monat]**: Zeigt vier Wochen des Kalenders an
   * **[!UICONTROL Woche]**: Zeigt eine Kalenderwoche an
   * **[!UICONTROL Gantt]**: Zeigt eine kontinuierliche Ansicht des Kalenders an\

     ![[!UICONTROL Gantt]-Kalenderbericht](assets/gantt-calendar-report.png)
Sie können weitere Ereignisse in einer [!UICONTROL Gantt“-Ansicht ], indem Sie nach unten oder seitlich scrollen. Ein Ladesymbol wird angezeigt, wenn Daten für die Ansicht gefüllt werden.
   >[!NOTE]
   >
   >In der [!UICONTROL Monat] und [!UICONTROL Woche]-Ansicht haben Ereignisse, die aktuell oder zukünftig sind (einschließlich Ereignisse, die sich über mehrere Tage erstrecken, sofern sie heute oder einen zukünftigen Tag enthalten), eine Schattierung, die der Farbe in dem Projekt oder der Kalendergruppierung entspricht. Vergangene Ereignisse haben eine hellere Schattierung, um anzuzeigen, dass sie nicht mehr aktuell sind. Sie können diese Ereignisse jedoch weiterhin auswählen und anzeigen.

1. (Optional) Wenn Sie den Kalender in der Ansicht [!UICONTROL Monat] oder [!UICONTROL Woche] anzeigen, können Sie Ihre Kalenderansicht mit den folgenden Optionen ändern:

   * Ein- oder Ausschließen von Wochenenden:

      1. Klicken Sie in **[!UICONTROL Kalender]**-Symbolleiste auf **[!UICONTROL Kalenderaktionen]** und wählen Sie dann in der Dropdown-Liste entweder **[!UICONTROL Wochenende anzeigen]** oder **[!UICONTROL Wochenende ausblenden]**.
   * So ändern Sie die angezeigten Daten schnell:

      1. Klicken Sie in **[!UICONTROL Kalender]**-Symbolleiste auf den linken Pfeil der Datumsanzeige, um im Kalender zurückzukehren, oder auf den rechten Pfeil, um fortzufahren.\

         ![Auf Pfeil klicken, um Datum zu ändern](assets/click-arrows-to-change-dates-calendar-report.png)\
         Die angezeigten Datumswerte werden durch ein Intervall angepasst, das auf Ihrer aktuellen Kalenderansicht basiert. Wenn Sie z. B. den Kalender in der Ansicht [!UICONTROL Woche] anzeigen, wird der Kalender je nach ausgewähltem Pfeil entweder eine Woche vor oder eine Woche zurück angezeigt.

      1. (Optional) Um zum aktuellen Tag zurückzukehren, klicken Sie auf **Today**.


1. (Optional) Um einen Kalender im Vollbildmodus anzuzeigen, klicken Sie auf die Vollbildpfeile auf der rechten Seite der Symbolleiste **[!UICONTROL Kalender]**.
   ![Auf Pfeil klicken, um Datum zu ändern](assets/click-arrows-to-change-dates-calendar-report.png)\
   Drücken Sie Esc, um zur normalen Kalenderansicht zurückzukehren.

1. (Optional) Um die Ereignisse für ein mit dem Kalender verknüpftes Projekt oder eine mit dem Kalender verknüpfte Kalendergruppierung auszublenden, löschen Sie das Projekt oder die Kalendergruppierung in der Projektliste.
   ![Ereignisse ausblenden](assets/hide-events-for-project-or-cal-grouping.png)\
   Sie können die Ereignisse wieder anzeigen, indem Sie das [!UICONTROL Projekt] oder die Kalendergruppierung in der Projektliste auswählen.

## Kalenderbericht-Ereignisdetails anzeigen

Sie können die Details eines Ereignisses in einem Kalender für aktuelle und vergangene Ereignisse anzeigen.

1. Navigieren Sie zum Ereignis, für das Sie die Details wissen möchten, und klicken Sie dann auf das Ereignis.\
   Eine Detailseite für das Ereignis wird geöffnet.\
   ![calendar_report_EventDetails.png](assets/calendar-report-eventdetails-350x145.png)

1. (Optional) So zeigen Sie zusätzliche Details zum Objekt an:

   1. Bewegen Sie den Mauszeiger über den Projekt-, Aufgaben- oder Problemnamen.

      Eine Detailseite für das Objekt wird geöffnet.\
      ![additional_object_details_-_calendar_report.png](assets/additional-object-details---calendar-report-350x131.png)

   1. (Optional) Klicken Sie auf den Titel des Objekts, um das verknüpfte Projekt, die zugehörige Aufgabe oder das zugehörige Problem zu öffnen.
   1. (Optional) Um alle geöffneten Detailseiten zu schließen, klicken Sie auf eine beliebige Stelle außerhalb der Ereignisdetailseiten.
