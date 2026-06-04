---
product-area: documents
navigation-topic: approvals
title: Übersicht über den Adobe Cloud-Speicher
description: Übersicht über den Adobe Cloud-Speicher
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YOO4BspMzbMr8iPoXRBKK65IbU5yfpiJndNuYvYF5SM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 958
ht-degree: 0%

---

# Übersicht über den Adobe Cloud-Speicher

Adobe Cloud-Speicher ist eine Cloud-basierte Speicherlösung, die als zentrales Repository für Assets in allen Adobe-Unternehmensprodukten dient. Die Integration von Workfront und Frame.io basiert auf dem Adobe Cloud-Speicher und ermöglicht eine nahtlose Zusammenarbeit und Asset-Management zwischen diesen Plattformen.

Diese Speicheroption ebnet auch den Weg für zukünftige Asset-Management-Integrationen mit anderen Adobe-Produkten wie Adobe Creative Cloud.

## Wichtigste Funktionen

* **Unified Storage Layer**: Der Adobe-Cloud-Speicher fungiert als gemeinsames Speicher-Backend für Workfront, Frame.io, Document Cloud und Creative Cloud. Dies ermöglicht eine nahtlose Zusammenarbeit und Asset-Management über diese Plattformen hinweg.

* **Aktivierung von Content supply chain**: Der Adobe-Cloud-Speicher ist eine grundlegende Komponente für Adobes Content-Supply chain-Vision. Sie ermöglicht es Teams, laufende Assets zu verwalten, ohne dass sie in verschiedenen Adobe-Anwendungen manuell heruntergeladen oder neu hochgeladen werden müssen.

* **Zentralisierte Berechtigungen und Zugriff**: Der Adobe Cloud-Speicher unterstützt Zugriffssteuerungen auf Unternehmensebene und integriert diese in Adobe IMS (Identity Management-System), um sichere und skalierbare Benutzerberechtigungen zu erhalten.

* **End-to-End-Asset-Sichtbarkeit**: Assets, das im Adobe-Cloud-Speicher gespeichert ist, kann direkt in Workfront-, Frame.io- und Creative Cloud-Apps angezeigt und verwaltet werden, um konsistente Metadaten, Versionierung und Audit-Trails bereitzustellen.

* **Integration mit Prüfungs- und Genehmigungs-Workflows**: Der Adobe-Cloud-Speicher ermöglicht kreative Prüfungs- und Genehmigungs-Workflows, da er als Datenquelle für alle Assets dient und sicherstellt, dass Feedback und Genehmigungen zentral verfolgt werden.

* **Skalierbarer Speicher und Kontingent-Management**: Der Adobe Cloud-Speicher bietet skalierbare Speicheroptionen und ein einheitliches Kontingent-Tracking für alle Adobe-Produkte.

## Integration mit Prüfungs- und Genehmigungs-Workflows

Die Integration von Workfront und Frame.io nutzt Adobe Cloud-Speicher, um eine einheitliche Prüfung und Genehmigung zu ermöglichen. Diese Integration ermöglicht es Projektkoordinatoren, Projekte zu verwalten und die Arbeit in Workfront zu planen, während Kreative, Marketing-Experten und Stakeholder Assets in Frame.io überprüfen und genehmigen können. Dadurch wird sichergestellt, dass alle Stakeholder Zugriff auf die neuesten Versionen von Assets haben und das Feedback an einem Ort zentralisiert wird.

Weitere Informationen zur Integration von Workfront und Frame.io finden Sie unter [Einheitliche Überprüfung und Genehmigung - Übersicht](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

## Unterschiede zwischen Adobe Cloud-Speicher und Legacy Workfront-Speicher

Bestehende Workfront-Umgebungen verfügen über eine Kombination aus Adobe-Cloud-Speicher und Legacy-Workfront-Speicher. Alle Objekte, die vor der Veröffentlichung des Adobe-Cloud-Speichers erstellt wurden, verwenden Legacy-Workfront-Speicher.

Sobald Sie die Adobe-Cloud-Datenspeicherung in Ihrer Umgebung aktiviert haben, können Sie sowohl Adobe-Cloud-Datenspeicher- als auch Legacy-Workfront-Speicherprojekte erstellen.

>[!NOTE]
>
>Für neue Umgebungen ist der Adobe-Cloud-Speicher standardmäßig aktiviert und es besteht keine Möglichkeit, den alten Workfront-Speicher zu verwenden.


### Dokumente

#### Bereich „Neue Dokumente“

Der neue Dokumentbereich ist ein einheitlicher Dokumentbereich, der für die Adobe-Cloud-Datenspeicherung neu gestaltet wurde.

Diese aktualisierte Benutzeroberfläche vereinfacht die Navigation, verbessert die Klarheit und erleichtert es Teams, Überprüfungen und Genehmigungen in einer einheitlichen Umgebung zu verwalten. Weitere Informationen finden Sie unter [Übersicht über den Dokumentbereich](/help/quicksilver/documents/managing-documents/documents-area.md).

#### Neues Dokumentberechtigungsmodell

>[!IMPORTANT]
>
>Im Adobe Cloud-Speicher funktionieren Dokumentberechtigungen anders als im alten Workfront-Speicher. Dokumente übernehmen Berechtigungen aus dem Projekt, der Aufgabe oder dem Problem, mit dem bzw. dem sie verknüpft sind.

Dokumente können nicht einzeln freigegeben werden. Stattdessen generiert das System automatisch einen Ordner für jede Aufgabe oder jedes Problem und erbt Berechtigungen von der Aufgabe oder dem Problem. Alle in die Aufgabe oder das Problem hochgeladenen Dokumente werden in diesem generierten Ordner gespeichert.

Weitere Informationen zum neuen Dokumentberechtigungsmodell finden Sie unter [Objektberechtigungen und Zugriffsebene - Übersicht für das Adobe Cloud-Speichermodell](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

##### Verknüpfte Objekte in Ordnern

Auf Projektebene zeigen systemgenerierte Ordner ein verknüpftes Objekt an. Der Ordner erhält automatisch denselben Namen wie die Aufgabe oder das Problem, zu der bzw. dem er gehört. Mithilfe verknüpfter Ordner weiß das System, für welche Aufgabe oder welches Problem der Ordner angezeigt werden soll.

Weitere Informationen finden Sie unter [Funktionsweise von Dokumentberechtigungen](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

## Workfront-Objekte

In der folgenden Tabelle werden die Funktionen des Adobe-Cloud-Speichers und des veralteten Workfront-Speichers für Workfront-Objekte verglichen.

Workfront-Objekte umfassen Portfolios, Programme, Projekte, Vorlagen, Aufgaben und Probleme.

| Cloud-Speicherplatz von Adobe | Legacy Workfront-Speicher |
|---|---|
| <ul><li>Verwendet Adobe Cloud-Speicher</li><li>Integriert mit Frame.io</li><li>Verwendet das neue Dokumenterlebnis</li><li>Erzwingt strikte Benennungskonventionen</li><li>Die direkte Dokumentfreigabe ist nicht verfügbar</li><li>Dokumente sind in anderen Adobe-Produkten wie Frame.io und Creative Cloud verfügbar</li></ul> | <ul><li>Verwendet Workfront-Speicher</li><li>Verwendet die Proofing-Anzeige</li><li>Unterstützt die Freigabe einzelner Dokumente</li></ul> |

### Verschieben, Kopieren und Konvertieren von Objekten

Sie können Workfront-Objekte wie Speichermodelle zwischen verschiedenen Modellen verschieben, kopieren und konvertieren. Sie können beispielsweise eine Aufgabe aus einem Adobe-Cloud-Speicherprojekt in ein anderes Adobe-Cloud-Speicherprojekt verschieben. Sie können eine Aufgabe nicht aus einem Adobe Cloud-Speicherprojekt in ein Legacy-Workfront-Speicherprojekt verschieben.

Diese Aktionen sind über das Menü Mehr zu einer Aufgabe oder einem Problem verfügbar. Jede Aktion respektiert die Dokumentintegrität, die Vererbung von Berechtigungen und die Adobe Cloud-Speicherregeln.

## Aktivieren von Adobe Cloud Storage

Sie müssen eine Version von Workfront verwenden, die den Adobe-Cloud-Speicher unterstützt. Wenn für Ihr Unternehmen noch keine unterstützte Version verfügbar ist, wenden Sie sich an den Adobe-Kundenbetreuer.

Informationen zur Aktivierung der Adobe-Cloud-Datenspeicherung in Ihrer Umgebung finden Sie unter [Aktivieren der Adobe-Cloud-Datenspeicherung für Ihr Unternehmen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

>[!NOTE]
>
>Für neue Kunden ist der Adobe-Cloud-Speicher standardmäßig aktiviert, und sie haben nicht die Möglichkeit, den alten Workfront-Speicher zu verwenden.



## Adobe Cloud-Speicher in Sandbox-Umgebungen

Der Adobe-Cloud-Speicher ist in [!DNL Workfront] Sandbox-Umgebungen verfügbar, sodass Sie ihn testen können, bevor Sie ihn in der Produktionsumgebung aktivieren. Der Frame.io-Viewer ist jedoch nicht in Sandbox verfügbar, sodass das vollständige, einheitliche Überprüfungs- und Validierungserlebnis in der Produktion validiert werden muss.

Wenn Sie über eine benutzerdefinierte Aktualisierungs-Sandbox verfügen, müssen Sie sie nach dem Upgrade auf eine Version von Workfront aktualisieren, die Adobe Cloud Storage unterstützt, um auf die Adobe Cloud Storage-Funktionen in der Sandbox zuzugreifen. Weitere Informationen finden Sie unter [Die benutzerdefinierte  [!DNL Adobe Workfront] -Sandbox-Umgebung](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

## Zu beachten

* Es ist möglich, dass Workfront nicht mehr mit Frame.io oder Creative Cloud synchronisiert ist, z. B. wenn ein Asset in Workfront gelöscht wird, aber weiterhin in Frame.io angezeigt wird, wenden Sie sich an den Workfront-Support, um Ihre Umgebung neu zu synchronisieren.


