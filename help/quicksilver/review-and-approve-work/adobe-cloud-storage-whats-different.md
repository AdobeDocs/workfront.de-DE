---
product-area: documents
navigation-topic: approvals
title: Unterschiede im Adobe Cloud-Speicher
description: Machen Sie sich mit den wichtigsten Unterschieden bei Adobe Cloud-Speicherobjekten vertraut, einschließlich des neuen Dokumentbereichs, des Frame.io-Viewers, der Dokumentberechtigungen, der Objektnamen, des Speicherkontingents und von Workfront Fusion.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 2b5d95ed0a5c72062700bf026a18b8301e4be421
workflow-type: tm+mt
source-wordcount: '1702'
ht-degree: 0%
---
# Unterschiede im Adobe Cloud-Speicher

Mit dem Adobe-Cloud-Speicher kann Ihre Umgebung zwei Objekttypen enthalten: Objekte auf dem alten Workfront-Speicher (die Objekte, die Sie heute haben) und Objekte, die mit dem Adobe-Cloud-Speicher erstellt wurden. Der neue Dokumentbereich, der Frame.io-Viewer und die anderen hier beschriebenen Verhaltensweisen gelten nur für Objekte, die den Adobe-Cloud-Speicher verwenden.

Eine Orientierung zum Verschieben finden Sie unter [Wechseln zu Workfront auf Adobe Cloud-Speicher](/help/quicksilver/review-and-approve-work/workfront-storage.md).

## Legacy-Workfront-Speicher und Adobe-Cloud-Speicher

Auf allgemeiner Ebene unterscheiden sich die beiden Speichermodelle je nachdem, wo die Daten gespeichert sind, welche Adobe-Produkte sie sehen können und welche Funktionen verfügbar sind:

|  | Objekt im alten Workfront-Speicher | Objekt im Adobe Cloud-Speicher |
|---|---|---|
| Speicher-Backend | Nur Workfront | Cloud-Speicherplatz von Adobe |
| Produktübergreifende Sichtbarkeit | Nur Workfront | Workfront, Frame.io und Creative Cloud |
| Funktionalität | Alte Funktionalität | Neue Funktionen |

Objekte, die vor dem Adobe-Cloud-Speicher erstellt wurden, verbleiben standardmäßig im alten Workfront-Speicher. Die in diesem Artikel beschriebenen Verhaltensweisen gelten nur für Adobe-Cloud-Speicherobjekte, die Sie und Ihre Benutzerinnen und Benutzer erstellen, sobald der Adobe-Cloud-Speicher der Standard ist.

## Zusammenfassung der Unterschiede

Die größte tägliche Änderung mit Adobe Cloud Storage ist der neue Dokumentbereich und der Frame.io-Viewer, der die Überprüfung und Genehmigung darin ermöglicht. Es gibt andere Unterschiede, die sich darauf auswirken, wie Sie Objekte, Dokumente und Reviews verwalten. Jeder Bereich in der folgenden Tabelle ist mit dem folgenden detaillierten Abschnitt verknüpft.

| Bereich | Was ist anders | Was Sie wissen sollten |
|---|---|---|
| [Der Bereich „Neue Dokumente“](#the-new-documents-area) | Ein neu gestalteter, einheitlicher Dokumentbereich ersetzt den alten Dokumentbereich. | Es gibt keinen Bereich für globale Dokumente. Sie greifen über ein Programm, ein Portfolio, ein Projekt, eine Aufgabe oder ein Problem auf Dokumente zu. |
| [Dokumentberechtigungen](#document-permissions) | Dokumente übernehmen Berechtigungen aus dem Projekt, der Aufgabe oder dem Problem, mit dem bzw. dem sie verknüpft sind. | Sie können keine Berechtigungen für einzelne Dokumente freigeben oder festlegen. Sie verwalten den gesamten Zugriff über das Modal „Objektfreigabe“ in Workfront, das an systemgenerierte Dokumentordner kaskadiert wird. |
| [Objektberechtigungszuordnung](#object-permissions-mapping) | Berechtigungen zum Verwalten und Beitragen sind beide in Frame.io den Optionen Bearbeiten und Freigeben zugeordnet. Karten nur zu Kommentaren anzeigen. | Berechtigungen werden in Workfront verwaltet. Benutzer von „Verwalten“ und „Beitragen“ erhalten in Frame.io externe Freigabefunktionen. |
| [Prüfungs- und Genehmigungs-Viewer](#review-and-approval-viewer) | Der Frame.io-Viewer ersetzt den Workfront Proofing Viewer. | Sie ist für alle Workfront-Benutzer enthalten, einschließlich externer Benutzer, die einer Überprüfung oder Genehmigung zugewiesen sind. Es unterstützt Markup, Kommentare mit Zeitstempel, Versionsverlauf, Mobile, 40+ Formate und Dateien mit bis zu 500 GB. |
| [Regeln für die Objektbenennung](#object-naming-rules) | Es gelten strenge Benennungsregeln: eindeutige Namen innerhalb eines Portfolios oder Projekts, keine Sonderzeichen, kein Punkt oder Leerzeichen am Ende und eine Beschränkung auf 255 Zeichen. | Workfront benennt Objekte bei Konflikten automatisch um. Prüfen Sie die Vorlagen, die neue Projektnamen und -strukturen generieren. |
| [Objektportabilität](#object-portability) | In den meisten Szenarien können Sie Objekte nur zwischen Speichermodellen verschieben, kopieren und konvertieren. | Sie können ein älteres Objekt in drei bestimmte Fälle in den Adobe-Cloud-Speicher konvertieren. Dokumente und Dokumentordner werden während der Konvertierung nicht aus dem alten Speicher verschoben. |
| [Funktionen nicht verfügbar](#capabilities-not-available-on-adobe-cloud-storage-objects) | Workfront Proof, der Workfront-Dokument-Viewer, Favoriten-Dokumente und Anfragedokumente sind nicht Teil des Erlebnisses. | Ältere Objekte behalten diese Funktionen bei. Workfront Proof erhält keine neuen Investitionen und wird in einer zukünftigen Version eingestellt. |
| [Speicherquote](#storage-quota) | Der Speicher wird für ältere Workfront-Projekte und Adobe-Cloud-Speicherprojekte mit 60 GB pro lizenziertem Anwender ohne feste Obergrenze gepoolt. | Systemadministratoren können die Speichernutzung auf der Seite „Kundeninformationen“ im Setup einsehen. |
| [Jährliche Begrenzung der Videoprüfung](#annual-video-review-cap) | Für Anfragen zum Nachweis von Videos gilt eine Obergrenze auf Unternehmensebene von 10 % der gebührenpflichtigen Workfront-Benutzerlizenzen (Standard und Light). | Sobald Sie die Obergrenze erreicht haben, können Sie bis zum nächsten Jahreszeitraum keine neuen Videoprüfungen erstellen. In-App-Benachrichtigungen werden zu 80 % bzw. 100 % empfangen. Die Begrenzung gilt nicht für Frame.io Enterprise-Kunden. |
| [Workfront Fusion](#workfront-fusion-on-adobe-cloud-storage-projects) | Vorhandene, auf Korrekturabzügen basierende Fusionsszenarien funktionieren nicht automatisch für Adobe Cloud-Speicherprojekte. | Szenarien, die sich auf Legacy-Projekte beziehen, funktionieren weiterhin. Jedes betroffene Szenario nutzt einen von drei Pfaden: Bearbeiten, Neuerstellen oder Außerkraftsetzung. |

## Der neue Dokumentbereich

Der neue Dokumentbereich ist ein einheitliches Dokumenterlebnis für die Adobe-Cloud-Datenspeicherung. Es vereinfacht die Navigation, konsolidiert Prüf- und Genehmigungsaktivitäten und ist der Einstiegspunkt für den Frame.io-Viewer.

Der Bereich Globale Dokumente ist nicht Teil der neuen -Version. In Adobe Cloud-Speicherprojekten können Sie von einem Programm, einem Portfolio, einem Projekt, einer Aufgabe oder einem Problem aus auf Dokumente zugreifen.

Weitere Informationen finden Sie unter [Bereich Dokumente](/help/quicksilver/documents/managing-documents/documents-area.md).

## Dokumentberechtigungen

Dokumentberechtigungen unterscheiden sich grundlegend von Adobe Cloud-Speicherprojekten:

* Sie können keine Berechtigungen für einzelne Dokumente freigeben oder festlegen. Stattdessen werden Berechtigungen auf die systemgenerierten Dokumentordner angewendet, die die Dokumente enthalten.
* Systemgenerierte Dokumentordner übernehmen Berechtigungen vom übergeordneten Projekt, der übergeordneten Aufgabe oder dem übergeordneten Problem.
* Unterordner erben Berechtigungen vom übergeordneten systemgenerierten Dokumentordner.
* Teilaufgaben erben keine Berechtigungen von übergeordneten Aufgaben. Sie müssen einer Unteraufgabe direkt hinzugefügt werden, um auf ihren systemgenerierten Dokumentenordner zuzugreifen.

Weitere Informationen zur Funktionsweise von Dokumentberechtigungen finden Sie unter [Objektberechtigungen und Zugriffsebene - Übersicht für das Adobe-Cloud-Speichermodell](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

## Zuordnung von Objektberechtigungen

Berechtigungen werden in Workfront festgelegt und fließen in eine Richtung durch zu Frame.io. Sie können Benutzende nicht zu einem Adobe-Cloud-Speicherprojekt in Frame.io einladen oder Benutzerberechtigungen in Frame.io ändern.

>[!TIP]
>
>Trainieren Sie Projektkoordinatoren dafür, dass der Zugriff auf Frame.io eine nachgelagerte Reflektion der Workfront-Berechtigungen ist. Wenn ein Stakeholder meldet, dass er nicht auf eine Überprüfung für ein Adobe Cloud-Speicherprojekt zugreifen kann, erfolgt die Fehlerbehebung in Workfront und nicht in Frame.io.

In der folgenden Tabelle sind Workfront-Objektberechtigungen den Frame.io-Berechtigungen zugeordnet:

| Berechtigung für Workfront | Frame.io-Berechtigung |
|---|---|
| Verwalten | Bearbeiten und Freigeben |
| Mitwirken | Bearbeiten und Freigeben |
| Ansicht | Nur Kommentar |

Zuordnung von Verwalten und Beitragen zur Bearbeitung und Freigabe in Frame.io. Berücksichtigen Sie bei der Überprüfung Ihrer Freigabemuster für Adobe Cloud-Speicherprojekte, ob es Ihrem Governance-Modell entspricht, dass Mitwirkende dieselben Funktionen für die Überprüfungsseite wie Manager haben, einschließlich der externen Freigabe.

Weitere Informationen finden Sie unter [Objektberechtigungen und Zugriffsebene - Übersicht für das Adobe-Cloud-Speichermodell](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#permission-mapping-to-frameio).

## Prüfer und Validierungsanzeiger

Bei Adobe-Cloud-Speicherobjekten ist der Frame.io-Viewer die Überprüfungs- und Validierungsoberfläche anstelle von Workfront Proof. Der Frame.io-Viewer ist für alle Workfront-Benutzer ohne zusätzliche Kosten enthalten, einschließlich externer Benutzer, die einer Überprüfung oder Genehmigung zugewiesen sind.

Der Frame.io-Viewer bietet:

* Markup- und Kommentar-Tools, einschließlich Freihandzeichnung und Standardformen wie Kreise, Pfeile und Quadrate
* Mit Zeitstempel versehene Kommentare mit rahmengenauer Präzision für Videobesprechungen
* Versionsverlauf und Versionsvergleich
* Mobile-Zugriff für Überprüfungen und Genehmigungen von unterwegs
* Unterstützung von über 40 Dateiformaten, einschließlich aller gängigen Video-, Bild-, Audio-, PDF- und Microsoft Office-Typen, mit nativer Wiedergabe für professionelle Videoformate wie ProRes, H.265 und DNxHD sowie Unterstützung für Dateien mit bis zu 500 GB

## Benennungsregeln für Objekte

Der Adobe Cloud-Speicher erzwingt strenge Benennungs- und Strukturregeln, um die Speicherschicht über alle Adobe-Produkte hinweg konsistent zu halten. Diese Regeln gelten für Objekte, die Sie in Adobe Cloud-Speicherprojekten erstellen. Bestehende ältere Projekte behalten ihre aktuellen Namen bei.

Die folgenden Regeln gelten für Adobe Cloud-Speicherprojekte:

| Regel | Detail |
|---|---|
| Eindeutige Programm- und Projektnamen | Programme und Projekte können nicht denselben Namen haben, wenn sie demselben Portfolio angehören. |
| Eindeutige Dokumentnamen | Dokumente können nicht denselben Namen haben, wenn sie zum selben Projekt gehören. Dokumentnamen müssen innerhalb desselben übergeordneten Elements in der Ordnerhierarchie eindeutig sein. |
| Unzulässige Zeichen | Programme, Portfolios, Projekte, Vorlagen, Aufgaben, Probleme, Dokumentordner und Dokumente dürfen keine der folgenden Sonderzeichen enthalten: `\ / : * ? " \| < >` |
| Nachfolgende Zeichen | Programme, Portfolios, Projekte, Vorlagen, Aufgaben, Probleme und Dokumentordner dürfen keine Namen haben, die mit einem Punkt oder einer Leerstelle enden. |
| Längenlimit für Namen | Objektnamen sind auf 255 Zeichen beschränkt. |

Wenn ein Name mit diesen Regeln in Konflikt steht, benennt Workfront das Objekt automatisch um, um den Konflikt zu lösen.

>[!TIP]
>
>Wenn Sie Adobe-Cloud-Speicherprojekte aus Vorlagen erstellen, überprüfen Sie Ihre vorhandenen Vorlagen, damit die Projektnamen und die Struktur, die sie generieren, den obigen Regeln entsprechen.

## Objektportabilität

In den meisten Szenarien können Sie Workfront-Objekte nur zwischen Speichermodellen verschieben, kopieren und konvertieren. Sie können beispielsweise eine Aufgabe von einem Adobe-Cloud-Speicherprojekt in ein anderes Adobe-Cloud-Speicherprojekt verschieben. In drei bestimmten Fällen können Sie ein veraltetes Workfront-Speicherobjekt in Adobe Cloud-Speicher konvertieren.

<!--
During a group-scoped rollout, only members of the group that has Adobe cloud storage can convert an Adobe cloud storage object, such as a request, into a project. Users outside the group, including Workfront administrators, see the error "User is not eligible for this operation."

For more information, see [Plan your Adobe cloud storage rollout](/help/quicksilver/review-and-approve-work/plan-adobe-cloud-storage-rollout.md).
-->

Weitere Informationen finden Sie unter [Konvertieren veralteter Objekte in Adobe Cloud-Speicher](/help/quicksilver/review-and-approve-work/convert-objects-to-adobe-cloud-storage.md).

## Funktionen nicht verfügbar in Adobe Cloud-Speicherobjekten

Die folgenden Funktionen sind nicht Teil von Adobe Cloud-Speicherobjekten:

* Workfront-Korrekturabzug
* Der Workfront-Dokument-Viewer
* Favoriten-Dokumente
* Dokumente anfordern

Ältere Projekte behalten den Zugriff auf Workfront Proof und die oben aufgeführten alten Dokumentfunktionen bei. Workfront Proof erhält in Zukunft keine neuen Investitionen mehr und wird in einer zukünftigen Version eingestellt.

## Speicherquote

Der Speicher wird für ältere Workfront-Objekte und Adobe-Cloud-Speicherobjekte gepoolt. Jeder lizenzierte Benutzer erhält 60 GB Speicher. Es gibt keine feste Obergrenze für die Speichernutzung, aber Workfront-Administratoren erhalten E-Mail-Benachrichtigungen, wenn die Nutzung 75 %, 90 % und 100 % des Kontingents erreicht.

Die aktuelle Speichernutzung und das aktuelle Kontingent finden Sie unter **Setup** > **System** > **Kundeninformationen**.

Weitere Informationen finden Sie unter [Überprüfen von Dokumentspeicherbeschränkungen](/help/quicksilver/documents/managing-documents/check-document-storage.md).

## Jährliche Begrenzung der Videoprüfung

Für Anfragen zum Nachweis von Videos gilt eine jährliche Obergrenze von 10 % der gesamten gebührenpflichtigen Workfront-Benutzerlizenzen Ihres Unternehmens (Standard und Light). Diese Begrenzung wird auf Organisationsebene angewendet.

* Workfront-Administratoren erhalten In-App-Benachrichtigungen, wenn die Nutzung 80 % und 100 % der Obergrenze erreicht.
* Wenn Sie die Obergrenze erreicht haben, können Sie bis zum nächsten Jahreszeitraum keine neuen Videoüberprüfungsanfragen erstellen.
* Diese Beschränkung gilt nicht für Frame.io Enterprise-Kunden. Wenn Ihr Unternehmen regelmäßig große Mengen an Videoinhalten überprüft, wenden Sie sich an Ihren Adobe-Kundenbetreuer, um mehr über die Frame.io Enterprise-Lizenzierung zu erfahren.

Weitere Informationen finden Sie in den häufig gestellten Fragen zum Überprüfen und Genehmigen von Assets und Videos unter [Einheitliche Überprüfung und Genehmigung - Übersicht](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

## Workfront Fusion in Adobe Cloud-Speicherprojekten

Bestehende Workfront Fusion-Szenarien, die auf veralteten Proofing-Tests basieren, funktionieren nicht automatisch für Adobe Cloud-Speicherprojekte. Testversandspezifische Module, Webhooks und API-Endpunkte haben in einigen Fällen direkte Entsprechungen, in anderen sind es signifikante Änderungen. Szenarien, die sich auf ältere Projekte beziehen, funktionieren weiterhin wie bisher.

Detaillierte Informationen zu den Auswirkungen auf gängige Szenario-Typen und zur Klassifizierung der einzelnen Szenarien als „Bearbeiten“, „Neu erstellen“ oder „Eingestellt“ basierend auf ihrer Funktionalität finden Sie unter [Aktualisieren von Workfront Fusion-Szenarien für eine einheitliche Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).
