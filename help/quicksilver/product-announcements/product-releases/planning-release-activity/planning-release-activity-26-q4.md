---
content-type: release-notes
title: Versionsaktivität für Adobe Workfront Planning im vierten Quartal 2026
description: Dies ist die Veröffentlichungsaktivität für das Adobe Workfront Planning-Produkt im vierten Quartal 2026.
author: Becky
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 20f5a513d8d33ecf8770f35bc73ee799a7de939e
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 0%

---

# Versionsaktivität für Adobe Workfront Planning im vierten Quartal 2026

In diesem Artikel werden die Funktionen beschrieben, die in Workfront Planning im vierten Quartal 2026 veröffentlicht werden.

Eine Liste aller für Adobe Workfront Planning veröffentlichten Funktionen finden Sie unter [Adobe Workfront Planning Release-Aktivität: Artikelindex](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Einführung in die Fähigkeiten des Workfront Planning Solution Architect

>[!NOTE]
>
>Vorschau: 10. August 2026
>Produktion: 10. August 2026

Wir stellen eine neue Qualifikation zur Verfügung, den Workfront Planning Solution Architect, der Best Practice-Beratung für Workfront Planning direkt in Claude integriert. Direkt in der Claude-Benutzeroberfläche können Sie jetzt Folgendes tun:

* Konfigurieren Sie einen neuen Planning-Arbeitsbereich, der Ihren Geschäftsanforderungen entspricht, wobei der Workfront MCP-Server das Setup in Ihrer Umgebung ausführt.
* Überprüfen Sie eine vorhandene Konfiguration im großen Maßstab auf Antimuster.
* Überprüfen Sie die Nutzung anhand der empfohlenen Limits.
* Stellen Sie Fragen zu Planning.

Weitere Informationen finden Sie unter [Kenntnisse für die direkte Installation verfügbar](/help/quicksilver/workfront-basics/workfront-mcp-server/direct-skills.md).

## Zeilen per Drag-and-Drop in die Tabellenansicht ziehen

>[!NOTE]
>
>Vorschau: 30. Juli 2026
>Produktions-Schnellveröffentlichung: 13. August 2026
>Produktion für alle: 15. Oktober 2026

Das Ziehen und Ablegen von Zeilen in der Tabellenansicht wurde visuell verbessert.

Weitere Informationen finden Sie unter [Verwalten der Tabellenansicht](/help/quicksilver/planning/views/manage-the-table-view.md).


## Abhängige verbundene Datensatzfelder

>[!NOTE]
>
>Vorschau: 30. Juli 2026
>Produktions-Schnellveröffentlichung: 13. August 2026
>Produktion für alle: 15. Oktober 2026

Workspace-Manager können jetzt Abhängigkeiten zwischen verbundenen Datensatztypen definieren. Stellen Sie beispielsweise sicher, dass in einem Feld Region nur Werte angezeigt werden, die mit der ausgewählten Geografie verknüpft sind. Dies wird direkt im Setup des Verbindungsfelds konfiguriert: Beim Hinzufügen einer Verbindung von einem Geodatensatztyp zu einem abhängigen Datensatztyp (wie Region) ermöglicht eine neue Einstellung es Workspace-Managern, sie als abhängig vom Geodatensatztyp zu markieren, wobei die bereits zwischen diesen Datensatztypen eingerichteten Beziehungen verwendet werden.

Nach der Konfiguration hat jeder Datensatztyp, der auf beide Felder verweist (z. B. eine Kampagne), sofort Auswirkungen: Wenn Sie einen Geo-Wert auswählen, wird die Regionsauswahl auf die tatsächlich mit dieser Geo-Region verknüpften Regionen beschränkt. Dadurch wird Ihre Datensatzstruktur automatisch erzwungen, sodass nicht übereinstimmende Kombinationen vermieden und die manuelle Bereinigung reduziert wird.

Die folgenden Funktionen sind in diesem Update enthalten:

* Der Abschnitt Neue Verbindungseinstellungen wurde auf der Registerkarte Neue Verbindung beim Verbinden von Datensatztypen hinzugefügt
* Im neuen Abschnitt wurde die Einstellung Verbindung abhängig machen hinzugefügt


Weitere Informationen finden Sie unter [Abhängige Verbindungen verwalten](/help/quicksilver/planning/architecture/manage-dependent-connections.md).




## Anzeige eines neuen Kommentars für einen Datensatz in der Tabellenansicht anzeigen

>[!NOTE]
>
>Vorschau: 30. Juli 2026
>Produktions-Schnellveröffentlichung: 13. August 2026
>Produktion für alle: 15. Oktober 2026

Wir haben einen neuen Indikator hinzugefügt, der anzeigt, wenn ein Datensatz ungelesene Kommentare enthält. Der Indikator wird in der oberen rechten Ecke des Primärfelds des Datensatzes in der Tabellenansicht angezeigt.

Weitere Informationen finden Sie unter [Verwalten von Datensatzkommentaren](/help/quicksilver/planning/records/manage-record-comments.md).

## Anpassbare Eintragsfarbe und verbindungsbasierte Farbcodierung

>[!NOTE]
> 
>Vorschau: 23. Juli 2026
>Produktions-Schnellveröffentlichung: 13. August 2026
>Produktion für alle: 15. Oktober 2026

Datensätze unterstützen jetzt anpassbare Farbpaletten, mit denen Sie die neuen Datensätzen automatisch zugewiesenen Farben auf Standard- oder benutzerdefinierte Farben aktualisieren können.

Die folgenden Änderungen sind in dieser Verbesserung enthalten: 

* Wir haben die Option Farbe zu den folgenden Bereichen hinzugefügt:
  * Das Symbol Felder in der Tabellenansicht. 
  * Der Abschnitt Balkenstil im Bereich Einstellungen einer Zeitleiste und einer Kalenderansicht

    Wenn die Farbeinstellung aktiviert ist, wird die einem neuen Datensatz zugewiesene Farbe überall dort angezeigt, wo der Datensatz in diesen Ansichten angezeigt wird. 

* Der Detailseite des Datensatzes wird ein Farbkreis hinzugefügt. 
* Sie können jetzt bei der Einfärbung nach Feldwerten Datensatzfelder mit Einzel- und Mehrfachauswahl sowie verbundene Datensatzfelder zur Farbcodierung von Balken in Zeitleisten- und Kalenderansichten hinzufügen. 
* Sie können aktivieren, um beim Erstellen von verbundenen Datensatzfeldern neben dem Namen und dem Bild eines Datensatzes auch die Farbe anzuzeigen. 
* Der Abschnitt Farbe im Bereich Einstellungen wurde ebenfalls optimiert, indem die Option „Keine“ entfernt wurde.  

Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md). 

## Die Planung von Designer erfordert jetzt die Zustimmung von Beta

>[!NOTE]
>Vorschau und Produktion für alle Kunden: 20. Juli 2026
>[!BADGE Außerplanmäßig]{type=Neutral}

Für die Planung von Designer ist jetzt eine gültige Beta-Vereinbarung erforderlich. Ihr Unternehmen ist nicht verpflichtet, eine KI-Vereinbarung zu unterzeichnen. Dies ist für alle Kunden verfügbar.

Dazu haben wir die Option Planning Designer im Abschnitt Setup unter dem Abschnitt Opt-in für KI-Beta verschoben.

Der Start von Planning Designer ohne eine akzeptierte Beta-Vereinbarung fordert jetzt zur Annahme auf, bevor Workspace Builder geöffnet wird.

Weitere Informationen finden Sie [Erste Schritte mit der Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).
