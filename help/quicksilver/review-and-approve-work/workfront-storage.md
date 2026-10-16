---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: Wechseln zu Workfront auf Adobe Cloud-Speicher
description: Planen Sie Ihren Wechsel zu Workfront im Adobe Cloud-Speicher. Erfahren Sie, was passiert, wenn Ihr Unternehmen aktiviert ist, was sich in Adobe Cloud-Speicherobjekten unterscheidet und wie Sie es zu Ihrem eigenen Zeitpunkt einführen können.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 7a21293ad984311b274fe6a7c79e081e9bc8b156
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---
# Wechseln zu Workfront auf Adobe Cloud-Speicher

Workfront auf Adobe Cloud Storage bietet das vollständige, einheitliche Prüf- und Genehmigungs-Erlebnis: Überprüfungen im Frame.io-Viewer, leistungsstarke Genehmigungs-Workflows, produktübergreifende Sichtbarkeit von Assets und mehr.

Dieser Artikel ist der Ausgangspunkt für Workfront-Administratoren, die zum Adobe Cloud-Speicher wechseln. Es erklärt, was passiert, wenn Sie die Adobe-Cloud-Datenspeicherung aktivieren, verweist auf die Details der Unterschiede und Links zu den Artikeln, die Sie bei der Planung und dem Rollout der Änderung unterstützen.

## Sie entscheiden, wann der Adobe-Cloud-Speicher aktiviert wird

Ihre Workfront-Umgebung ändert sich erst, wenn ein Workfront-Administrator die Adobe-Cloud-Datenspeicherung als standardmäßige Speicheroption unter **Setup** > **System** > **Voreinstellungen** aktiviert. Bis dahin bleiben Ihre bestehenden Projekte und alle neuen Projekte, die Sie erstellen, auf veraltetem Workfront-Speicher und behalten den Genehmigungs-Service, den Sie heute verwenden.

Wenn ein Administrator die Adobe-Cloud-Datenspeicherung als standardmäßige Speicheroption aktiviert:

* Neue Projekte verwenden Adobe Cloud-Speicher
* Frame.io ist der Standard-Viewer
* Einheitliche Genehmigungen sind der Standard-Genehmigungsdienst

Bestehende Projekte ändern sich nicht.

Da Sie den zeitlichen Ablauf steuern, können Sie das Erlebnis testen, Ihre Workfront Fusion-Szenarien aktualisieren und Berichtsänderungen planen, bevor jemand damit arbeitet. Eine schrittweise Anleitung finden Sie unter [Aktivieren von Adobe Cloud Storage für Ihr Unternehmen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

## Funktionsweise von Validierungen im Adobe Cloud-Speicher

Adobe Cloud-Speicherprojekte verwenden standardmäßig einheitliche Genehmigungen, die im Frame.io-Viewer überprüft und genehmigt werden. Objekte, die im alten Workfront-Speicher verbleiben, behalten den von ihnen bereits verwendeten Genehmigungsdienst bei: ältere Dokumentengenehmigungen oder einheitliche Genehmigungen.

>[!NOTE]
>
>Wenn Sie Adobe-Cloud-Speicher als Standard festlegen, ändert sich der Genehmigungs-Service, der bereits in Ihren veralteten Workfront-Speicherobjekten verwendet wird, nicht. Einheitliche Genehmigungen sind die Standardeinstellung nur für neue Objekte, die im Adobe Cloud-Speicher erstellt wurden.

Stellen Sie vor dem Rollout des Adobe-Cloud-Speichers sicher, dass die Personen, die die Genehmigungen verwalten, wissen, was zu erwarten ist. Weitere Informationen finden Sie unter [Von alten Dokumentengenehmigungen zu einheitlichen Genehmigungen &#x200B;](/help/quicksilver/review-and-approve-work/move-to-unified-approvals.md).

## Umzug planen

Bearbeiten Sie diese Artikel bei der Vorbereitung in der richtigen Reihenfolge:

* [Was sich beim Adobe-Cloud-Speicher unterscheidet](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md): Die wichtigsten Unterschiede bei Adobe-Cloud-Speicherobjekten, vom neuen Dokumentbereich und dem Frame.io-Viewer bis zu Benennungsregeln, Speicherkontingent und Fusion.
* [Planen des Adobe Cloud-Speicher-Rollouts](/help/quicksilver/review-and-approve-work/plan-adobe-cloud-storage-rollout.md): Wählen Sie eine Rollout-Konfiguration, führen Sie Pilotprojekte mit einer einzigen Gruppe durch und Sequenzieren Sie die Arbeit, damit es für Ihre Anwender keine Überraschungen gibt.
* [Aktivieren der Adobe-Cloud-Datenspeicherung für Ihr &#x200B;](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md): Die Schritte zum Festlegen der Standardspeicheroption für Ihr gesamtes Unternehmen oder für bestimmte Gruppen.
* [Ältere Objekte in Adobe-Cloud-Speicher konvertieren](/help/quicksilver/review-and-approve-work/convert-objects-to-adobe-cloud-storage.md) Die drei Fälle, in denen Sie ein älteres Objekt in Adobe-Cloud-Speicher konvertieren können und was während jeder Konvertierung bewegt wird.


## Verwandte Artikel

* [Übersicht über den Adobe Cloud-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md)
* [Einheitliche Prüfung und Genehmigung - Übersicht](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Erste Schritte mit der einheitlichen Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Der Bereich „Dokumente“](/help/quicksilver/documents/managing-documents/documents-area.md)
* [Objektberechtigungen und Übersicht über die Zugriffsebene für das Adobe-Cloud-Speichermodell](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)
