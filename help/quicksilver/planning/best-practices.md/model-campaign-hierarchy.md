---
title: 'Die Architektur des Erfolgs: Modellieren der Kampagnenhierarchie'
description: Erfahren Sie, wie Sie Ihre komplexen Geschäftsprozesse mithilfe von „Schwerpunkten“ und einer Architektur mit mehreren Arbeitsbereichen in eine skalierbare, gesteuerte Kampagnenhierarchie übersetzen können.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 0%

---


# Die Architektur des Erfolgs: Modellieren der Kampagnenhierarchie

<!--see the file again for additional comments from Seth and others-->

## Ziel

Erfahren Sie, wie Sie Ihre komplexen Geschäftsprozesse mithilfe von „Schwerpunkten“ und einer Architektur mit mehreren Arbeitsbereichen in eine skalierbare, gesteuerte Kampagnenhierarchie übersetzen können.



## Übersicht

Mit der Skalierung Ihrer Marketing-Vorgänge steigt auch die Komplexität Ihrer Daten. Ohne einen klaren Entwurf kann Ihr Marketing-Aufzeichnungssystem (MSOR) schnell zu einer „Junk-Schublade“ mit getrennten Datensätzen, widersprüchlicher Terminologie und Reporting-Silos werden.



Der „Blueprint of Success“ ist ein Framework zur Modellierung Ihrer Kampagnenhierarchie in Workfront Planning. Sie versetzt Sie vom „Tabellenchaos“ in ein geregeltes, objektorientiertes Modell, das sicherstellt, dass jedes Team dieselbe Sprache spricht und gleichzeitig die Agilität beibehält, die es ausführen muss.



## Die Hierarchie: Ermitteln der Absichtsebenen

Um Klarheit und Skalierbarkeit zu gewährleisten, empfehlen wir, mit einem bewährten **Core Path** zu beginnen. Unternehmen können diese Hierarchie im Zuge der Weiterentwicklung ihrer betrieblichen Anforderungen zwar erweitern, aber mit diesen drei Ebenen zu beginnen, stellt eine starke Brücke zwischen Strategie und Ausführung sicher.



### Der zentrale Weg: Strategie zum Handeln

Die meisten erfolgreichen Implementierungen basieren auf einem sauberen, dreistufigen Modell, das sowohl Planungs- als auch Workflow-Aspekte umfasst:



1. **Ebene 1: Kampagnen (Planungsmodul)**

   * **Schwerpunkt:** Langfristige strategische Säulen und jährliche Initiativen (z. B. „FY26 Global Brand Awareness„).

   * **Persona:** CMO, VP of Marketing, Strategic Leads.

2. **Level 2: Channel-Taktiken (Planungsmodul)**

   * **Fokus:** Die operativen Briefs, die das „Was“ für bestimmte Kanäle definieren (z. B. „Q1 Social Media Blitz„). Dies ist die letzte Ebene der strategischen Absicht, bevor die Arbeit beginnt.

   * **Persona:** Marketing-Opportunities, Kanal-Leads, Kampagnen-Manager.

3. **Ebene 3: Workflow-Projekte (Workflow-Modul)**

   * **Fokus:** Die tatsächliche Ausführung von „Erlebnissen“ oder „Aktivitäten“ (z. B. bestimmte Social-Media-Posts, E-Mails, Web-Seiten).

   * **Implementierung:** Planungstaktiken sind direkt mit **Projekten** im Workflow-Modul verknüpft, in dem einzelne Ergebnisse als Aufgaben und Probleme verwaltet werden.

   * **Persona:** Kreative, einzelne Mitwirkende.



### Strategische Erweiterung: Mehr Ebenen hinzufügen

Sobald der Kernpfad festgelegt ist, können Unternehmen nach sorgfältiger Abwägung ihrer spezifischen Geschäftskomplexität weitere Ebenen hinzufügen:



* **Kanalpläne:** eine Ebene zwischen *Kampagnen* und *Taktiken*, um funktionsübergreifende Strategien zu gruppieren (z. B. „Digitale Strategie„).

* **Workfront-Planungsaktivitäten:** In Umgebungen mit niedrigerem Volumen (in der Regel &lt; 5.000 Leistungen/Jahr) verfolgen einige Teams lieber einzelne „Erlebnisse“ als Workfront-Planungsdatensätze, bevor sie zu Projekten werden.


>[!TIP]
>
>**Wichtiger Tipp: Die 5.000-Schwelle für Ergebnisse**
>
>Wenn Ihr Unternehmen mehr als 5.000 Aktivitäten pro Jahr produziert, sollten Sie **immer** individuelles Tracking der Ergebnisse auf das **Workflow-Modul** auslagern. Die Verwaltung umfangreicher „Erlebnis“-Datensätze in Planning kann zu einer Datenakkumulation führen, die Ihre strategische Sichtbarkeit verdunkelt. Verwenden Sie Planning für das „Warum“ und „Was“ und das Workflow-Modul für das volumenreiche „Wie“.



## Architektur: Schwerpunkte

Ein MSOR der Unternehmensklasse wird nicht in einem einzigen Arbeitsbereich erstellt. Es verwendet eine „Hub-and-Spoke“-Architektur, bei der Datensatztypen in ihren natürlichen **Schwerpunkten“ verwaltet**.



### &#x200B;1. Der Taxonomie-Hub (Klassifizierungen)

Erstellen Sie einen zentralen Arbeitsbereich für Ihre „globalen Klassifizierungen“ (z. B. Marken, Regionen, Produkte, Rollen).

* **Primärer Speicherort:** Dieser Arbeitsbereich ist das &quot;Source der Wahrheit“ für diese Objekte.

* **Der Vorteil:** Durch die Syndizierung dieser Definitionen für den Rest des Unternehmens lösen Sie die „semantische Drift“ - und stellen sicher, dass „Region: EMEA“ für jedes Team dasselbe bedeutet.



### &#x200B;2. Strategische Planung Workspace (Exekutivzentrum)

Dies ist der Ort, an dem **(Kampagnen** (und alle **Kanalpläne**) leben.

* **Primärer Standort:** Dies ist der exekutive Schwerpunkt und bietet eine geräuschfreie Umgebung für strategische Entscheidungen.

* **Der Vorteil:** Führung kann das Portfolio verwalten, ohne das tagtägliche taktische Chaos zu sehen.



### &#x200B;3. Funktions-Spokes (Team-Arbeitsbereiche)

Funktionseinheiten (Social, Creative, E-Mail) verfügen über eigene Arbeitsbereiche zur Verwaltung ihrer **Taktiken**.

* **Primärer Standort:** Diese Arbeitsbereiche bilden den Schwerpunkt für die Ausführung lokaler Teams.

* **Der Vorteil:** Teams „konsumieren“ die globalen Kampagnen und Klassifizierungen über die Hubs, während sie ihre eigenen lokalen Objekte (wie *Media Outlets* oder *Verwendungsrechte*) beibehalten.



## Substantivbasierte Governance: Eine Sprache sprechen

Um sicherzustellen, dass Ihr Blueprint unter Druck steht, folgen Sie dem Prinzip **Substantivbasierte Governance**.



* **Substantive, keine Verben verwenden:** Benennen Sie Ihre Datensatztypen nach den „Dingen“, die Sie nachverfolgen (`Campaign`, `Tactic`), nicht nach den „Aktionen“ (`Campaigning`, `Planning`).

* **Nomenklatur standardisieren** Verwenden Sie dieselben Namen für alle Arbeitsbereiche. Auf diese Weise können Sie Daten für das Executive Reporting über das gesamte Portfolio hinweg aggregieren.



## Was ist mit bestehenden Portfolios und Programmen?

Eine häufige Frage für etablierte Organisationen ist, wie die Portfolios und Programme gehandhabt werden sollen, die sie bereits im **Workflow-Modul** erstellt haben. In der Vergangenheit wurden diese Objekte oft verwendet, um strategische Planung nachzuahmen.



### &#x200B;1. Portfolios und Programme → Datensatztypen

In vielen Organisationen **Portfolios** zur Darstellung von Marken oder Geschäftseinheiten (BUs) auf hoher Ebene verwendet, während **Programme** strategische Themen darstellen.

* **Die Änderung** Diese werden am besten als **Datensatztypen** in Ihrem **Taxonomie-Hub** modelliert. Indem Sie „Marke“ oder „Geschäftseinheit“ als Datensatztyp behandeln, können Sie sie mit einer beliebigen Kampagne oder Taktik im gesamten Unternehmen verknüpfen und so eine viel flexiblere Berichterstellung ermöglichen als eine statische Portfolio-/Programmstruktur.



### &#x200B;2. Die „Reporting-Bridge&quot;-Strategie

Workfront Planning ist zwar die Zukunft der strategischen Absicht, doch die native Berichterstellung über **Canvas-Dashboards** ist noch nicht ausgereift. Viele Unternehmen sind noch immer auf die robusten Berichtsfunktionen angewiesen, die mit ihren veralteten Portfolio- und Programmstrukturen im Workflow-Modul verknüpft sind.

* **Die Empfehlung** Löschen Sie Ihre Portfolios und Programme noch nicht. Verwenden Sie stattdessen **Fusion-Automatisierungen**, um eine Brücke zu erstellen.

* **Funktionsweise:** Wenn in Workfront Planning eine Taktik oder Kampagne erstellt wird, kann Fusion diesen Datensatz automatisch in eine entsprechende Portfolio oder ein entsprechendes Programm im Workflow-Modul spiegeln. Auf diese Weise können Sie:

   1. Nutzen Sie die überlegene **strategische Visualisierung“ (**/Kalender) von Workfront Planning.

   2. Pflegen Sie Ihre **veralteten Berichte** im Workflow-Modul für Stakeholder, die noch nicht bereit sind, zur Arbeitsfläche zu wechseln.

## Best Practices und Tipps

### Führen Sie Folgendes aus:

* **Halten Sie sich zuerst an den Kernpfad.** Richten Sie Ihren Workflow von Campaign zu Taktik zu Projekt ein, bevor Sie mehr Komplexität hinzufügen.

* **Bestimmen Primärer Arbeitsbereiche.** Stellen Sie sicher, dass jeder Datensatztyp über einen „Home“-Arbeitsbereich (den Schwerpunkt) verfügt, der als Aggregator für das Reporting dient.

* **Priorisieren von Forms für die Aufnahme.** Verwenden Sie Datensatzformulare für Gruppen mit weniger Komplexität in der Workfront-Planung, um die Integrität der Metadaten sicherzustellen. Während Power-User von der direkten Dateneingabe in Tabellenansichten profitieren können, sollte dies mit Vorsicht angegangen werden. Massenänderungen in einer Tabelle können leicht zu Datenproblemen für andere Stakeholder führen.


### Nicht:

* **Sag nicht „Core“.** beziehen sich speziell auf das **Workflow-Modul** und die **Projekt**-Objekte, wenn von der Ausführung gesprochen wird.

* **Komplizieren Sie es nicht übermäßig.** Jede zusätzliche Hierarchieebene fügt eine „Managementsteuer“ hinzu. Fügen Sie nur Ebenen hinzu, die eine geschäftliche Frage beantworten, die Sie derzeit nicht beantworten können.

* **Erstellen Sie keine Silos.** Stellen Sie sicher, dass Ihre Datensatztypen in allen Arbeitsbereichen gemeinsam verwendet werden, sodass Teams dieselben Daten nicht erneut eingeben.




