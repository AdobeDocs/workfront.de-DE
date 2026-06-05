---
content-type: release-notes
title: Versionsaktivität 2026 für Adobe Workfront Eingeschränkte Verfügbarkeit - Funktionen
description: Dies ist die Veröffentlichungsaktivität für Funktionen mit begrenzter Verfügbarkeit in Adobe Workfront im zweiten Quartal 2026.
author: Lisa
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
hide: true
exl-id: 32c616b2-5bba-434e-9918-c27f6518693d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/8cp64ljvxCaGBh-1eGxVc6llJ6xFZwdBXur1AkIxaHk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 372
ht-degree: 3%

---

# Veröffentlichungen für Adobe Workfront im zweiten Quartal 2026 – Funktionen mit begrenzter Verfügbarkeit

In diesem Artikel wird die begrenzte Verfügbarkeit von Workfront-Funktionen beschrieben, die im zweiten Quartal 2026 veröffentlicht werden.

<!--keep the sentence below for all future quarterly release pages-->

Eine Liste aller Funktionen mit eingeschränkter Verfügbarkeit, die für Adobe Workfront veröffentlicht wurden, finden Sie unter [Versionsaktivität der Funktionen mit eingeschränkter Verfügbarkeit von Adobe Workfront: Artikelindex](/help/quicksilver/product-announcements/product-releases/limited-availability-release-activity/limited-availability-release-activity-article-index.md).

## Versionshinweise für Funktionen mit begrenzter Verfügbarkeit

Dieser Abschnitt enthält die Versionshinweise für neue Funktionen.

### Aktualisiertes Erlebnis bei der Zuweisung von Aufgaben im Single- oder Bulk-Modus

>[!NOTE]
>
>Produktionsveröffentlichungsdatum: 12. Februar 2026

Der Abschnitt „Zuweisungen“ im Feld „Aufgaben bearbeiten“ wurde aktualisiert, wenn einzelne Aufgaben bearbeitet oder stapelweise bearbeitet wurden.

Es gibt ein neues Erlebnis zum Zuweisen von Ressourcen zu Aufgaben. Dies ist jetzt sowohl beim Bearbeiten einer Aufgabe als auch beim Massenbearbeiten mehrerer Aufgaben verfügbar. Wir haben die folgenden Felder zum Abschnitt Arbeitsaufträge hinzugefügt:

* Zuteilungen
* Verantwortlicher oder Aufgabenbesitzer
* Rolle des Zugewiesenen

Weitere Informationen finden Sie unter [Aufgaben bearbeiten](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md).

### Abrechnungssätze für Personalpläne beibehalten

>[!NOTE]
>
>Produktionsveröffentlichungsdatum: 5. März 2026

Wir haben das Feld **Abrechnung beibehalten** zum Abschnitt Finanzen auf der Seite „Personalplandetails“ hinzugefügt.

Wenn diese Einstellung auf „false“ (falsch) gesetzt ist, werden die Abrechnungssätze nicht beibehalten und die Tarifhierarchie wird für die Berechnung des Abrechnungssatzes verwendet.

Wenn dieses Flag auf „True“ (ein) gesetzt ist:

* Die aktuellen Abrechnungssätze für die im Stellenplan zugewiesenen Ressourcen werden beibehalten, und Änderungen an den Sätzen in der Hierarchie werden nicht im Bereich Ressourcen des Stellenplans berücksichtigt.
* Wenn Sie der Ressourcentabelle eine neue Zeile hinzufügen, wird der ursprüngliche Abrechnungssatz, der aus der Abrechnungssatzhierarchie stammt, beibehalten.
* Wenn ein(e) Benutzende(r) den Abrechnungssatzwert manuell überschrieben hat, bevor das Flag aktiviert wurde, bleibt der Überschreibungssatz erhalten. Sobald die Markierung aktiviert ist, sind Überschreibungen des manuellen Abrechnungssatzes nicht mehr zulässig.

Sobald die Aufbewahrung aktiviert wurde, kann sie nicht mehr deaktiviert werden.

Wenn Sie einen Personalplan kopieren, bei dem die Markierung aktiviert ist, wird die Markierung in der Kopie automatisch deaktiviert. Der Ressourcenmanager muss das Flag aktivieren, wenn es im neuen Personalplan benötigt wird.

<!--
### Title

>[!NOTE]
>
>Production release date: MONTH DAY, 2026

text
-->

<!--

## Maintenance Updates for limited availability features

This section describes the issues fixed in the weekly Workfront updates for limited availability features.



### Maintenance Updates week of March 1-7, 2026

**Title**

text

### Maintenance Updates week of March 8-14, 2026

**Title**

text

### Maintenance Updates week of March 15-21, 2026

**Title**

text
-->
