---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Verwenden des Adobe Workfront MCP-Servers
description: Verwenden Sie den Adobe Workfront-MCP-Server, um Workfront-Elemente über eine Sprachkonversation in einer KI-Agentenplattform zu suchen, zu erstellen, zu aktualisieren und zu verwalten.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 152486b7850e01f3de23f22bbe3729c5cd3d3aa2
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 1%

---


# Verwenden des Adobe Workfront MCP-Servers

Mit dem [!DNL Adobe Workfront] MCP-Server können Sie Workfront-Elemente suchen, erstellen, aktualisieren und verwalten, indem Sie eine KI-Agentenplattform in einfachem Englisch anfragen. Die -Plattform entscheidet, welche Workfront-Aktionen aufgerufen werden sollen, und übernimmt die Unterhaltung mit Workfront für Sie.

[!DNL Claude] ist derzeit die einzige unterstützte KI-Agentenplattform. Die Beispiele und Muster in diesem Artikel gelten jedoch für alle KI-Agentenplattformen, die den Workfront MCP-Server unterstützen.

In diesem Artikel wird davon ausgegangen, dass Sie die Verbindung bereits eingerichtet haben. Weitere Informationen zum Setup finden Sie unter [Konfigurieren des Adobe Workfront MCP-Servers](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md). Weitere Informationen zum Workfront MCP-Server finden Sie unter [Übersicht über den Adobe Workfront MCP-Server](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-overview.md).

## Verfügbare Tools

Der Workfront MCP-Server stellt eine Reihe von Tools bereit, die die KI-Agentenplattform in Ihrem Namen aufruft, z. B. Tools zum Durchsuchen von Workfront, Erstellen von Elementen, Aktualisieren von Feldern und Verwalten von Genehmigungen. Die vollständige Referenzliste, gruppiert nach Workfront-Bereich, finden Sie unter [Adobe Workfront MCP Server Tools](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

>[!IMPORTANT]
>
>Wenn Sie eine KI-Agentenplattform mit Workfront verbinden, wird sie in Workfront mithilfe Ihres Workfront-Kontos und Ihrer Berechtigungen ausgeführt. Die Aktionen der Plattform haben dieselbe Wirkung wie Aktionen, die Sie direkt in der Workfront-Benutzeroberfläche ausführen.
>
>Sie und Ihr KI-Agent-Plattformanbieter sind für die Aktionen verantwortlich, die die Plattform in Workfront durchführt. Adobe übernimmt keine Verantwortung für Änderungen, die die KI-Agentenplattform an Ihren Workfront-Daten vornimmt.
>
>Bevor Sie die KI-Agent-Plattform mit einer Anfrage fortfahren lassen, bestätigen Sie, dass Sie verstehen, was sie zu tun beabsichtigt, insbesondere für Aktionen, die Daten ändern oder löschen.


## Beispiele für Fragen

Geben Sie nach der Herstellung der Verbindung Anfragen in natürlicher Sprache in Ihre KI-Agentenplattform ein. Die KI-Agentplattform entscheidet, welche Workfront-Aktionen aufgerufen werden sollen, und gibt die Ergebnisse zurück.

### Suchen und Anzeigen Ihrer Arbeit

Um in Workfront nach Elementen zu suchen, die dem Gesuchten entsprechen, fragen Sie:

* *Zeigen Sie mir alle aktiven Projekte für das Marken-Marketing-Team.*
* *Erhalte alle Aufgaben, die Joan Harris zugewiesen sind.*
* *Alle Ausgaben im Projekt „Website-Neugestaltung“ in der Kategorie „Technisch“ anzeigen.*

### Neue Elemente erstellen

Um Projekte, Aufgaben oder andere Workfront-Elemente zu erstellen, fragen Sie:

* *Erstellen Sie ein leeres Projekt mit dem Namen „Q2 Innovation Sandbox“, das am 10. März beginnt und am 30. April endet. Legen Sie mich als Besitzer fest.*
* *Fügen Sie eine neue Aufgabe mit dem Namen „Landingpage-QA“ zum Projekt hinzu und planen Sie sie vom 22. April bis zum 26. April.*
* *Erstellen Sie einen neuen Kampagnendatensatz mit dem Namen „Summer Sale 2026“*

### Vorhandene Elemente aktualisieren

Um Änderungen an Elementen vorzunehmen, die sich bereits in Workfront befinden, fragen Sie:

* *Aktualisieren Sie die Aufgabe „Design Review“ so, dass sie am 18. April abgeschlossen ist, und weisen Sie sie dem Kreativ-Team zu.*
* *Für das Projekt „Lucent AI Launch - NA“ schieben Sie die Ziellinie bis Mitte April und erhöhen Sie das Budget auf 150.000 Dollar.*
* *Aktualisieren Sie das Budgetfeld im Datensatz „Sommerkampagne“ auf 75.000 US-Dollar.*

### Elemente löschen

Um Workfront-Elemente zu entfernen, fragen Sie:

* *Löschen Sie das Projekt „Q1 Test Campaign“.*
* *Entfernen Sie die Aufgabe „Asset-Produktion drucken“ aus dem Projekt.*
* *Löschen Sie den Kampagnendatensatz mit dem Namen „Alte Promotion“*

>[!WARNING]
>
>Das Löschen von Elementen in Workfront über eine KI-Agentenplattform entspricht dem Löschen in der Workfront-Benutzeroberfläche. Bestätigen Sie, was die KI-Agent-Plattform löschen soll, bevor Sie sie fortfahren lassen.

### Arbeiten mit Genehmigungen

Um Dokument- und Asset-Genehmigungen zu verwalten, fragen Sie:

* *Fügen Sie Sarah Chen und Miguel Alvarez als genehmigende Personen für das aktuelle Dokument hinzu.*
* *Erinnerung an genehmigende Personen, die nicht geantwortet haben, bezüglich des Assets „Frühlingskampagnenvideo“ senden.*
* *Wenden Sie die Genehmigungsvorlage „Marketing-Launch“ auf das Asset „Frühling-Kampagnenvideo“ an*


### Arbeiten mit Planungsdatensätzen

Um Planungsdatensätze zu verwalten, fragen Sie:

* *Erstellen Sie einen neuen Planungsdatensatz mit dem Namen „Q2-Marketing-Plan“ für das Brand Marketing-Team.*
* *Fügen Sie eine neue Aufgabe namens „Social Media Audit“ zum Planungsdatensatz hinzu.*
* *Aktualisieren Sie die Aufgabe „Social Media Audit“, sodass sie am 18. April abgeschlossen ist, und weisen Sie sie dem Kreativ-Team zu.*

### Arbeiten mit Workflows

Um den Workflow zu verwalten, fragen Sie:

* *Verlegen Sie das Projekt „Q2 Innovation Sandbox“ an das Innovation Review Board.*
* *Aktualisieren des Datensatzes „Sommerkampagne“ auf den Status „Startbereit“.*
* *Genehmigen Sie den Datensatz „Sommerkampagne“.*


### Anforderungen in einer Konversation verketten

Sie können Anfragen in einer einzigen Konversation verketten. Die KI-Agent-Plattform behält den Kontext bei, sodass jede Anfrage auf der vorherigen aufbauen kann. Beispiel:

1. Nach einer Reihe von Elementen fragen: *Finde meine überfälligen Aufgaben.*
1. Nachdem Sie die Liste erhalten haben, bitten Sie um eine Aktion für die Ergebnisse: *Aktualisieren Sie alle bis zum nächsten Freitag.*

<!-- NEEDS DETAIL: Test multi-step prompt chaining in a working setup and document the patterns that produce reliable results. -->

## Zu beachten

Beachten Sie bei der Verwendung des Workfront MCP-Servers die folgenden Punkte.

### Die KI-Agent-Plattform kann Informationen aus früheren Gesprächen verwenden

KI-Agentenplattformen verwenden manchmal Daten aus früheren Konversationen, anstatt Workfront nach den neuesten zu fragen. Wenn sich in Workfront seit der letzten Ansicht der KI-Agentenplattform etwas geändert hat, werden möglicherweise veraltete Informationen angezeigt.

Um die KI-Agent-Plattform zu zwingen, neue Daten abzurufen, fragen Sie explizit danach. Beispiel:

* *Erhalten Sie die neuesten Daten aus Workfront. Keine zwischengespeicherten Ergebnisse verwenden.*

### Der Workfront MCP-Server wird automatisch aktualisiert

Wenn Adobe eine neue Version des Workfront MCP-Servers veröffentlicht, verwendet Ihre KI-Agentenplattform die neue Version automatisch. Sie müssen nichts auf Ihrer Seite neu verbinden oder ändern.

## Daten und Sicherheit

<!-- NEEDS DETAIL: Document Adobe's official position on data handling and security when Workfront data is passed through an AI agentic platform. Cover: what data leaves Workfront, where it goes, whether it is retained or used for training by the AI agentic platform provider, what happens to it after the conversation ends, and any differences between AI agentic platforms (for example, Anthropic's enterprise data handling policies for Claude). This section needs sign-off from security and legal before publication. -->

### Welche Daten Workfront verlassen

<!-- NEEDS DETAIL: List the categories of Workfront data that can be sent to the AI agentic platform (item names, field values, attachments, user identifiers, etc.) and any data that the MCP server explicitly does not expose. -->

### Handhabung von Workfront-Daten durch KI-Plattformanbieter

<!-- NEEDS DETAIL: For each supported AI agentic platform, summarize the provider's data handling stance: retention, training opt-out, and enterprise vs. consumer differences. Link to the provider's official documentation. Start with Claude (Anthropic). -->

### Unterschiede zwischen KI-magnetischen Plattformen

<!-- NEEDS DETAIL: Note any meaningful differences in how each supported AI agentic platform handles Workfront data once additional AI agentic platforms are supported. -->

## Fehlerbehebung bei der täglichen Verwendung

+++ Erweitern Sie , um Tipps zur Fehlerbehebung bei der täglichen Verwendung des Workfront MCP-Servers zu erhalten.

| Problem | Wahrscheinliche Ursache | Korrigieren |
|---|---|---|
| Die KI-Agent-Plattform liefert Ihnen veraltete Informationen. | Die KI-Agentenplattform verwendet Daten aus früheren Phasen der Konversation wieder. | Fordern Sie neue Daten von Workfront an. |
| Die KI-Agent-Plattform hat Daten von falschen Workfront-Elementen zurückgegeben. | Die KI-Agentenplattform wählte die falschen Elemente basierend auf mehrdeutigen Formulierungen aus. | Fragen Sie erneut mit spezifischeren Namen, IDs oder Filtern. |
| Eine Aktualisierung oder Löschung wurde in Workfront nicht wirksam. | Die KI-Agent-Plattform hat die Aktion noch nicht aufgerufen, oder Ihre Berechtigungen lassen dies nicht zu. | Bestätigen Sie mit der KI-Agentplattform, dass die Aktion ausgeführt wurde, und überprüfen Sie dann Ihre Workfront-Berechtigungen. |

Weitere Informationen zu Setup- und Authentifizierungsproblemen finden Sie unter [Fehlerbehebung bei Setup und Authentifizierung](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication) in [Konfigurieren des Adobe Workfront MCP-Servers](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

+++

## Häufig gestellte Fragen

+++ Erweitern Sie , um häufig gestellte Fragen zur Verwendung des Workfront MCP-Servers anzuzeigen.

### Mit welchen Workfront-Elementen kann ich über eine KI-Agentenplattform arbeiten?

Alle Elemente, auf die Sie in Workfront über Zugriffsebenen und Objektberechtigungen Zugriff haben.

<!-- NEEDS DETAIL: List the supported Workfront object types. -->

### Werden meine Workfront-Daten an den Anbieter der KI-Agentenplattform gesendet oder von diesem gespeichert?

Weitere Informationen finden Sie unter [ und Sicherheit ](#data-and-security) diesem Artikel.

### Was passiert, wenn eine neue Version des Workfront MCP-Servers veröffentlicht wird?

Der MCP-Server wird automatisch aktualisiert. Sie müssen keine Verbindung wiederherstellen oder etwas ändern.

### Muss ich die Workfront-API kennen, um den Workfront MCP-Server zu verwenden?

Nein. Die KI-Agentenplattform übersetzt Ihre Anfragen in natürlicher Sprache in die richtigen Workfront-Aktionen. Wenn Sie bereits mit der Workfront-API vertraut sind, fühlen sich die Aktionen vertraut an, sind aber keine Voraussetzung.

+++
