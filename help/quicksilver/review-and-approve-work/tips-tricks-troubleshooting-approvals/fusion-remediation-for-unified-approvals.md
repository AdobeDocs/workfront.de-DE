---
product-area: documents
navigation-topic: approvals
title: Aktualisieren von Workfront Fusion-Szenarien für eine einheitliche Überprüfung und Genehmigung
description: Inventarisieren, klassifizieren und beheben Sie Workfront Fusion-Szenarien, die auf dem alten Workfront-Proofing basieren, während Ihr Unternehmen Adobe Cloud-Speicher und einheitliche Prüfung und Genehmigung einsetzt.
author: Courtney
feature: Work Management, Digital Content and Documents
role: Admin
source-git-commit: a3ef3b4ea00298e23ebc8b6196c951417e75eebe
workflow-type: tm+mt
source-wordcount: '802'
ht-degree: 1%

---

# Aktualisieren von Workfront Fusion-Szenarien für eine einheitliche Überprüfung und Genehmigung

Workfront Fusion-Szenarien, die auf veralteten Workfront-Proofing-Tests basieren, funktionieren nicht automatisch für Adobe-Cloud-Speicherprojekte. Testversandspezifische Module, Webhooks und API-Endpunkte haben in einigen Fällen direkte Entsprechungen, in anderen sind es signifikante Änderungen. In diesem Artikel erfahren Sie, wie Sie betroffene Szenarien inventarisieren, klassifizieren und einen Korrekturpfad festlegen können, bevor Sie Teams, die von diesen Szenarien abhängig sind, in Ihren Rollout von Adobe Cloud-Speicher integrieren.

Szenarien, die sich auf veraltete Workfront-Projekte beziehen, funktionieren weiterhin wie bisher. Die in diesem Artikel beschriebenen Korrekturmaßnahmen gelten für Szenarien, die Sie für Adobe-Cloud-Speicherprojekte ausführen möchten.

>[!IMPORTANT]
>
>Der Adobe Workfront Unified Review and Approvals-Connector ist jetzt in Workfront Fusion verfügbar. Es wird empfohlen, diesen Connector für einfachere und zuverlässigere Szenarien zu verwenden, wenn Sie Fusion mit Adobe Cloud Storage verwenden.
>
>Informationen und Anweisungen finden Sie unter [Einheitliche Adobe Workfront-Prüfungs- und Genehmigungs-Module](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/workfront-review-and-approvals-modules) in der Dokumentation zu Workfront Fusion.

Verwenden Sie diesen Artikel, um Szenarien zu inventarisieren und zu klassifizieren und zu verstehen, wie Sie Ihre Fusion-Szenarien am besten aktualisieren können, um den Adobe-Cloud-Speicher zu berücksichtigen.

Eine allgemeine Zusammenfassung der Änderungen, die auftreten, wenn Ihr Unternehmen auf Workfront im Adobe Cloud-Speicher umstellt, finden Sie unter [Wechseln zu Workfront im Adobe Cloud-Speicher](/help/quicksilver/review-and-approve-work/workfront-storage.md).


## Änderungen für Fusion in Adobe Cloud-Speicherprojekten

Bestehende Fusion-Szenarien, die auf Workfront Proof basieren, basieren auf Korrekturabzugsmodulen, Webhook-Triggern und API-Endpunkten, die nicht Teil des einheitlichen Überprüfungs- und Genehmigungsdatenmodells sind. In der folgenden Tabelle sind die gängigen Szenario-Typen ihren erwarteten Auswirkungen und dem künftigen Weg zugeordnet:

| Szenario-Typ | Wirkung | Weiterleitung |
|---|---|---|
| Erstellung und Weiterleitung von Korrekturabzügen | Pausen | Neuaufbau mit der API für einheitliche Genehmigungen im 3. Quartal 2026 |
| Webhooks zum Korrekturabzugsstatus | Pausen | Mit neuen Triggern für Genehmigungsereignisse im 3. Quartal 2026 neu erstellen |
| Trigger beim Hochladen von Dokumenten | Teilweise: Erneuter Test erforderlich | Audit und erneuter Test nach der Migration im 3. Quartal 2026 |
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

1. **Inventar jetzt.** Abrufen einer vollständigen Liste der aktiven Fusion-Szenarien und Markieren aller Szenarien, die auf die Erstellung von Korrekturabzügen, den Status von Korrekturabzügen, Dokumentgenehmigungen oder das Genehmigungs-Routing verweisen. Warten Sie nicht, bis der Adobe-Cloud-Speicher aktiviert ist.
1. **Klassifizieren Sie jedes** als „Bearbeiten“, „Neu erstellen“ oder „Einstellen“ basierend auf den Kriterien im vorherigen Abschnitt.
1. **Korrekturabzug-abhängige Szenarien anhalten** bevor Sie Teams, die von ihnen abhängig sind, in Ihr Pilotprojekt für Cloud-Speicher in Adobe aufnehmen. Das Ausführen veralteter, auf Korrekturabzügen basierender Automatisierungen für das neue Modell kann zu stillen Fehlern oder doppelten Aktionen führen.
1. **Verwenden Sie Genehmigungsvorlagen, um einfache Routing-Logik zu ersetzen.** Native mehrstufige Genehmigungsvorlagen mit Deadline-Automatisierung können viele Anwendungsfälle verarbeiten, für die zuvor Fusion erforderlich war. Weitere Informationen finden Sie unter [Erstellen einer Genehmigungsvorlage für Assets und Dokumente](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).
1. **Verwenden Sie beim Neuaufbau den Adobe Workfront Unified Review and Approvals Connector.** Die aktualisierten Connectoren stellen Module zur Verfügung, die speziell für die einheitliche Überprüfung und Genehmigung entwickelt wurden, und machen Neuaufbauten deutlich einfacher und zuverlässiger. Es wird nicht empfohlen, vorab eine Neuerstellung anhand der Workfront-API-Version 22 durchzuführen.
1. **Testen Sie neu erstellte Szenarien End-to-End in einer Sandbox** Instanz, bevor Sie sie in der Produktion aktivieren. Achten Sie besonders auf die Payloads von Ereignisabonnements - Feldnamen und Schemata unterscheiden sich von alten Korrekturabzug-Ereignissen.

>[!TIP]
>
>Viele Unternehmen haben Fusion-Szenarien gesammelt, die Lücken in der Legacy-Proofing-Prüfung umgingen. Durch native, einheitliche Überprüfungs- und Genehmigungsfunktionen - einschließlich Genehmigungsvorlagen, Terminerinnerungen und mehrstufiges Routing - werden einige dieser Szenarien nicht mehr benötigt. Evaluieren Sie bei der Klassifizierung jedes Szenarios, ob es durch eine native Funktion ersetzt werden kann. Ein Szenario außer Kraft zu setzen ist langfristig oft sauberer als es wieder aufzubauen.

## Verwandte Artikel

* [Wechseln zu Workfront auf Adobe Cloud-Speicher](/help/quicksilver/review-and-approve-work/workfront-storage.md)
* [Einheitliche Prüfung und Genehmigung - Übersicht](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Erste Schritte mit der einheitlichen Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Erstellen einer Genehmigungsvorlage für Assets und Dokumente](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
