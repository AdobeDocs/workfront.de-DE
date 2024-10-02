---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Kalenderberichte und Ereignisdetails anzeigen
description: Sie können Kalenderberichte und Ereignisdetails anzeigen, die Sie in Adobe Workfront erstellt haben oder für Sie freigegeben wurden.
author: Lisa
feature: Reports and Dashboards
exl-id: db016e91-43e4-400c-ac9d-1639c7f94479
source-git-commit: 1723609ce790566c072d071f9ac627dba7dc5350
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---

# Kalenderberichte und Ereignisdetails anzeigen

Sie können Kalenderberichte und Ereignisdetails anzeigen, die Sie in Adobe Workfront erstellt haben oder für Sie freigegeben wurden.

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
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Anforderung] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>[!UICONTROL Ansicht] oder höher Zugriff auf [!UICONTROL Berichte], [!UICONTROL Dashboards] und [!UICONTROL Kalender]</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Ansicht] oder höhere Berechtigungen für den Kalenderbericht</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Kalenderberichte anzeigen

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und klicken Sie dann auf **[!UICONTROL Kalender]**.![](assets/main-menu-icon.png)

   Je nach Zugriffsebene werden möglicherweise die folgenden Kalender angezeigt:

   * Ihr standardmäßiger [!DNL Adobe Workfront] Kalender

     Workfront erstellt einen Kalender für Sie basierend auf den Projekten, Aufgaben und Problemen, die Ihnen zugewiesen sind oder die Teams, Gruppen oder Rollen zugewiesen sind, denen Sie zugewiesen sind.
   * Von Ihnen erstellte Kalender

     Weitere Informationen zum Erstellen von Kalendern finden Sie unter [Übersicht über Kalenderberichte](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

   * Kalender, die andere Benutzer für Sie freigegeben haben

     Weitere Informationen zum Freigeben von Kalendern finden Sie unter [[!UICONTROL Kalenderbericht freigeben]](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md) .

1. (Bedingt) Klicken Sie auf die Dropdownliste **[!UICONTROL Ansicht]** und wählen Sie dann die Kalenderdauer aus, die Sie anzeigen möchten.\
   ![Kalenderdauer](assets/view-menu-calendar-report-350x189.png)\
   Sie können aus den folgenden Kalenderberichtsansichten auswählen:

   * **[!UICONTROL Monat]**: Zeigt vier Wochen im Kalender an
   * **[!UICONTROL Woche]**: Zeigt eine Woche im Kalender an
   * **[!UICONTROL Gantt]**: Zeigt eine kontinuierliche Ansicht des Kalenders an\

     ![[!UICONTROL Gantt] Kalenderbericht](assets/gantt-calendar-report.png)
Sie können weitere Ereignisse in einer [!UICONTROL Gantt]-Ansicht sehen, indem Sie nach unten oder nach unten scrollen. Ein Ladesymbol wird angezeigt, wenn Daten für die Ansicht aufgefüllt werden.
   >[!NOTE]
   >
   >In den Ansichten [!UICONTROL Monat] und [!UICONTROL Woche] haben Ereignisse, die aktuell oder künftig sind (einschließlich Ereignissen, die mehrere Tage umfassen, solange sie heute oder einen künftigen Tag enthalten) eine Schattierung, die der Farbe im Projekt oder in der Kalendergruppierung entspricht. Frühere Ereignisse haben eine hellere Schattierung, um anzuzeigen, dass sie nicht mehr aktuell sind. Sie können diese Ereignisse jedoch weiterhin auswählen und anzeigen.

1. (Optional) Wenn Sie den Kalender in den Ansichten [!UICONTROL Monat] oder [!UICONTROL Woche] anzeigen, können Sie Ihre Kalenderansicht mit den folgenden Optionen ändern:

   * So schließen Sie Wochenenden ein oder aus:

      1. Klicken Sie in der Symbolleiste **[!UICONTROL Kalender]** auf **[!UICONTROL Kalenderaktionen]** und wählen Sie dann aus der Dropdownliste entweder **[!UICONTROL Wochenende einblenden]** oder **[!UICONTROL Wochenende ausblenden]** aus.
   * So ändern Sie schnell die angezeigten Daten:

      1. Klicken Sie in der Symbolleiste **[!UICONTROL Kalender]** auf den linken Pfeil der Datumsanzeige, um im Kalender zurückzukehren, oder auf den Pfeil nach rechts, um fortzufahren.\

         ![Klicken Sie auf den Pfeil, um das Datum zu ändern](assets/click-arrows-to-change-dates-calendar-report.png)\
         Die angezeigten Daten werden nach einem Intervall angepasst, das auf Ihrer aktuellen Kalenderansicht basiert. Wenn Sie beispielsweise den Kalender in der Ansicht [!UICONTROL Woche] anzeigen, zeigt der Kalender je nach ausgewähltem Pfeil entweder eine Woche vor oder eine Woche vor.

      1. (Optional) Um zum aktuellen Tag zurückzukehren, klicken Sie auf **Today**.


1. (Optional) Um einen Kalender im Vollbildmodus anzuzeigen, klicken Sie auf die Vollbildpfeile auf der rechten Seite der Symbolleiste **[!UICONTROL Kalender]** .
   ![Klicken Sie auf den Pfeil, um das Datum zu ändern](assets/click-arrows-to-change-dates-calendar-report.png)\
   Drücken Sie Esc , um zur normalen Kalenderansicht zurückzukehren.

1. (Optional) Um die Ereignisse für ein mit dem Kalender verknüpftes Projekt oder eine mit dem Kalender verknüpfte Kalendergruppierung auszublenden, löschen Sie das Projekt oder die Kalendergruppierung in der Projektliste.
   ![Ereignisse ausblenden](assets/hide-events-for-project-or-cal-grouping.png)\
   Sie können die Ereignisse wieder sichtbar machen, indem Sie in der Projektliste das [!UICONTROL Projekt] oder die Kalendergruppierung auswählen.

## Kalenderberichtereignisdetails anzeigen

Sie können die Details eines Ereignisses in einem Kalender sowohl für aktuelle als auch für vergangene Ereignisse anzeigen.

1. Gehen Sie zu dem Ereignis, für das Sie die Details kennen möchten, und klicken Sie dann auf das Ereignis.\
   Eine Detailseite für das Ereignis wird geöffnet.\
   ![calendar_report_EventDetails.png](assets/calendar-report-eventdetails-350x145.png)

1. (Optional) So zeigen Sie zusätzliche Details zum Objekt an:

   1. Bewegen Sie den Mauszeiger über das Projekt, die Aufgabe oder den Namen des Problems.

      Für das Objekt wird eine Detailseite geöffnet.\
      ![additional_object_details_-_calendar_report.png](assets/additional-object-details---calendar-report-350x131.png)

   1. (Optional) Klicken Sie auf den Titel des Objekts, um das zugehörige Projekt, die Aufgabe oder das Problem zu öffnen.
   1. (Optional) Klicken Sie zum Schließen aller geöffneten Detailseiten auf eine beliebige Stelle außerhalb der Ereignisdetailseiten.
