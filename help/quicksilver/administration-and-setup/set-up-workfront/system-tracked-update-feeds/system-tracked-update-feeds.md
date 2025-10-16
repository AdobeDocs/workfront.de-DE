---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Übersicht über die vom System verfolgten Aktualisierungen
description: Adobe Workfront erfasst die Aktivitäten, die an bestimmten Objekten stattfinden, indem Statusinformationen im Bereich [!UICONTROL Aktualisierungen] des Objekts protokolliert werden.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---

# Übersicht über die vom System verfolgten Aktualisierungen

<!-- Audited: 08/2025-->

[!DNL Adobe Workfront] erfasst die Aktivitäten, die an bestimmten Objekten stattfinden, indem Statusinformationen im Abschnitt [!UICONTROL Updates“ &#x200B;] Objekts protokolliert werden.

Weitere Informationen zum Abschnitt „Aktualisierungen“ finden Sie [Übersicht über den Abschnitt „Aktualisierungen](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md).

Der [!UICONTROL Updates] umfasst die folgenden Arten von Aktualisierungen:

* **Benutzeraktualisierungen:** von Benutzern manuell eingegeben. Auch als Kommentare, Antworten und Notizen bezeichnet. Benutzeraktualisierungen werden auf den Registerkarten „Kommentare“ und „Alle“ des Abschnitts „Aktualisierungen“ eines Objekts angezeigt.

  Weitere Informationen zum Konfigurieren von Benutzeraktualisierungen finden Sie unter [Konfigurieren von Voreinstellungen für Benutzeraktualisierungen](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![Updates](assets/updates-qs-350x125.png)

* **Systemaktualisierungen:** vom System automatisch vorgenommen. Eine Systemaktualisierung enthält einen kurzen Hinweis, der beschreibt, welche Änderungen am Element vorgenommen wurden. Systemaktualisierungen werden in der Systemaktivität und auf den Registerkarten Alle des Abschnitts Aktualisierungen eines Objekts angezeigt.

  Weitere Informationen zu Systemaktualisierungsfeeds und deren Aktivierung finden Sie unter [Systemaktualisierungen konfigurieren](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  ![Beispiel für Systemaktualisierungen](assets/system-updates-example-unified-stream.png)


  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## Überlegungen zu Aktualisierungen, die vom System verfolgt werden

System-getrackte Aktualisierungen sind nicht für alle Objekte verfügbar, die über den Bereich Aktualisierungen verfügen.

* Der [!UICONTROL Updates]-Bereich ist für die folgenden Objekte verfügbar:

   * [!UICONTROL Projekt]
   * [!UICONTROL Aufgabe]
   * [!UICONTROL Probleme]
   * [!UICONTROL Portfolio]
   * [!UICONTROL Programm]
   * [!UICONTROL Benutzer]
   * [!UICONTROL Vorlage]
   * [!UICONTROL Vorlagenaufgabe]
   * [!UICONTROL Team]
   * [!UICONTROL Dokument]
   * [!UICONTROL Arbeitszeittabelle]
   * [!UICONTROL Story]

     [!DNL Workfront] ist eine Geschichte eine Aufgabe.
   * [!UICONTROL Iteration]
   * [!UICONTROL Ziel]

     Nicht alle Workfront-Pakete enthalten Workfront Goals. Weitere Informationen finden Sie unter [Voraussetzungen für die Verwendung von Workfront-Zielen](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL Karte] auf einer Pinnwand

     Weitere Informationen zu Aktualisierungen auf Karten finden Sie unter [Verwenden von verbundenen Karten auf Pinnwänden](../../../agile/get-started-with-boards/connected-cards.md).

* [!DNL Workfront] verfolgt keine Systemaktualisierungen für die folgenden Objekte:

   * [!UICONTROL Team]
   * [!UICONTROL Vorlage]
   * [!UICONTROL Vorlagenaufgabe]
   * Ad-hoc [!UICONTROL Karte]
   * [!UICONTROL Iterationen]


<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* Benutzeraktualisierungen werden auf der Registerkarte Kommentare und Systemaktualisierungen auf den Registerkarten Systemaktivität und Alle angezeigt.

  Eine Liste der Objekte, die nicht über die Systemaktivität oder die Registerkarten „Alle“ verfügen, finden Sie [Update-Abschnitt - Übersicht](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/updates-tab-overview.md)

* Sie können keine Antwort auf eine Systemaktualisierung hinzufügen. Alle Antworten auf Systemaktivitätsdatensätze, die im alten Kommentar-Erlebnis vor dem 11. April 2024 eingegangen sind, werden jedoch auf der Registerkarte Systemaktivität schreibgeschützt eingetragen.

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

* [!DNL Workfront] Admins können im Bereich [!UICONTROL Updates“ festlegen, welche Änderungen das System &#x200B;] soll. Nicht alle Objekte mit einem [!UICONTROL Updates]-Bereich verfügen auch über konfigurierbare [!UICONTROL Update]-Feeds. Die folgenden Objekte haben einen Bereich [!UICONTROL Updates], der vom System verfolgte Update-Feeds erfasst, aber keine konfigurierbaren Update-Feeds hat:

   * [!UICONTROL Dokument]
   * [!UICONTROL Arbeitszeittabelle]
   * [!UICONTROL Iteration]
   * [!UICONTROL Ziel]


