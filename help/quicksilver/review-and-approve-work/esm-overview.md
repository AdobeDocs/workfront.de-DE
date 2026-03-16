---
product-area: documents
navigation-topic: approvals
title: Überblick über Adobe-Unternehmensspeicher
description: Überblick über Adobe-Unternehmensspeicher
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 16c564a9-abd7-4b07-be3e-9c823f40177d
source-git-commit: 7f17ffc179914747d29c4acb08b34341c5a4b7b4
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 1%

---

# Überblick über Adobe-Unternehmensspeicher

Adobe Enterprise Storage ist eine Cloud-basierte Speicherlösung, die als zentrales Repository für Assets in allen Adobe Enterprise-Produkten dient. Die Integration von Workfront und Frame.io basiert auf Adobe Enterprise Storage und ermöglicht eine nahtlose Zusammenarbeit und Asset-Management zwischen diesen Plattformen.

Diese Speicheroption ebnet auch den Weg für zukünftige Asset-Management-Integrationen mit anderen Adobe-Produkten wie Adobe Creative Cloud.

## Wichtigste Funktionen

* **Unified Storage Layer**: Adobe Enterprise-Speicher fungiert als gemeinsam genutztes Speicher-Backend für Workfront, Frame.io, Document Cloud und Creative Cloud. Dies ermöglicht eine nahtlose Zusammenarbeit und Asset-Management über diese Plattformen hinweg.

* **Aktivierung von Content supply chain**: Adobe Enterprise Storage ist eine grundlegende Komponente für Adobe Content Supply chain und ermöglicht es Teams, laufende Assets zu verwalten, ohne dass sie in verschiedenen Adobe-Anwendungen manuell heruntergeladen oder neu hochgeladen werden müssen.

* **Zentralisierte Berechtigungen und Zugriff**: Adobe Enterprise Storage unterstützt Zugriffssteuerungen auf Unternehmensebene und integriert diese in Adobe IMS (Identity Management-System), um sichere und skalierbare Benutzerberechtigungen zu erhalten.

* **End-to-End-Asset-Sichtbarkeit**: Assets, das im Adobe Enterprise-Speicher gespeichert ist, kann direkt in Workfront-, Frame.io- und Creative Cloud-Apps angezeigt und verwaltet werden, um konsistente Metadaten, Versionierung und Audit-Trails bereitzustellen.

* **Integration mit Prüfungs- und Genehmigungs-Workflows**: Adobe Enterprise Storage ermöglicht kreative Prüfungs- und Genehmigungs-Workflows, da sie als Datenquelle für alle Assets dienen und sicherstellen, dass Feedback und Genehmigungen zentral verfolgt werden.

* **Skalierbarer Speicher und Quotenverwaltung**: Adobe Enterprise-Speicher bietet skalierbare Speicheroptionen und eine einheitliche Quotenverfolgung für alle Adobe-Produkte.

## Integration mit Prüfungs- und Genehmigungs-Workflows

Die Integration von Workfront und Frame.io nutzt Adobe Enterprise Storage, um eine einheitliche Prüfung und Genehmigung zu ermöglichen. Diese Integration ermöglicht es Projektkoordinatoren, Projekte zu verwalten und die Arbeit in Workfront zu planen, während Kreative, Marketing-Experten und Stakeholder Assets in Frame.io überprüfen und genehmigen können. Dadurch wird sichergestellt, dass alle Stakeholder Zugriff auf die neuesten Versionen von Assets haben und das Feedback an einem Ort zentralisiert wird.

Weitere Informationen zur Integration von Workfront und Frame.io finden Sie unter [Übersicht über die Frame.io-Integration](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md).

## Unterschiede zwischen Adobe Enterprise-Speicher und Legacy-Workfront-Speicher

Bestehende Workfront-Umgebungen verfügen über eine Kombination aus Adobe Enterprise-Speicher und Legacy-Workfront-Speicher. Alle Objekte, die vor der Veröffentlichung von Adobe Enterprise Storage erstellt wurden, verwenden Legacy-Workfront-Speicher.

Sobald Sie Adobe Enterprise-Speicher in Ihrer Umgebung aktiviert haben, können Sie sowohl Adobe Enterprise-Speicher als auch ältere Workfront-Speicherprojekte erstellen.

>[!NOTE]
>
>Für neue Umgebungen ist standardmäßig Adobe Enterprise Storage aktiviert, und es besteht keine Option zur Verwendung des alten Workfront-Speichers.


### Dokumente

#### Bereich „Neue Dokumente“

Der neue Dokumentbereich ist ein einheitlicher Dokumentbereich, der für Adobe Enterprise-Speicher neu konzipiert wurde.

Diese aktualisierte Benutzeroberfläche vereinfacht die Navigation, verbessert die Klarheit und erleichtert es Teams, Überprüfungen und Genehmigungen in einer einheitlichen Umgebung zu verwalten. Weitere Informationen finden Sie unter [Übersicht über den Dokumentbereich](/help/quicksilver/documents/managing-documents/documents-area.md).

#### Neues Dokumentberechtigungsmodell

>[!IMPORTANT]
>
>Im Adobe Enterprise-Speicher funktionieren Dokumentberechtigungen anders als im alten Workfront-Speicher. Dokumente übernehmen Berechtigungen aus dem Projekt, der Aufgabe oder dem Problem, mit dem bzw. dem sie verknüpft sind.

Dokumente können nicht einzeln freigegeben werden. Stattdessen generiert das System automatisch einen Ordner für jede Aufgabe oder jedes Problem und erbt Berechtigungen von der Aufgabe oder dem Problem. Alle in die Aufgabe oder das Problem hochgeladenen Dokumente werden in diesem generierten Ordner gespeichert.

Weitere Informationen zum neuen Dokumentberechtigungsmodell finden Sie unter [Objektberechtigungen und Zugriffsebene - Übersicht für das Adobe Enterprise-Speichermodell](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

##### Verknüpfte Objekte in Ordnern

Auf Projektebene zeigen systemgenerierte Ordner ein verknüpftes Objekt an. Der Ordner erhält automatisch denselben Namen wie die Aufgabe oder das Problem, zu der bzw. dem er gehört. Mithilfe verknüpfter Ordner weiß das System, für welche Aufgabe oder welches Problem der Ordner angezeigt werden soll.

Weitere Informationen finden Sie unter [Funktionsweise von Dokumentberechtigungen](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

## Workfront-Objekte

In der folgenden Tabelle werden die Funktionen von Adobe Enterprise Storage und Legacy Workfront Storage für Workfront-Objekte verglichen.

Workfront-Objekte umfassen Portfolios, Programme, Projekte, Vorlagen, Aufgaben und Probleme.

| Adobe Enterprise-Speicher | Legacy Workfront-Speicher |
|---|---|
| <ul><li>Verwendet Adobe Enterprise-Speicher</li><li>Integriert mit Frame.io</li><li>Verwendet das neue Dokumenterlebnis</li><li>Erzwingt strikte Benennungskonventionen</li><li>Die direkte Dokumentfreigabe ist nicht verfügbar</li><li>Dokumente sind in anderen Adobe-Produkten wie Frame.io und Creative Cloud verfügbar</li></ul> | <ul><li>Verwendet Workfront-Speicher</li><li>Verwendet die Proofing-Anzeige</li><li>Unterstützt die Freigabe einzelner Dokumente</li></ul> |

### Verschieben, Kopieren und Konvertieren von Objekten

Sie können Workfront-Objekte wie Speichermodelle zwischen verschiedenen Modellen verschieben, kopieren und konvertieren. Sie können beispielsweise eine Aufgabe aus einem Adobe Enterprise-Speicherprojekt in ein anderes Adobe Enterprise-Speicherprojekt verschieben. Sie können eine Aufgabe nicht aus einem Adobe Enterprise-Speicherprojekt in ein Legacy-Workfront-Speicherprojekt verschieben.

Diese Aktionen sind über das Menü Mehr zu einer Aufgabe oder einem Problem verfügbar. Jede Aktion respektiert die Dokumentintegrität, die Vererbung von Berechtigungen und die Speicherregeln von Adobe Enterprise.

## Adobe Enterprise Storage aktivieren

Bestehende Kunden können bei Vertragsverlängerung Adobe Enterprise Storage in ihrer Umgebung aktivieren. Weitere Informationen zur Aktivierung von Adobe Enterprise Storage finden Sie unter [Aktivieren von Adobe Enterprise Storage für Ihr Unternehmen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

>[!NOTE]
>
>Bei neuen Kunden ist der Adobe Enterprise-Speicher standardmäßig aktiviert, und sie haben nicht die Möglichkeit, den alten Workfront-Speicher zu verwenden.



## Aspekte

* Es ist möglich, dass Workfront nicht mehr mit Frame.io oder Creative Cloud synchronisiert ist, z. B. wenn ein Asset in Workfront gelöscht wird, aber weiterhin in Frame.io angezeigt wird. Wenden Sie sich an den Workfront-Support, um Ihre Umgebung neu zu synchronisieren.


