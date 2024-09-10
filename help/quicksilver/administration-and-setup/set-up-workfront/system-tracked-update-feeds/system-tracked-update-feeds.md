---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Vom System verfolgte Aktualisierungen
description: Adobe Workfront erfasst die Aktivität, die auf bestimmten Objekten stattfindet, indem Statusinformationen im Bereich [!UICONTROL Aktualisierungen] des Objekts protokolliert werden.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: 439303273239549bb326c171be44eea321f5bb5f
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 0%

---

# Systemverfolgte Aktualisierungen

<!-- Audited: April, 2024-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>-->

[!DNL Adobe Workfront] erfasst die Aktivität, die auf bestimmten Objekten stattfindet, indem Statusinformationen im Abschnitt [!UICONTROL Aktualisierungen] des Objekts protokolliert werden.

Weitere Informationen zum Abschnitt Updates finden Sie unter [Überblick über den Abschnitt Updates](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

Der Bereich [!UICONTROL Updates] umfasst die folgenden Arten von Updates:

* **Benutzeraktualisierungen:** Von Benutzern manuell eingegeben. Auch als Kommentare, Antworten und Anmerkungen bezeichnet. Benutzeraktualisierungen werden auf den Registerkarten Kommentare und Alle im Abschnitt Updates eines Objekts angezeigt.

  Weitere Informationen zum Konfigurieren von Benutzeraktualisierungen finden Sie unter [Voreinstellungen für Benutzeraktualisierungen konfigurieren](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![](assets/updates-qs-350x125.png)

* **Systemaktualisierungen:** Wird automatisch vom System vorgenommen. Eine Systemaktualisierung enthält einen kurzen Hinweis, in dem beschrieben wird, welche Art von Änderung am Artikel vorgenommen wurde. Systemaktualisierungen werden in der Systemaktivität und auf den Registerkarten Alle im Abschnitt Updates eines Objekts angezeigt.

  Weitere Informationen zu System-Update-Feeds und deren Aktivierung finden Sie unter [Konfigurieren von Systemaktualisierungen](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  ![](assets/system-updates-example-unified-stream.png)


  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## Überlegungen zu systemverfolgten Aktualisierungen

Vom System getrackte Aktualisierungen sind nicht für alle Objekte mit dem Bereich Updates verfügbar.

* Der Bereich [!UICONTROL Aktualisierungen] ist für die folgenden Objekte verfügbar:

   * [!UICONTROL Projekt]
   * [!UICONTROL Aufgabe]
   * [!UICONTROL Probleme]
   * [!UICONTROL Portfolio]
   * [!UICONTROL Programm]
   * [!UICONTROL Benutzer]
   * [!UICONTROL Vorlage]
   * [!UICONTROL Vorlagenaufgabe]
   * [!UICONTROL Team]
   * [!UICONTROL Document]
   * [!UICONTROL Zeitblatt]
   * [!UICONTROL Geschichte]

     In [!DNL Workfront] ist eine Geschichte eine Aufgabe.
   * [!UICONTROL Iteration]
   * [!UICONTROL Ziel]

     Sie müssen über eine zusätzliche Lizenz verfügen, um Zugriff auf den Bereich [!UICONTROL Ziele] zu haben. Weitere Informationen finden Sie unter [Voraussetzungen für die Verwendung von Workfront-Zielen](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL Karte] auf einer Pinnwand

     Weitere Informationen zu Aktualisierungen auf Karten finden Sie unter [Verwenden Sie verbundene Karten auf Pinnwänden](../../../agile/get-started-with-boards/connected-cards.md).

* [!DNL Workfront] verfolgt keine Systemaktualisierungen für die folgenden Objekte:

   * [!UICONTROL Team]
   * [!UICONTROL Vorlage]
   * [!UICONTROL Vorlagenaufgabe]
   * Ad-hoc-Karte [!UICONTROL Karte]
   * [!UICONTROL Iterationen]


<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* Benutzeraktualisierungen werden auf der Registerkarte Kommentare angezeigt und Systemaktualisierungen werden auf den Registerkarten Systemaktivität und Alle angezeigt.

  Eine Liste der Objekte, die nicht über die Registerkarten &quot;Systemaktivität&quot;oder &quot;Alle&quot;verfügen, finden Sie unter [Übersicht über den Abschnitt &quot;Aktualisieren&quot;](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)

* Sie können einer Systemaktualisierung keine Antwort hinzufügen. Antworten, die vor dem 11. April 2024 auf Systemaktivitätsdatensätze im alten Kommentierungserlebnis erstellt wurden, werden jedoch auf der Registerkarte Systemaktivität als schreibgeschützt ausgefüllt.

<!--
* The following are differences between the new and the legacy commenting experience: 

   * When using the new commenting experience, user updates display in the Comments tab and system updates display in the System Activity <span class="preview">and the All</span> tabs.  

      For more information about the new commenting experience, see [New commenting experience](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

      <span class="preview">For a list of objects that do not have the System Activity or the All tabs, see [Update section overview](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)</span>

   * <span class="preview">When using the new commenting experience, you cannot add a comment to a system update. However, any replies made to system activity records in the legacy commenting experience are populated on the System Activity tab as read-only in the new commenting experience.</span>
   * When using the legacy commenting experience, the system and user updates display in one continuous feed. 

   * When using the legacy commenting experience, users can view system updates by default or they can choose to not display them. Disabling system updates is not possible when using the new commenting experience. 

      For information about disabling the display of system updates, see the section [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) in the article [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).  

   * <span class="preview">The legacy commenting experience has been disabled in the Preview environment. For more information, see [Second Quarter 2024 Update stream and notification enhancements](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-update-stream-enhancements.md).</span>
-->

* [!DNL Workfront] -Administratoren können festlegen, welche Art von Änderungen das System im Bereich [!UICONTROL Aktualisierungen] verfolgen soll. Nicht alle Objekte mit dem Bereich [!UICONTROL Aktualisierungen] verfügen auch über konfigurierbare [!UICONTROL Update]-Feeds. Die folgenden Objekte verfügen über den Bereich [!UICONTROL Aktualisierungen] , der vom System getrackte Update-Feeds erfasst, aber keine konfigurierbaren Update-Feeds aufweist:

   * [!UICONTROL Document]
   * [!UICONTROL Zeitblatt]
   * [!UICONTROL Iteration]
   * [!UICONTROL Ziel]


