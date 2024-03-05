---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Vom System getrackte Aktualisierungen
description: Adobe Workfront erfasst die Aktivität, die auf bestimmten Objekten stattfindet, indem Statusinformationen im Objekt protokolliert werden. [!UICONTROL Updates] Bereich.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: d76ab0e165d280f84718b52cc72a9b4c152a0897
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# Vom System getrackte Aktualisierungen

{{highlighted-preview}}

<!--remove new experience and legacy notes when we remove legacy in the UI - Jan 24???-->

[!DNL Adobe Workfront] erfasst die Aktivität, die auf bestimmten Objekten stattfindet, indem Statusinformationen in der [!UICONTROL Updates] Bereich.

Die [!UICONTROL Updates] umfasst die folgenden Aktualisierungstypen:

* **Benutzeraktualisierungen:** Manuelle Eingabe durch Benutzer. Auch als Kommentare, Antworten und Anmerkungen bezeichnet.

  Weitere Informationen zum Konfigurieren von Benutzeraktualisierungen finden Sie unter [Voreinstellungen für Benutzeraktualisierungen konfigurieren](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![](assets/updates-qs-350x125.png)

* **Systemaktualisierungen:** Automatisch vom System erstellt. Eine Systemaktualisierung enthält einen kurzen Hinweis, in dem beschrieben wird, welche Art von Änderung am Artikel vorgenommen wurde.

  Weitere Informationen zu System-Update-Feeds und deren Aktivierung finden Sie unter [Systemaktualisierungen konfigurieren](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  ![](assets/system-updates-example-unified-stream.png)

  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## Überlegungen zu systemverfolgten Aktualisierungen

Vom System getrackte Aktualisierungen sind nicht für alle Objekte mit dem Bereich Updates verfügbar.

* Die [!UICONTROL Updates] Bereich ist für die folgenden Objekte verfügbar:

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
   * [!UICONTROL Datenblatt]
   * [!UICONTROL Geschichte]

     In [!DNL Workfront], eine Geschichte ist eine Aufgabe.
   * [!UICONTROL Iteration]
   * [!UICONTROL Ziel]

     Sie benötigen eine zusätzliche Lizenz, um Zugriff auf die [!UICONTROL Ziele] Bereich. Weitere Informationen finden Sie unter [Voraussetzungen für die Verwendung von Workfront-Zielen](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL Karte] auf einer Pinnwand

     Weitere Informationen zu Kartenaktualisierungen finden Sie unter [Angeschlossene Karten auf Pinnwänden verwenden](../../../agile/get-started-with-boards/connected-cards.md).

* [!DNL Workfront] verfolgt keine Systemaktualisierungen für die folgenden Objekte:

   * [!UICONTROL Team]
   * [!UICONTROL Vorlage]
   * [!UICONTROL Vorlagenaufgabe]
   * Ad-hoc [!UICONTROL Karte]
   * [!UICONTROL Iterationen]


<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* Im Folgenden werden die Unterschiede zwischen dem neuen und dem alten Kommentierungserlebnis beschrieben:

   * Bei Verwendung des neuen Kommentierungserlebnisses werden Benutzeraktualisierungen auf der Registerkarte Kommentare angezeigt und Systemaktualisierungen werden auf der Registerkarte Systemaktivität angezeigt.

     Weitere Informationen zum neuen Kommentierungserlebnis finden Sie unter [Neues Kommentierungserlebnis](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

   * <span class="preview">Bei Verwendung der neuen Kommentarfunktion können Benutzer einem Systemupdate keinen Kommentar hinzufügen. Antworten, die auf Systemaktivitätsdatensätze im alten Kommentierungserlebnis erstellt wurden, werden jedoch auf der Registerkarte Systemaktivität auf der Registerkarte Systemaktivität als schreibgeschützt im neuen Kommentierungserlebnis eingetragen.</span>
   * Bei Verwendung des veralteten Kommentierungserlebnisses werden System- und Benutzeraktualisierungen in einem kontinuierlichen Feed angezeigt.

   * Bei der Verwendung des bisherigen Kommentierungserlebnisses können Benutzer standardmäßig Systemaktualisierungen anzeigen oder festlegen, dass sie nicht angezeigt werden. Die Deaktivierung von Systemaktualisierungen ist bei Verwendung des neuen Kommentierungserlebnisses nicht möglich.

     Informationen zum Deaktivieren der Anzeige von Systemaktualisierungen finden Sie im Abschnitt . [Systemaktualisierungen aktivieren oder deaktivieren](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) im Artikel [Update der Arbeit](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

* Workfront zeichnet vom System getrackte Aktualisierungen für die folgenden Objekte auf, es gibt jedoch keine Option, die Anzeige zu deaktivieren:

   * [!UICONTROL Portfolio]
   * [!UICONTROL Programm]
   * [!UICONTROL Iteration]

* [!DNL Workfront] Administratoren können festlegen, welche Arten von Änderungen das System im [!UICONTROL Updates] Bereich. Nicht alle Objekte mit [!UICONTROL Updates] -Bereich auch konfigurierbar [!UICONTROL update] Feeds. Die folgenden Objekte haben eine [!UICONTROL Updates] -Bereich, der vom System getrackte Update-Feeds erfasst, aber keine konfigurierbaren Update-Feeds hat:

   * [!UICONTROL Dokument]
   * [!UICONTROL Datenblatt]
   * [!UICONTROL Iteration]
   * [!UICONTROL Ziel]


