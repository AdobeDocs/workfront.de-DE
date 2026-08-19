---
product-area: documents
navigation-topic: approvals
title: Von alten Dokumentengenehmigungen zu einheitlichen Genehmigungen wechseln
description: Erfahren Sie, was mit Ihren bestehenden Dokumentgenehmigungs-Workflows geschieht, wenn Ihr Unternehmen auf eine Version von Workfront wechselt, die einheitliche Genehmigungen unterstützt.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 8f3c5ed32c6496a13703a5dce771a84462aa7f05
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 3%

---

# Von alten Dokumentengenehmigungen zu einheitlichen Genehmigungen wechseln

Der Wechsel zu einer Version von Workfront, die Adobe Cloud Storage unterstützt, verschiebt Ihr Unternehmen auch von veralteten Dokumentengenehmigungen zu einheitlichen Genehmigungen. Dieser Artikel enthält Informationen dazu, welche Funktionen bei einheitlichen Genehmigungen verfügbar sein werden, sowie Empfehlungen für Workfront-Administratoren, die ältere Dokumentgenehmigungen für Benutzer deaktivieren.


>[!IMPORTANT]
>
>Diese Änderung gilt organisationsweit, sobald Sie zu einer Version von Workfront wechseln, die Adobe Cloud Storage unterstützt. Es gibt keine Option für die Pilotgruppe oder den schrittweisen Rollout für den Wechsel von alten Dokumentengenehmigungen zu einheitlichen Genehmigungen.<br>
>Einzelheiten zu den Änderungen am Adobe-Cloud-Speicher finden Sie unter [Wechseln zu Workfront im Adobe-Cloud-Speicher](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Verstehen, was sich von alten Dokumentengenehmigungen zu einheitlichen Genehmigungen ändert

|  | Legacy-Dokumentgenehmigungen | Einheitliche Genehmigungen |
| --- | --- | --- |
| Genehmigende Personen und Prüfende | Nur von einzelnen Benutzern genehmigen | Validierung oder Überprüfung durch einzelne Benutzer oder Teams |
| Termine und Erinnerungen | Keine automatischen Erinnerungen | Automatische Erinnerungen: 72 Stunden, 24 Stunden und am Fälligkeitsdatum |
| Genehmigungsphasen und -pfade | Eine Genehmigungsphase, keine parallelen Pfade | [Mehrere Genehmigungsphasen und parallele Prüfpfade](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) |
| Genehmigungsvorlagen | Jede Genehmigung von Grund auf neu konfiguriert | [Wiederverwendbare Vorlagen](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) im Workfront-Setup verfügbar |
| Überprüfung und Markup | Proofing-Betrachter | [Proofing Viewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md) auf alten Workfront-Speicherobjekten oder der [Frame.io-Viewer](/help/quicksilver/review-and-approve-work/workfront-storage.md#review-and-approval-viewer) auf Adobe-Cloud-Speicherobjekten |
| KI-gestützte Überprüfung | Nicht verfügbar | Automatische Prüfung der Markenkonformität mit [Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md) |
| Reporting | Legacy-Reporting | Startseite-KPI-Widgets und [Arbeitsflächen-Dashboards](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) |

### Was passiert mit bereits laufenden Genehmigungen?

In-Flight-Genehmigungen, die mit Legacy-Dokumentgenehmigungen erstellt wurden, funktionieren weiterhin wie vor dem Upgrade. Neue Genehmigungen, die nach dem Upgrade erstellt werden, verwenden jedoch einheitliche Genehmigungen.


## Vorbereiten des Upgrades

* Teilen Sie den [Erste Schritte mit der einheitlichen Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) mit Ihren Endbenutzern.
* Überprüfen Sie Ihre vorhandenen Workfront Fusion-Szenarien. Wenn Sie veraltete Dokumentengenehmigungen mit Proofing verwenden, lesen Sie [Aktualisieren von Workfront Fusion-Szenarien für eine einheitliche Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md) bevor Ihr Unternehmen Upgrades durchführt.
* Richten Sie in den Arbeitsflächen-Dashboards ein Prüfungs- und Genehmigungs-Dashboard ein, um alte Genehmigungsberichte zu ersetzen. Weitere [ finden Sie unter „Erstellen eines Dashboards für ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) und Validierungen“.


### Hilfeartikel für Endbenutzer

* [Erste Schritte mit der einheitlichen Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Verfügbare Funktionen für Dokumentgenehmigungen](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md)
* [Einheitliche Prüfung und Genehmigung - Übersicht](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Überprüfen und Genehmigen mit dem Frame.io-Viewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)
* [Gemeinsames Verwenden von einheitlichen Genehmigungen und Proofing](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)
* [Überblick über den Entscheidungsstatus eines Dokuments](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)
* [Erste Schritte mit dem Workfront Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)