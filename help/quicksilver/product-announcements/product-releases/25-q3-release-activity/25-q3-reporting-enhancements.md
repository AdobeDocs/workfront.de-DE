---
title: Verbesserungen beim Reporting im dritten Quartal 2025
description: Projektverbesserungen im dritten Quartal 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6e53dca8-285a-471b-a646-1773722554f3
source-git-commit: a0a7ad2770b99ee1d45169372e64e460701ccc10
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Verbesserungen beim Reporting im dritten Quartal 2025

Auf dieser Seite werden alle Verbesserungen beim Reporting in der Vorschau-Umgebung beschrieben, die mit der Version vom dritten Quartal 2025 vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im dritten Quartal 2025 verfügbar sind, finden Sie unter [Versionsübersicht für das dritte Quartal 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Verbesserte Sicherheit bei der Berichtbereitstellung

* Vorschau: 26. Juni 2025
* Produktion: Schrittweiser Rollout vom 26. Juni 2025 bis zum 9. Juli 2025

Wir haben die geplante Bereitstellung von Berichten verbessert, um sicherzustellen, dass Workfront-Benachrichtigungen nur an E-Mail-Domains gesendet werden, die in der -Zulassungsliste genehmigt wurden.

Wenn Ihr Unternehmen zuvor eine Einschränkung für die E-Mail-Domains mit Workfront-Benachrichtigungen definiert hätte, würden wir eine Prüfung mit der -Zulassungsliste durchführen, wenn E-Mails hinzugefügt würden.

Jetzt führen wir auch während des Versands der E-Mail eine Überprüfung durch, um sicherzustellen, dass die eingegebene E-Mail-Adresse mit der E-Mail-Zulassungsliste übereinstimmt. Diese verbesserte Prüfung gilt sowohl für E-Mail-Adressen, die mit Benutzenden verknüpft sind, als auch für Ad-hoc-E-Mails, die der Liste der Berichtsempfängerinnen und -empfänger hinzugefügt wurden.

Weitere Informationen finden Sie unter [Planen einer automatischen Berichtsbereitstellung](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).


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
