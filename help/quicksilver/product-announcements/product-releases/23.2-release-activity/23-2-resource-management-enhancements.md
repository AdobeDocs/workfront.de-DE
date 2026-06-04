---
title: Verbesserungen beim Ressourcen-Management in Version 23.2
description: Verbesserungen beim Ressourcen-Management in Version 23.2
author: Courtney
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: b225ae19-eee7-4329-a42d-2a2bf9adad01
TQID: https://experienceleague.adobe.com/QzjHfD9RX0nF8Bk84Rq3yFTJvQpKMJPq9YmIXjJ9QJw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 277
ht-degree: 8%

---

# Verbesserungen beim Ressourcen-Management in Version 23.2

Auf dieser Seite werden alle Verbesserungen beim Ressourcenmanagement beschrieben, die mit Version 23.2 an der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden mit Version 23.2 in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im Versionszyklus 23.2 verfügbar sind, finden Sie unter Übersicht über Version [23.2](/help/quicksilver/product-announcements/product-releases/23.2-release-activity/23-2-release-overview.md).

## Einführung in das Feld Arbeitszeit zur korrekten Berechnung der Benutzerkapazität

>[!NOTE]
>
>Vorschau-Version: 16. Februar 2023; geplante Produktionsversion: 2. März 2023

Damit Ressourcenmanager die Verfügbarkeit ihrer Benutzer genau berechnen und die Zeit berücksichtigen können, die Benutzer für die tatsächliche, projektbezogene Arbeit aufwenden, führen wir das Arbeitszeitkonzept in Adobe Workfront ein.

Sie können den Wert des Felds Arbeitszeit für jeden Benutzer definieren, wenn Sie dessen Profil erstellen oder bearbeiten. Weitere Informationen finden Sie [Bearbeiten des Benutzerprofils](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

Das Feld Arbeitszeit gibt den Prozentsatz der Vollzeitäquivalenzzeit (FTE) an, die der Benutzer für die tatsächliche Arbeit zur Verfügung hat, ohne Gemeinkosten. Die Arbeitszeit muss eine Dezimalzahl mit einem Wert zwischen 0 und 1 sein. So würde beispielsweise eine Verfügbarkeit von 20 % für die tatsächliche Arbeit 0,2 betragen.

Der Standardwert des Feldes ist 1. Dies bedeutet, dass ein Benutzer sein gesamtes FTE für die tatsächliche, projektbezogene Arbeit verwendet.

Als Ergebnis dieser Aktualisierung berechnet Workfront die Verfügbarkeit der Benutzenden anhand der unten stehenden Formeln und hängt von der Auswahl im Bereich „Voreinstellungen für die Ressourcenverwaltung“ ab:

* Standardzeitplan:
* Benutzerkapazität = [(Geplante Stunden - Zeitplanausnahmen) `*` VZÄ - Auszeiten] `*` Arbeitszeit
* Zeitplan des Benutzers:
* Benutzerkapazität = (Geplante Stunden - Zeitplanausnahmen - Ausfallzeit) `*` Arbeitszeit.

Weitere Informationen finden Sie unter [Konfigurieren von [!UICONTROL Ressourcenverwaltung] Einstellungen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

[Sehen Sie sich eine Videodemonstration zu dieser Funktion an](https://video.tv.adobe.com/v/3415608/){target=_blank}
