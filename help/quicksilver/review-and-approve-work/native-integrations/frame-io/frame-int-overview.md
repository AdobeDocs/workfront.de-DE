---
product-area: documents
navigation-topic: approvals
title: Übersicht über die Frame.io-Integration
description: Übersicht über die Frame.io-Integration
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 701f3fc2c885363b5f61fb9d77049c7d4c41963d
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 0%

---


# Übersicht über die Frame.io-Integration

Die Integration von Workfront und Frame.io ermöglicht es Projektkoordinatoren, Projekte zu verwalten und die Arbeit in Workfront zu planen, während Kreative, Marketing-Experten und Stakeholder Assets in Frame.io überprüfen und genehmigen können.

## Basiert auf Adobe Enterprise Storage Management

Kernstück dieser Integration ist Adobe Enterprise Storage Management (ESM) - eine Cloud-basierte Speicherlösung, die als zentrales Repository für Assets in allen Adobe-Unternehmensprodukten dient, einschließlich Workfront und Frame.io.

Zu den wichtigsten Vorteilen von Adobe Enterprise Storage Management gehören:

* Unified Storage Layer für das Kreativ- und Arbeits-Management von Assets
* Zentralisierte Berechtigungen über Adobe IMS für eine sichere Zugriffskontrolle
* End-to-End-Asset-Sichtbarkeit in Workfront-, Frame.io- und Creative Cloud-Apps <!--coming soon?-->
* Skalierbares Speicher- und Kontingent-Management für Unternehmensanforderungen

Weitere Informationen finden Sie unter [Übersicht über das Adobe Enterprise-Speichermanagement](help/quicksilver/review-and-approve-work/esm-overview.md).

## Einheitliche Überprüfung und Genehmigung

Die Integration von Workfront und Frame.io verwendet die einheitlichen Genehmigungsfunktionen von Workfront, um Überprüfungen und Genehmigungen zu verwalten. Mit einheitlichen Genehmigungen können Sie:

* Erstellen und Verwalten von Überprüfungen und Genehmigungen direkt aus Workfront
* Verfolgen Sie den Status von Überprüfungen und Genehmigungen in Echtzeit
* Zentralisieren von Feedback und Validierungen an einem Ort
* Sicherstellen, dass alle Beteiligten Zugriff auf die neuesten Versionen von Assets haben
* Verwendung von KI-Reviewern zur Automatisierung von Überprüfungen der Markenkonformität
* und weitere

Weitere Informationen finden Sie unter [Einheitliche Dokumentengenehmigungen: Artikelindex](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md).


### Frame.io-Viewer verwenden

Die Integration stellt auch eine Verbindung mit dem Frame.io-Viewer her. Der Frame.io-Viewer bietet

* Markup- und Kommentierungswerkzeuge
* Versionsverlauf und -vergleich
* Kommentare mit Zeitstempel für Videobewertungen
* Mobile-Zugriff für Überprüfungen und Genehmigungen von unterwegs

Weitere Informationen finden Sie unter [Erste Schritte mit der Frame.io-Integration](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md).

#### Einschränkungen bei der Videoüberprüfung

<!--need to confirm these-->

#### Unterstützte Dateitypen im Frame.io-Viewer

Der Frame.io-Viewer unterstützt alle gängigen Video-, Bild-, Audio-, PDF- und MS® Office-Typen. Eine detaillierte Liste der unterstützten Dateien finden Sie unter [Typen in Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Zugriff und Lizenzierung für den Frame.io-Viewer

Der Frame.io-Viewer steht allen Workfront-Benutzern mit einer gebührenpflichtigen Lizenz zur Verfügung. Für die Verwendung des Frame.io Viewers für Reviews und Genehmigungen mit dieser Integration ist keine zusätzliche Frame.io-Lizenz erforderlich.

Wenn Ihr Unternehmen zusätzliche Frame.io-Funktionen nutzen möchte, z. B. das direkte Hochladen von Assets in Projekte in Frame.io, können Sie eine Frame.io Enterprise-Lizenz erwerben. <!--link to Frame.io enterprise license info or who to contacT?-->

Die Workfront-Proofing-Funktion ist in dieser Integration nicht verfügbar.

## Leistungsstarkes Projektmanagement in Workfront

Mit der Integration von Workfront und Frame.io können Projektkoordinatoren die leistungsstarken Projektmanagement-Funktionen von Workfront nutzen, um ihre Arbeit zu planen, zu verfolgen und zu verwalten.

Weitere Informationen zum Verwalten von Projekten in Workfront finden Sie [Projekte: Artikelindex](/help/quicksilver/manage-work/projects/projects-toc.md).

### Erzwungene Struktur- und Namenskonventionen

Da diese Integration mithilfe von ESM erstellt wird, müssen beim Verwalten von Projekten und Dokumenten einige erzwungene Struktur- und Benennungskonventionen beachtet werden.

* Objektnamen müssen eindeutig sein und können nicht dupliziert werden
* ESM erfordert eindeutige Namen für Peer-Objekte mit demselben übergeordneten Element in der Hierarchiestruktur
* Dokumente können nicht denselben Namen haben, wenn sie zum selben Projekt gehören

Unter Berücksichtigung dieser Einschränkungen benennt Workfront Objekte oder Dokumente automatisch nach Bedarf um, um Konflikte zu vermeiden.

### Dokumentenverwaltung in Workfront

Dokumente werden mit dieser Integration auf Projektebene verwaltet und können derzeit nicht in Aufgaben oder Probleme hochgeladen werden.

Der Dokumentzugriff wird auch auf Projektebene verwaltet. Wenn ein(e) Benutzende(r) Zugriff auf ein Projekt hat, kann er/sie auf alle mit diesem Projekt verbundenen Dokumente zugreifen.

<!--Documents can't be dragged as full folders.-->

### Einschränkungen beim Dokumenterlebnis

Da diese Integration mit ESM erstellt wird, gibt es einige Einschränkungen beim Original-Dokumenterlebnis in Workfront:

#### Einschränkungen

Die folgenden Funktionen sind nicht in dieser Integration enthalten:

* Externe Dokumentanbieter
* Zugriff auf Proofing
* Dokument-Viewer in Workfront


#### Temporäre Einschränkungen

Derzeit sind die folgenden Funktionen nicht verfügbar:

* Favoriten-Dokumente
* Dokumente anfordern
* Senden von Dokumenten an Adobe Experience Manager Assets
* Mehrstufige Genehmigungen
* Hochladen von Dokumenten zu Kommentaren oder Aktualisierungen in Workfront
* Hochladen von Dokumenten zu Aufgaben oder Problemen in Workfront



