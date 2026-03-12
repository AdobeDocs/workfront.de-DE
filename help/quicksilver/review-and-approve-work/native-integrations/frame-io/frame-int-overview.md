---
product-area: documents
navigation-topic: approvals
title: Überblick über die Frame.io-Integration
description: Überblick über die Frame.io-Integration
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: b5f0150b-40b5-4386-98bc-374e7ca65b74
source-git-commit: e93f8662acb95029e4997ec270b23511d3e880dd
workflow-type: tm+mt
source-wordcount: '859'
ht-degree: 1%

---

# Überblick über die Frame.io-Integration

Die Integration von Workfront und Frame.io ermöglicht es Projektkoordinatoren, Projekte zu verwalten und die Arbeit in Workfront zu planen, während Kreative, Marketing-Experten und Stakeholder Assets in Frame.io überprüfen und genehmigen können.

## Integrationsanforderungen

* Workfront und Frame.io müssen in derselben Identity Management System (IMS)-Organisation bereitgestellt werden.

* Benutzende können nur zu einer Workfront-Instanz innerhalb der IMS-Organisation gehören.

* Die Workfront-Instanz muss im einheitlichen Adobe Experience Manager- und Adobe Enterprise-Speicher aktiviert werden.

* Die Integration muss von Adobe Professional Services konfiguriert werden.


## Auf Adobe Enterprise Storage aufbauend

Kernstück dieser Integration ist Adobe Enterprise Storage, eine Cloud-basierte Speicherlösung, die als zentrales Repository für Assets in allen Adobe-Unternehmensprodukten dient, einschließlich Workfront und Frame.io. <!--, and Creative Cloud.-->

Zu den wichtigsten Vorteilen von Adobe Enterprise Storage gehören:

* Unified Storage Layer für das Kreativ- und Arbeits-Management von Assets
* Zentralisierte Berechtigungen über das Adobe Identity Management System (IMS) für eine sichere Zugriffskontrolle
* End-to-End-Asset-Sichtbarkeit in Workfront- und Frame.io-<!--, and Creative Cloud apps -->
* Skalierbares Speicher- und Kontingent-Management für Unternehmensanforderungen

Weitere Informationen finden Sie unter [Übersicht über Adobe Enterprise Storage](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Einheitliche Überprüfung und Genehmigung

Die Integration von Workfront und Frame.io verwendet die einheitlichen Genehmigungsfunktionen von Workfront, um Überprüfungen und Genehmigungen zu verwalten. Mit einheitlichen Genehmigungen können Sie:

* Erstellen und Verwalten von Überprüfungen und Genehmigungen direkt aus Workfront
* Verfolgen Sie den Status von Überprüfungen und Genehmigungen in Echtzeit
* Zentralisieren von Feedback und Validierungen an einem Ort
* Sicherstellen, dass alle Beteiligten Zugriff auf die neuesten Versionen von Assets haben
* Verwendung von KI-Reviewern zur Automatisierung von Überprüfungen der Markenkonformität
* und mehr

Weitere Informationen finden Sie unter [Einheitliche Dokumentengenehmigungen: Artikelindex](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-reviews-and-approvals.md).


### Frame.io-Viewer verwenden

Die Integration stellt auch eine Verbindung mit dem Frame.io-Viewer her. Der Frame.io-Viewer bietet

* Markup- und Kommentierungswerkzeuge
* Versionsverlauf und -vergleich
* Kommentare mit Zeitstempel für Videobewertungen
* Mobile-Zugriff für Überprüfungen und Genehmigungen von unterwegs

Weitere Informationen finden Sie unter [Erste Schritte mit der Frame.io-Integration](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/get-started-with-frame-integration.md).

#### Grenzwerte für Videoprüfungen

Für Anfragen zum Nachweis von Videos gilt eine jährliche Obergrenze von 10 % der gesamten gebührenpflichtigen Workfront-Benutzerlizenzen eines Unternehmens - Standard und Light. Diese Begrenzung wird auf Organisationsebene angewendet.

Workfront-Administratoren erhalten Benachrichtigungen, wenn die Nutzung 80 % und 100 % der Obergrenze erreicht.

Diese Beschränkung gilt nicht für Frame.io Enterprise-Kunden.

#### Unterstützte Dateitypen im Frame.io-Viewer

Der Frame.io-Viewer unterstützt alle gängigen Video-, Bild-, Audio-, PDF- und MS® Office-Typen. Eine detaillierte Liste der unterstützten Dateien finden Sie unter [Unterstützte Dateitypen auf Frame.io](https://help.frame.io/en/articles/9436564-supported-file-types-on-frame-io).

#### Zugriff und Lizenzierung für den Frame.io-Viewer

Der Frame.io-Viewer ist der Standard-Viewer für alle Workfront-Prüfungs- und Genehmigungs-Workflows. Es ist automatisch für alle Workfront-Benutzer mit einer gebührenpflichtigen Lizenz enthalten. Für die Verwendung des Frame.io Viewers für Reviews und Genehmigungen ist keine zusätzliche Frame.io-Lizenz erforderlich.

Wenn Ihr Unternehmen die zusätzlichen Frame.io-Funktionen nutzen möchte, die mit dieser Integration verfügbar sind, z. B. das direkte Hochladen von Assets in Projekte in Frame.io, können Sie eine Frame.io Enterprise-Lizenz erwerben. Wenden Sie sich an Ihren Adobe-Kundenbetreuer, um eine Demo zu planen und die Vorteile der vollständigen Frame.io-Lösung zu erkunden.

Die Workfront-Proofing-Funktion ist in dieser Integration nicht verfügbar.

## Leistungsstarkes Projektmanagement in Workfront

Mit der Integration von Workfront und Frame.io können Projektkoordinatoren die leistungsstarken Projektmanagement-Funktionen von Workfront nutzen, um ihre Arbeit zu planen, zu verfolgen und zu verwalten.

Weitere Informationen zum Verwalten von Projekten in Workfront finden Sie [Projekte: Artikelindex](/help/quicksilver/manage-work/projects/create-projects/create-project.md).

### Erzwungene Struktur- und Namenskonventionen

Da diese Integration mit Adobe Enterprise Storage erstellt wird, müssen beim Verwalten von Projekten und Dokumenten einige erzwungene Struktur- und Benennungskonventionen beachtet werden.

* Objektnamen müssen eindeutig sein und können nicht dupliziert werden
* Der Adobe Enterprise-Speicher erfordert eindeutige Namen für Peer-Objekte mit demselben übergeordneten Element in der Hierarchiestruktur
* Dokumente können nicht denselben Namen haben, wenn sie zum selben Projekt gehören
* Dokumentnamen dürfen keines der folgenden Sonderzeichen enthalten: \ / : * ? &quot; | &lt; >
* Dokumentnamen sind auf maximal 255 Zeichen beschränkt

Unter Berücksichtigung dieser Einschränkungen benennt Workfront Objekte oder Dokumente automatisch nach Bedarf um, um Konflikte zu vermeiden.

### Freigabe und Berechtigungen

Im Rahmen der Integration werden Benutzerberechtigungen in Workfront gesteuert und fließen nach unten zu Frame.io. Das bedeutet, dass Sie einen Benutzer nicht zu einem Projekt in Frame.io einladen oder Benutzerberechtigungen in Frame.io ändern können. Diese Aktionen müssen über das Modal „Projektfreigabe“ in Workfront durchgeführt werden.

Die folgende Tabelle zeigt, wie Workfront-Berechtigungen Frame.io-Berechtigungen zugeordnet sind:

<table>
<tr>
<th>Workfront-Benutzerberechtigung</th>
<th>Frame.io-Benutzerberechtigung</th>
</tr>
<tr>
<td>Verwalten</td>
<td>Bearbeiten und Freigeben</td>
</tr>
<tr>
<td>Mitwirken</td>
<td>Bearbeiten und Freigeben</td>
</tr>
<tr>
<td>Ansicht</td>
<td>Nur Kommentar</td>
</tr>
</table>



### Dokumentenverwaltung in Workfront

In Workfront hochgeladene Dokumente werden im Adobe Enterprise-Speicher gespeichert und stehen sowohl in Workfront als auch in Frame.io zur Verfügung. Wenn Sie ein Dokument zu einer Aufgabe oder einem Problem in Workfront hochladen, wird im Adobe Enterprise-Speicher ein systemgenerierter Ordner erstellt, der die Berechtigungen von der Aufgabe oder dem Problem erbt. Alle Dokumente, die in diese Aufgabe oder dieses Problem hochgeladen wurden, werden in diesem Ordner gespeichert und übernehmen Berechtigungen davon. Weitere Informationen zu Dokumenten in Workfront finden Sie unter [Der neue Dokumentbereich - Übersicht](/help/quicksilver/documents/managing-documents/documents-area.md) und [Objektberechtigungen und Zugriffsebene - Übersicht für das Unternehmensspeichermodell von Adobe](/help/quicksilver/review-and-approve-work/esm-access-permissions.md).

### Einschränkungen beim Dokumenterlebnis

Da diese Integration mit dem Adobe Enterprise-Speicher erstellt wird, gibt es einige Einschränkungen beim Original-Dokumenterlebnis in Workfront:

#### Einschränkungen

Die folgenden Funktionen sind nicht in dieser Integration enthalten:

<!--* External document providers-->
* Zugriff auf Proofing in Workfront
* Dokument-Viewer in Workfront
* Favoriten-Dokumente
* Dokumente anfordern