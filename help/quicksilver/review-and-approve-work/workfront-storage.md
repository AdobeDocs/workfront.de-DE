---
product-area: documents
navigation-topic: approvals
title: Wechsel zu Workfront auf Adobe Enterprise Storage
description: Planen Sie den Rollout von Workfront auf Adobe Enterprise Storage. Erfahren Sie, was sich bei Adobe Enterprise-Speicherobjekten unterscheidet, einschließlich des neuen Dokumentbereichs und des Prüfungserlebnisses von Frame.io, und entscheiden Sie, wie Adobe Enterprise-Speicher in Ihrer Umgebung eingesetzt wird.
author: Courtney
feature: System Setup and Administration, Work Management, Digital Content and Documents
role: Admin
source-git-commit: 8daaeacae50e0f0245c2783fd6c827da192ae706
workflow-type: tm+mt
source-wordcount: '2360'
ht-degree: 0%

---

# Wechsel zu Workfront auf Adobe Enterprise Storage

Workfront auf Adobe Enterprise Storage ermöglicht die vollständige, einheitliche Überprüfung und Genehmigung: Überprüfungen im Frame.io-Viewer, leistungsstarke Genehmigungs-Workflows, produktübergreifende Sichtbarkeit von Assets und mehr.

Die vorhandenen Objekte funktionieren weiterhin so, wie sie es heute tun. Der neue Dokumentbereich, der Frame.io-Viewer und andere Verhaltensweisen von Adobe Enterprise Storage gelten nur für Objekte, die Adobe Enterprise Storage verwenden.

Dieser Artikel richtet sich an Workfront-Administratoren, die den Rollout von Workfront auf Adobe Enterprise Storage vorbereiten. Es behandelt die wichtigsten Unterschiede zu Adobe Enterprise-Speicherobjekten, die Wahl des Rollout-Typs und die Frage, was zu beachten ist, bevor Sie Adobe Enterprise-Speicher für Ihre Anwender aktivieren.

>[!IMPORTANT]
>
>Ihr Workfront-Vertrag muss eine v2 Workfront SKU enthalten, damit der Frame.io-Viewer und Adobe Enterprise Storage verwendet werden können. Weitere Informationen finden Sie in den häufig gestellten Fragen unter [Einheitliche Überprüfung und Genehmigung - Übersicht](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md#getting-started-with-unified-review-and-approval).



## Legacy-Speicher von Workfront und Adobe Enterprise-Speicher

Nachdem Ihr Vertrag aktualisiert wurde, um das neue einheitliche Überprüfungs- und Validierungserlebnis einzuschließen, kann Ihre Umgebung zwei Objekttypen enthalten: Objekte auf veraltetem Workfront-Speicher (die Objekte, die Sie heute haben) und Objekte, die mit Adobe Enterprise-Speicher erstellt wurden. Auf allgemeiner Ebene unterscheiden sich die beiden Speichermodelle je nachdem, wo die Daten gespeichert sind, welche Adobe-Produkte sie sehen können und welche Funktionen verfügbar sind:

|  | Objekt im alten Workfront-Speicher | Objekt im Adobe Enterprise-Speicher |
|---|---|---|
| Speicher-Backend | Nur Workfront | Adobe Enterprise-Speicher |
| Produktübergreifende Sichtbarkeit | Nur Workfront | Workfront, Frame.io und Creative Cloud |
| Funktionalität | Alte Funktionalität | Neue Funktionen |

Objekte, die erstellt wurden, bevor der Adobe Enterprise-Speicher im Bereich „Setup“ aktiviert wurde, verbleiben im alten Workfront-Speicher. Die in diesem Artikel beschriebenen neuen Verhaltensweisen gelten nur für Adobe Enterprise-Speicherobjekte, die Sie und Ihre Benutzerinnen und Benutzer erstellen, sobald Adobe Enterprise-Speicher aktiviert ist.

## Was ist anders bei Adobe Enterprise Storage?

Die größte tägliche Änderung mit Adobe Enterprise Storage ist der neue Dokumentbereich und der Frame.io-Viewer, der die Überprüfung und Genehmigung innerhalb des Bereichs ermöglicht. Es gibt weitere Unterschiede, die sich auf die Verwaltung von Objekten, Dokumenten und Reviews auswirken.

In der folgenden Tabelle sind die wichtigsten Unterschiede beim Wechsel zu Adobe Enterprise Storage aufgeführt. Jeder Bereich in der Tabelle ist mit dem folgenden detaillierten Abschnitt verknüpft.

| Bereich | Was ist anders | Was Sie wissen sollten |
|---|---|---|
| [Der Bereich „Neue Dokumente“](#the-new-documents-area) | Ein neu gestalteter, einheitlicher Dokumentbereich ersetzt den alten Dokumentbereich. | Kein globaler Dokumentbereich. Zugriff auf Dokumente aus einem Programm, Portfolio, Projekt, einer Aufgabe oder einem Problem. |
| [Dokumentberechtigungen](#document-permissions) | Dokumente übernehmen Berechtigungen aus dem Projekt, der Aufgabe oder dem Problem, mit dem bzw. dem sie verknüpft sind. | Sie können keine Berechtigungen für einzelne Dokumente freigeben oder festlegen. Sie verwalten den gesamten Zugriff über das Modal „Objektfreigabe“ in Workfront, das an systemgenerierte Dokumentordner kaskadiert wird. |
| [Objektberechtigungszuordnung](#object-permissions-mapping) | Die Berechtigungen Verwalten und Beitragen von Workfront sind beide in Frame.io den Optionen Bearbeiten und Freigeben zugeordnet. Karten nur zu Kommentaren anzeigen. | Berechtigungen werden in Workfront verwaltet. Benutzer von „Verwalten“ und „Beitragen“ erhalten in Frame.io externe Freigabefunktionen. |
| [Prüfungs- und Genehmigungs-Viewer](#review-and-approval-viewer) | Der Frame.io-Viewer ersetzt den Workfront Proofing Viewer. | Enthalten für alle Workfront-Anwender mit einer kostenpflichtigen -Lizenz. Unterstützt Markup, Kommentare mit Zeitstempel, Versionsverlauf, Mobile, 40+ Formate, Dateien mit bis zu 500 GB. |
| [Regeln für die Objektbenennung](#object-naming-rules) | Es gelten strenge Benennungsregeln: eindeutige Namen innerhalb eines Portfolios oder Projekts, keine Sonderzeichen, kein abschließender Punkt oder Leerzeichen, 255-Zeichen-Limit. | Workfront benennt Objekte bei Konflikten automatisch um. Audit-Vorlagen, die neue Projektnamen und -strukturen generieren. |
| [Objektportabilität](#object-portability) | Sie können Objekte nur wie Speichermodelle zwischen Objekten verschieben, kopieren und konvertieren. | Adobe Enterprise-Speicherobjekte können nicht in ältere Projekte verschoben werden oder umgekehrt. Wenn Sie ein Adobe Enterprise-Speicherprojekt in ein veraltetes Portfolio oder Programm verschieben, wird das übergeordnete Element in Adobe Enterprise-Speicher konvertiert. |
| [Funktionen nicht verfügbar](#capabilities-not-available-on-adobe-enterprise-storage-objects) | Workfront Proof, der Workfront-Dokument-Viewer, Favoriten-Dokumente und Anfragedokumente sind nicht Teil des Erlebnisses. | Ältere Objekte behalten diese Funktionen bei. Workfront Proof erhält keine neuen Investitionen und wird in einer zukünftigen Version eingestellt. |
| [Speicherquote](#storage-quota) | Der Speicher wird für ältere Workfront-Projekte und Adobe-Unternehmensprojekte zusammengelegt. 60 GB pro lizenziertem Benutzer. Keine feste Mütze. | Systemadministratoren können die Speicherverwendung auf der Seite „Kundeninformationen“ im Setup einsehen. |
| [Jährliche Begrenzung der Videoprüfung](#annual-video-review-cap) | Obergrenze auf Organisationsebene für Anfragen zu Videoprüfungen bei 10 % der gebührenpflichtigen Workfront-Benutzerlizenzen (Standard und Light). | Nach dem Erreichen werden bis zum nächsten Jahreszeitraum keine neuen Videoprüfungen durchgeführt. In-App-Benachrichtigungen bei 80 % und 100 %. Gilt nicht für Frame.io Enterprise-Kunden. |
| [Workfront Fusion](#workfront-fusion-on-adobe-enterprise-storage-projects) | Vorhandene, auf Korrekturabzügen basierende Fusion-Szenarien funktionieren nicht automatisch für Adobe Enterprise-Speicherprojekte. | Szenarien, die sich auf Legacy-Projekte beziehen, funktionieren weiterhin. Jedes betroffene Szenario erhält einen von drei Pfaden: bearbeiten, neu erstellen oder einstellen. Für das 3. Quartal 2026 werden neue Connectoren erwartet. |

### Der neue Dokumentbereich

Der neue Dokumentbereich ist ein einheitliches Dokumenterlebnis für Adobe Enterprise-Speicher. Es vereinfacht die Navigation, konsolidiert Prüf- und Genehmigungsaktivitäten und ist der Einstiegspunkt für den Frame.io-Viewer.

Der Bereich Globale Dokumente ist nicht Teil der neuen -Version. In Enterprise-Speicherprojekten von Adobe greifen Sie über ein Programm, ein Portfolio, ein Projekt, eine Aufgabe oder ein Problem auf Dokumente zu.

Weitere Informationen finden Sie unter [Bereich Dokumente](/help/quicksilver/documents/managing-documents/documents-area.md).

### Dokumentberechtigungen

Dokumentberechtigungen unterscheiden sich grundlegend von Adobe Enterprise-Speicherprojekten:

* Sie können keine Berechtigungen für einzelne Dokumente freigeben oder festlegen. Stattdessen werden Berechtigungen auf systemgenerierte Dokumentordner angewendet, die die Dokumente enthalten.
* Systemgenerierte Dokumentordner übernehmen Berechtigungen vom übergeordneten Projekt, der übergeordneten Aufgabe oder dem übergeordneten Problem.
* Unterordner erben Berechtigungen vom übergeordneten systemgenerierten Dokumentordner.
* Teilaufgaben erben keine Berechtigungen von übergeordneten Aufgaben. Sie müssen einer Unteraufgabe direkt hinzugefügt werden, um auf ihren systemgenerierten Dokumentenordner zuzugreifen.


Weitere Informationen zur Funktionsweise von Dokumentberechtigungen finden Sie unter [Objektberechtigungen und Zugriffsebene - Übersicht für das Adobe Enterprise-Speichermodell](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).


### Zuordnung von Objektberechtigungen

Berechtigungen werden in Workfront festgelegt und fließen in eine Richtung durch zu Frame.io. Sie können Benutzende nicht zu einem Adobe Enterprise-Speicherprojekt in Frame.io einladen oder Benutzerberechtigungen in Frame.io ändern.

>[!TIP]
>
>Trainieren Sie Projektkoordinatoren dafür, dass der Zugriff auf Frame.io eine nachgelagerte Reflektion der Workfront-Berechtigungen ist. Wenn ein Stakeholder meldet, dass er nicht auf eine Überprüfung für ein Adobe Enterprise-Speicherprojekt zugreifen kann, erfolgt die Fehlerbehebung in Workfront - nicht in Frame.io.

In der folgenden Tabelle sind Workfront-Objektberechtigungen den Frame.io-Berechtigungen zugeordnet:

| Berechtigung für Workfront | Frame.io-Berechtigung |
|---|---|
| Verwalten | Bearbeiten und Freigeben |
| Mitwirken | Bearbeiten und Freigeben |
| Ansicht | Nur Kommentar |

Zuordnung von Verwalten und Beitragen zu **Bearbeiten und Freigeben** in Frame.io. Berücksichtigen Sie bei der Überprüfung Ihrer Freigabemuster für Adobe Enterprise-Speicherprojekte, ob es Ihrem Governance-Modell entspricht, dass Mitwirkende dieselben Funktionen für die Überprüfungsseite wie Manager haben, einschließlich der externen Freigabe.

Weitere Informationen finden Sie unter [Objektberechtigungen und Zugriffsebene - Übersicht für das Adobe Enterprise-Speichermodell](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#permission-mapping-to-frameio).


### Prüfer und Validierungsanzeiger

Bei Adobe Enterprise-Speicherobjekten ist der Frame.io-Viewer die Überprüfungs- und Validierungsoberfläche anstelle von Workfront Proof. Der Frame.io-Viewer ist für alle Workfront-Benutzer mit einer kostenpflichtigen -Lizenz enthalten.

Der Frame.io-Viewer bietet:

* Markup- und Kommentar-Tools, einschließlich Freihandzeichnung und Standardformen wie Kreise, Pfeile und Quadrate
* Mit Zeitstempel versehene Kommentare mit rahmengenauer Präzision für Videobesprechungen
* Versionsverlauf und Versionsvergleich
* Mobile-Zugriff für Überprüfungen und Genehmigungen von unterwegs
* Unterstützung von über 40 Dateiformaten, einschließlich aller gängigen Video-, Bild-, Audio-, PDF- und Microsoft Office-Typen, mit nativer Wiedergabe für professionelle Videoformate wie ProRes, H.265 und DNxHD sowie Unterstützung für Dateien mit bis zu 500 GB


### Benennungsregeln für Objekte

Adobe Enterprise Storage erzwingt strenge Benennungs- und Strukturregeln, um die Speicherschicht über alle Adobe-Produkte hinweg konsistent zu halten. Diese Regeln gelten für Objekte, die Sie in Enterprise-Speicherprojekten von Adobe erstellen. Bestehende ältere Projekte behalten ihre aktuellen Namen bei.

Die folgenden Regeln gelten für Adobe Enterprise Storage-Projekte:

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
>Wenn Sie Adobe Enterprise-Speicherprojekte aus Vorlagen erstellen, überprüfen Sie Ihre vorhandenen Vorlagen, damit die Projektnamen und die Struktur, die sie generieren, den obigen Regeln entsprechen.


### Objektportabilität

Sie können Workfront-Objekte wie Speichermodelle zwischen verschiedenen Modellen verschieben, kopieren und konvertieren. Sie können beispielsweise eine Aufgabe von einem Adobe Enterprise-Speicherprojekt in ein anderes Adobe Enterprise-Speicherprojekt verschieben. Sie können eine Aufgabe oder ein Problem nicht aus einem Adobe Enterprise-Speicherprojekt in ein Legacy-Projekt oder umgekehrt verschieben oder kopieren.

Wenn Sie heute ein Adobe Enterprise-Speicherprojekt erstellen oder in ein veraltetes Portfolio oder Programm verschieben, wird das Portfolio oder Programm automatisch in ein Adobe Enterprise-Speicherobjekt konvertiert. In einer zukünftigen Version erhalten Systemadministratoren mehr Kontrolle darüber, welche Objekte automatisch konvertiert werden.

### Funktionen für Adobe Enterprise-Speicherobjekte nicht verfügbar

Die folgenden Funktionen sind nicht Teil von Adobe Enterprise-Speicherobjekten:

* Workfront-Korrekturabzug
* Der Workfront-Dokument-Viewer
* Favoriten-Dokumente
* Dokumente anfordern

Ältere Projekte behalten den Zugriff auf Workfront Proof und die oben aufgeführten alten Dokumentfunktionen bei. Workfront Proof erhält in Zukunft keine neuen Investitionen mehr und wird in einer zukünftigen Version eingestellt.

### Speicherquote

Der Speicher wird für ältere Workfront-Objekte und Adobe Enterprise-Speicherobjekte gepoolt. Jeder lizenzierte Benutzer erhält 60 GB Speicher. Es gibt keine feste Obergrenze für die Speichernutzung, aber Workfront-Administratoren erhalten E-Mail-Benachrichtigungen, wenn die Nutzung 75 %, 90 % und 100 % des Kontingents erreicht.

Systemadministratoren können unter **Setup** > **System** > **Kundeninformationen** die aktuelle Speichernutzung und das aktuelle Kontingent anzeigen.

Weitere Informationen finden Sie unter [Überprüfen von Dokumentspeicherbeschränkungen](/help/quicksilver/documents/managing-documents/check-document-storage.md).


### Jährliche Begrenzung der Videoprüfung

Für Anfragen zum Nachweis von Videos gilt eine jährliche Obergrenze von 10 % der gesamten gebührenpflichtigen Workfront-Benutzerlizenzen Ihres Unternehmens (Standard und Light). Diese Begrenzung wird auf Organisationsebene angewendet.

* Workfront-Administratoren erhalten In-App-Benachrichtigungen, wenn die Nutzung 80 % und 100 % der Obergrenze erreicht.
* Sobald die Obergrenze erreicht ist, können Sie erst im nächsten Jahreszeitraum neue Videoüberprüfungsanfragen erstellen.
* Diese Beschränkung gilt nicht für Frame.io Enterprise-Kunden. Wenn Ihr Unternehmen regelmäßig große Mengen an Videoinhalten überprüft, wenden Sie sich an Ihren Adobe-Kundenbetreuer, um mehr über die Frame.io Enterprise-Lizenzierung zu erfahren.

Weitere Informationen finden Sie in den häufig gestellten Fragen zum Überprüfen und Genehmigen von Assets und Videos unter [Einheitliche Überprüfung und Genehmigung - Übersicht](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

### Workfront Fusion für Enterprise-Storage-Projekte in Adobe

Vorhandene Workfront Fusion-Szenarien, die auf veralteten Proofing-Tests basieren, funktionieren nicht automatisch für Adobe Enterprise-Speicherprojekte. Testversandspezifische Module, Webhooks und API-Endpunkte haben in einigen Fällen direkte Entsprechungen, in anderen sind es signifikante Änderungen. Szenarien, die sich auf ältere Projekte beziehen, funktionieren weiterhin wie bisher.

Fusion-Connectoren mit nativer Unterstützung für einheitliche Überprüfung und Genehmigung werden voraussichtlich im 3. Quartal 2026 verfügbar sein.

Detaillierte Informationen zu den Auswirkungen auf gängige Szenario-Typen und zur Klassifizierung der einzelnen Szenarien als „Bearbeiten“, „Neu erstellen“ oder „Eingestellt“ basierend auf ihrer Funktionalität finden Sie unter [Aktualisieren von Workfront Fusion-Szenarien für eine einheitliche Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).


## Auswählen, wie Adobe Enterprise Storage eingeführt wird

Sie entscheiden, wie Ihre Anwender Adobe Enterprise Storage sehen. Es gibt zwei Konfigurationen, von denen eine auf Ihr gesamtes Unternehmen oder auf bestimmte Workfront-Gruppen angewendet werden kann.

Eine schrittweise Anleitung finden Sie unter [Aktivieren von Adobe Enterprise Storage für Ihr Unternehmen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

* **Nur Adobe Enterprise-Speicher**: Für neue Projekte wird standardmäßig Adobe Enterprise-Speicher verwendet. Benutzende können keine Legacy-Projekte erstellen.
* **Adobe Enterprise Storage und Legacy Workfront Storage**: Wenn Benutzer ein Projekt erstellen, wählen sie zwischen Adobe Enterprise Storage (mit der Bezeichnung „Neues Projekt„) und Legacy Workfront Storage (mit der Bezeichnung „Legacy Storage„).

  ![Wählen Sie einen Projekttyp](assets/choose-project-type.png)



>[!TIP]
>
>Um Adobe Enterprise-Speicher vor ein kleineres Team zu stellen, wenden Sie beide Konfigurationen auf eine einzelne Workfront-Gruppe an. Auf diese Weise können Sie ein zielgerichtetes Pilotprojekt ausführen, bevor Sie es allgemeiner einführen. Es wird empfohlen, mit einem Rollout auf Gruppenebene für kontrolliertes Tempo zu beginnen und dann auf die gesamte Organisation auszuweiten, sobald die Pilotgruppe das Erlebnis validiert hat.

Vorhandene Objekte behalten das Speichermodell bei, mit dem sie erstellt wurden. Durch Ändern der standardmäßigen Speichervoreinstellung wird kein vorhandenes Objekt geändert.

## Planen des Rollouts

Jede Workfront-Umgebung ist anders. Bevor Sie Adobe Enterprise Storage für Ihre Benutzer aktivieren, nehmen Sie sich etwas Zeit, um zu planen, wie ein erfolgreicher Rollout für Ihr Unternehmen aussieht. Die folgenden Vorschläge sind keine Checkliste, sondern ein Ausgangspunkt für Ihren eigenen Plan.

**1. Wählen Sie eine Pilotgruppe.** Bei einem Rollout im Gruppenbereich können Sie den Adobe Enterprise-Speicher vor ein kleineres Team stellen, Feedback einholen und vor einem größeren Rollout anpassen. Wählen Sie eine Gruppe aus, deren Arbeitsmuster repräsentativ genug sind, um Probleme aufzudecken, über die Sie frühzeitig Bescheid wissen möchten.

**2. Kommunizieren Sie die Änderung an die Endbenutzer.** Die größte sichtbare Änderung für Prüfende, genehmigende Personen und Projektbesitzende ist der neue Dokumentbereich und der Frame.io-Viewer, der die Überprüfung und Genehmigung für Adobe Enterprise-Speicherprojekte ermöglicht. Planen Sie, wie Sie diese vorstellen, damit die Anwender wissen, was sie erwarten können, wenn sie auf ihr erstes Adobe Enterprise Storage-Projekt stoßen. Der [Erste Schritte mit der einheitlichen Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md) ist ein nützlicher Ausgangspunkt für Material, das für Endbenutzer bestimmt ist.

**3. Planen Sie die Verfügbarkeit des Workfront Fusion-Connectors.** Fusion-Connectoren mit nativer Unterstützung für einheitliche Überprüfung und Genehmigung werden voraussichtlich im 3. Quartal 2026 verfügbar sein. Bestehende proofbasierte Fusion-Szenarien funktionieren weiterhin an alten Projekten. Bevor Sie Teams, die von diesen Szenarien abhängig sind, in Ihr Pilotprojekt für Unternehmensspeicher in Adobe aufnehmen, entscheiden Sie, ob Sie auf die neuen Connectoren warten, die aktuelle API neu erstellen oder diese Szenarien durch native, einheitliche Prüf- und Genehmigungsfunktionen ersetzen möchten.

Detaillierte Informationen zu den Auswirkungen auf gängige Szenario-Typen und zur Klassifizierung der einzelnen Szenarien als „Bearbeiten“, „Neu erstellen“ oder „Eingestellt“ basierend auf ihrer Funktionalität finden Sie unter [Aktualisieren von Workfront Fusion-Szenarien für eine einheitliche Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/tips-tricks-troubleshooting-approvals/fusion-remediation-for-unified-approvals.md).


## Verwandte Artikel

* [Überblick über Adobe-Unternehmensspeicher](/help/quicksilver/review-and-approve-work/esm-overview.md)
* [Aktivieren von Adobe Enterprise Storage für Ihr Unternehmen](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md)
* [Einheitliche Prüfung und Genehmigung - Übersicht](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)
* [Erste Schritte mit der einheitlichen Überprüfung und Genehmigung](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Der Bereich „Dokumente“](/help/quicksilver/documents/managing-documents/documents-area.md)
* [Objektberechtigungen und Übersicht auf Zugriffsebene für das Adobe Enterprise-Speichermodell](/help/quicksilver/review-and-approve-work/esm-access-permissions.md)

