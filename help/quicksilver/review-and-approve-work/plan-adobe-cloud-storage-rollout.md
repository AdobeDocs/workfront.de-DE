---
user-type: administrator
product-area: documents
navigation-topic: approvals
title: Planen des Rollouts von Adobe Cloud-Speicher
description: Wählen Sie aus, wie der Adobe-Cloud-Speicher Ihren Benutzern angezeigt wird, testen Sie ihn in einer einzigen Gruppe und gestalten Sie die Arbeit so, dass es keine Überraschungen für Prüfer, genehmigende Personen und Projektbesitzer gibt.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
recommendations: noDisplay, noCatalog
exl-id: b4413742-c250-4110-9097-6d38842355a4
source-git-commit: 2b5d95ed0a5c72062700bf026a18b8301e4be421
workflow-type: tm+mt
source-wordcount: '832'
ht-degree: 0%

---
# Planen des Rollouts von Adobe Cloud-Speicher

Sie entscheiden, wie und wann der Adobe-Cloud-Speicher Ihre Anwender erreicht. Es ändert sich nichts, bis ein Workfront-Administrator den Adobe-Cloud-Speicher als standardmäßige Speicheroption im Setup-Bereich festlegt, sodass Sie Zeit haben, das Erlebnis zu testen und Ihre Teams vorzubereiten, bevor jemand daran arbeitet.

In diesem Artikel werden die Rollout-Konfigurationen, die Sie auswählen können, die Pilotierung mit einer einzigen Gruppe und ein empfohlener Arbeitsauftrag behandelt.

## Auswählen, wie der Adobe-Cloud-Speicher bereitgestellt wird

Es gibt zwei Konfigurationen, und Sie können entweder eine auf Ihr gesamtes Unternehmen oder auf bestimmte Workfront-Gruppen anwenden. Jedes Projekt, das im Adobe-Cloud-Speicher erstellt wird, verwendet standardmäßig einheitliche Genehmigungen und den Frame.io-Viewer.

Eine schrittweise Anleitung finden Sie unter [Aktivieren von Adobe Cloud Storage für Ihr Unternehmen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

### Konfigurationsoptionen

* **Nur Adobe-Cloud-Speicher**: Für neue Projekte wird standardmäßig der Adobe-Cloud-Speicher verwendet. Benutzende können keine Legacy-Projekte erstellen.
* **Adobe-Cloud-Speicher und Legacy-Workfront-Speicher**: Wenn Benutzer ein Projekt erstellen, wählen sie zwischen Adobe-Cloud-Speicher (mit „Neues Projekt“ beschriftet) und Legacy-Workfront-Speicher (mit „Legacy-Speicher“ beschriftet). Diese Option wird aktiviert, indem **Kontrollkästchen „Benutzer darf Speicheranbieter auswählen** im Setup-Bereich aktiviert wird.

>[!TIP]
>
>Um den Adobe-Cloud-Speicher vor ein kleineres Team zu stellen, wenden Sie beide Konfigurationen auf eine einzelne Workfront-Gruppe an. Auf diese Weise können Sie ein zielgerichtetes Pilotprojekt ausführen, bevor Sie es allgemeiner einführen. Es wird empfohlen, mit einem Rollout auf Gruppenebene für kontrolliertes Tempo zu beginnen und dann auf die gesamte Organisation auszuweiten, sobald die Pilotgruppe das Erlebnis validiert hat.

Vorhandene Objekte behalten das Speichermodell bei, mit dem sie erstellt wurden. Durch Ändern der standardmäßigen Speichervoreinstellung wird kein vorhandenes Objekt geändert.

![Speichervoreinstellungen im Setup](assets/storage-preference-groups.png)

## Planen des Rollouts

Jede Workfront-Umgebung ist anders. Bevor Sie den Adobe-Cloud-Speicher als Standard für Ihre Benutzerinnen und Benutzer festlegen, sollten Sie sich einige Zeit nehmen, um zu planen, wie ein erfolgreicher Rollout für Ihr Unternehmen aussieht. Die folgenden Vorschläge sind keine exakte Checkliste, sondern ein Ausgangspunkt für Ihren eigenen Plan.

### Pilotengruppe auswählen

Bei einem Rollout im Gruppenbereich können Sie den Adobe-Cloud-Speicher vor ein kleineres Team stellen, Feedback einholen und vor einem größeren Rollout anpassen. Wählen Sie eine Gruppe aus, deren Arbeitsmuster repräsentativ genug sind, um Probleme aufzudecken, über die Sie frühzeitig Bescheid wissen möchten.

<!--
>[!IMPORTANT]
>
>Only members of the pilot group can convert an Adobe cloud storage object, such as a request or a task, into a project. Users outside the group, including Workfront administrators, see the error "User is not eligible for this operation."
-->

### Vor der Live-Schaltung testen

Der Adobe-Cloud-Speicher ist in Workfront-Sandbox-Umgebungen verfügbar, sodass Sie einen Großteil des Erlebnisses vor der Produktion validieren können. Der Frame.io-Viewer ist in Sandbox nicht verfügbar. Daher müssen Sie die vollständige Überprüfung und Genehmigung in der Produktion mit Ihrer Pilotgruppe validieren. Weitere Informationen finden Sie unter [Aktivieren von Adobe-Cloud-Speicher für Ihr Unternehmen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

### Kommunizieren der Änderung an die Endbenutzer

Die größte sichtbare Änderung für Prüfende, genehmigende Personen und Projektbesitzende ist der neue Dokumentbereich und der Frame.io-Viewer, der die Überprüfung und Genehmigung für Adobe Cloud-Speicherprojekte ermöglicht. Planen Sie, wie Sie diese einführen, damit die Anwender wissen, was sie erwarten können, wenn sie auf ihr erstes Adobe Cloud-Speicherprojekt stoßen. Der [Erste Schritte mit der einheitlichen Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) ist ein nützlicher Ausgangspunkt für Material, das für Endbenutzer bestimmt ist.

### Überprüfen Sie Ihre Berechtigungen und Governance

Bei Adobe-Cloud-Speicherprojekten ordnen sowohl Verwalten als auch Beitragen in Frame.io „Bearbeiten und Freigeben“ zu, was die externe Freigabe umfasst. Überprüfen Sie Ihre Freigabemuster und entscheiden Sie, ob dies zu Ihrem Governance-Modell passt, bevor Sie Teams in den Adobe Cloud-Speicher einbinden. Weitere Informationen finden Sie unter [Was sich im Adobe Cloud-Speicher unterscheidet](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md#object-permissions-mapping).

### Audit-Vorlagen und Benennung

Der Adobe-Cloud-Speicher erzwingt strikte Benennungsregeln, und Workfront benennt Objekte, die mit ihnen in Konflikt stehen, automatisch um. Wenn Sie Projekte aus Vorlagen erstellen, überprüfen Sie diese Vorlagen so, dass die Namen und die Struktur, die sie generieren, den Regeln entsprechen. Weitere Informationen finden Sie unter [Was sich im Adobe Cloud-Speicher unterscheidet](/help/quicksilver/review-and-approve-work/adobe-cloud-storage-whats-different.md#object-naming-rules).

### Planen Sie um Workfront Fusion

Vorhandene, auf Korrekturabzügen basierende Fusion-Szenarien funktionieren weiterhin in alten Projekten, funktionieren jedoch nicht automatisch in Adobe Cloud-Speicherprojekten. Bevor Sie Teams, die von diesen Szenarien abhängig sind, in den Adobe-Cloud-Speicher einbinden, klassifizieren Sie jedes Szenario als „Bearbeiten“, „Neu erstellen“ oder „Auslaufen“. Weitere Informationen finden Sie unter [&#x200B; von Workfront Fusion-Szenarien für eine einheitliche Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).

### Planen von Berichtsänderungen

Einheitliche Validierungs-Workflow-Daten und -Berichte werden in den Arbeitsflächen-Dashboards angezeigt. Alte Genehmigungsberichte werden nicht automatisch übernommen. Richten Sie daher ein Ersatz-Dashboard ein, bevor Ihre Pilot-Teams es benötigen. Weitere Informationen finden Sie unter [Erstellen eines Berichts-Dashboards zur Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).

## Vorgeschlagene Sequenz

Diese Reihenfolge als Vorlage verwenden und an Ihre Umgebung anpassen:

1. Testen Sie das Erlebnis in einer Sandbox und mit einer Pilotgruppe in der Produktion.
2. Klassifizieren und aktualisieren Sie Ihre Fusion-Szenarien und erstellen Sie Ihre Berichte für Canvas-Dashboards.
3. Überprüfen Sie Ihre Vorlagen und überprüfen Sie Ihre Berechtigungen und Ihr Freigabemodel.
4. Kommunizieren Sie die Änderung an die validierungsverantwortlichen Personen, genehmigenden Personen und Projektbesitzer, die sie verwenden werden.
5. Legen Sie den Adobe-Cloud-Speicher als Standard für die Pilotgruppe fest und erweitern Sie dann auf weitere Gruppen oder das gesamte Unternehmen, sobald das Pilotprojekt das Erlebnis validiert hat.
