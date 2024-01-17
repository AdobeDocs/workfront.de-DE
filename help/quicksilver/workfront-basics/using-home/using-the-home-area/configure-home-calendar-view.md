---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: Einstellungen für die Ansicht des Home-Kalenders konfigurieren
description: Sie können die Einstellungen des Home-Kalenders so konfigurieren, dass sie in eine webbasierte Version von Outlook integriert werden, und Sie können Ihre Arbeitslast anhand Ihrer verfügbaren Arbeitszeiten verfolgen.
author: Nolan
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: 644e2487dae0d3b2f7931660fb8e6ed68e6b8b93
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---

# Konfigurieren Sie Ihre [!UICONTROL Startseitenkalender] Ansichtseinstellungen

Sie können die [!UICONTROL Startseitenkalender] -Einstellungen, um Folgendes zu tun:

* Integration in eine webbasierte Version von [!DNL Outlook] in Cloud-gehostet [!DNL Office 365] oder [!DNL Outlook Live]. Sie können alle Ereignisse aus Ihrem Outlook-Kalender sowie alle von Ihnen ausgewählten Kalender, wie z. B. Geburtstage und Feiertage-Kalender, in Ihren [!UICONTROL Startseitenkalender].
* Helfen Sie Ihnen, Ihre Arbeitslast anhand der verfügbaren Arbeitszeiten auf der [!UICONTROL Zuordnung] Bar.

Weitere Informationen zum Home-Kalender finden Sie unter [[!UICONTROL Startseitenkalender] Ansicht](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

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
   <td> <p>[!UICONTROL Arbeit] oder höher</p> </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Über die Integration [!DNL Microsoft Outlook] Kalender

Beachten Sie Folgendes, wenn Sie Ihren Home-Kalender mit Ihrem [!DNL Microsoft Outlook] calendar:

* Sie können nur eine webbasierte Version von [!DNL Outlook] in Cloud-gehostet [!DNL Office 365] oder [!DNL Outlook Live].

  Vor Ort [!DNL Outlook] und [!DNL Outlook] auf einem Cloud-basierten Unternehmen [!DNL Exchange] -Server werden nicht unterstützt.

  Wenn Ihr Unternehmen Single Sign-On verwendet, benötigen Sie [!DNL Microsoft 365 E3] oder [!DNL E5].

* Anlagen, die mit Ihrer [!DNL Outlook] -Ereignisse nicht an die [!DNL Outlook] Ereignisse in Ihrem Home-Kalender.
* Integration mit einer [!DNL Outlook] Der Kalender muss für jeden Benutzer einzeln ausgefüllt werden.
* Ereignisse, die in [!UICONTROL aufgrund] Die Leiste wird nicht in Ihrer [!DNL Microsoft] Kalender, es sei denn, Sie haben sie aus dem [!UICONTROL Arbeitsliste] auf [!DNL Adobe Workfront] Kalender. Weitere Informationen finden Sie unter [[!UICONTROL aufgrund] bar](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) und [Arbeitsliste auf der [!UICONTROL Startseitenkalender]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) in [[!UICONTROL Startseitenkalender] Ansicht](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* Wenn Sie die Integration mit [!DNL Outlook], nur Arbeitselemente, die auf die [!UICONTROL Startseitenkalender] ab diesem Zeitpunkt synchronisiert. Elemente, die sich vor der Aktivierung der Integration im Home-Kalender befanden, werden nicht angezeigt. Sie müssen sie erneut in den Home-Kalender ziehen, wenn Sie sie in [!DNL Outlook].
* Wenn Sie eine [!DNL Outlook] Kalender mit anderen Personen oder wenn Sie die Berechtigungsebene für einen Kalender ändern, den Sie für andere freigeben, wirkt sich diese Änderung nicht auf deren Kalender aus (weitere Informationen finden Sie unter [!DNL Microsoft Outlook] Dokumentation).\
   Wenn Sie die [!DNL Workfront] Kalender mit [!DNL Outlook] Kalender, den Sie für andere Benutzer freigeben, sehen diese Ihre [!DNL Workfront] Kalendereinträge für ca. 30 Minuten.

>[!NOTE]
>
>Die [!DNL Outlook] Die Kalenderkonfiguration ist vollständig von der [!DNL Outlook] Add-in ([!UICONTROL [!DNL Outlook] Integration] oder [!DNL Workfront Outlook]). Es ist keine Installation erforderlich, um den Kalender zu konfigurieren, es ist jedoch eine Installation für die [!DNL Outlook] Add-In. Weitere Informationen über [!DNL Outlook] Add-In siehe [Einrichten [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## Konfigurieren Sie Ihre [!UICONTROL Startseitenkalender] Ansichtseinstellungen

1. Im [!UICONTROL Startseitenkalender] Ansicht, klicken Sie auf die **[!UICONTROL Einstellungen]** Zahnradsymbol ![Calendar_Settings_Zahnradsymbol.png](assets/calendar-settings-gear-icon.png) in der oberen rechten Ecke, um die **[!UICONTROL Kalendereinstellungen]** auf der rechten Seite des Fensters angezeigt.

   Wenn Sie Informationen zum Zugriff auf die [!UICONTROL Startseitenkalender] Ansicht, siehe [Anzeigen der [!UICONTROL Startseitenkalender]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. (Optional) So integrieren Sie Ihre [!DNL Microsoft Outlook] Kalender, klicken Sie **[!UICONTROL Konto hinzufügen]** in der oberen rechten Ecke des **[!UICONTROL Kalendereinstellungen]** Bedienfeld. Wenn Sie dazu aufgefordert werden, geben Sie [!DNL Microsoft Outlook] Login-Informationen. Sie können diesen Schritt wiederholen, um mehrere [!DNL Outlook] Konten.

   >[!NOTE]
   >
   >Du musst geben [!DNL Workfront] Zugriffsberechtigung für Ihre [!DNL Outlook] Kalender. Genehmigungen erteilen [!DNL Workfront] Lesen Sie Ihre [!DNL outlook] Profil erstellen und Ihre [!DNL Microsoft] Kalender.

1. Aktualisieren Sie das Browser-Fenster, um Informationen aus Ihrem [!DNL Outlook] im Kalender und im [!UICONTROL Kalendereinstellungen] Bedienfeld.
1. Klicken Sie auf **[!UICONTROL Einstellungen]** Zahnradsymbol in der oberen rechten Ecke, um die **[!UICONTROL Kalendereinstellungen]** Bedienfeld. ![Calendar_Settings_Zahnradsymbol.png](assets/calendar-settings-gear-icon.png)

1. (Optional) Unter jedem [!DNL Microsoft] Konto, das Sie im vorherigen Schritt hinzugefügt haben, wählen Sie **[!UICONTROL Ansicht]** oder **[!UICONTROL Synchronisieren]**:

   * **[!UICONTROL Ansicht]**: Diese schreibgeschützte Option wird angezeigt. [!DNL Microsoft] Kalenderereignisse in Ihrer [!UICONTROL Startseitenkalender].
   * **[!UICONTROL Synchronisieren]**: Diese Option ermöglicht eine bidirektionale Synchronisation zwischen [!DNL Microsoft] und [!UICONTROL Startseite] Kalender. Mit anderen Worten: [!DNL Workfront] [!UICONTROL Startseitenkalender] -Elemente exportieren [!DNL Microsoft] Kalender und [!DNL Microsoft] Kalenderelemente in Workfront importieren [!UICONTROL Startseitenkalender] in Echtzeit.

     ![](assets/view-sync-checkboxes-qs.png)

1. (Optional) Unter Ihrer [!DNL Workfront] -Konto oder ein integriertes Konto die zugehörigen Kalender auswählen, die Sie auf Ihrem [!UICONTROL Startseitenkalender] (z. B. Ihr PTO-, Geburtstags- oder Feiertagskalender), klicken Sie dann auf die [!UICONTROL Aktualisieren] oder [!UICONTROL Neu laden] -Schaltfläche, um Ihre Änderungen anzuzeigen.

1. (Optional) Im **[!UICONTROL Allgemein]** Abschnitt unter **[!UICONTROL Woche beginnen am]** wählen Sie den Tag aus, den Sie als ersten Tag Ihrer Arbeitswoche im Startkalender anzeigen möchten.

1. Konfigurieren Sie die folgenden Optionen:

   * **[!UICONTROL Meine Arbeitstage]:** Wählen Sie die Arbeitstage aus.
   * **[!UICONTROL Meine übliche Startzeit]:** Wählen Sie den Zeitpunkt aus, zu dem Sie Ihren Arbeitstag beginnen.
   * **[!UICONTROL Meine übliche Endzeit]:** Wählen Sie die Zeit aus, zu der Sie Ihren Arbeitstag beenden.

   [!DNL Workfront] verwendet diese drei Einstellungen, um die Anzahl der Stunden zu berechnen, die Sie in einer Woche arbeiten. Diese Zahl wirkt sich auf die [!UICONTROL Zuordnung] -Leiste, die Ihnen dabei hilft, Ihre Arbeitslast anhand Ihrer verfügbaren Arbeitszeiten zu verfolgen. Weitere Informationen finden Sie unter [[!UICONTROL Zuordnung] bar](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) im Artikel [[!UICONTROL Startseitenkalender] Ansicht](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. Klicken Sie außerhalb der **[!UICONTROL Kalendereinstellungen]** -Bereich, um ihn zu schließen.

   [!DNL Workfront] speichert Ihre Änderungen automatisch.

Informationen zur Verwendung der [!UICONTROL Kalender] Informationen zur Verwaltung Ihrer Arbeitsaufgaben und integrierten Kalenderereignisse finden Sie unter [Verwenden Sie die [!UICONTROL Startseitenkalender] Ansicht](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
