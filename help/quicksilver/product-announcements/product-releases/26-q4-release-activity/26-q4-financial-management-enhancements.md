---
title: Verbesserungen beim Finanzmanagement für das vierte Quartal 2026
description: Verbesserungen beim Finanzmanagement für das vierte Quartal 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 4ca5bba5090d9e3a72c8964bdf6cca1085c314db
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 3%

---

# Verbesserungen beim Finanzmanagement für das vierte Quartal 2026

Auf dieser Seite werden die Verbesserungen des Finanzmanagements beschrieben, die mit der Version für das vierte Quartal 2026 in der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im vierten Quartal 2026 des Versionszyklus verfügbar sind, finden Sie unter [Versionsübersicht für das vierte Quartal 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Verbesserungen der Abrechnungssätze für Unternehmen

>[!NOTE]
>
>Vorschau: 3. September 2026
>Produktions-Schnellveröffentlichung: 17. September 2026
>Produktion für alle: 15. Oktober 2026

An der Funktion Abrechnungssätze für Unternehmen wurden mehrere Aktualisierungen vorgenommen.

### Für Kunden mit allen Workfront- und Workflow-Paketen

* Die Dialogfelder zum Hinzufügen und Bearbeiten von Abrechnungssätzen für Unternehmen wurden durch ein moderneres Design aktualisiert, das mit anderen Bereichen von Workfront übereinstimmt.
* Mit der Einstellung „Zulassen, dass Abrechnungssätze auf Firmenebene Abrechnungssätze auf Projektebene überschreiben“ werden die Abrechnungssätze überschrieben, wenn eine Firma zu einem Projekt hinzugefügt wird. Die Berechnungen für den geplanten Umsatz verwenden die Abrechnungssätze auf Firmenebene.
* Benutzende ohne Zugriff auf „Allgemeine Finanzen bearbeiten“ und „Abrechnungssätze bearbeiten“ auf Projektebene können keine Firma mehr zu einem Projekt hinzufügen.

### Nur für Kunden mit dem Workflow-Ultimate-Paket

Tarifattribute sind jetzt verfügbar und können auf Abrechnungssätze auf Firmenebene angewendet werden. Das Datum des In-Kraft-Tretens kann auch auf Firmensätze angewendet werden.

HINWEIS: Die Tarife auf Firmenebene wurden nicht zur Tarifierhierarchie hinzugefügt.

Weitere Informationen finden Sie unter [Überschreiben von Abrechnungssätzen für Aufgabengebiete auf Firmenebene](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md) und [Überschreiben von Abrechnungssätzen auf Projektebene mit Abrechnungssätzen auf Firmenebene](/help/quicksilver/manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md).

## Attributhierarchien bleiben jetzt automatisch verbunden

>[!NOTE]
>
>Vorschau: 3. September 2026
>Produktions-Schnellveröffentlichung: 17. September 2026
>Produktion für alle: 15. Oktober 2026
>Diese Funktion ist nur für Organisationen im Workflow-Ultimate-Paket verfügbar.

Bei Verwendung von Ratenattributen als Filter in verschiedenen Bereichen von Workfront, z. B. „Erweiterte Zuweisungen“, wird jetzt eine zusätzliche Validierung auf die Filterung übergeordneter Elemente angewendet.

Wenn Sie zuvor ein Attribut mit einem übergeordneten Element verknüpft haben und dieses übergeordnete Element mit einem Großelternteil, hat das System das ursprüngliche Attribut auch nicht automatisch als zum Großelterteil gehörend erkannt. Wenn Sie nun das Attribut der untersten Ebene auswählen, wird jede darüber liegende Ebene automatisch zugewiesen.

Weitere Informationen zu Attributen finden [&#x200B; unter „Tarifattribute definieren](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).
