---
title: 23.2 Verbesserungen bei der Ressourcenverwaltung
description: 23.2 Verbesserungen bei der Ressourcenverwaltung
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b225ae19-eee7-4329-a42d-2a2bf9adad01
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '271'
ht-degree: 0%

---

# 23.2 Verbesserungen bei der Ressourcenverwaltung

Auf dieser Seite werden alle Verbesserungen der Ressourcenverwaltung beschrieben, die mit Version 23.2 der Vorschaufunktion vorgenommen wurden. Diese Verbesserungen werden mit Version 23.2 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die derzeit im 23.2-Versionszyklus verfügbar sind, finden Sie unter [23.2 - Versionsübersicht](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## Einführung des Felds Arbeitszeit zur genauen Berechnung der Benutzerkapazität

>[!NOTE]
>
>Vorschau-Version: 16. Februar 2023; geplante Produktionsversion: 2. März 2023

Damit Ressourcenmanager die Verfügbarkeit ihrer Benutzer genau berechnen und die Zeit berücksichtigen können, die Benutzer tatsächlich projektbezogener Arbeit widmen, führen wir das Arbeitszeitkonzept für Adobe Workfront ein.

Sie können den Wert des Felds &quot;Arbeitszeit&quot;für jeden Benutzer definieren, wenn Sie sein Profil erstellen oder bearbeiten. Weitere Informationen finden Sie unter [Profil eines Benutzers bearbeiten](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Das Feld &quot;Arbeitszeit&quot;stellt den Prozentsatz der Vollzeitäquivalenzzeit (FTE) dar, die der Benutzer für die tatsächliche Arbeit zur Verfügung hat, ohne dass der Mehraufwand eingeschlossen ist. Die Arbeitszeit muss eine Dezimalzahl mit einem Wert zwischen 0 und 1 sein. Eine Verfügbarkeit von 20 % für tatsächliche Arbeit wäre beispielsweise 0,2.

Der Standardwert des Felds ist 1, was bedeutet, dass ein Benutzer seine gesamte FTE für tatsächliche, projektbezogene Arbeiten ausgibt.

Aufgrund dieser Aktualisierung berechnet Workfront die Verfügbarkeit des Benutzers anhand der unten stehenden Formeln, abhängig von Ihrer Auswahl im Bereich Voreinstellungen für die Ressourcenverwaltung:

* Standardzeitplan:
* Benutzerkapazität = [(Stunden planen - Ausnahmen planen) * FTE - Zeit ab ] * Arbeitszeit
* Benutzerzeitplan:
* Benutzerkapazität = (Zeitplanzeiten - Ausnahmen planen - Zeitlimit) * Arbeitszeit.

Weitere Informationen finden Sie unter [Konfigurieren der Voreinstellungen für die Ressourcenverwaltung]](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).[!UICONTROL 

[Sehen Sie sich eine Videodemonstration für diese Funktion an](https://video.tv.adobe.com/v/3415608/){target=_blank}
