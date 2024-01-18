---
title: 2.2 Verbesserungen bei der Ressourcenverwaltung
description: 2.2 Verbesserungen bei der Ressourcenverwaltung
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

# 2.2 Verbesserungen bei der Ressourcenverwaltung

Auf dieser Seite werden alle Verbesserungen an der Ressourcenverwaltung beschrieben, die mit Version 22.2 der Vorschaufunktion vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung verfügbar gemacht

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

die Woche vom 4. April 2022.

Eine Liste aller in Version 22.2 verfügbaren Änderungen finden Sie unter [2.2 Versionsübersicht](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Verbesserungen der Navigation des Workload Balancer

Um Ihr Erlebnis bei der Verwendung des Workload Balancer zu verbessern, haben wir die folgenden Verbesserungen eingeführt:

* Die Schaltflächen Abbrechen und Speichern beim Anpassen der Zuordnungen sind jetzt fixierbar, selbst wenn die Aufgabe länger ist als der auf dem Bildschirm angegebene Zeitraum oder wenn das Bedienfeld Zusammenfassung angezeigt wird.
* Das linke Bedienfeld, das die Namen der Benutzer und Arbeitselemente anzeigt, ist jetzt fixierbar, damit Sie einen horizontalen Bildlauf über längere Zeiträume durchführen können und weiterhin die Namen der im Bedienfeld aufgelisteten Elemente lesen können.
* Sie können alle im linken Bereich aufgelisteten Elemente mit einem Klick reduzieren und erweitern, anstatt sie auf Benutzer- oder Projektebene zu verwenden.
* Die Größe des linken Bedienfelds kann jetzt ebenfalls geändert werden.
* Es gibt jetzt einen Vollbildmodus für den Arbeitslastausgleich.

Weitere Informationen zum Navigieren in Workload Balancer finden Sie unter [Navigieren Sie zum Lastenausgleich .](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Zugriff auf erweiterte Zuweisungen im Arbeitslastausgleich

Um das Zuweisen von Arbeitselementen zu vereinfachen und genauer zu gestalten, können Sie jetzt erweiterte Zuweisungen vornehmen, wenn Sie Arbeitselemente manuell im Arbeitslastausgleich zuweisen. Vor dieser Verbesserung konnten Sie beim Bearbeiten von Elementen über die Kopfzeilen der Elemente oder in Listen auf erweiterte Zuweisungen zugreifen.

Weitere Informationen finden Sie unter [Manuelles Zuweisen von Arbeiten mithilfe des Lastenausgleichs](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Neue Formel zur Berechnung der Benutzerverfügbarkeit bei Auswahl der Voreinstellung Standardzeitplan

Um genauere Informationen in den Tools zur Ressourcenverwaltung bereitzustellen, wurde die Formel, die Workfront verwendet, um die Benutzerverfügbarkeit zu berechnen, geändert, wenn der Workfront-Administrator unter &quot;Voreinstellungen für die Ressourcenverwaltung&quot;die Option &quot;Standardzeitplan&quot;auswählt. Mit der neuen Aktualisierung berechnet Workfront die Benutzerverfügbarkeit anhand der folgenden Formel:

Verfügbare Stunden des Benutzers = (Standardzeitplan - Ausnahmen) &#42; FTE - Zeitdauer

Vor dieser Aktualisierung verwendete Workfront die folgende Formel, um die Benutzerverfügbarkeit bei Auswahl des Standardzeitplans zu berechnen:

Verfügbare Stunden des Benutzers = (Standardzeitplan - (Ausnahmen planen + Zeitdauer)) &#42; FTE-Wert des Benutzers

Weitere Informationen finden Sie unter [Voreinstellungen für die Ressourcenverwaltung konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

