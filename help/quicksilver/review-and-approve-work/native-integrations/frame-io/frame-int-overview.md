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
source-git-commit: c4e1961092883f523d04adaacd58129a0379783d
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---


# Übersicht über die Frame.io-Integration

Die Integration von Workfront und Frame.io ermöglicht es Projektkoordinatoren, Projekte zu verwalten und die Arbeit in Workfront zu planen, während Kreative, Marketing-Experten und Stakeholder Assets in Frame.io überprüfen und genehmigen können.

## Auf Adobe Enterprise Storage aufbauend

Kernstück dieser Integration ist Adobe Enterprise Storage, eine Cloud-basierte Speicherlösung, die als zentrales Repository für Assets in allen Adobe-Unternehmensprodukten dient, einschließlich Workfront, Frame.io und Creative Cloud.

Zu den wichtigsten Vorteilen von Adobe Enterprise Storage gehören:

* Unified Storage Layer für das Kreativ- und Arbeits-Management von Assets
* Zentralisierte Berechtigungen über Adobe IMS für eine sichere Zugriffskontrolle
* End-to-End-Asset-Sichtbarkeit in Workfront-, Frame.io- und Creative Cloud-Apps <!--coming soon?-->
* Skalierbares Speicher- und Kontingent-Management für Unternehmensanforderungen

Weitere Informationen finden Sie unter [Übersicht über Adobe Enterprise Storage](/help/quicksilver/review-and-approve-work/esm-overview.md).

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

#### Grenzwerte für Videoprüfungen

Für Anfragen zum Nachweis von Videos gilt eine jährliche Obergrenze von 10 % der gesamten gebührenpflichtigen Workfront-Benutzerlizenzen eines Unternehmens (Standard und Light). Diese Begrenzung wird auf Organisationsebene angewendet.

Workfront-Administratoren erhalten Benachrichtigungen, wenn die Nutzung 80 % und 100 % der Obergrenze erreicht.

Diese Beschränkung gilt nicht für Frame.io Enterprise-Kunden.

#### Unterstützte Dateitypen im Frame.io-Viewer

Der Frame.io-Viewer unterstützt alle gängigen Video-, Bild-, Audio-, PDF- und MS® Office-Typen. Eine detaillierte Liste der unterstützten Dateien finden Sie unter [Typen in Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Zugriff und Lizenzierung für den Frame.io-Viewer

Der Frame.io-Viewer steht allen Workfront-Benutzern mit einer gebührenpflichtigen Lizenz zur Verfügung. Für die Verwendung des Frame.io Viewers für Reviews und Genehmigungen mit dieser Integration ist keine zusätzliche Frame.io-Lizenz erforderlich.

Wenn Ihr Unternehmen zusätzliche Frame.io-Funktionen nutzen möchte, z. B. das direkte Hochladen von Assets in Projekte in Frame.io, können Sie eine Frame.io Enterprise-Lizenz erwerben. Wenden Sie sich an Ihren Adobe-Kundenbetreuer, um eine Demo zu planen und die Vorteile der vollständigen Frame.io-Lösung zu erkunden.

Die Workfront-Proofing-Funktion ist in dieser Integration nicht verfügbar.

## Leistungsstarkes Projektmanagement in Workfront

Mit der Integration von Workfront und Frame.io können Projektkoordinatoren die leistungsstarken Projektmanagement-Funktionen von Workfront nutzen, um ihre Arbeit zu planen, zu verfolgen und zu verwalten.

Weitere Informationen zum Verwalten von Projekten in Workfront finden Sie [Projekte: Artikelindex](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

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

<!--* External document providers-->
* Zugriff auf Proofing
* Dokument-Viewer in Workfront
* Favoriten-Dokumente
* Dokumente anfordern


<!--#### Temporary limitations

For now, the following capabilities are not available:

* Send documents to Adobe Experience Manager Assets
* Multi-stage approvals
* Upload documents to comments or updates in Workfront
* Upload documents to tasks or issues in Workfront-->



