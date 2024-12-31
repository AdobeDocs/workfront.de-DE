---
content-type: overview
product-area: documents
navigation-topic: proofing-overview
title: Übersicht über die automatisierten Workflow-Phasen
description: Die Korrekturabzugsschritte sind Zeitabschnitte, in denen verschiedene Benutzende einen Korrekturabzug überprüfen. Wenn der Korrekturabzug von einem Schritt zum nächsten wechselt, werden die validierungsverantwortlichen Personen von Adobe Workfront benachrichtigt, wenn es Zeit ist, ihn zu bearbeiten.
author: Courtney
feature: Digital Content and Documents
exl-id: a03d2cf2-edb3-43b7-a739-32600f2ae2a0
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 0%

---

# Übersicht über die automatisierten Workflow-Phasen

Die Korrekturabzugsschritte sind Zeitabschnitte, in denen verschiedene Benutzende einen Korrekturabzug überprüfen. Wenn der Korrekturabzug von einem Schritt zum nächsten wechselt, werden die validierungsverantwortlichen Personen von Adobe Workfront benachrichtigt, wenn es Zeit ist, ihn zu bearbeiten.

![stages_diagram.png](assets/stages-diagram-350x63.png)

Stadien treten in zwei verschiedenen Situationen auf:

* [Erstellen eines Korrekturabzugs mit einem automatisierten Workflow](#create-a-proof-with-an-automated-workflow)
* [Zuweisen von Fristen für verschiedene Prüfer zu einem Korrekturabzug](#assign-deadlines-for-different-reviewers-on-a-proof)

## Erstellen eines Korrekturabzugs mit einem automatisierten Workflow {#create-a-proof-with-an-automated-workflow}

Wenn Sie einem Korrekturabzug einen automatisierten Workflow hinzufügen, richten Sie die Phasen der Prüfungsarbeit ein, die ausgeführt werden sollen.

Beim Einrichten von Phasen für einen Korrekturabzug mit einem automatischen Workflow:

* Sie können die Phasen so konfigurieren, dass sie nacheinander oder gleichzeitig ausgeführt werden.
* Sie können einige Phasen so konfigurieren, dass sie erst aktiv werden, nachdem eine vorherige Phase abgeschlossen ist.
* Man kann einige Stadien privat machen. Dies ist beispielsweise für eine Agentur nützlich, die einen Korrekturabzug prüft, bevor er für einen Kunden freigegeben wird, und nicht möchte, dass die resultierenden Kommentare für den Kunden sichtbar sind.

Anweisungen zum Erstellen von Phasen für einen Korrekturabzug mit einem automatisierten Workflow finden Sie unter [Erstellen eines erweiterten Korrekturabzugs mit einem automatisierten Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

>[!NOTE]
>
>Wenn ein(e) Benutzende(r) nicht in einem Schritt enthalten ist, aber Zugriff auf das Dokument hat und den Korrekturabzug öffnet, erstellt das System einen Schritt namens *Workfront*.
>
>Dem Benutzer, der den Korrekturabzug geöffnet hat, wird die Rolle zugewiesen, die in Setup > Überprüfung und Genehmigung > Rollen für Nicht-Empfänger angegeben ist, die einen Korrekturabzug für ein Dokument öffnen.

## Zuweisen von Fristen für verschiedene Prüfer zu einem Korrekturabzug {#assign-deadlines-for-different-reviewers-on-a-proof}

Wenn Sie den Validierungsverantwortlichen für einen Korrekturabzug unterschiedliche Korrekturabzugsfristen zuweisen, erstellt das System für jeden Termin einen Schritt und gruppiert die Validierungsverantwortlichen für jeden Termin im entsprechenden Schritt. 

**Beispiel** Wenn Sie beispielsweise einen Korrekturabzug mit vier Prüfern erstellen:

* Für die Prüfer Olivia und Tony gibt man in einigen Tagen eine Frist von 14:00 Uhr an.
* Für Aaron und Amy gibt man eine Frist bis 17:00 Uhr ein paar Tage später an.
* Für sich selbst gibt es keine Frist.

Das System erstellt einen Schritt für jede dieser drei „Gruppen“ von Validierungsverantwortlichen:

![stage.png](assets/stages-350x239.png)

Wenn Sie den Korrekturabzug für andere Prüfende freigeben und keine Frist angeben, fügt Workfront die Benutzenden zu Schritt 3 hinzu, für den keine Frist festgelegt ist. 
