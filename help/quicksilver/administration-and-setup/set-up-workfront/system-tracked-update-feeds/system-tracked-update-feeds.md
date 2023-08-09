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
source-git-commit: 413e5ff710b4c77b7ea2d870b34bb0627a4fcd86
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 6%

---

# Vom System getrackte Aktualisierungen

[!DNL Adobe Workfront] erfasst die Aktivität, die auf bestimmten Objekten stattfindet, indem Statusinformationen in der [!UICONTROL Updates] Bereich.

Die [!UICONTROL Updates] umfasst die folgenden Aktualisierungstypen:

* **Benutzeraktualisierungen:** Manuelle Eingabe durch Benutzer. Auch als Kommentare, Antworten und Anmerkungen bezeichnet.

  Weitere Informationen zum Konfigurieren von Benutzeraktualisierungen finden Sie unter [Voreinstellungen für Benutzeraktualisierungen konfigurieren](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

  ![](assets/updates-qs-350x125.png)

* **Systemaktualisierungen:** Automatisch vom System erstellt. Eine Systemaktualisierung enthält einen kurzen Hinweis, in dem beschrieben wird, welche Art von Änderung am Artikel vorgenommen wurde.

  Weitere Informationen zu System-Update-Feeds und deren Aktivierung finden Sie unter [Systemaktualisierungen konfigurieren](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md).

  <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

## Überlegungen zu systemverfolgten Aktualisierungen

* Vom System getrackte Aktualisierungen sind nicht für alle Objekte mit dem Bereich Updates verfügbar. Die [!UICONTROL Updates] Bereich ist für die folgenden Objekte verfügbar:

   * [!UICONTROL Projekt]
   * [!UICONTROL Aufgabe]
   * [!UICONTROL Probleme]
   * [!UICONTROL Portfolio]
   * [!UICONTROL Programm]
   * [!UICONTROL Benutzerin oder Benutzer]
   * [!UICONTROL Vorlage]
   * [!UICONTROL Vorlagenaufgabe]
   * [!UICONTROL Team]
   * [!UICONTROL Dokument]
   * [!UICONTROL Arbeitszeittabelle]
   * [!UICONTROL Story]

     In [!DNL Workfront], eine Geschichte ist eine Aufgabe.
   * [!UICONTROL Wiederholung]
   * [!UICONTROL Ziel]

     Sie benötigen eine zusätzliche Lizenz, um Zugriff auf die [!UICONTROL Ziele] Bereich. Weitere Informationen finden Sie unter [Voraussetzungen für die Verwendung von Workfront-Zielen](../../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
   * [!UICONTROL Karte] auf einer Pinnwand

     Weitere Informationen zu Kartenaktualisierungen finden Sie unter [Hinzufügen einer Ad-hoc-Karte zu einer Pinnwand](../../../agile/get-started-with-boards/add-card-to-board.md).


* [!DNL Workfront] verfolgt keine Systemaktualisierungen für die folgenden Objekte:

   * [!UICONTROL Team]
   * [!UICONTROL Vorlage]
   * [!UICONTROL Vorlagenaufgabe]

<!--hiding this bit because this is not true, at this time (August 2023). Users with a Work or Review license can see system updates by default as well.

Your [!DNL Workfront] license determines whether system updates display by default in the [!UICONTROL Updates] area of objects. [!DNL Workfront] users with a [!UICONTROL Plan] license have system updates displayed in the [!UICONTROL Updates] area by default. However, users can filter out system updates, as described in the [Enable or disable system updates](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) section in [Update work](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). All other [!DNL Workfront] licenses filter system updates by default.
-->

* Die Benutzer können Systemaktualisierungen standardmäßig anzeigen oder sie nicht anzeigen lassen.

  Informationen zum Deaktivieren der Anzeige von Systemaktualisierungen finden Sie im Abschnitt . [Systemaktualisierungen aktivieren oder deaktivieren](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) im Artikel [Update der Arbeit](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

  >[!NOTE]
  >
  >Wir gestalten derzeit das Kommentierungserlebnis und die [!UICONTROL Updates] Gebiet in [!DNL Workfront].
  >
  > Systemaktualisierungen können bei der Verwendung des neuen Kommentierungserlebnisses nicht ausgeblendet werden.
  > 
  >Weitere Informationen zum neuen Kommentierungserlebnis finden Sie unter [Neues Kommentierungserlebnis](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).

* Workfront zeichnet vom System getrackte Aktualisierungen für die folgenden Objekte auf, es gibt jedoch keine Option, die Anzeige zu deaktivieren:

   * [!UICONTROL Portfolio]
   * [!UICONTROL Programm]
   * [!UICONTROL Wiederholung]

* [!DNL Workfront] Administratoren können festlegen, welche Arten von Änderungen das System im [!UICONTROL Updates] Bereich. Nicht alle Objekte mit [!UICONTROL Updates] -Bereich auch konfigurierbar [!UICONTROL update] Feeds. Die folgenden Objekte haben eine [!UICONTROL Updates] -Bereich, der vom System getrackte Update-Feeds erfasst, aber keine konfigurierbaren Update-Feeds hat:

   * [!UICONTROL Dokument]
   * [!UICONTROL Arbeitszeittabelle]
   * [!UICONTROL Wiederholung]

