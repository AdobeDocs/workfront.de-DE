---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Verwenden des Adobe Workfront MCP-Servers
description: Verwenden Sie den Adobe Workfront MCP-Server, um Workfront-Elemente über eine Konversation in natürlicher Sprache in einem KI-Assistenten zu suchen, zu erstellen, zu aktualisieren und zu verwalten.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 4517d45ecc653d27d435a8192a612241120dd33f
workflow-type: tm+mt
source-wordcount: '1243'
ht-degree: 2%

---


# Verwenden des Adobe Workfront MCP-Servers

Mit dem [!DNL Adobe Workfront] MCP-Server können Sie Workfront-Elemente suchen, erstellen, aktualisieren und verwalten, indem Sie einen KI-Assistenten in einfachem Englisch anfragen. Der KI-Assistent entscheidet, welche Workfront-Aktionen aufgerufen werden sollen, und übernimmt die Unterhaltung mit Workfront für Sie.

[!DNL Claude] ist derzeit der einzige unterstützte KI-Assistent. Die Beispiele und Muster in diesem Artikel gelten jedoch für alle KI-Assistenten, die den Workfront MCP-Server unterstützen.

In diesem Artikel wird davon ausgegangen, dass Sie die Verbindung bereits eingerichtet haben. Weitere Informationen zum Setup finden Sie unter [Konfigurieren des Adobe Workfront MCP-Servers](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md). Weitere Informationen zum Workfront MCP-Server finden Sie unter [Übersicht über den Adobe Workfront MCP-Server](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).



## Über den Workfront MCP-Server verfügbare Aktionen

Der Workfront MCP-Server umfasst Aktionen für Genehmigungen, Planung und Workflows.

<!-- NEEDS DETAIL: Confirm the full inventory of actions exposed through the Workfront MCP server. The five core actions below are confirmed from Hamilton's walkthrough. The approvals, planning, and workflow sections need to be filled in from Jeff's engineering channel post, hands-on access, and the deck Oznur published in the MCP external channel. -->

>[!IMPORTANT]
>
>Ein KI-Assistent agiert in Workfront unter Verwendung Ihres Workfront-Kontos und Ihrer Berechtigungen. Sie und Ihr KI-Assistenzanbieter sind für die Aktionen verantwortlich, die der KI-Assistent in Ihrem Auftrag durchführt. Bestätigen Sie, was der KI-Assistent tun wird, bevor Sie ihn fortfahren lassen.


## Verantwortung für KI-Assistenzmaßnahmen

Wenn Sie einen KI-Assistenten mit Workfront verbinden, agiert der KI-Assistent in Workfront mithilfe Ihres Workfront-Kontos und Ihrer Berechtigungen. Die Aktionen des KI-Assistenten haben dieselbe Wirkung wie Aktionen, die Sie direkt in der Workfront-Benutzeroberfläche ausführen.

Sie und Ihr KI-Assistentenanbieter sind für die Aktionen verantwortlich, die der KI-Assistent in Workfront durchführt. Adobe übernimmt keine Verantwortung für Änderungen, die der KI-Assistent an Ihren Workfront-Daten vornimmt.

Bevor Sie den KI-Assistenten mit einer Anfrage fortfahren lassen, bestätigen Sie, dass Sie verstehen, was er zu tun beabsichtigt, insbesondere für Aktionen, die Daten ändern oder löschen.

### Zentrale Aktionen

Der Workfront MCP-Server umfasst die folgenden Kernaktionen:

| Aktion | Funktion |
|---|---|
| Erstellen | Erstellt neue Elemente in Workfront. |
| Suchen | Sucht und ruft Elemente aus Workfront ab. |
| Aktualisieren | Ändert bestehende Elemente in Workfront. |
| Löschen | Entfernt Elemente aus Workfront. |
| Auflösen von Feldnamen | Sucht die richtigen Workfront-Feldnamen, damit der KI-Assistent genaue Anfragen für Ihre Daten erstellen kann. |

<!-- NEEDS DETAIL: Confirm which Workfront object types are supported across the core actions (projects, tasks, issues, portfolios, programs, custom forms, planning records, approvals, etc.). -->

### Genehmigungsaktionen

<!-- NEEDS DETAIL: List the approval-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request a marketer might make. -->

### Planungsaktionen

<!-- NEEDS DETAIL: List the planning-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request. -->

### Workflow-Aktionen

<!-- NEEDS DETAIL: List the workflow-specific actions exposed through the Workfront MCP server. For each action, document what it does, what inputs it expects, and an example request. -->

## Beispiele für Fragen

Geben Sie nach der Verbindung Anfragen in natürlicher Sprache in Ihren KI-Assistenten ein. Der KI-Assistent entscheidet, welche Workfront-Aktionen aufgerufen werden sollen, und gibt die Ergebnisse zurück.

<!-- NEEDS DETAIL: Example prompts in this section are adapted from the Workflow Optimization Agent (WOA) examples doc on another branch. Validate each example against a working Claude + Workfront MCP server setup before publication, since WOA and the MCP server may expose different action inventories. -->

### Suchen und Anzeigen Ihrer Arbeit

Bitten Sie den KI-Assistenten, in Workfront nach Elementen zu suchen, die dem Gesuchten entsprechen. Beispiel:

* *Zeigen Sie mir alle aktiven Projekte für das Marken-Marketing-Team.*
* *Erhalte alle Aufgaben, die Joan Harris zugewiesen sind.*
* *Alle Ausgaben im Projekt „Website-Neugestaltung“ in der Kategorie „Technisch“ anzeigen.*

### Neue Elemente erstellen

Bitten Sie den KI-Assistenten, Projekte, Aufgaben oder andere Workfront-Elemente zu erstellen. Beispiel:

* *Erstellen Sie ein leeres Projekt mit dem Namen „Q2 Innovation Sandbox“, das am 10. März beginnt und am 30. April endet. Legen Sie mich als Besitzer fest.*
* *Fügen Sie eine neue Aufgabe mit dem Namen „Landingpage-QA“ zum Projekt hinzu und planen Sie sie vom 22. April bis zum 26. April.*
* *Erstellen Sie einen neuen Kampagnendatensatz mit dem Namen „Summer Sale 2026“*

### Vorhandene Elemente aktualisieren

Bitten Sie den KI-Assistenten, Änderungen an Elementen vorzunehmen, die sich bereits in Workfront befinden. Beispiel:

* *Aktualisieren Sie die Aufgabe „Design Review“ so, dass sie am 18. April abgeschlossen ist, und weisen Sie sie dem Kreativ-Team zu.*
* *Für das Projekt „Lucent AI Launch - NA“ schieben Sie die Ziellinie bis Mitte April und erhöhen Sie das Budget auf 150.000 Dollar.*
* *Aktualisieren Sie das Budgetfeld im Datensatz „Sommerkampagne“ auf 75.000 US-Dollar.*

### Elemente löschen

Bitten Sie den KI-Assistenten, Workfront-Elemente zu entfernen. Beispiel:

* *Löschen Sie das Projekt „Q1 Test Campaign“.*
* *Entfernen Sie die Aufgabe „Asset-Produktion drucken“ aus dem Projekt.*
* *Löschen Sie den Kampagnendatensatz mit dem Namen „Alte Promotion“*

>[!WARNING]
>
>Das Löschen von Elementen in Workfront über einen KI-Assistenten entspricht dem Löschen in der Workfront-Benutzeroberfläche. Bestätigen Sie, was der KI-Assistent löschen soll, bevor Sie ihn fortfahren lassen.

### Arbeiten mit Genehmigungen

Bitten Sie den KI-Assistenten, Dokument- und Asset-Genehmigungen zu verwalten. Beispiel:

* *Fügen Sie Sarah Chen und Miguel Alvarez als genehmigende Personen für das aktuelle Dokument hinzu.*
* *Erinnerung an genehmigende Personen, die nicht geantwortet haben, bezüglich des Assets „Frühlingskampagnenvideo“ senden.*
* *Wenden Sie die Genehmigungsvorlage „Marketing-Launch“ auf das Asset „Frühling-Kampagnenvideo“ an*

<!-- NEEDS DETAIL: Add approvals-specific context from the WOA examples doc, including: content approvals must be enabled for the organization, the AI assistant cannot approve or reject on behalf of humans (except via the Workfront AI Reviewer), and best experience is with the Unified Approvals experience. -->

### Arbeiten mit Planungsdatensätzen

Bitten Sie den KI-Assistenten, Planungsdatensätze zu verwalten. Beispiel:

* *Erstellen Sie einen neuen Planungsdatensatz mit dem Namen „Q2-Marketing-Plan“ für das Brand Marketing-Team.*
* *Fügen Sie eine neue Aufgabe namens „Social Media Audit“ zum Planungsdatensatz hinzu.*
* *Aktualisieren Sie die Aufgabe „Social Media Audit“, sodass sie am 18. April abgeschlossen ist, und weisen Sie sie dem Kreativ-Team zu.*

### Arbeiten mit Workflows

Bitte den KI-Assistenten, den Workflow zu verwalten. Beispiel:

* *Verlegen Sie das Projekt „Q2 Innovation Sandbox“ an das Innovation Review Board.*
* *Aktualisieren des Datensatzes „Sommerkampagne“ auf den Status „Startbereit“.*
* *Genehmigen Sie den Datensatz „Sommerkampagne“.*


### Anforderungen in einer Konversation verketten

Sie können Anfragen in einer einzigen Konversation verketten. Der KI-Assistent behält den Kontext bei, sodass jede Anfrage auf der vorherigen aufbauen kann. Beispiel:

1. Bitten Sie den KI-Assistenten, eine Reihe von Elementen zu finden: *Finden Sie meine überfälligen Aufgaben.*
1. Nachdem der KI-Assistent die Liste zurückgegeben hat, bitten Sie ihn, die Ergebnisse zu bearbeiten: *Aktualisieren Sie alle auf nächsten Freitag.*

<!-- NEEDS DETAIL: Test multi-step prompt chaining in a working setup and document the patterns that produce reliable results. -->

## Zu beachten

Beachten Sie bei der Verwendung des Workfront MCP-Servers die folgenden Punkte.

### Der KI-Assistent kann Informationen aus früheren Gesprächen verwenden

KI-Assistenten verwenden manchmal Daten aus früheren Versionen in einem Gespräch wieder, anstatt Workfront nach dem neuesten zu fragen. Wenn sich in Workfront seit der letzten Überprüfung des KI-Assistenten etwas geändert hat, werden möglicherweise veraltete Informationen angezeigt.

Um den KI-Assistenten zu zwingen, neue Daten abzurufen, fragen Sie explizit danach. Beispiel:

* *Erhalten Sie die neuesten Daten aus Workfront. Keine zwischengespeicherten Ergebnisse verwenden.*

### Der Workfront MCP-Server wird automatisch aktualisiert

Wenn Adobe eine neue Version des Workfront MCP-Servers veröffentlicht, verwendet Ihr KI-Assistent die neue Version automatisch. Sie müssen nichts auf Ihrer Seite neu verbinden oder ändern.

## Daten und Sicherheit

<!-- NEEDS DETAIL: Document Adobe's official position on data handling and security when Workfront data is passed through an AI assistant. Cover: what data leaves Workfront, where it goes, whether it is retained or used for training by the AI assistant provider, what happens to it after the conversation ends, and any differences between AI assistants (for example, Anthropic's enterprise data handling policies for Claude). This section needs sign-off from security and legal before publication. -->

### Welche Daten Workfront verlassen

<!-- NEEDS DETAIL: List the categories of Workfront data that can be sent to the AI assistant (item names, field values, attachments, user identifiers, etc.) and any data that the MCP server explicitly does not expose. -->

### Handhabung von Workfront-Daten durch KI-Assistentenanbieter

<!-- NEEDS DETAIL: For each supported AI assistant, summarize the provider's data handling stance: retention, training opt-out, and enterprise vs. consumer differences. Link to the provider's official documentation. Start with Claude (Anthropic). -->

### Unterschiede zwischen KI-Assistenten

<!-- NEEDS DETAIL: Note any meaningful differences in how each supported AI assistant handles Workfront data once additional AI assistants are supported. -->

## Fehlerbehebung bei der täglichen Verwendung

Weitere Informationen zu Setup- und Authentifizierungsproblemen finden Sie unter [Fehlerbehebung bei Setup und Authentifizierung](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication) in [Konfigurieren des Adobe Workfront MCP-Servers](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

| Problem | Wahrscheinliche Ursache | Korrigieren |
|---|---|---|
| Der KI-Assistent gibt Ihnen veraltete Informationen. | Der KI-Assistent verwendet Daten aus früheren Gesprächen wieder. | Bitten Sie den KI-Assistenten, neue Daten aus Workfront abzurufen. |
| Der KI-Assistent hat Daten aus den falschen Workfront-Elementen zurückgegeben. | Der KI-Assistent wählte die falschen Elemente aufgrund mehrdeutiger Formulierungen aus. | Fragen Sie erneut mit spezifischeren Namen, IDs oder Filtern. |
| Eine Aktualisierung oder Löschung wurde in Workfront nicht wirksam. | Der KI-Assistent hat die Aktion noch nicht aufgerufen, oder Ihre Berechtigungen lassen dies nicht zu. | Bestätigen Sie mit dem KI-Assistenten, dass die Aktion ausgeführt wurde, und überprüfen Sie dann Ihre Workfront-Berechtigungen. |

<!-- NEEDS DETAIL: Add additional day-to-day troubleshooting scenarios discovered during hands-on testing. -->

## Häufig gestellte Fragen

### Mit welchen Workfront-Elementen kann ich über einen KI-Assistenten arbeiten?

Alle Elemente, auf die Sie in Workfront über Zugriffsebenen und Objektberechtigungen Zugriff haben.

<!-- NEEDS DETAIL: List the supported Workfront object types. -->

### Werden meine Workfront-Daten an den KI-Assistentenanbieter gesendet oder von diesem gespeichert?

Weitere Informationen finden Sie unter [ und Sicherheit ](#data-and-security) diesem Artikel.

### Was passiert, wenn eine neue Version des Workfront MCP-Servers veröffentlicht wird?

Der MCP-Server wird automatisch aktualisiert. Sie müssen keine Verbindung wiederherstellen oder etwas ändern.

### Muss ich die Workfront-API kennen, um den Workfront MCP-Server zu verwenden?

Nein. Der KI-Assistent übersetzt Ihre Anfragen in natürlicher Sprache in die richtigen Workfront-Aktionen. Wenn Sie bereits mit der Workfront-API vertraut sind, fühlen sich die Aktionen vertraut an, sind aber keine Voraussetzung.
