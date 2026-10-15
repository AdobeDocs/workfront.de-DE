---
product-area: documents
navigation-topic: approvals
title: Von alten Dokumentengenehmigungen zu einheitlichen Genehmigungen wechseln
description: Erfahren Sie, was mit Ihren bestehenden Dokumentgenehmigungs-Workflows geschieht, wenn Ihr Unternehmen auf eine Version von Workfront wechselt, die einheitliche Genehmigungen unterstützt.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 4f63b6c4f4c73bedba707aed6b02c9046f9b356c
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 3%
---
# Von alten Dokumentengenehmigungen zu einheitlichen Genehmigungen wechseln

Adobe Cloud-Speicherprojekte verwenden standardmäßig einheitliche Genehmigungen. In diesem Artikel werden die Funktionen beschrieben, die bei einheitlichen Genehmigungen im Vergleich zu alten Dokumentgenehmigungen verfügbar sind.


>[!NOTE]
>
>Einheitliche Genehmigungen sind die Standardeinstellung nur für neue Objekte, die im Adobe Cloud-Speicher erstellt wurden. Ältere Workfront-Speicherobjekte behalten ihren aktuellen Genehmigungs-Service bei.<br>
>Weitere Informationen finden Sie unter [Wechseln zu Workfront auf Adobe Cloud-Speicher](/help/quicksilver/review-and-approve-work/workfront-storage.md).

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

In-Flight-Genehmigungen, die in Legacy-Dokumentgenehmigungen erstellt wurden, funktionieren weiterhin wie zuvor. Neue Genehmigungen für Adobe Cloud-Speicherobjekte verwenden einheitliche Genehmigungen. Neue Genehmigungen für veraltete Workfront-Speicherobjekte behalten den Genehmigungs-Service bei, den diese Objekte bereits verwenden.


## Vorbereiten des Wechsels

* Teilen Sie den [Erste Schritte mit der einheitlichen Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) mit Ihren Endbenutzern.
* Überprüfen Sie Ihre vorhandenen Workfront Fusion-Szenarien. Wenn Sie veraltete Dokumentengenehmigungen mit Proofing verwenden, lesen Sie [Aktualisieren von Workfront Fusion-Szenarien für eine einheitliche Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md) bevor Sie Teams in den Adobe Cloud-Speicher integrieren.
* Richten Sie in den Arbeitsflächen-Dashboards ein Prüfungs- und Genehmigungs-Dashboard ein, um alte Genehmigungsberichte zu ersetzen. Weitere [ finden Sie unter „Erstellen eines Dashboards für ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md) und Validierungen“.


### Hilfeartikel für Endbenutzer

* [Erste Schritte mit der einheitlichen Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Verfügbare Funktionen für Dokumentgenehmigungen](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/asset-review-and-approval.md)
* [Einheitliche Prüfung und Genehmigung - Übersicht](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Überprüfen und Genehmigen mit dem Frame.io-Viewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/review-with-frame.md)
* [Gemeinsames Verwenden von einheitlichen Genehmigungen und Proofing](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md)
* [Überblick über den Entscheidungsstatus eines Dokuments](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md)
* [Erste Schritte mit dem Workfront Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md)
