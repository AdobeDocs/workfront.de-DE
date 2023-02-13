---
user-type: administrator
content-type: reference;overview
product-area: system-administration
navigation-topic: system-tracked-update-feeds
title: Vom System verfolgte Aktualisierungen
description: Adobe Workfront erfasst die Aktivität, die auf bestimmten Objekten stattfindet, indem Statusinformationen im Objekt protokolliert werden. [!UICONTROL Updates] Bereich.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c88823a7-100b-40dd-b4f1-bead53ae5dc4
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '238'
ht-degree: 5%

---

# Vom System verfolgte Aktualisierungen

[!DNL Adobe Workfront] erfasst die Aktivität, die auf bestimmten Objekten stattfindet, indem Statusinformationen in der [!UICONTROL Updates] Bereich.

Die [!UICONTROL Updates] umfasst die folgenden Aktualisierungstypen:

* **Benutzeraktualisierungen:** Manuelle Eingabe durch Benutzer. Auch als Kommentare, Antworten und Anmerkungen bezeichnet.

   ![](assets/updates-qs-350x125.png)

* **Systemaktualisierungen:** Automatisch vom System erstellt. Eine Systemaktualisierung enthält einen kurzen Hinweis, in dem beschrieben wird, welche Art von Änderung am Artikel vorgenommen wurde.

   <!--
  DRAFTED IN FLARE:
  Timestamps for system updates are based on your operating system's timezone.
  
  -->

Die folgenden Objekte können aktualisiert werden:

* Projekt
* Aufgabe
* Anfrage
* Portfolio
* Programm
* Benutzer
* Vorlagen
* Vorlagenaufgaben
* Dokumente
* Arbeitszeittabellen

Ihre [!DNL Workfront] -Lizenz bestimmt, ob Systemaktualisierungen standardmäßig in der [!UICONTROL Updates] Objektbereich. [!DNL Workfront] Benutzern mit [!UICONTROL Plan] -Lizenz die Anzeige von Systemaktualisierungen im [!UICONTROL Updates] standardmäßig ein. Benutzer können jedoch Systemaktualisierungen herausfiltern, wie im Abschnitt [[!UICONTROL Aktivieren] oder deaktivieren Sie Systemaktualisierungen](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#enable) Abschnitt in [Update der Arbeit](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md). Alle anderen [!DNL Workfront] -Lizenzen Filtersystemaktualisierungen standardmäßig.

[!DNL Workfront] Administratoren können festlegen, welche Arten von Änderungen das System im [!UICONTROL Updates] Bereich. Nicht alle Objekte verfügen über konfigurierbare [!UICONTROL update] Status-Feeds. Die folgenden Objekte haben eine [!UICONTROL Updates] -Bereich, der vom System getrackte Update-Feeds erfasst, aber keine konfigurierbaren Update-Status-Feeds hat:

* Vorlagen
* Vorlagenaufgaben
* Dokumente
* Arbeitszeittabellen

Weitere Informationen zu System-Update-Feeds und deren Aktivierung finden Sie unter [Systemaktualisierungen konfigurieren](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md). Weitere Informationen zum Konfigurieren von Benutzeraktualisierungen finden Sie unter [Voreinstellungen für Benutzeraktualisierungen konfigurieren](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).
