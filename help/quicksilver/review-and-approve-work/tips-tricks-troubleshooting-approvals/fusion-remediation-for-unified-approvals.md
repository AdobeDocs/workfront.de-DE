---
product-area: documents
navigation-topic: approvals
title: Aktualisieren von Workfront Fusion-Szenarien für eine einheitliche Überprüfung und Genehmigung
description: Inventarisieren, klassifizieren und beheben Sie Workfront Fusion-Szenarien, die auf veralteten Workfront-Korrekturabzügen basieren, während Ihr Unternehmen Adobe Enterprise-Speicher und einheitliche Prüfung und Genehmigung einsetzt.
author: Courtney
feature: Work Management, Digital Content and Documents
role: Admin
source-git-commit: 722ba7f6617e3ccc1a1dcbf51f5d539c550617ab
workflow-type: tm+mt
source-wordcount: '795'
ht-degree: 1%

---

# Aktualisieren von Workfront Fusion-Szenarien für eine einheitliche Überprüfung und Genehmigung

Workfront Fusion-Szenarien, die auf veralteten Workfront-Proofing-Tests basieren, funktionieren nicht automatisch für Adobe Enterprise-Speicherprojekte. Testversandspezifische Module, Webhooks und API-Endpunkte haben in einigen Fällen direkte Entsprechungen, in anderen sind es signifikante Änderungen. In diesem Artikel erfahren Sie, wie Sie betroffene Szenarien inventarisieren, klassifizieren und einen Korrekturpfad festlegen können, bevor Sie Teams, die von diesen Szenarien abhängig sind, in Ihren Unternehmensspeicher-Rollout von Adobe integrieren.

Szenarien, die sich auf veraltete Workfront-Projekte beziehen, funktionieren weiterhin wie bisher. Die in diesem Artikel beschriebenen Korrekturmaßnahmen gelten für Szenarien, in denen Sie Speicherprojekte für Unternehmen in Adobe ausführen möchten.

Fusion-Connectoren mit nativer Unterstützung für einheitliche Überprüfung und Genehmigung werden voraussichtlich im 3. Quartal 2026 verfügbar sein. Planen Sie die Neuerstellung jetzt, wir empfehlen jedoch, vor der Erstellung auf die neuen Connectoren zu warten. Szenarien werden einfacher und zuverlässiger sein als das, was sie ersetzen.

Detaillierte Automatisierungshandbücher werden zusammen mit der Version des Fusion-Connectors für das 3. Quartal 2026 veröffentlicht. Verwenden Sie diesen Artikel, um Szenarien jetzt zu inventarisieren und zu klassifizieren, damit Sie bereit sind zu handeln, sobald diese Anleitung verfügbar ist.

Eine allgemeine Zusammenfassung der Änderungen, die auftreten, wenn Ihr Unternehmen auf Adobe Enterprise Storage zu Workfront wechselt, finden Sie unter [Wechseln zu Workfront auf Adobe Enterprise Storage](/help/quicksilver/review-and-approve-work/workfront-storage.md).


## Änderungen für Fusion bei Enterprise-Speicherprojekten in Adobe

Bestehende Fusion-Szenarien, die auf Workfront Proof basieren, basieren auf Korrekturabzugsmodulen, Webhook-Triggern und API-Endpunkten, die nicht Teil des einheitlichen Überprüfungs- und Genehmigungsdatenmodells sind. In der folgenden Tabelle sind die gängigen Szenario-Typen ihren erwarteten Auswirkungen und dem künftigen Weg zugeordnet:

| Szenario-Typ | Wirkung | Weiterleitung |
|---|---|---|
| Erstellung und Weiterleitung von Korrekturabzügen | Pausen | Neu erstellen mit der einheitlichen Validierungs-API |
| Webhooks zum Korrekturabzugsstatus | Pausen | Mit neuen Triggern für Genehmigungsereignisse neu erstellen |
| Trigger beim Hochladen von Dokumenten | Teilweise: Erneuter Test erforderlich | Prüfen und erneutes Testen nach der Migration |
| Erinnerungsbenachrichtigungen für Genehmigungen | Pausen | Mit Fristen für Genehmigungsvorlagen ersetzen |
| Validierungsentscheidungs-Routing | Pausen | Neu erstellen mit neuen Entscheidungsstatusfeldern |
| Benutzerdefinierte Genehmigungsberichte | Teilweise: Feldnamen können sich ändern | Ordnen Sie ältere Felder dem neuen Schema zu |


## Klassifizieren Sie jedes Szenario als Bearbeiten, Neu erstellen oder außer Kraft setzen

Welche Arbeit für jedes Szenario erforderlich ist, hängt davon ab, was es tut und was in der einheitlichen Überprüfung und Genehmigung verfügbar ist. Verwenden Sie die folgenden Klassifizierungen:

* **Bearbeiten**: Die vorhandene Korrekturabzugsaktion entspricht direkt der einheitlichen Überprüfung und Genehmigung. Sie können das Szenario aktualisieren, um die neue Aktion zu verwenden.
* **Neu erstellen**: Die zugrunde liegenden Schritte haben sich erheblich geändert, oder es gibt neue Funktionen, die das Szenario verwenden sollte, sodass das Szenario von Grund auf neu erstellt werden muss.
* **Retire**: Native einheitliche Überprüfungs- und Genehmigungsfunktionen, wie z. B. mehrstufige Genehmigungsvorlagen mit Terminerinnerungen, ersetzen das, wofür das Szenario erstellt wurde.

Überprüfen Sie jedes Szenario anhand Ihrer spezifischen Geschäftslogik, um über seine Klassifizierung zu entscheiden.

## Sanierungsansatz

Verwenden Sie den folgenden Ansatz, um die Fusion-Behebung zu planen und auszuführen:

1. **Inventar jetzt.** Abrufen einer vollständigen Liste der aktiven Fusion-Szenarien und Markieren aller Szenarien, die auf die Erstellung von Korrekturabzügen, den Status von Korrekturabzügen, Dokumentgenehmigungen oder das Genehmigungs-Routing verweisen. Warten Sie nicht, bis der Adobe Enterprise-Speicher aktiviert ist.
1. **Klassifizieren Sie jedes** als „Bearbeiten“, „Neu erstellen“ oder „Einstellen“ basierend auf den Kriterien im vorherigen Abschnitt.
1. **Korrekturabzug-abhängige Szenarien pausieren** bevor Sie Teams, die von ihnen abhängig sind, in Ihr Enterprise-Speicherpilotsystem für Adobe aufnehmen. Das Ausführen veralteter, auf Korrekturabzügen basierender Automatisierungen für das neue Modell kann zu stillen Fehlern oder doppelten Aktionen führen.
1. **Verwenden Sie Genehmigungsvorlagen, um einfache Routing-Logik zu ersetzen.** Native mehrstufige Genehmigungsvorlagen mit Deadline-Automatisierung können viele Anwendungsfälle verarbeiten, für die zuvor Fusion erforderlich war. Weitere Informationen finden Sie unter [Erstellen einer Genehmigungsvorlage für Assets und Dokumente](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).
1. **Warten Sie vor dem Neuaufbau auf die Updates des Fusion-Connectors für das 3. Quartal 2026.** Die aktualisierten Connectoren stellen Module zur Verfügung, die speziell für die einheitliche Überprüfung und Genehmigung entwickelt wurden, und machen Neuaufbauten deutlich einfacher und zuverlässiger. Es wird nicht empfohlen, vorab eine Neuerstellung anhand der Workfront-API-Version 22 durchzuführen. Wenn Sie mit einem zeitkritischen Szenario fortfahren, planen Sie, diese Arbeit erneut aufzurufen, sobald die neuen Connectoren veröffentlicht werden.
1. **Testen Sie neu erstellte Szenarien End-to-End in einer Sandbox** Instanz, bevor Sie sie in der Produktion aktivieren. Achten Sie besonders auf die Payloads von Ereignisabonnements - Feldnamen und Schemata unterscheiden sich von alten Korrekturabzug-Ereignissen.

>[!TIP]
>
>Viele Unternehmen haben Fusion-Szenarien gesammelt, die Lücken in der Legacy-Proofing-Prüfung umgingen. Durch native, einheitliche Überprüfungs- und Genehmigungsfunktionen - einschließlich Genehmigungsvorlagen, Terminerinnerungen und mehrstufiges Routing - werden einige dieser Szenarien nicht mehr benötigt. Evaluieren Sie bei der Klassifizierung jedes Szenarios, ob es durch eine native Funktion ersetzt werden kann. Ein Szenario außer Kraft zu setzen ist langfristig oft sauberer als es wieder aufzubauen.

## Verwandte Artikel

* [Wechsel zu Workfront auf Adobe Enterprise Storage](/help/quicksilver/review-and-approve-work/workfront-storage.md)
* [Einheitliche Prüfung und Genehmigung - Übersicht](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Erste Schritte mit der einheitlichen Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Erstellen einer Genehmigungsvorlage für Assets und Dokumente](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
