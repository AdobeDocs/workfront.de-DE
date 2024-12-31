---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: Automatisierter Workflow - Übersicht
description: Automatisierte Workflows ermöglichen es Ihnen, eine Reihe sequenzieller oder paralleler Überprüfungsphasen zu erstellen, Abhängigkeiten zwischen diesen Phasen festzulegen und die Sichtbarkeit für bestimmte Benutzer zu begrenzen. Wenn es voneinander abhängige Phasen in Ihrem Prüfungsprozess gibt, leiten automatisierte Workflows Ihren Korrekturabzug automatisch durch die Phasen und benachrichtigen dabei die entsprechenden Prüfer und genehmigenden Personen.
author: Courtney
feature: Digital Content and Documents
exl-id: d643970a-c00c-4fb4-94bc-fca4e090dcc9
source-git-commit: 1fd3b135682c096f1715e5da0455fed12e882582
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# Automatisierter Workflow - Übersicht

<!-- Audited: 01/2024 -->

Automatisierte Workflows ermöglichen es Ihnen, eine Reihe sequenzieller oder paralleler Überprüfungsphasen zu erstellen, Abhängigkeiten zwischen diesen Phasen festzulegen und die Sichtbarkeit für bestimmte Benutzer zu begrenzen. Wenn es voneinander abhängige Phasen in Ihrem Prüfungsprozess gibt, leiten automatisierte Workflows Ihren Korrekturabzug automatisch durch die Phasen und benachrichtigen dabei die entsprechenden Prüfer und genehmigenden Personen. Informationen zum Einrichten eines automatisierten Workflows finden Sie unter [Erstellen eines erweiterten Korrekturabzugs mit einem automatisierten Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

**Beispiele:** Automatisierte Workflows helfen Ihnen bei der Verwaltung komplexer Korrekturabzugsüberprüfungsprozesse, wie z. B.:

* Wenn verschiedene Gruppen oder Reviewer Inhalte in einer bestimmten Reihenfolge überprüfen müssen
* Wann es Abhängigkeiten zwischen der Aktivität von Benutzern gibt, wenn diese Inhalte überprüfen
* Wenn Inhalte regelmäßig von denselben Personengruppen überprüft werden
* Wenn Sie den Zeitraum steuern möchten, in dem Reviewer Inhalte anzeigen
* Wenn Sie einige Prüfungsaktivitäten privat halten möchten

## Phasen

Für jede Phase des automatisierten Workflows können Sie Einstellungen wie eine Frist für die Phase, eine Sperre für die Phase, einen Prüfer, der als Entscheidungsträger für die Phase festgelegt ist, und eine Datenschutzeinstellung konfigurieren, die es nur bestimmten Personen ermöglicht, Prüfer-Kommentare auf der Phase zu sehen.

Die Phasen können manuell aktiviert werden, bei der Erstellung eines Korrekturabzugs, beim Erreichen einer Frist, zu einem bestimmten Datum und zu einer bestimmten Uhrzeit oder wenn eine Entscheidung über die übergeordnete Phase getroffen wird.

Die Stadien können manuell gesperrt werden. Dies gilt auch für den Zeitpunkt, zu dem die nächste Phase beginnt oder alle Entscheidungen auf der Bühne getroffen werden. Sie können auch festlegen, dass eine Bühne nie gesperrt werden soll.

Sie können einen primären Entscheidungsträger für eine Phase ernennen. Die Entscheidung dieser Person macht alle anderen Entscheidungen für die Phase überflüssig.

Ebenso können Sie festlegen, dass für eine Phase nur eine Entscheidung erforderlich ist. In diesem Fall wird der Überprüfungsprozess für die Phase als abgeschlossen markiert, nachdem einer der Empfänger seine Entscheidung über die Phase getroffen hat.

Sie können festlegen, dass alle Reviewer über ihre Einladungen zur Inhaltsüberprüfung informiert werden, wenn der Überprüfungsprozess beginnt, oder dass alle Reviewer nur benachrichtigt werden, wenn ihr Schritt aktiviert ist.

## Private Stadien

Standardmäßig sind Kommentare, die von Validierungsverantwortlichen in allen Phasen hinterlassen werden, für alle sichtbar, die den Inhalt überprüfen und E-Mail-Benachrichtigungen und Kommentar-Zusammenfassungen über den Überprüfungsprozess erhalten.

Wenn Sie verhindern möchten, dass bestimmte Gruppen von Reviewern die Kommentare anderer Reviewer sehen, können Sie private Bühnen erstellen.

Private Phasen sind nur für Prüfer sichtbar, die zu diesen Phasen hinzugefügt werden. Sie sind auch für Benutzende sichtbar, die Bearbeitungsrechte für den Korrekturabzug oder Bearbeitungsrechte für alle Elemente haben, die im Adobe Workfront-Konto Ihres Unternehmens erstellt wurden (Supervisor und höher oder Benutzende mit benutzerdefinierten Profilen, für die die Bearbeitung von Informationen anderer Personen aktiviert ist).

Kommentare, die von Teilnehmern des privaten Stadiums hinzugefügt wurden, sind nicht in E-Mail-Benachrichtigungen und Zusammenfassungen von Korrekturabzugskommentaren enthalten, die von Personen angefordert wurden, die nicht über die Berechtigung zum Anzeigen verfügen.

## Workflow-Diagramm

Das Workflow-Diagramm ist eine visuelle Darstellung des Überprüfungsprozesses Ihres Korrekturabzugs. Es zeigt die Reihenfolge der Stadien und alle Abhängigkeiten zwischen den Stadien an, wenn Sie die Details eines Korrekturabzugs erstellen oder anzeigen. Alle privaten Stadien werden mit einem Schlüsselsymbol angezeigt.

![intro-to-aw-example-diagram.png](assets/intro-to-aw-example-diagram-350x199.png)

In Live-Korrekturabzügen werden Stadienabhängigkeiten für inaktive Stadien mit einer gestrichelten grauen Linie oder für aktive Stadien mit einer durchgezogenen schwarzen Linie angezeigt. Die Phasen werden grün angezeigt, wenn der Genehmigungsprozess innerhalb der angegebenen Frist abgeschlossen wurde. Stadien, die sich ihren Terminen nähern, werden orange und Stadien, die nach den Terminen liegen, rot angezeigt.

![workflow_2.png](assets/workflow-2-350x183.png)

## Automatisierte Workflow-Vorlagen

Wenn Ihr Unternehmen denselben Prüfungsprozess für mehrere Korrekturabzüge verwendet, kann Ihr Workfront-Administrator automatisierte Workflow-Vorlagen erstellen, um die Erstellung von Korrekturabzügen zu vereinfachen. Sie können während der Konfiguration eines Korrekturabzugs eine automatisierte Workflow-Vorlage auswählen, um die Phasen und Prüfer in dieser Vorlage zum Korrekturabzug hinzuzufügen. Sie können die auf den Korrekturabzug angewendete Vorlage nach Bedarf vor und nach der Erstellung des Korrekturabzugs ändern.

Ihr Workfront-Administrator kann eine unbegrenzte Anzahl von Vorlagen entsprechend den Anforderungen Ihres Unternehmens erstellen.

Weitere Informationen zum Erstellen, Verwenden und Verwalten von Vorlagen erhalten Sie von Ihrem Workfront-Administrator.
