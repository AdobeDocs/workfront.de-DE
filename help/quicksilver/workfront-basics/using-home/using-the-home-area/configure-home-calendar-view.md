---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: Einstellungen für die Ansicht des Home-Kalenders konfigurieren
description: Sie können die Einstellungen des Home-Kalenders so konfigurieren, dass sie in eine webbasierte Version von Outlook integriert werden, und Sie können Ihre Arbeitslast anhand Ihrer verfügbaren Arbeitszeiten verfolgen.
author: Nolan
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 1%

---

# Ansichtseinstellungen für den [!UICONTROL Home-Kalender] konfigurieren

<!--Audited: 01/2024-->

Sie können die Einstellungen für [!UICONTROL Home Calendar] wie folgt konfigurieren:

* Integration mit einer Web-basierten Version von [!DNL Outlook] in [!DNL Office 365] oder [!DNL Outlook Live] auf der Cloud. Sie können alle Ereignisse aus Ihrem Outlook-Kalender sowie alle zugehörigen Kalender anzeigen, die Sie in Ihrem [!UICONTROL Home-Kalender] in Adobe Workfront auswählen.
* Helfen Sie Ihnen, Ihre Arbeitslast anhand der verfügbaren Arbeitszeiten in der Symbolleiste [!UICONTROL Zuordnung] zu verfolgen.

Weitere Informationen zum Home-Kalender finden Sie unter [[!UICONTROL Home Calendar] view](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

In diesem Artikel wird beschrieben, wie Sie die Einstellungen des Home-Kalenders konfigurieren und den Home-Kalender in Ihren externen Outlook-Kalender integrieren können.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>Aktuell: [!UICONTROL Arbeit] oder höher</p> 
   Oder
   <p>Neu: [!UICONTROL Standard]</p> 
   </td> 
  </tr> 
   </tbody> 
</table>

*Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan oder welchen Lizenztyp Sie haben. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Über die Integration von [!DNL Microsoft Outlook]-Kalendern

Beachten Sie Folgendes bei der Konfiguration Ihres Home-Kalenders mit Ihrem [!DNL Microsoft Outlook] -Kalender:

* Sie können nur eine webbasierte Version von [!DNL Outlook] in Cloud-gehostete [!DNL Office 365] oder [!DNL Outlook Live] integrieren.

  On-Premise [!DNL Outlook] und [!DNL Outlook] auf einem Cloud-basierten Enterprise [!DNL Exchange]-Server werden nicht unterstützt.

  Wenn Ihr Unternehmen Single Sign-On verwendet, benötigen Sie [!DNL Microsoft 365 E3] oder [!DNL E5].

* Anlagen, die mit Ihren [!DNL Outlook] -Ereignissen verknüpft sind, sind nicht an die [!DNL Outlook] -Ereignisse in Ihrem Home-Kalender angehängt.
* Die Integration in einen [!DNL Outlook] -Kalender muss für jeden Benutzer einzeln abgeschlossen sein.
* Ereignisse, die in der Leiste [!UICONTROL Fälligkeit] erscheinen, werden nicht in Ihrem [!DNL Microsoft] Kalender angezeigt, es sei denn, Sie haben sie aus der [!UICONTROL Arbeitsliste] in Ihren [!DNL Adobe Workfront] Kalender gezogen. Weitere Informationen finden Sie unter [[!UICONTROL Fälligkeit] Leiste](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) und [Liste &quot;Arbeit&quot;im [!UICONTROL Home-Kalender]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) in der Ansicht [[!UICONTROL Home Calendar]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* Wenn Sie die Integration mit [!DNL Outlook] aktivieren, werden nur Arbeitselemente synchronisiert, die ab diesem Zeitpunkt in den [!UICONTROL Home Calendar] gezogen werden. Elemente, die sich vor der Aktivierung der Integration im Home-Kalender befanden, werden nicht angezeigt. Sie müssen sie erneut in den Home-Kalender ziehen, wenn sie in [!DNL Outlook] angezeigt werden sollen.
* Wenn Sie einen [!DNL Outlook] -Kalender für andere Personen freigeben (oder die Freigabe aufheben) oder die Berechtigungsstufe für einen Kalender ändern, den Sie für andere freigeben, wirkt sich diese Änderung nicht auf deren Kalender aus (ca. 30 Minuten). Weitere Informationen finden Sie in der Dokumentation zu [!DNL Microsoft Outlook] .\
   Wenn Sie also [!DNL Workfront] Kalender in einen [!DNL Outlook] -Kalender integrieren, den Sie für andere Benutzer freigeben, werden diese Ihre [!DNL Workfront] Kalenderelemente für ca. 30 Minuten nicht sehen.

>[!NOTE]
>
>Die Kalenderkonfiguration [!DNL Outlook] ist vollständig getrennt vom [!DNL Outlook] Add-in ([!UICONTROL [!DNL Outlook] Integration] oder [!DNL Workfront Outlook]). Es ist keine Installation erforderlich, um den Kalender zu konfigurieren, aber es ist eine Installation für das [!DNL Outlook]-Add-in erforderlich. Weitere Informationen zum [!DNL Outlook] Add-In finden Sie unter [Einrichten [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## Konfigurieren Sie die Anzeigeeinstellungen für den [!UICONTROL Home-Kalender] und integrieren Sie sie in Outlook-Kalender.

1. Klicken Sie in der Ansicht [!UICONTROL Home Calendar] auf das Zahnradsymbol **[!UICONTROL Einstellungen]** ![Calendar_Settings_Zahnradsymbol.png](assets/calendar-settings-gear-icon.png) oben rechts, um das Bedienfeld **[!UICONTROL Kalendereinstellungen]** auf der rechten Seite zu öffnen.

   Informationen zum Zugriff auf die Ansicht [!UICONTROL Home Calendar] finden Sie unter [Anzeigen des [!UICONTROL Home Calendar]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. (Optional) Um Ihren [!DNL Microsoft Outlook] -Kalender zu integrieren, klicken Sie oben rechts im Bedienfeld **[!UICONTROL Kalendereinstellungen]** auf **[!UICONTROL Konto hinzufügen]** . Geben Sie dann, wenn Sie dazu aufgefordert werden, Ihre [!DNL Microsoft Outlook] Anmeldedaten ein. Sie können diesen Schritt wiederholen, um mehrere [!DNL Outlook] -Konten hinzuzufügen.

   >[!NOTE]
   >
   >Sie müssen [!DNL Workfront] die Berechtigung erteilen, auf Ihren [!DNL Outlook] -Kalender zuzugreifen. Durch die Erteilung der Berechtigung kann [!DNL Workfront] den Zugriff auf Kalenderdaten aufrechterhalten, Ihr [!DNL outlook] -Profil lesen und Ihren [!DNL Microsoft] -Kalender lesen und aktualisieren.

1. Aktualisieren Sie das Browser-Fenster, um Informationen aus Ihrem [!DNL Outlook] -Konto im Kalender und im Bedienfeld [!UICONTROL Kalendereinstellungen] anzuzeigen.
1. Klicken Sie erneut oben rechts auf das Zahnradsymbol **[!UICONTROL Einstellungen]** , um das Bedienfeld **[!UICONTROL Kalendereinstellungen]** zu öffnen. ![Calendar_Settings_Zahnrad_icon.png](assets/calendar-settings-gear-icon.png)

1. (Optional) Wählen Sie unter jedem [!DNL Microsoft] -Konto, das Sie im vorherigen Schritt hinzugefügt haben, **[!UICONTROL Ansicht]** oder **[!UICONTROL Synchronisation]** aus:

   * **[!UICONTROL Ansicht]**: Dies ist eine schreibgeschützte Option, mit der [!DNL Microsoft] Kalenderereignisse im [!UICONTROL Home-Kalender] angezeigt werden.
   * **[!UICONTROL Sync]**: Diese Option ermöglicht eine bidirektionale Synchronisation zwischen Ihren [!DNL Microsoft]- und [!UICONTROL Home]-Kalendern. Mit anderen Worten: [!DNL Workfront] [!UICONTROL Home Calendar] -Elemente werden in Ihren [!DNL Microsoft] Kalender und in Ihren [!DNL Microsoft] -Kalendereintrag in Echtzeit in Ihren Workfront [!UICONTROL Home Calendar] importiert.

     ![](assets/view-sync-checkboxes-qs.png)

1. (Optional) Wählen Sie unter Ihrem [!DNL Workfront] -Konto oder einem integrierten Konto die zugehörigen Kalender aus, die Sie im [!UICONTROL Home Calendar] anzeigen möchten (z. B. Ihren PTO-, Geburtstags- oder Feiertagskalender), und klicken Sie dann auf die Schaltfläche [!UICONTROL Aktualisieren] oder [!UICONTROL Neu laden] Ihres Browsers, um Ihre Änderungen anzuzeigen.

1. (Optional) Wählen Sie im Abschnitt **[!UICONTROL Allgemein]** unter **[!UICONTROL Woche starten am]** den Tag aus, der als erster Tag Ihrer Arbeitswoche im Home-Kalender angezeigt werden soll.

   ![](assets/general-section-home-calendar-settings-panel.png)

1. Konfigurieren Sie die folgenden Optionen:

   * **[!UICONTROL Meine Arbeitstage]:** Wählen Sie die Arbeitstage aus.
   * **[!UICONTROL Meine übliche Startzeit]:** Wählen Sie die Zeit aus, zu der Sie Ihren Arbeitstag beginnen.
   * **[!UICONTROL Meine übliche Endzeit]:** Wählen Sie die Zeit aus, zu der Sie Ihren Arbeitstag beenden.

   [!DNL Workfront] verwendet diese drei Einstellungen, um die Anzahl der Stunden zu berechnen, die Sie in einer Woche arbeiten. Diese Zahl wirkt sich auf die Leiste [!UICONTROL Zuordnung] aus, mit der Sie Ihre Arbeitslast anhand Ihrer verfügbaren Arbeitszeiten nachverfolgen können. Weitere Informationen finden Sie unter [[!UICONTROL Zuordnung] bar](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) im Artikel [[!UICONTROL Home Calendar] view](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. Klicken Sie außerhalb des Bereichs **[!UICONTROL Kalendereinstellungen]** , um ihn zu schließen.

   [!DNL Workfront] speichert Ihre Änderungen automatisch.

Informationen zur Verwendung der Ansicht [!UICONTROL Kalender] zur Verwaltung Ihrer Arbeitszuweisungen und integrierten Kalenderereignisse finden Sie unter [Verwenden der Ansicht [!UICONTROL Home Calendar]](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
