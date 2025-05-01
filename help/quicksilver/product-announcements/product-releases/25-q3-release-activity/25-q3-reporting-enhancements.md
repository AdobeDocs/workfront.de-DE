---
title: Verbesserungen beim Reporting im dritten Quartal 2025
description: Projektverbesserungen im dritten Quartal 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: b36cfdc4587bc440867a6a84b9460eaeaf4daf88
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Verbesserungen beim Reporting im dritten Quartal 2025

Auf dieser Seite werden alle Verbesserungen beim Reporting in der Vorschau-Umgebung beschrieben, die mit der Version vom dritten Quartal 2025 vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im dritten Quartal 2025 verfügbar sind, finden Sie unter [Versionsübersicht für das dritte Quartal 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Benutzer-Platzhalter geben beim Filtern keine Ergebnisse mehr mit einem Nullwert zurück

>[!NOTE]
>
>* Vorschau: 30. April 2025
>* Produktions-Schnellveröffentlichung: 15. Mai 2025
>* Produktion für alle Kunden: 17. Juli 2025

Das Verhalten der Benutzer-Platzhalter wurde aktualisiert, um beim Filtern eines Berichts einen Nullwert auszuschließen. Diese Änderung hilft dem Filter, genauere Ergebnisse zu erzielen, anstatt Ergebnisse zurückzugeben, bei denen ein Benutzer nicht richtig konfiguriert ist (ein Nullergebnis).

Wenn ein Benutzer-Platzhalter bisher einen Nullwert erzeugt hat, zeigt ein Bericht alle Datensätze an, die ebenfalls einen Nullwert aufweisen.

Diese Änderung gilt für die folgenden Platzhalterfilter:

* `$$USER.homeTeamID`
* `$$USER.otherTeamIDs`
* `$$USER.roleID`
* `$$USER.roleIDs`
* `$$USER.companyID`

