---
title: 20.4 Verbesserungen bei der Ressourcenverwaltung
description: 20.4 Verbesserungen bei der Ressourcenverwaltung
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 9f660a38-4a59-4135-8178-0841088cc7d6
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 0%

---

# 20.4 Verbesserungen bei der Ressourcenverwaltung

Auf dieser Seite werden alle Verbesserungen an der Ressourcenverwaltung beschrieben, die mit Version 20.4 der Vorschaufunktion vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung ab dem 9. November 2020 verfügbar sein.

Eine Liste aller in Version 20.4 verfügbaren Änderungen finden Sie unter [Übersicht über die Version 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Planen Sie Arbeiten mit Arbeitsaufwand anstelle von geplanten Stunden.

Um Ihnen Flexibilität bei der Projektplanung zu geben, haben wir das neue Konzept des Arbeitsaufwands für Aufgaben eingeführt. Sie können schätzen, ob der Arbeitsaufwand für eine Aufgabe gering, mittel oder groß ist, ohne die geplanten Arbeitszeiten für die Aufgabe manuell abzuschätzen. Jeder Aufwand wird basierend auf einem Prozentsatz der Zeit aus den typischen Stunden pro Tag berechnet, wie in Ihrer Instanz konfiguriert.

Die folgenden Verbesserungen sind jetzt mit dieser neuen Funktion verfügbar:

* Aktivieren Sie diese Einstellung für Projekte und Vorlagen, um sie für Aufgaben und Vorlagenaufgaben verfügbar zu machen.
* Aktualisieren Sie diese Einstellung für jede Aufgabe mit dem Typ Einfache Dauer , wodurch automatisch die geplanten Stunden der Aufgabe aktualisiert werden.
* Deaktivieren Sie diese Einstellung mithilfe einer Layout-Vorlage für Benutzer, die die geplanten Stunden weiterhin verwenden möchten.
* Zeigen Sie den Wert dieses neuen Felds in einer Aufgabenliste oder einem Bericht an.

Weitere Informationen zu den Arbeitsbemühungen finden Sie unter [Übersicht über den Arbeitsaufwand](../../../manage-work/tasks/task-information/work-effort.md).

Diese Funktion ist jetzt im [Planergrundlagen, Teil 2-Lernpfad](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-2-plan-a-project-20Y0z000000bm79EAA) auf Workfront One.

## Projekt-Status-basierte Farben für Arbeitselemente im Arbeitslastausgleich

Für eine bessere Sichtbarkeit und eine bessere Anpassung Ihres Erlebnisses im Arbeitslade-Balancer können Sie jetzt die Farben der Projekte und ihrer Arbeitselemente so ändern, dass sie dem Status der Projekte entsprechen. Die Farben entsprechen den Projektstatus auf Gruppen- oder Systemebene. Die angezeigten Farben können sowohl dem System- als auch dem benutzerdefinierten Projektstatus entsprechen.

Informationen zum Anpassen der Ansicht im Arbeitslastausgleich finden Sie unter [Navigieren Sie zum Lastenausgleich .](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Anpassen der Benutzerzuordnung mithilfe von Prozentwerten im Arbeitslastausgleich

Sie können jetzt die Zuordnungen Ihrer Benutzer im Lastenausgleich mit Prozentsätzen anstelle von Stunden verwalten.

Informationen zum Verwalten von Zuordnungen im Arbeitslastausgleich finden Sie unter [Verwalten von Benutzerzuordnungen im Lastenausgleich](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Anzeigen oder Ausblenden abgeschlossener Arbeiten im Arbeitslastausgleich

Mit einer neuen Einstellung können Sie jetzt abgeschlossene Arbeitselemente im Arbeitslastausgleich ein- oder ausblenden. Die Einstellung ist standardmäßig aktiviert, und abgeschlossene Arbeitselemente, die den Filterkriterien und dem ausgewählten Zeitrahmen entsprechen, werden im Arbeitslastausgleich angezeigt.

Vor dieser Verbesserung werden abgeschlossene Arbeitselemente immer im Arbeitslastausgleich angezeigt.

Weitere Informationen zum Anpassen der Einstellungen im Arbeitslastausgleich finden Sie unter [Navigieren Sie zum Lastenausgleich .](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Verbesserungen der Benutzerfreundlichkeit im Arbeitslastausgleich

Um eine optimierte und benutzerfreundliche Benutzererfahrung bei der Verwaltung Ihrer Ressourcen im Workload Balancer sicherzustellen, sind jetzt die folgenden Verbesserungen an der Benutzerfreundlichkeit verfügbar:

* Sie können jetzt die Zusammenfassung für Probleme und Aufgaben über das Symbol Zusammenfassung anstelle des Menüs Mehr öffnen. Dieses Erlebnis entspricht nun dem von Listen.

  >[!NOTE]
  >
  >Diese Option ist nur im neuen Adobe Workfront-Erlebnis verfügbar.

* Sie können auf das Menü &quot;Mehr&quot;links neben einer Objektleiste und nicht am Ende einer Objektleiste zugreifen. Dies erleichtert die Suche nach Objekten, die einen langen Zeitraum umfassen.
* Sie können die Zuweisungsfunktionen über einen Tastaturbefehl aufrufen. Zuvor war dies nur über das Menü Mehr verfügbar.
* Sie können alle verbleibenden Elemente unter dem Namen eines Benutzers laden, anstatt nur die folgenden 20 Elemente zu verwenden, indem Sie auf Mehr laden klicken.

Weitere Informationen zum Navigieren in Workload Balancer finden Sie unter [Navigieren Sie zum Lastenausgleich .](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Benutzerzuordnungsdiagramm im Lastenausgleich

Damit Sie innerhalb eines bestimmten Zeitraums eine allgemeine visuelle Darstellung der Zuordnung von Benutzern haben können, ermöglicht eine neue Einstellung jetzt eine Diagrammansicht dazu, wie die Zuordnungen im Arbeitslastausgleich angezeigt werden. Wenn Sie diese Einstellung aktivieren, wird die Zuordnung der Benutzer in einem Liniendiagramm angezeigt, das die Überallokationen in roten Blöcken und die Unterzuordnungen in blau anzeigt.

Weitere Informationen zum Konfigurieren von Einstellungen im Arbeitslastausgleich finden Sie unter [Navigieren Sie zum Lastenausgleich .](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Visualisieren der abgeschlossenen Arbeit im Arbeitslastausgleich

Damit Sie bereits abgeschlossene Arbeiten einfach identifizieren und Benutzerzuweisungen korrekt verwalten können, wurde im Arbeitslastausgleich ein visueller Indikator aktiviert, der anzeigt, wann Elemente für einen ausgewählten Zeitraum abgeschlossen sind. Sie können jetzt ein grünes Häkchen für Aufgaben sehen, Probleme, wenn sie abgeschlossen sind. Das Projekt zeigt auch das grüne Häkchen an, wenn während des auf dem Bildschirm angezeigten Zeitraums Arbeitselemente abgeschlossen sind.

Informationen zum Anzeigen von Informationen im Arbeitslastausgleich finden Sie unter [Navigieren Sie zum Lastenausgleich .](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Neuer Standardfilter für den Bereich &quot;Zugewiesene Arbeit&quot;im Lastenausgleich

Der Standardfilter für den Bereich &quot;Zugewiesene Arbeit&quot;im Arbeitslastausgleich zeigt jetzt nur Benutzer an, die Mitglieder aller Teams sind, mit denen Sie als angemeldeter Benutzer verknüpft sind. Der neue Filter zeigt Ihnen jetzt standardmäßig die relevantesten Informationen an.

Vor dieser Verbesserung wurden alle Benutzer, auf die Sie Zugriff hatten, in diesem Bereich angezeigt.

Informationen zur Verwendung von Filtern im Arbeitslade-Balancer finden Sie unter [Verwalten von Filtern im Lastenausgleich](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

## Neues Symbol zum Wechseln zwischen Stunden- und Prozentwerten oder zugewiesener und verbleibender Zeit im Arbeitslastausgleich

Wir haben eine neue Einstellung hinzugefügt, mit der Sie zwischen zugewiesenen Stunden und Prozentwerten wechseln können, während Sie den Arbeitslastausgleich anzeigen. Mit diesem neuen Symbol haben wir auch den Abschnitt &quot;Benutzerarbeitslast&quot;im Bereich &quot;Einstellungen&quot;eliminiert. Der Lastenausgleich zeigt die zugewiesene Zeit standardmäßig an, und wir haben die Einstellung Verbleibende Stunden auf das neue Symbol Prozentsatz oder Stunden verschoben.

Diese Verbesserung beseitigt Klicks und erleichtert die Navigation im Arbeitslastausgleich.

Informationen zum Verwalten der Einstellungen für den Lastenausgleich finden Sie unter [Navigieren Sie zum Lastenausgleich .](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Ein neuer integrierter Filter für den Lastenausgleich: Benutzer in Projekten

Um Ihr Filtererlebnis im Arbeitslastausgleich effizienter zu gestalten, haben wir einen neuen integrierten Filter im Bereich Zugewiesene Arbeit hinzugefügt. Sie können jetzt den Filter Benutzer auf Projekte anwenden, der Benutzer anzeigt, die Aufgaben und Problemen in den von Ihnen angegebenen Projekten zugewiesen sind.

Informationen zur Verwendung von Filtern im Arbeitslade-Balancer finden Sie unter [Filtern von Informationen im Arbeitslastausgleich](../../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

