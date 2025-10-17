---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Anzeigen von Kalenderberichten und Ereignisdetails
description: Sie können Kalenderberichte und Ereignisdetails anzeigen, die Sie in Adobe Workfront erstellt haben oder die für Sie freigegeben wurden.
author: Jenny
feature: Reports and Dashboards
exl-id: db016e91-43e4-400c-ac9d-1639c7f94479
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# Anzeigen von Kalenderberichten und Ereignisdetails

Sie können Kalenderberichte und Ereignisdetails anzeigen, die Sie in Adobe Workfront erstellt haben oder die für Sie freigegeben wurden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Mitwirkender oder Mitwirkende</p>
       <p>Anfrage</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Anzeigen oder Erweitern des Zugriffs auf Berichte, Dashboards und Kalender</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>Anzeigen von oder höheren Berechtigungen für den Kalenderbericht</td> 
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

     Workfront erstellt einen Kalender für Sie basierend auf den Projekten, Aufgaben und Problemen, die Ihnen zugewiesen sind oder die Teams, Gruppen oder Rollen zugewiesen sind, denen Sie zugewiesen sind.

   * Von Ihnen erstellte Kalender

     Informationen zum Erstellen von Kalendern finden Sie unter [Übersicht über Kalenderberichte](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

   * Kalender, die andere Benutzer für Sie freigegeben haben

     Weitere Informationen zum Freigeben von Kalendern finden Sie unter [[!UICONTROL Freigeben &#x200B;] Kalenders](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

1. (Bedingt) Klicken Sie auf die **[!UICONTROL Ansicht]** und wählen Sie dann die Kalenderdauer aus, die Sie anzeigen möchten.
   ![Kalenderdauer](assets/view-menu-calendar-report-350x189.png)
Sie können aus den folgenden Kalenderberichtsansichten wählen:

   * **[!UICONTROL Monat]**: Zeigt vier Wochen des Kalenders an
   * **[!UICONTROL Woche]**: Zeigt eine Kalenderwoche an
   * **[!UICONTROL Gantt]**: Zeigt eine kontinuierliche Ansicht des Kalenders an

     Sie können weitere Ereignisse in einer **Gantt“-Ansicht**, indem Sie nach unten oder seitlich scrollen. Ein Ladesymbol wird angezeigt, wenn Daten für die Ansicht gefüllt werden.

   >[!NOTE]
   >
   >In der **Monat** und **Woche**-Ansicht haben Ereignisse, die aktuell oder zukünftig sind (einschließlich Ereignisse, die sich über mehrere Tage erstrecken, sofern sie heute oder einen zukünftigen Tag enthalten), eine Schattierung, die der Farbe in dem Projekt oder der Kalendergruppierung entspricht. Vergangene Ereignisse haben eine hellere Schattierung, um anzuzeigen, dass sie nicht mehr aktuell sind. Sie können diese Ereignisse jedoch weiterhin auswählen und anzeigen.

1. (Optional) Wenn Sie den Kalender in der Ansicht **Monat** oder **Woche** anzeigen, können Sie Ihre Kalenderansicht mit den folgenden Optionen ändern:

   <!--   * To include or exclude weekends:
      1. On the **[!UICONTROL Calendar]** toolbar, click **[!UICONTROL Calendar Actions]**, then from the drop-down list select either **[!UICONTROL Show Weekend]** or **[!UICONTROL Hide Weekend]**.-->

   * So ändern Sie die angezeigten Daten schnell:

      1. Klicken Sie in **[!UICONTROL Kalender]**-Symbolleiste auf den linken Pfeil der Datumsanzeige, um im Kalender zurückzukehren, oder auf den rechten Pfeil, um fortzufahren.

         ![Auf Pfeil klicken, um Datum zu ändern](assets/click-arrows-to-change-dates-calendar-report.png)

         Die angezeigten Datumswerte werden durch ein Intervall angepasst, das auf Ihrer aktuellen Kalenderansicht basiert. Wenn Sie z. B. den Kalender in der Ansicht **Woche** anzeigen, wird der Kalender je nach ausgewähltem Pfeil entweder eine Woche vor oder eine Woche zurück angezeigt.

      1. (Optional) Um zum aktuellen Tag zurückzukehren, klicken Sie auf [!UICONTROL **Heute**].

1. (Optional) Um die Ereignisse für ein mit dem Kalender verknüpftes Projekt oder eine mit dem Kalender verknüpfte Kalendergruppierung auszublenden, löschen Sie das Projekt oder die Kalendergruppierung in der Projektliste.
   ![Ereignisse ausblenden](assets/hide-events-for-project-or-cal-grouping.png)
Sie können die Ereignisse wieder anzeigen, indem Sie das [!UICONTROL Projekt] oder die Kalendergruppierung in der Projektliste auswählen.

## Kalenderbericht-Ereignisdetails anzeigen

Sie können die Details eines Ereignisses in einem Kalender für aktuelle und vergangene Ereignisse anzeigen.

1. Navigieren Sie zum Ereignis, für das Sie die Details wissen möchten, und klicken Sie dann auf das Ereignis. Die Details werden in einem Bedienfeld auf der rechten Seite geöffnet.
1. (Optional) Klicken Sie auf den Titel des Objekts, um das verknüpfte Projekt, die zugehörige Aufgabe oder das zugehörige Problem zu öffnen.
