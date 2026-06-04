---
title: Verbesserungen beim Ressourcen-Management in Version 22.2
description: Verbesserungen beim Ressourcen-Management in Version 22.2
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
TQID: https://experienceleague.adobe.com/X2dBmB8Qyiwg9hM60af6GRBDGT4KkH6Jjs2A-S-TWVg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: c33d85a1-be85-4290-854c-87408c10aa80
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 376
ht-degree: 5%

---

# Verbesserungen beim Ressourcen-Management in Version 22.2

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

Weitere Informationen finden Sie unter [Konfigurieren von Voreinstellungen für das Ressourcen-Management](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

