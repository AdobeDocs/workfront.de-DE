---
title: Verbesserungen beim Reporting für das zweite Quartal 2026
description: Verbesserungen beim Reporting für das zweite Quartal 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4bc2fee9-fa86-41c7-80e7-44bf3e8077d8
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 1ef6ead705231a41cbf62b8a8b35f480da004970
workflow-type: tm+mt
source-wordcount: '872'
ht-degree: 8%

---

# Verbesserungen beim Reporting für das zweite Quartal 2026

Auf dieser Seite werden die Verbesserungen beim Reporting in der Vorschau-Umgebung beschrieben, die mit der Version vom zweiten Quartal 2026 vorgenommen wurden. Diese Verbesserungen werden wie angegeben in der Produktionsumgebung verfügbar gemacht.

Eine Liste aller Änderungen, die zu diesem Zeitpunkt im zweiten Quartal 2026 verfügbar sind, finden Sie unter [Versionsübersicht für das zweite Quartal 2026](/help/quicksilver/product-announcements/product-releases/26-q1-release-activity/26-q1-release-overview.md).

## Feld „Aktuelle Version“ für Dokumentversionen

>[!NOTE]
>
>Vorschau: 2. April 2026
>Produktions-Schnellveröffentlichung: Donnerstag, 15. April 2026
>Produktion für alle: Freitag, 16. April 2026

Wir haben dem Dokumentversionsobjekt ein `currentVersion` boolesches Feld hinzugefügt, damit Sie die neueste Version eines Dokuments leichter identifizieren und darüber berichten können.
Mit diesem Update:

* Sie können `currentVersion` in Filtern, Ansichten, Gruppierungen und Diagrammen verwenden.
* Das Feld ist in der Feldauswahl der Arbeitsfläche für Dokumentversionsberichte verfügbar.

* Wenn eine neue Version hochgeladen wird:

   * Die neue Version wird als `TRUE` gekennzeichnet
   * Frühere Versionen sind als `FALSE` gekennzeichnet

* Berichte können aktuelle Versionen in allen Arbeitsflächen-Dashboards und in Legacy-Berichten konsistent identifizieren

Vorhandene Filter für klassische Berichte, die `isCurrentVersion` oder `isDocumentCurrentVersion` verwenden, funktionieren weiterhin wie dokumentiert.

## Die geplante Bereitstellung von Berichten unterstützt jetzt verknüpfungsbasierte E-Mails

>[!NOTE]
>
>Vorschau: 3. April 2026
>Produktions-Schnellveröffentlichung: Donnerstag, 15. April 2026
>Produktion für alle: Freitag, 16. April 2026

Workfront enthält jetzt einen neuen Bereitstellungstyp Link für geplante Berichte. Anstatt eine Datei zu generieren und anzuhängen, sendet diese Option eine E-Mail mit einem direkten Link zum Bericht in Workfront, damit die Empfängerinnen und Empfänger {{$include }} aktuellen Daten in der Anwendung anzeigen können.

Die Option Link ist jetzt der Standardversandtyp für neu erstellte Bereitstellungsregeln für terminierte Berichte, während bestehende dateibasierte Formate (HTML, PDF, Excel und TSV) weiterhin verfügbar sind.

Mit dieser Änderung haben wir auch das Erscheinungsbild der Berichtversand-E-Mail aktualisiert.

Weitere Informationen finden Sie unter [Planen einer automatischen Berichtsbereitstellung](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

## Berichte als bestimmter Benutzer in Arbeitsflächen-Dashboards ausführen

>[!NOTE]
>
>Vorschau: 2. April 2026
>Produktions-Schnellveröffentlichung: Donnerstag, 15. April 2026
>Produktion für alle: Freitag, 16. April 2026
>
>Canvas Dashboards befindet sich derzeit in der Beta-Phase.

Sie können jetzt Berichte auf Arbeitsflächen-Dashboards so konfigurieren, dass sie als ein bestimmter Benutzer ausgeführt werden. Wenn diese Option aktiviert ist, zeigt der Bericht Daten basierend auf dem Zugriff des ausgewählten Benutzers anstelle der Berechtigungen des Viewers an.

Dadurch werden konsistentere und zuverlässigere Daten über alle Dashboard-Viewer hinweg sichergestellt, auch wenn der Zugriff auf Planning-Arbeitsbereiche, Datensatztypen oder Autorisierungseinstellungen unterschiedlich ist.

Weitere Informationen finden Sie unter [Erstellen eines KPI-Berichts in einem Arbeitsflächen-Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md), [Erstellen eines Diagrammberichts in einem Arbeitsflächen-Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md) oder [Erstellen eines Tabellenberichts in einem Arbeitsflächen-Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md).

## Neue Authentifizierungsoptionen für die Datenverbindung

>[!NOTE]
>
>Vorschau: 12. März 2026
>Produktions-Schnellveröffentlichung: Freitag, 12. März 2026
>Produktion für alle: Freitag, 16. April 2026

Sie können sich jetzt mit RSA-Schlüsseln oder programmgesteuerten Zugriffstoken (PAT)-Verbindungen bei Data Connect authentifizieren und so sicherere und flexiblere Alternativen zu herkömmlichen Benutzernamen-/Passwort-Anmeldeinformationen hinzufügen.

Diese neuen Optionen ermöglichen es Unternehmen, stabile Verbindungen von Power BI, Tableau und anderen BI-Tools von Drittanbietern aufrechtzuerhalten, ohne auf benutzerbasierte Anmeldemethoden angewiesen zu sein.

>[!IMPORTANT]
>
>Im Juni 2026 werden Anmeldeinformationen für Benutzernamen/Kennwort erforderlich sein, um die Multi-Faktor-Authentifizierung (MFA) zu verwenden. Wir empfehlen die Umstellung auf RSA- oder PAT-basierte Authentifizierung für Service-Benutzerkonten, die zum Laden von Daten von Data Connect in Visualisierungs-Tools von Drittanbietern, Datenprozessoren und Skripte verwendet werden, die nicht mit MFA im Authentifizierungsprozess funktionieren.

## Benutzerdefinierte Feldbezeichnungen, die beim Erstellen von Berichten angezeigt werden

>[!NOTE]
>
>Vorschau: 26. Februar 2026
>Produktions-Schnellveröffentlichung: Freitag, 12. März 2026
>Produktion für alle: Freitag, 16. April 2026

Die benutzerdefinierte Feldbezeichnung wird jetzt vor dem Feldnamen und dem -Objekt in den Tools zum Erstellen von Berichten angezeigt, sodass Sie Felder leichter finden können. Feldbezeichnungen werden auch beim Definieren von Filtern, Ansichten und Gruppierungen in Listen angezeigt.

Die benutzerdefinierte Feldbezeichnung ist für die Systemschnittstelle vorgesehen, während der Feldname häufig für die API- und Backend-Speicherung verwendet wird und beim Auffinden eines Felds möglicherweise nicht so hilfreich ist.

Weitere Informationen finden Sie unter [Erstellen eines benutzerdefinierten Berichts](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Freigebbare Berichtsordner

>[!NOTE]
>
>Vorschau: 26. Februar 2026
>Produktions-Schnellveröffentlichung: Freitag, 12. März 2026
>Produktion für alle: Freitag, 16. April 2026

Sie können jetzt Berichte mithilfe von freigebbaren Berichtsordnern organisieren und freigeben. Diese neue Funktion hilft Teams, die große Mengen an Berichten verwalten, skalierbare und konsistente Zugriffskontrolle zu gewährleisten:

* **Organisierte Ordnerstrukturen erstellen**: Systemadministratoren können Ordner der obersten Ebene erstellen, und Benutzer mit dem Zugriff „Verwalten“ können Unterordner mit bis zu vier Ebenen erstellen.
* **Granulare Berechtigungssteuerungen**: Freigeben von Ordnern mit zwei Berechtigungsebenen:
   * Anzeigen: Benutzer können Berichte öffnen und Ordner freigeben
   * Verwalten : Benutzer können Ordnerdetails bearbeiten, Elemente hinzufügen/entfernen und automatisch Verwaltungszugriff auf alle Berichte im Ordner erhalten
* **Geerbte Berechtigungen**: Berechtigungen werden von übergeordneten Ordnern an alle Unterordner und Berichte innerhalb der Ordnerstruktur weitergegeben
* **Erweitertes Listenerlebnis**: Wenn Sie freigebbare Ordner aktivieren, haben Sie Zugriff auf das erweiterte Listenerlebnis. Weitere Informationen finden Sie unter [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


Weitere Informationen finden Sie unter [Verwenden von freigebbaren Berichtsordnern](/help/quicksilver/reports-and-dashboards/reports/report-usage/use-sharable-report-folders.md).

## Verbesserte Datumsbeschriftungen für Diagrammgruppierungen in Arbeitsflächen-Dashboards

>[!NOTE]
>
>Vorschau: 26. Februar 2026
>Produktions-Schnellveröffentlichung: Freitag, 12. März 2026
>Produktion für alle: Freitag, 16. April 2026

>[!NOTE]
>
>Canvas Dashboards befindet sich derzeit in der Beta-Phase.

Diagramme, die Daten nach Datum gruppieren, zeigen jetzt klarere, besser lesbare Datumsbeschriftungen an. Mit diesem Update werden Datumsbeschriftungen basierend auf der ausgewählten Option Gruppieren nach dynamisch angepasst, z. B. nach Tag, Woche, Monat oder Jahr, wodurch Diagramme leichter zu lesen und zu interpretieren sind:

<table> <tbody> <tr> <td>Day</td> <td>Zeigt das vollständige Datum an. Beispiel: 3/12/2026</td> </tr> <tr> <td>Woche</td> <td>Zeigt ein formatiertes Startdatum der Woche an. Beispiel, 8. März 2026</td> </tr> <tr> <td>Month</td> <td>Zeigt Monat und Jahr an. Beispiel März 2026</td> </tr> <tr> <td>Year</td> <td>Anzeige nur des Jahres. Beispiel: 2026</td> </tr> </tbody> </table>

Zuvor zeigten die Diagrammgruppierungen immer das Startdatum des ausgewählten Zeitraums in einem numerischen Format an.
