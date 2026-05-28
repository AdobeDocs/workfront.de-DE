---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Verwenden des Adobe Workfront MCP-Servers
description: Verwenden Sie den Adobe Workfront-MCP-Server, um Workfront-Elemente über eine Sprachkonversation in einer KI-Agentenplattform zu suchen, zu erstellen, zu aktualisieren und zu verwalten.
author: Courtney
feature: Get Started with Workfront
source-git-commit: f96afd17e9f4e726ac545a9cb0c54ace5a4fcffe
workflow-type: tm+mt
source-wordcount: '1642'
ht-degree: 0%

---


# Verwenden des Adobe Workfront MCP-Servers

{{highlighted-preview-article-level}}

Mit dem [!DNL Adobe Workfront] MCP-Server können Sie Workfront-Elemente suchen, erstellen, aktualisieren und verwalten, indem Sie eine KI-Agentenplattform in natürlicher Sprache anfordern. Die -Plattform entscheidet, welche Workfront-Aktionen aufgerufen werden sollen, und übernimmt die Unterhaltung mit Workfront für Sie.

>[!IMPORTANT]
>
>Derzeit steht der Workfront MCP-Server nur Kunden in den USA zur Verfügung, die AWS verwenden.

## Voraussetzungen

In diesem Artikel wird davon ausgegangen, dass Sie die Verbindung bereits eingerichtet haben. Weitere Informationen zum Setup finden Sie unter [Konfigurieren des Adobe Workfront MCP-Servers](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

## Verfügbare Tools

Der Workfront MCP-Server stellt eine Reihe von Tools bereit, die die KI-Agentenplattform in Ihrem Namen aufruft. Beispielsweise Tools zum Durchsuchen von Workfront, Erstellen von Elementen, Aktualisieren von Feldern und Verwalten von Genehmigungen. Die vollständige Referenzliste finden Sie unter [Adobe Workfront MCP-Server-Tools](/help/quicksilver/workfront-basics/workfront-mcp-server/workfront-mcp-server-tools.md).

>[!IMPORTANT]
>
>Wenn Sie eine KI-Agentenplattform mit Workfront verbinden, wird sie in Workfront mithilfe Ihres Workfront-Kontos und Ihrer Berechtigungen ausgeführt. Die Aktionen der Plattform haben dieselbe Wirkung wie Aktionen, die Sie direkt in der Workfront-Benutzeroberfläche ausführen.<br>
>
>Sie und Ihr KI-Agent-Plattformanbieter sind für die Aktionen verantwortlich, die die Plattform in Workfront durchführt. Adobe übernimmt keine Verantwortung für Änderungen, die die KI-Agentenplattform an Ihren Workfront-Daten vornimmt.<br>
>
>Bevor Sie die KI-Agent-Plattform mit einer Anfrage fortfahren lassen, bestätigen Sie, dass Sie verstehen, was sie zu tun beabsichtigt, insbesondere für Aktionen, die Daten ändern oder löschen.


## Beispiele für Fragen

Geben Sie nach der Herstellung der Verbindung Anfragen in natürlicher Sprache in Ihre KI-Agentenplattform ein. Die KI-Agentplattform entscheidet, welche Workfront-Aktionen aufgerufen werden sollen, und gibt die Ergebnisse zurück.

>[!NOTE]
>
>Einige Aktionen sind möglicherweise aufgrund von Admin-Steuerelementen im Bereich &quot;Workfront-Setup“ nicht verfügbar. Sie können beispielsweise keine Elemente erstellen, wenn der Workfront-Administrator Schreibaktionen für den MCP-Server deaktiviert hat.


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


## Zu beachten

Beachten Sie bei der Verwendung des Workfront MCP-Servers die folgenden Punkte:

### Die KI-Agent-Plattform kann Informationen aus früheren Gesprächen verwenden

KI-Agentenplattformen verwenden manchmal Daten aus früheren Konversationen, anstatt Workfront nach den neuesten zu fragen. Wenn sich in Workfront seit der letzten Ansicht der KI-Agentenplattform etwas geändert hat, werden möglicherweise veraltete Informationen angezeigt.

Um die KI-Agent-Plattform zu zwingen, neue Daten abzurufen, fragen Sie explizit danach. Beispiel:

* *Erhalten Sie die neuesten Daten aus Workfront. Keine zwischengespeicherten Ergebnisse verwenden.*

### Auf Updates für den Workfront MCP-Server prüfen

Sie sollten Ihre Verbindung zum Workfront MCP-Server regelmäßig aktualisieren, um sicherzustellen, dass Sie über die neuesten Tools und Funktionen verfügen.

Die meisten Aktualisierungen sollten automatisch erfolgen. Es wird jedoch empfohlen, die Versionshinweise zu Workfront regelmäßig zu lesen.


## Daten und Sicherheit

Die Workfront MCP-Server-Tools sind konsistent mit der Funktionsweise von API-Aufrufen. Workfront speichert keine Eingabeaufforderungen, Antworten oder andere Daten. Die gewünschten Workfront-Daten sind über die Workfront-Plattform verfügbar.

Ihre Zugriffsebene und Ihre Objektberechtigungen bestimmen, wonach Sie Abfragen durchführen oder in Workfront schreiben können. Ihr Workfront-Administrator hat die Kontrolle über die MCP-Lese- und Schreibaktionen im Bereich &quot;Workfront Setup“.

### Welche Daten Workfront verlassen

Der Anbieter der KI-Agentenplattform hat Zugriff auf die Workfront-Daten, mit denen Sie über den Workfront MCP-Server interagieren. Weitere Informationen erhalten Sie von Ihrem KI-Agenten-Plattformanbieter.


### Handhabung von Workfront-Daten durch KI-Plattformanbieter

Workfront hat keine Kontrolle darüber, wie der KI-Plattformanbieter Ihre Workfront-Daten verarbeitet. Weitere Informationen erhalten Sie von Ihrem KI-Agenten-Plattformanbieter.

## Fehlerbehebung bei der täglichen Verwendung

+++ Erweitern Sie , um Tipps zur Fehlerbehebung bei der täglichen Verwendung des Workfront MCP-Servers zu erhalten.

| Problem | Wahrscheinliche Ursache | Korrigieren |
|---|---|---|
| Die KI-Agent-Plattform liefert Ihnen veraltete Informationen. | Die KI-Agentenplattform verwendet Daten aus früheren Phasen der Konversation wieder. | Fordern Sie neue Daten von Workfront an. |
| Die KI-Agent-Plattform hat Daten von falschen Workfront-Elementen zurückgegeben. | Die KI-Agentenplattform wählte die falschen Elemente basierend auf mehrdeutigen Formulierungen aus. | Fragen Sie erneut mit spezifischeren Namen, IDs oder Filtern. |
| Eine Aktualisierung oder Löschung wurde in Workfront nicht wirksam. | Ihr Workfront-Administrator hat Schreibaktionen für den Workfront MCP-Server deaktiviert oder Sie sind nicht berechtigt, die Aktion für das jeweilige Element durchzuführen. | Bestätigen Sie mit der KI-Agent-Plattform, dass die Aktion ausgeführt wurde. Vergewissern Sie sich anschließend, dass Schreibaktionen für den Workfront MCP-Server aktiviert sind und dass Sie berechtigt sind, das Element zu ändern. |

Weitere Informationen zu Setup- und Authentifizierungsproblemen finden Sie unter [Fehlerbehebung bei Setup und Authentifizierung](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md#troubleshoot-setup-and-authentication) in [Konfigurieren des Adobe Workfront MCP-Servers](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

+++

## Häufig gestellte Fragen

+++ Erweitern Sie , um häufig gestellte Fragen zur Verwendung des Workfront MCP-Servers anzuzeigen.

### Was ist eine KI-Agentenplattform?

Eine KI-Agent-Plattform ist ein KI-Tool, mit dem Sie in Ihrem Namen Aktionen durchführen können.
Andere Systeme beantworten nicht nur Fragen. Wenn Sie eine Verbindung zu Workfront herstellen
über den MCP-Server kann es Workfront finden, erstellen, aktualisieren und löschen
Elemente basierend auf dem, was Sie es in natürlicher Sprache fragen. Beispiele sind Claude
Desktop, ChatGPT und andere MCP-kompatible KI-Clients.


### Muss ich Workfront-Administrator sein, um den Workfront MCP-Server zu verwenden?

Nein. Jeder Workfront-Benutzer kann den Workfront MCP-Server über eine verbundene
KI-Agent-Plattform. Die KI-Agentenplattform verwendet Ihre Workfront
Konto-, Zugriffsebenen- und Objektberechtigungen, sodass Sie nur das tun können, was Sie auch tun
Konnte bereits direkt in Workfront.

### Warum kann die KI-Agent-Plattform keine Elemente für mich erstellen, aktualisieren oder löschen?

Ihr Workfront-Administrator steuert, welche MCP-Aktionen in der
Workfront-Setup-Bereich. Wenn Schreibaktionen deaktiviert sind, nutzt die KI-Agent-Plattform
Workfront-Elemente können weiterhin gefunden und gelesen, aber keine Änderungen vorgenommen werden. Sie auch
Sie benötigen die richtige Zugriffsebene und Objektberechtigungen für die spezifischen Elemente
Du arbeitest mit.

### Fragt mich die KI-Agentenplattform, bevor sie Workfront-Daten ändert oder löscht?

Das hängt von der KI-Agentenplattform ab, nicht von Workfront. Die meisten Plattformen
Sie vor der Ausführung einer Aktion zur Bestätigung auffordern, insbesondere bei Löschvorgängen.
Bevor Sie eine Anfrage genehmigen, lesen Sie, was die Plattform sagt, dass sie tun wird —
Die Änderungen erfolgen in Workfront auf die gleiche Weise wie bei einer Vornahme
sich selbst in der Benutzeroberfläche.

<!--

### Can I undo something the AI agentic platform did in Workfront?

Changes the AI agentic platform makes in Workfront work the same way as 
changes you make in the interface. If Workfront supports undoing or 
restoring a particular action (for example, restoring a deleted item from 
the Recycle Bin), the same options apply. If Workfront doesn't normally let 
you undo an action, you can't undo it through the AI agentic platform either.

-->

### Warum hat die KI-Agent-Plattform die falschen Workfront-Elemente zurückgegeben?

Die KI-Agent-Plattform wählt Elemente basierend auf den von Ihnen verwendeten Wörtern aus. Wenn Ihre
Die Anfrage ist mehrdeutig - z. B. haben zwei Projekte ähnliche Namen - sie
Sie könnten sich die falsche aussuchen. Fragen Sie erneut mit spezifischeren Namen, IDs, Daten,
oder Filtern, um die Ergebnisse einzugrenzen.


### Mit welchen Workfront-Elementen kann ich über eine KI-Agentenplattform arbeiten?

Alle Elemente, auf die Sie in Workfront über Ihre Zugriffsebene Zugriff haben, und
Objektberechtigungen. Dazu gehören Projekte, Aufgaben, Probleme, Dokumente,
Validierungen, Planungsunterlagen und mehr.

### Können andere Leute meine Konversationen mit der KI-Agentenplattform sehen?

Workfront speichert weder Ihre Eingabeaufforderungen noch die Antworten der KI-Agentenplattform.
Wer auch immer Ihre KI-Agentenplattform bereitstellt, steuert, wie Ihre Konversationen
werden gespeichert oder freigegeben. Fragen Sie Ihren KI-Agenten-Plattformanbieter nach
Details.

### Muss ich die Workfront-API kennen oder welches MCP-Tool ich verwenden?

Nein. Die KI-Agentenplattform übersetzt Ihre Anforderung in natürlicher Sprache in
Wählen Sie die richtigen Workfront-Aktionen und die richtigen Tools für Sie aus. Wenn Sie
Sie sind bereits mit der Workfront-API vertraut.
Aber das ist keine Voraussetzung.

### Werden meine Workfront-Daten an den Anbieter der KI-Agentenplattform gesendet oder von diesem gespeichert?

Weitere Informationen finden Sie unter [Daten und Sicherheit](#data-and-security) in diesem Abschnitt
Artikel.

### Was passiert, wenn eine neue Version des Workfront MCP-Servers veröffentlicht wird?

Der MCP-Server wird im Allgemeinen automatisch aktualisiert. Möglicherweise müssen Sie jedoch Ihre Verbindung zum MCP-Server gelegentlich aktualisieren, um die neuesten Tools und Funktionen zu sehen.

+++
