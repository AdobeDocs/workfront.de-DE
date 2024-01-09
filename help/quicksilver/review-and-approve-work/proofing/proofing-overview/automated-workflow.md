---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: Übersicht über den automatisierten Workflow
description: Mithilfe automatisierter Workflows können Sie eine Reihe sequenzieller oder paralleler Prüfungsschritte erstellen, Abhängigkeiten zwischen diesen Phasen festlegen und deren Sichtbarkeit auf bestimmte Benutzer beschränken. Wenn Ihr Überprüfungsprozess voneinander abhängig ist, verschieben die automatisierten Workflows Ihren Testversand automatisch durch die Phasen und benachrichtigen dabei die relevanten Validierer und Genehmiger.
author: Courtney
feature: Digital Content and Documents
exl-id: d643970a-c00c-4fb4-94bc-fca4e090dcc9
source-git-commit: 1fd3b135682c096f1715e5da0455fed12e882582
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# Übersicht über den automatisierten Workflow

<!-- Audited: 01/2024 -->

Mithilfe automatisierter Workflows können Sie eine Reihe sequenzieller oder paralleler Prüfungsschritte erstellen, Abhängigkeiten zwischen diesen Phasen festlegen und deren Sichtbarkeit auf bestimmte Benutzer beschränken. Wenn Ihr Überprüfungsprozess voneinander abhängig ist, verschieben die automatisierten Workflows Ihren Testversand automatisch durch die Phasen und benachrichtigen dabei die relevanten Validierer und Genehmiger. Informationen zum Einrichten eines automatisierten Workflows finden Sie unter [Erstellen eines erweiterten Testversands mit einem automatisierten Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

**Beispiele:**  Automatisierte Workflows helfen Ihnen bei der Verwaltung komplexer Testprozesse wie:

* Wenn verschiedene Gruppen oder Validierer Inhalte in einer bestimmten Reihenfolge überprüfen müssen
* Wenn es Abhängigkeiten zwischen der Aktivität von Benutzern beim Überprüfen von Inhalten gibt
* Wenn Inhalte regelmäßig von denselben Personengruppen geprüft werden
* Wann Sie den Zeitraum steuern möchten, in dem die validierenden Benutzer den Inhalt ansehen
* Wenn Sie eine Prüfungsaktivität privat halten möchten

## Phasen

Für jede Phase des automatisierten Workflows können Sie Einstellungen wie einen Termin für die Bühne, eine Sperrung auf einer Bühne, einen als Entscheidungsträger für die Bühne festgelegten Überprüfer und eine Datenschutzeinstellung konfigurieren, die es nur bestimmten Personen ermöglicht, Reviewer-Kommentare auf der Bühne zu sehen.

Die Phasen können manuell, bei der Erstellung eines Testversands, beim Erreichen eines Termins, zu einem bestimmten Datum und einer bestimmten Uhrzeit oder bei einer Entscheidung über die übergeordnete Phase aktiviert werden.

Phasen können manuell gesperrt werden, ebenso wie der Zeitpunkt, zu dem die nächste Phase beginnt oder alle Entscheidungen auf der Bühne getroffen werden. Sie können auch wählen, eine Bühne nie zu sperren.

Sie können einen Entscheidungsträger für eine Phase bestimmen. Die Entscheidung dieser Person macht alle anderen Entscheidungen für die Phase überflüssig.

Ebenso können Sie festlegen, dass nur eine Entscheidung für eine Phase erforderlich ist. Wenn Sie dies tun, wird der Überprüfungsprozess für die Phase als abgeschlossen markiert, nachdem ein Empfänger seine Entscheidung auf der Bühne getroffen hat.

Sie können alle validierungsverantwortlichen Benutzer über ihre Einladung zur Inhaltsüberprüfung benachrichtigen lassen, wenn der Überprüfungsprozess beginnt, oder Sie können jeden Validierer nur benachrichtigen lassen, wenn seine Phase aktiviert ist.

## Private Phasen

Standardmäßig sind Kommentare, die von Validierern in allen Phasen hinterlassen werden, für alle sichtbar, die den Inhalt überprüfen und E-Mail-Benachrichtigungen sowie Kommentar-Zusammenfassungen zum Review-Prozess erhalten.

Wenn Sie verhindern möchten, dass bestimmte Gruppen von Validierern die Kommentare anderer Validierer sehen, können Sie private Bühnen erstellen.

Private Bühnen sind nur für validierende Benutzer sichtbar, die diesen Bühnen hinzugefügt wurden. Sie sind auch für Benutzer sichtbar, die über Bearbeitungsrechte für Testversand- oder Bearbeitungsrechte für alle Elemente verfügen, die im Adobe Workfront-Konto Ihres Unternehmens erstellt wurden (Supervisor und höher oder Benutzer mit benutzerdefinierten Profilen, für die die Bearbeitung von Informationen anderer Personen aktiviert ist).

Kommentare, die von Teilnehmern privater Phasen hinzugefügt werden, sind nicht in E-Mail-Benachrichtigungen und in Zusammenfassungen von Testkommentaren enthalten, die von Personen angefordert werden, die nicht über die Berechtigung zum Anzeigen verfügen.

## Workflow-Diagramm

Das Workflow-Diagramm ist eine visuelle Darstellung des Überprüfungsprozesses Ihres Testversands. Während Sie die Details eines Testversands erstellen oder anzeigen, werden Ihnen die Reihenfolge der Bühnen und alle Abhängigkeiten zwischen Bühnen angezeigt. Alle privaten Bühnen werden mit einem Schlüsselsymbol angezeigt.

![intro-to-aw-example-chart.png](assets/intro-to-aw-example-diagram-350x199.png)

In Live-Testsendungen werden Staging-Abhängigkeiten mit einer gestrichelten grauen Linie für inaktive Bühnen oder einer durchgehenden schwarzen Linie für aktive Bühnen angezeigt. Die Phasen werden grün angezeigt, wenn der Genehmigungsprozess innerhalb der festgelegten Frist abgeschlossen wurde. Phasen, die sich ihren Terminen nähern, werden orange dargestellt und Phasen, die ihre Termine überschreiten, werden rot dargestellt.

![workflow_2.png](assets/workflow-2-350x183.png)

## Automatisierte Workflow-Vorlagen

Wenn Ihr Unternehmen denselben Überprüfungsprozess für mehrere Testsendungen verwendet, kann Ihr Workfront-Administrator automatisierte Workflow-Vorlagen erstellen, um die Erstellung von Testsendungen erheblich zu vereinfachen. Sie können eine Vorlage für den automatisierten Workflow auswählen, während Sie einen Testversand konfigurieren, um die Bühnen und Validierer in dieser Vorlage zum Testversand hinzuzufügen. Sie können die auf den Testversand angewendete Vorlage nach Bedarf vor und nach der Erstellung des Testversands ändern.

Ihr Workfront-Administrator kann entsprechend den Anforderungen Ihres Unternehmens eine unbegrenzte Anzahl von Vorlagen erstellen.

Weitere Informationen zum Erstellen, Verwenden und Verwalten von Vorlagen erhalten Sie von Ihrem Workfront-Administrator.
