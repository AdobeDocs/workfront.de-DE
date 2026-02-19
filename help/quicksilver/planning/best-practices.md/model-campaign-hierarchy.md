---
title: 'Gestalten Sie Ihren Erfolg: Modellieren Ihrer Kampagnenhierarchie'
description: Erfahren Sie, wie Sie Ihre komplexen Geschäftsprozesse mithilfe von „Schwerpunkten“ und einer Architektur mit mehreren Arbeitsbereichen in eine skalierbare, gesteuerte Kampagnenhierarchie übersetzen können.
feature: Workfront Planning
role: Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 02e3b55f-9188-42bf-8d0b-c9fed86c63c4
source-git-commit: 7f3ca12d89a2a5fbebc12b3df8a40edbb17d0ead
workflow-type: tm+mt
source-wordcount: '1537'
ht-degree: 0%

---

# Gestalten Sie Ihren Erfolg: Modellieren Ihrer Kampagnenhierarchie

<!--see the file again for additional comments from Seth and others-->

>[!IMPORTANT]
>
>Die Informationen in diesem Artikel beziehen sich auf Adobe Workfront Planning, eine zusätzliche Funktion von Adobe Workfront.
>
>Ihr Unternehmen muss über ein Workfront Planning Prime-Paket oder ein höheres Paket verfügen, um die in diesem Artikel empfohlenen Funktionen unterstützen zu können.
>
>Eine Liste der Anforderungen für den Zugriff auf Workfront Planning finden Sie unter [Zugriffsübersicht für Adobe Workfront Planning](/help/quicksilver/planning/access/access-overview.md).
> 
>Allgemeine Informationen zu Workfront Planning finden Sie unter [Erste Schritte mit Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

Erfahren Sie, wie Sie Ihre komplexen Geschäftsprozesse mithilfe von Schwerpunkten und einer Arbeitsbereichsarchitektur in Adobe Workfront Planning in eine skalierbare, gesteuerte Kampagnenhierarchie übersetzen können.

Dieses Handbuch richtet sich an Workfront-Administratoren und -Hauptbenutzer, die die Architektur Ihrer Umgebung in Workfront Planning implementieren und entwerfen.

## Überblick über die Architektur des Erfolgs

Mit zunehmender Reife Ihrer Marketing-Vorgänge steigt auch die Komplexität Ihrer Daten. Ohne klare Blueprints kann Ihr Marketing-Aufzeichnungssystem schnell zu einer Junk-Schublade mit getrennten Datensätzen, widersprüchlicher Terminologie und Reporting-Silos werden.

Wenn Sie eine erfolgreiche Architektur erstellen, erstellen Sie ein Framework für die Modellierung Ihrer Kampagnenhierarchie in Workfront Planning. Damit gelangen Sie vom Tabellenchaos zu einem gesteuerten, objektorientierten Modell, das sicherstellt, dass jedes Team dieselbe Sprache spricht und gleichzeitig die Agilität beibehält, die es ausführen muss.

## Erstellen Sie eine Hierarchie, um Ihre Absichtsebenen zu definieren

Um Klarheit und Skalierbarkeit zu gewährleisten, empfehlen wir, beim Entwerfen Ihres Workflows in Workfront Planning mit einem bewährten Kernpfad zu beginnen.

Von dort aus können Sie Ihre Strategie erweitern, indem Sie Ihrer Architektur weitere Ebenen hinzufügen.

### Der Kernpfad: Wie man von der Strategie zur Tat kommt

Unternehmen können diese Hierarchie im Zuge der Weiterentwicklung ihrer betrieblichen Anforderungen zwar erweitern, aber mit den drei in den folgenden Abschnitten beschriebenen Ebenen zu beginnen, stellt eine starke Brücke zwischen Strategie und Ausführung sicher.

Aus unseren Ergebnissen geht hervor, dass die meisten erfolgreichen Implementierungen von Workfront Planning auf einem sauberen, dreistufigen Modell basieren, das sowohl Planning als auch Workfront umfasst.

Im Folgenden finden Sie die Ebenen einer erfolgreichen Planungsimplementierung und die Artefakte, die Sie erstellen können, um Sie bei diesem Prozess zu unterstützen:

* **Ebene 1: Kampagnen (Workfront-Planung)**

   * **Schwerpunkt:** Definieren Sie die langfristigen strategischen Säulen und jährlichen Initiativen. Definieren Sie beispielsweise eine Initiative für Ihr Unternehmen mit dem Namen „Globale Markenbekanntheit für das Geschäftsjahr 26“. Dies ist der Fokus für einen bestimmten Zeitrahmen. Erstellen Sie Kampagnen zur Unterstützung dieser Initiative.

   * **Personas:** Stakeholder für diese Ebene können Marketing-Beauftragte, VP von Marketing oder andere strategische Leads sein.

  Weitere Informationen finden Sie [Datensatztypen erstellen](/help/quicksilver/planning/architecture/create-record-types.md).

* **Ebene 2: Kanaltaktiken (Workfront-Planung)**

   * **Fokus:** Definieren Sie die operativen Briefs, die das „Was“ für bestimmte Kanäle umreißen. Dies ist die letzte Ebene der strategischen Absicht, bevor die Arbeit beginnt. Erstellen Sie beispielsweise die Taktik „Q1 Social Media Blitz“. Sie können sie dann mit Ihren Kampagnen verbinden.

   * **Personas:** Die wichtigsten Stakeholder sind Marketing-Operations-Leader, Kanal-Leader oder Kampagnen-Manager.

* **Ebene 3: Projekte (Planning und Workfront)**

   * **Fokus:** Führen Sie genau die Erlebnisse oder Aktivitäten aus, die letztendlich Ihre Initiative umsetzen werden. Einige der Ergebnisse sind spezifisch, z. B. Social-Media-Beiträge, E-Mails, Web-Seiten.

   * **Implementierung:** Sie können in Planning Taktiken erstellen und diese direkt mit **Projekten** in Workfront verknüpfen, wo einzelne Ergebnisse als Aufgaben und Probleme verwaltet werden.

   * **Persona:** Hauptakteure sind hier Kreative, einzelne Mitwirkende und alle, die für die Arbeit zur Unterstützung der Initiative verantwortlich sind.

### Strategische Erweiterung: Weitere Ebenen hinzufügen

Sobald Sie den Kernpfad festgelegt haben, können Sie nach sorgfältiger Abwägung der jeweiligen geschäftlichen Komplexität weitere Ebenen hinzufügen.

Es kann nützlich sein, die folgenden zusätzlichen Elemente zu erstellen:

* **Kanalpläne:** eine Ebene zwischen Kampagnen und Taktiken, um funktionsübergreifende Strategien zu gruppieren. Zum Beispiel ein Plan namens „Digitale Strategie“.

* **Aktivitäten:** Wenn Sie in einer Umgebung mit geringerem Volumen arbeiten (Sie haben möglicherweise 5.000 oder weniger Ergebnisse pro Jahr), ziehen einige Teams es möglicherweise vor, einzelne Erlebnisse als Workfront-Planungsdatensätze zu verfolgen, bevor sie zu Workfront-Projekten werden.

>[!IMPORTANT]
>
>Wenn Ihr Unternehmen mehr als 5.000 Aktivitäten pro Jahr produziert, sollten Sie das individuelle Tracking der zu erbringenden Leistungen nach Workfront verschieben.
>
>Die Verwaltung umfangreicher Erlebnisdatensätze in Planning kann zu einer Datenakkumulation führen, die Ihre strategische Sichtbarkeit verdunkelt.
>Wir empfehlen diese grobe Richtlinie für maximale Effizienz:
>
>* Verwenden der Planung für das „Warum“ und „Was“
>* Verwenden Sie Workfront für das umfangreiche „Wie“.

## Grundlegendes zu den Schwerpunkten beim Aufbau Ihrer Architektur

Ein Aufzeichnungssystem für das Marketing im Unternehmensmaßstab wird nicht in einem einzigen Arbeitsbereich erstellt. Es verwendet eine „Hub-and-Spoke“-Architektur, bei der Datensatztypen in ihren natürlichen Schwerpunkten verwaltet werden.

Weitere Informationen finden Sie unter [Rollout your Strategic Home: a 30-day launchpad](/help/quicksilver/planning/best-practices.md/30-day-launchpad.md).

Um Ihre Architektur mit dem Hub-and-Spoke-Ansatz zu erstellen, müssen Sie Folgendes erstellen:

* Ein Taxonomie-Hub
* Ein strategischer Planungsarbeitsbereich
* Funktionsspeichen

### Erstellen Sie den Taxonomie-Hub als Klassifizierungen

Zunächst müssen Sie einen zentralen Arbeitsbereich für Ihre globalen Klassifizierungen einrichten, um die wichtigsten Konzepte zu definieren, die jeder in Ihrem Unternehmen verstehen muss. Erstellen Sie beispielsweise die folgenden Datensatztypen in einem zentralen Arbeitsbereich: Marken, Regionen, Produkte, Rollen.

Weitere Informationen finden Sie [Datensatztypen erstellen](/help/quicksilver/planning/architecture/create-record-types.md).

Legen Sie beim Erstellen Ihrer Klassifizierungen Folgendes fest:

* **Primärer Speicherort:** Sie einen primären Arbeitsbereich aus. Dieser Arbeitsbereich sollte die Quelle der Wahrheit für die von Ihnen erstellten Datensatztypen sein.

* **Der Vorteil:** Sie diese Definitionen für den Rest des Unternehmens zusammenfassen, klären Sie, dass Konzepte wie „Region: EMEA“ für jedes Team das Gleiche bedeuten.

### Erstellen Sie den Arbeitsbereich Strategische Planung als Executive Center

Das Executive Center ist der Ort, an dem Kampagnen auf hoher Ebene (und alle Kanalpläne) live sind.

* **Primärer Standort:** Dies ist der Schwerpunkt der Geschäftsleitung und bietet eine geräuschfreie Umgebung für strategische Entscheidungen.

* **Der Vorteil:** Führung kann das Portfolio von Kampagnen verwalten, ohne dem täglichen taktischen Lärm Gehör zu schenken.

### Definieren der Funktionsbereiche als Arbeitsbereiche Ihrer Teams

Funktionale Einheiten (Social, Creative, E-Mail) verfügen über eigene Arbeitsbereiche, um ihre Taktiken zu verwalten.

* **Primärer Standort:** Diese Arbeitsbereiche sind die individuellen Schwerpunkte für die Ausführung lokaler Teams.

* **Der Vorteil:** Teams nutzen die globalen Kampagnen und Klassifizierungen von den Hubs aus und behalten dabei ihre eigenen lokalen Objekte bei.

  Beispielsweise kann das Team den Kampagnen-Datensatztyp aus dem zentralen Arbeitsbereich zum Arbeitsbereich des Teams hinzufügen, jedoch nur Kampagnen erstellen, die für den jeweiligen Arbeitsbereich relevant sind. Beispiele für Kampagnen sind „Medien-Outlets“ oder „Nutzungsrechte“.

## Verwenden eines noun-basierten Governance-Ansatzes

Um sicherzustellen, dass Ihre Architektur unter Druck steht, folgen Sie dem Prinzip der Substantivbasierten Governance.

Beim Erstellen von Entitäten in Workfront Planning empfehlen wir Folgendes:

* **Verwenden Sie Substantive, keine Verben:** Benennen Sie Ihre Datensatztypen nach den Dingen, die Sie nachverfolgen (nennen Sie sie „Kampagne“ oder „Taktik„), nicht nach den zu erledigenden Aktionen (nennen Sie sie nicht „Kampagne“ oder „Planung„).

* **Nomenklatur standardisieren** Verwenden Sie dieselben Namen für alle Arbeitsbereiche. Auf diese Weise können Sie Daten für das Executive Reporting über das gesamte Portfolio hinweg aggregieren.

## Was ist mit bestehenden Portfolios und Programmen?

Eine häufige Frage für etablierte Unternehmen ist, wie sie die Portfolios und Programme handhaben können, die sie bereits in Workfront erstellt haben. In der Vergangenheit wurden diese Objekte oft verwendet, um strategische Planung nachzuahmen.

Jetzt empfehlen wir Ihnen, diesen Ansatz auf Workfront Planning zu übertragen, was natürlich zu dem strategischen Ansatz für Planning passt.

### Portfolios und Programme durch Datensatztypen ersetzen

In vielen Unternehmen werden Portfolios zur Darstellung von Marken oder Geschäftsbereichen auf hoher Ebene verwendet, während Programme strategische Themen darstellen.

In Workfront Planning können diese am besten als Datensatztypen in Ihrem Taxonomie-Hub modelliert werden.

Indem Sie eine Marke oder einen Geschäftsbereich als Datensatztyp behandeln, können Sie sie mit einer Kampagne oder Taktik im gesamten Unternehmen verknüpfen und so eine flexiblere Berichterstellung ermöglichen als eine statische Portfolio-Programmstruktur.

### Verwenden einer Reporting-Bridge-Strategie

Workfront Planning ist zwar die Zukunft der strategischen Absicht, doch das native Reporting über das Canvas-Dashboard ist noch nicht ausgereift.

Viele Unternehmen sind noch immer auf die robusten Reporting-Funktionen angewiesen, die mit ihren veralteten Portfolio- und Programmstrukturen in Workfront verknüpft sind.

Wir empfehlen Folgendes:

* Löschen Sie Ihre Portfolios und Programme nicht.
* Verwenden Sie Planungsautomatisierungen, um eine Brücke zwischen Ihren Datensatztypen und Portfolios und Programmen zu schlagen.

  Wenn in Workfront Planning eine Taktik oder Kampagne erstellt wird, kann dieser Datensatz ein entsprechendes Portfolio oder Programm in Workfront generieren.

  Weitere Informationen finden Sie unter [Erstellen von Objekten mithilfe von Adobe Workfront Planning-Datensatzautomatisierungen](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

Auf diese Weise können Sie:

* Nutzen Sie die überlegene strategische Visualisierung von Workfront Planning mithilfe von Timelines und Kalendern.

* Pflegen Sie Ihre veralteten Berichte in Workfront für Stakeholder, die noch nicht bereit sind, zur Arbeitsfläche zu wechseln.

## Best Practices und Tipps

### DOS

* **Bleiben Sie beim Ansatz „Core Path-First“:** Richten Sie Ihren Workflow von Campaign zu einer Taktik zu einem Projekt ein, bevor Sie mehr Komplexität hinzufügen.

* **Bestimmen primärer Arbeitsbereiche:** Stellen Sie sicher, dass jeder Datensatztyp über einen Hauptarbeitsbereich verfügt (beachten Sie, dass sein Schwerpunkt liegt), der als Aggregator für das Reporting dient.

* **Priorisieren Sie Anfrageformulare für den Aufnahmeprozess:** Verwenden Sie Datensatzformulare für Gruppen mit weniger Komplexität in der Workfront-Planung, um die Integrität der Metadaten sicherzustellen.

  >[!CAUTION]
  >
  >Obwohl Power-User von der direkten Dateneingabe in Tabellenansichten profitieren können, sollte dies mit Vorsicht angegangen werden.
  >Massenänderungen in einer Tabelle können anderen Stakeholdern Datenprobleme bereiten.

### Ist das nicht

* **Verwenden Sie keine Verallgemeinerungen:** Wenn Sie beispielsweise über eine „Core“-Umgebung sprechen, verweisen Sie speziell auf Workfront und das Project-Objekt, wenn Sie über die Ausführung sprechen.

* **Komplizieren Sie das nicht** Jede zusätzliche Hierarchieebene erhöht die Verwaltungssteuer. Fügen Sie nur Ebenen hinzu, die eine geschäftliche Frage beantworten, die Sie derzeit nicht beantworten können.

* **Erstellen Sie keine Silos:** Stellen Sie sicher, dass Ihre Datensatztypen in allen Arbeitsbereichen gemeinsam genutzt werden, sodass Teams nicht dieselben Daten erneut eingeben.


<!--original content:


## Goal 

Learn how to translate your complex business processes into a scalable, governed campaign hierarchy using "Centers of Gravity" and a multi-workspace architecture. 

 

## Overview 

As your marketing operations scale, so does the complexity of your data. Without a clear blueprint, your Marketing System of Record (MSOR) can quickly become a "junk drawer" of disconnected records, conflicting terminology, and reporting silos. 

 

The "Blueprint of Success" is a framework for modeling your campaign hierarchy in Workfront Planning. It moves you from "spreadsheet chaos" to a governed, object-oriented model that ensures every team speaks the same language while maintaining the agility they need to execute. 

 

## The Hierarchy: Finding Your Levels of Intent 

To maintain clarity and scalability, we recommend starting with a proven **Core Path**. While organizations can expand this hierarchy as their operational needs evolve, beginning with these three levels ensures a strong bridge between strategy and execution. 

 

### The Core Path: Strategy to Action 

Most successful implementations thrive on a clean, three-tier model that spans both Planning and Workflow: 

 

1. **Level 1: Campaigns (Planning Module)** 

    * **Focus:** Long-term strategic pillars and annual initiatives (e.g., "FY26 Global Brand Awareness").  

    * **Persona:** CMO, VP of Marketing, Strategic Leads. 

2. **Level 2: Channel Tactics (Planning Module)** 

    * **Focus:** The operational briefs defining the "what" for specific channels (e.g., "Q1 Social Media Blitz"). This is the final layer of strategic intent before work begins. 

    * **Persona:** Marketing Ops, Channel Leads, Campaign Managers. 

3. **Level 3: Workflow Projects (Workflow Module)** 

    * **Focus:** The actual execution of "Experiences" or "Activities" (e.g., specific social posts, emails, web pages).  

    * **Implementation:** Tactics in Planning link directly to **Projects** in the Workflow module, where individual deliverables are managed as tasks and issues. 

    * **Persona:** Creatives, Individual Contributors. 

 

### Strategic Expansion: Adding More Levels 

Once the core path is established, organizations may choose to add additional layers after careful consideration of their specific business complexity: 

 

* **Channel Plans:** A layer between *Campaigns* and *Tactics* to group cross-functional strategies (e.g., "Digital Strategy"). 

* **Workfront Planning Activities:** In lower-volume environments (typically <5,000 deliverables/year), some teams prefer to track individual "Experiences" as Workfront Planning records before they become projects. 


>[!TIP]
>
>**Crucial Tip: The 5,000 Deliverable Threshold** 
>
>If your organization produces more than 5,000 activities per year, you should **always** offload individual deliverable tracking to the **Workflow module**. Managing high-volume "Experience" records in Planning can lead to data accumulation that obscures your strategic visibility. Use Planning for the "Why" and "What," and the Workflow module for the high-volume "How." 

 

## Architecture: Centers of Gravity 

An enterprise-grade MSOR isn't built in a single workspace. It uses a "Hub-and-Spoke" architecture where record types are managed in their natural **Centers of Gravity**. 

 

### 1. The Taxonomy Hub (Classifications) 

Establish one centralized workspace for your "Global Classifications" (e.g., Brands, Regions, Products, Personas). 

* **Primary Location:** This workspace is the "Source of Truth" for these objects. 

* **The Benefit:** By syndicating these definitions to the rest of the business, you solve "Semantic Drift"—ensuring that "Region: EMEA" means the same thing to every team. 

 

### 2. The Strategic Planning Workspace (Executive Center) 

This is where high-level **Campaigns** (and any **Channel Plans**) live.  

* **Primary Location:** This is the executive center of gravity, providing a noise-free environment for strategic decision-making. 

* **The Benefit:** Leadership can manage the portfolio without seeing the day-to-day tactical mess. 

 

### 3. Functional Spokes (Team Workspaces) 

Functional units (Social, Creative, Email) have their own workspaces to manage their **Tactics**. 

* **Primary Location:** These workspaces are the center of gravity for local team execution.  

* **The Benefit:** Teams "consume" the global campaigns and classifications from the hubs, while maintaining their own local objects (like *Media Outlets* or *Usage Rights*). 

 

## Noun-Based Governance: Speak One Language 

To ensure your blueprint holds up under pressure, follow the principle of **Noun-Based Governance**.  

 

* **Use Nouns, Not Verbs:** Name your record types after the "things" you are tracking (`Campaign`, `Tactic`), not the "actions" (`Campaigning`, `Planning`). 

* **Standardize Nomenclature:** Use the same names across all workspaces. This allows you to aggregate data across the entire portfolio for executive reporting. 

 

## What About Existing Portfolios and Programs? 

A common question for mature organizations is how to handle the Portfolios and Programs they've already built in the **Workflow module**. In the past, these objects were often used to mimic strategic planning. 

 

### 1. Portfolios & Programs → Record Types 

In many organizations, **Portfolios** are used to represent high-level Brands or Business Units (BUs), while **Programs** represent strategic themes. 

* **The Shift:** These are best modeled as **Record Types** in your **Taxonomy Hub**. By treating "Brand" or "Business Unit" as a record type, you can link them to any campaign or tactic across the entire enterprise, providing much more flexible reporting than a static Portfolio/Program structure. 

 

### 2. The "Reporting Bridge" Strategy 

While Workfront Planning is the future of strategic intent, its native reporting via **Canvas Dashboards** is still maturing. Many organizations still rely on the robust reporting capabilities tied to their legacy Portfolio and Program structures in the Workflow module. 

* **The Recommendation:** Don't delete your Portfolios and Programs yet. Instead, use **Fusion automations** to create a bridge.  

* **How it Works:** When a Tactic or Campaign is created in Workfront Planning, Fusion can automatically mirror that record into a corresponding Portfolio or Program in the Workflow module. This allows you to: 

    1. Enjoy Workfront Planning's superior **strategic visualization** (Timelines/Calendars). 

    2. Maintain your **legacy reporting** in the Workflow module for stakeholders who aren't yet ready to move to Canvas. 

## Best Practices & Tips 

### Do: 

* **Stick to the Core Path first.** Establish your Campaign-to-Tactic-to-Project flow before adding more complexity. 

* **Designate Primary Workspaces.** Ensure each record type has one "home" workspace (its center of gravity) that acts as the aggregator for reporting. 

* **Prioritize Forms for Intake.** Use record forms for groups with less sophistication in Workfront Planning to ensure metadata integrity. While Power Users may benefit from direct data entry in Table views, this should be approached with caution—bulk changes in a table can easily create data headaches for other stakeholders. 
 

### Don't: 

* **Don't say "Core".** Refer specifically to the **Workflow module** and the **Project** objects when talking about execution. 

* **Don't over-complicate.** Every additional level of hierarchy adds a "management tax." Only add levels that answer a business question you can't currently answer. 

* **Don't create silos.** Ensure your record types are shared across workspaces so teams aren't re-typing the same data.
-->