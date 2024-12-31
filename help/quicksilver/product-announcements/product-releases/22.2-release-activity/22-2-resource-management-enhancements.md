---
title: 22.2 Verbesserungen beim Ressourcenmanagement
description: 22.2 Verbesserungen beim Ressourcenmanagement
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 22.2 Verbesserungen beim Ressourcenmanagement

Auf dieser Seite werden alle Verbesserungen des Ressourcen-Managements beschrieben, die mit der Version 22.2 an der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung verfügbar gemacht

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

die Woche vom 4. April 2022.

Eine Liste aller Änderungen, die mit Version 22.2 verfügbar sind, finden Sie unter Übersicht über Version [22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Verbesserungen an der Workload Balancer-Navigation

Um die Verwendung des Workload Balancer zu verbessern, haben wir die folgenden Verbesserungen eingeführt:

* Die Schaltflächen Abbrechen und Speichern beim Anpassen der Zuweisungen bleiben jetzt erhalten, auch wenn die Aufgabe länger ist als der auf dem Bildschirm angezeigte Zeitraum oder wenn das Bedienfeld Zusammenfassung angezeigt wird.
* Das linke Bedienfeld, das die Namen der Benutzer und Arbeitselemente anzeigt, bleibt jetzt erhalten, damit Sie über längere Zeiträume horizontal scrollen und die Namen der im Bedienfeld aufgelisteten Elemente weiterhin lesen können.
* Sie können alle im linken Bedienfeld aufgelisteten Elemente mit einem Klick reduzieren und erweitern, anstatt auf Benutzer- oder Projektebene.
* Die Größe des linken Bedienfelds kann jetzt ebenfalls geändert werden.
* Es gibt jetzt einen Vollbildmodus für den Workload-Balancer.

Weitere Informationen zum Navigieren im Workload Balancer finden Sie unter [Navigieren im Workload Balancer](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Zugriff auf erweiterte Zuweisungen im Workload Balancer

Um die Zuweisung von Arbeitselementen einfacher und genauer zu gestalten, können Sie jetzt erweiterte Zuweisungen vornehmen, wenn Sie Arbeitselemente manuell im Workload Balancer zuweisen. Vor dieser Verbesserung konnten Sie beim Bearbeiten von Elementen, in den Kopfzeilen von Elementen oder in Listen auf erweiterte Zuweisungen zugreifen.

Weitere Informationen finden Sie unter [Arbeiten manuell über den Workload Balancer zuweisen](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Neue Formel zur Berechnung der Benutzerverfügbarkeit, wenn die Voreinstellung Standardzeitplan ausgewählt ist

Um genauere Informationen in den Tools für das Ressourcen-Management bereitzustellen, haben wir die Formel geändert, mit der Workfront die Benutzerverfügbarkeit berechnet, wenn der Workfront-Administrator in den Voreinstellungen für das Ressourcen-Management den Standardzeitplan auswählt. Mit dem neuen Update verwendet Workfront die folgende Formel zur Berechnung der Benutzerverfügbarkeit:

Verfügbare Stunden für Benutzer = (Standardzeitplan - Stunden - Ausnahmen) &#42; VZÄ - Ausfallzeiten

Vor diesem Update hat Workfront die folgende Formel zur Berechnung der Benutzerverfügbarkeit bei Auswahl des Standardzeitplans verwendet:

Verfügbare Stunden des Benutzers = (Standardzeitplan - Stunden für Zeitplanausnahmen + Ausfallzeiten) &#42; Wert für VZÄ des Benutzers

Weitere Informationen finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

