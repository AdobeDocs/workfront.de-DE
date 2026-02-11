---
title: 'Playbook: Managed Scaling, nach dem ersten Sieg'
description: Erfahren Sie, wie Sie Adobe Workfront Planning nach Ihrer ersten erfolgreichen Implementierung einführen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
exl-id: 54df36b3-01a3-4fd3-b2d3-64ffb2fe5918
source-git-commit: 52bf41e146a11a4af4fbebfe5bb20a9765f2bc7b
workflow-type: tm+mt
source-wordcount: '2025'
ht-degree: 0%

---

# Playbook: gemanagte Skalierung, nach dem ersten Sieg

{{planning-important-intro}}

**Version**: 1.0

**Kontext**: „Wir haben unseren ersten Anwendungsfall landen lassen, und jetzt wollen alle mit.“



## &#x200B;1. Die „Erfolgsfalle“

Manchmal fühlt es sich an, als wäre die gefährlichste Phase der WFP-Einführung unmittelbar nach dem ersten erfolgreichen Anwendungsfall oder POC. Die Begeisterung ist groß, aber die Angst vor „technischer Verschuldung“ und einer „administrativen Zersiedelung“ kann zu zwei gleichermaßen schädlichen Reaktionen führen:

1. **Over-Governance**: Das System so eng einfrieren, dass neue Teams auf Tabellen zurückgreifen.

2. **Zero-Governance**: Jedes Team kann seine eigenen Felder und Datensatztypen erstellen und so die fragmentierte Zunahme an Metadaten in Legacy-Umgebungen reproduzieren.



## &#x200B;2. Die Kernphilosophie: WFP als „Abstimmungsmaschine“

Anstatt zu versuchen, Teams daran zu hindern, anders zu sein, positionieren wir das WFP als den Ort, an dem diese Unterschiede sichtbar **gemacht, damit sie in Einklang gebracht werden können**.



* **Verwaltung der Umsetzungsgeschwindigkeit**: Es ist nur natürlich, vorsichtig mit der Erweiterung auf ein neues Tool zu sein, bevor bestehende Umgebungen „bereinigt“ werden. Die Entscheidung für **Vereinfachung zuerst** bietet eine hochgradig verwaltete Grundlage, kann aber die Wertschöpfungszeit für Teams, die bereit sind, sich anzupassen, verzögern. Wir glauben, dass der effektivste Weg, um durch diese Veränderung zu führen, darin besteht anzuerkennen, dass **Sichtbarkeit Schritt 1 ist**. Die Dynamik hin zu einem gemeinsamen, einsatzbereiten Tool (weg von der Vielzahl von PPTs und Tabellenkalkulationen) ist es, was langfristige Ziele letztendlich freischaltet.



  **Empfehlung**: Anstelle eines „Clean Up First“-Mandats empfehlen wir, einen kleineren Teil der Ressourcen für die laufende Wartung und einen wesentlich größeren Teil für die Lösung dringender Geschäftsanforderungen bereitzustellen. So ergibt beispielsweise ein Jahr ausschließlich für die „Bereinigung“ von Taxonomien wenig inkrementellen Wert. Die Bereitstellung **teamübergreifenden Sichtbarkeit** (z. B. über einen einheitlichen Unternehmenskalender oder eine konsolidierte GTM-Roadmap) bietet jedoch den transformativen Wert, den Ihre Stakeholder benötigen, und bietet gleichzeitig die einheitliche Datenstruktur, die Sie für die Verwaltung der Umgebung im Laufe der Zeit benötigen.

* **Erkenne die Realität**: Unabhängige Teams entwickeln ganz natürlich ihre eigenen Prozesse, die oft in isolierten Tabellen verborgen bleiben. Die Umstellung auf das WEP schafft kein Chaos; sie beleuchtet das bereits bestehende. Indem Sie diese Prozesse in einer gemeinsamen Umgebung sichtbar machen, stellen Sie sie an einen Ort, an dem sie endlich angesprochen und verbessert werden können.

* **Das Fortschrittssignal**: Wenn ein Team nach seinen eigenen Feldern fragt, ist es kein „ausuferndes“ - es ist **Adoption**. Das bedeutet, dass sie das WFP als ihren Arbeitsbereich sehen.

* **Schulden verwalten, nicht verstecken**: Es ist nur natürlich, sich später um den Aufwand zu kümmern, um divergierende Taxonomien zu bereinigen. Die Alternative jedoch - die zu frühe Erzwingung strenger Standards - bringt Teams oft zurück in die Tabellenkalkulation, wo ihre Prozesse (und ihre Schulden) verborgen bleiben. Indem Sie es Teams ermöglichen, im WEP mit ihren aktuellen Klassifizierungen zu beginnen, verschieben Sie diese Schulden in eine sichtbare, verwaltete Umgebung. Dies macht die letztendliche Abstimmung zu einer iterativen Aufgabe statt zu einem einzigen, überwältigenden Migrationsprojekt.



## &#x200B;3. Das Governance-Modell „Fahrspuren auf einer Straße“

Skalieren Sie ohne Schulden, indem Sie „globale Spuren“ und „lokale Spielplätze“ definieren.



### A. Die globalen Fahrspuren

* **Kontrollierte Objekte**: Objekte, die jedes Team für das Reporting in Unternehmen verwenden muss (z. B. `Strategic Pillar`, `Region`, `Fiscal Quarter`).

* **Verwaltet von**: Der zentrale COE-/Marketing-Ops-Administrator.

* **Regel**: Diese Felder sind „Freigegeben“ und obligatorisch.



### B. Die lokalen Spielplätze (Speichen)

* **Experimentelle Objekte**: Felder oder Datensatztypen, die für die taktischen Anforderungen eines Teams spezifisch sind (z. B. die `Influencer Handle` eines Social-Media-Teams oder die `URL Slug` eines Web-Teams).

* **Verwaltet von**: Der Teamleiter (mit leichter Anleitung).

* **Regel**: Teams können hier innovativ sein. Wenn ein Feld „Lokal“ von > 3 Teams übernommen wird, wird es zu einer globalen Spur „befördert“.



## &#x200B;4. Das Governance-Paradoxon: Teams zuerst, Standards folgen

Eine häufige Herausforderung bei der Skalierung des WEP ist die Entscheidung, welche an erster Stelle steht: **Enterprise Governance** oder **Team Operational Alignment**.



Wir glauben, dass der effektivste Weg, dies zu bewältigen, darin besteht, anzuerkennen, dass der Unternehmenswert auf einer Zwei-Wege-Straße aufbaut:

1. **Teams benötigen Relevanz**: Das Unternehmen erzielt erst dann einen Wert, wenn seine Teams aktiv an der Ausführung arbeiten. Aus diesem Grund muss die Governance **Teams dienen** indem eine Struktur bereitgestellt wird, die ihren bekannten operativen Anforderungen entspricht.

2. **Das Unternehmen benötigt Sichtbarkeit**: Nur wenn die Daten sauber genug sind, um aggregiert zu werden, kann die Führung fundierte Entscheidungen treffen. Aus diesem Grund müssen die Teams **dem Unternehmen dienen** indem sie die für die Portfoliosichtbarkeit erforderlichen Mindestmetadaten bereitstellen.



Das Ziel von „Managed Scaling“ besteht darin, den Schnittpunkt dieser beiden Anforderungen zu finden - ausreichend standardisiert, um Sichtbarkeit zu bieten, aber nicht so sehr, dass Sie die Teamausführung blockieren.



### A. Abstimmen der Prioritäten: Daten vs. Visualisierung

Beachten Sie bei der Skalierung, dass die Definition von „Wert“ je nach Personas unterschiedlich ist:

* **Der Administrator/Produktinhaber**: Werte **einheitliche Taxonomien und Klassifizierungen**. Ihr Ziel ist eine saubere Datenarchitektur, die eine langfristige Skalierbarkeit unterstützt.

* **Der Stakeholder/Leader**: Werte **Visualisierung und insight** (z. B. ein globaler Kalender oder eine Portfolio-Zeitleiste). Ihr Ziel ist der „Lightning Moment“, der die Daten verwertbar macht.



**Die Strategie**: Verwenden Sie den Visualisierungsbedarf der Stakeholder als *Anreiz*, damit das Team den Datenstandard-Bedarf des Administrators einhält. Sie erhalten die einheitliche Taxonomie, indem Sie den „Superkalender“ bereitstellen, den die Führung verlangt.



### B. Die „dienstlich geführte“ Beobachtungsphase

Während des frühen Scale-ups besteht die Rolle des Administrators darin, diesen Austausch zwischen Teams und Unternehmen zu erleichtern.

* **Priorisieren des Betriebs vor**: Es ist besser, Teams aktiv in isolierten Arbeitsbereichen zu planen, als sie durch einen Mangel an globalen Definitionen zum Stillstand zu bringen. Diese Aktivität sind die „Rohdaten“, die zum Aufbau gesunder, realer Standards erforderlich sind.

* **Identifizieren Sie die „Sichtbarkeitsminima“**: Arbeiten Sie mit Führungskräften zusammen, um die 3-5 Felder zu identifizieren, *für das Reporting in Unternehmen sauber* müssen (z. B. `Strategic Alignment`, `Start Date`, `Budget`). Konzentrieren Sie Ihre Durchsetzungsenergie NUR hier.



### B. Rückwirkende Harmonisierung (Governance as a Service)

Sobald sich in allen Teams ein Muster „bekannter Bedürfnisse“ herausbildet, kann das Unternehmen diese Muster zu einem globalen Service konsolidieren.

1. **Erfolgreiche Muster beobachten**: Identifizieren Sie die „erfolgreichsten“ Taxonomien, die Teams bereits erstellt und übernommen haben.

2. **The Collaborative Handshake**: Teammitglieder zusammenbringen, um ihre lokalen Erfolge in einen gemeinsamen Unternehmensstandard zu integrieren.

3. **Bereitstellung als Service**: Einführung der neuen globalen Spuren nicht als „Einschränkung“, sondern als Möglichkeit, das Reporting und die teamübergreifende Ausrichtung für die Mitarbeitenden zu vereinfachen.



**Wichtige Neuerung**: Governance sollte eine Antwort auf den operativen Erfolg sein und keine Voraussetzung dafür.



## &#x200B;5. Skalierungsmechanik: Das auf dem Muster basierende Wachstumsmodell

Die Anwendung dieser Philosophie erfordert einen durchdachten Ansatz in Bezug auf die Datenstruktur. Um eine ausufernde Regierungsführung zu vermeiden, widerstehen Sie dem Drang, für jede einzelne Anfrage globale Felder zu errichten. Verwenden Sie stattdessen den **Feldreifepfad**, damit Ihre Unternehmensstandards von der Verwendung in der Praxis geleitet werden:



1. **Ebene 1: Lokales Experiment**: Team A erstellt ein benutzerdefiniertes Feld in seinem Arbeitsbereich.

2. **Ebene 2: Mustererkennung**: Der Administrator bemerkt, dass Teams B und C ein ähnliches Feld verwenden oder anfordern.

3. **Ebene 3: Unternehmensstandardisierung**: Der Administrator erstellt eine einzelne, standardisierte Version dieses Felds als Datensatztyp in der **Globalen Taxonomie-Workspace** und stellt sie Teams zur Verfügung.



### Die Mechanik des „Soft Retirement“

Da das WFP derzeit keine native „Archiv“-Funktion für Felder aufweist, ist zum Außerkraftsetzen eines lokalen Felds ein absichtlicher „Soft Retirement“-Prozess erforderlich, um historische Daten beizubehalten, ohne die Benutzeroberfläche zu überladen:



1. **Datenmigration**: Verwenden Sie eine Tabellenansicht (oder Fusion), um Werte aus dem lokalen Feld „Shadow“ in das neue Feld „Global Lane“ zu kopieren. Stellen Sie sicher, dass die Daten während dieses Verschiebevorgangs validiert und bereinigt werden.

2. **Für veraltete** umbenennen: Benennen Sie das lokale Feld mit einem Präfix wie `[DEPRECATED]` oder `z_` um (z. B. `z_Language (Old)`). Dadurch wird das Feld in den Feldauswahl ganz nach unten verschoben und den Benutzern signalisiert, dass es nicht mehr das &quot;Source der Wahrheit“ ist.

3. **Formularentfernung**: **Dies ist der kritischste Schritt.** Entfernen Sie das verworfene Feld aus allen **Datensatz-Forms**. Dadurch wird verhindert, dass neue Daten eingegeben werden, während die alten Daten in vorhandenen Tabellenansichten oder Berichten bei Bedarf sichtbar bleiben.

4. **Der „Sunset“-Zeitraum**: Behalten Sie das verworfene Feld (mit Präfix und außerhalb der Form) 30 bis 60 Tage lang bei, um sicherzustellen, dass während der Migration keine Daten verpasst wurden. Nach diesem Zeitraum kann das lokale Feld aus dem Arbeitsbereich gelöscht werden, wenn die Daten auf der globalen Spur vollständig abgestimmt sind.



## &#x200B;6. Vermeiden der „Kerndrift“ (die Abstraktionsregel)

So verhindern Sie, dass die Planung so unübersichtlich wird wie Core:

* **Die Abstraktionsebene**: Jedes Feld im WFP sollte eine &quot;**Frage“**. Wenn ein Feld nur für das taktische Tracking verwendet wird (z. B. „Wurde dieser Korrekturabzug genehmigt?„), behalten Sie es im Kern bei.

* **Konsolidierung zuerst**: Wenn ein Team ein neues Metadatenfeld möchte, laden Sie es ein, zunächst die globale Taxonomie zu überprüfen. Dazu müssen Sie Team-Leads **Nur-Lese-Zugriff** auf den Arbeitsbereich Globale Taxonomie gewähren (siehe Abschnitt 7). Indem Sie ihre taktischen Anforderungen einem vorhandenen strategischen Feld zuordnen, vermeiden Sie unnötige Duplizierungen und behalten die Integrität des Reportings bei.



## &#x200B;7. Das Sichtbarkeitsmodell „Nur-Lese-Zugriff“

Lösen Sie das „isolierte“ Gefühl ohne das Geräusch der „isolierten“ Arbeit.

* **Das Problem**: Teams in Sprechern fühlen sich isoliert, weil sie nur ihre eigenen Aufzeichnungen sehen.

* **Die Lösung**: Gewähren Sie Teams **schreibgeschützten Zugriff auf die Arbeitsbereiche, die für diese freigegebenen Datensatztypen als &quot;Primär&quot;** sind.

* **Das Ergebnis**: Sie können den umfassenderen Unternehmenskontext für Inspiration und Ausrichtung sehen, aber ihr lokaler Arbeitsbereich bleibt sauber und auf ihre spezifischen Aufgaben konzentriert.



## &#x200B;8. Wachstumsmanagement durch Workshops

Die Skalierung des WEP ist ebenso eine kulturelle wie eine technische Herausforderung. Nutzen Sie gezielte Workshops, um die „Governance-Lücke“ zu schließen.



### A. Der Discovery-Workshop zur „notwendigen Unordnung“

* **Zielgruppe**: Regionale Marketing-Leads und Ops-Champions.

* **Goal**: Dokumentieren Sie die aktuelle „Siloed Reality“ (die fragmentierten operativen Daten).

* **Die Nachricht**: „Wir sind nicht hier, um Ihre Felder zu löschen. Wir sind hier, um zu verstehen, wie sie mit der globalen Strategie zusammenhängen.“

* **Ergebnis**: Entwurf einer Zuordnung lokaler taktischer Felder zu globalen strategischen Fahrspuren.



### B. Die Ausrichtungssitzung „Strategische Sichtbarkeit“

* **Zielgruppe**: Hochrangige Marketing-Stakeholder (Führung).

* **Ziel**: Ändern Sie die Angst vor der „Vereinfachung zuerst“.

* **Die Nachricht**: „Wir brauchen keine perfekte Taxonomie, um zu beginnen. Wir verwenden das WFP als Umgebung, um *die perfekte* aufzubauen“.

* **Ergebnis**: Genehmigung für die Weiterentwicklung von WFP als Abstimmungsmaschine, während Core in seinem aktuellen Zustand bleibt.



### C. Der „Spoke-to-Global“-Showcase

* **Audience**: Neue Teams erkunden das WFP.

* **Ziel**: Reduzieren Sie das „isolierte“ Gefühl.

* **Die Nachricht**: „Sehen Sie sich an, wie die lokale Arbeit von Team A automatisch die vorgesehene Primäre Workspace befüllt? Dieselbe Sichtbarkeit können Sie auch für Ihre Arbeit erreichen.“

* **Ergebnis**: Opt-in aus neuen Abteilungen, die den Vorteil einer „Vernetzung“ sehen, ohne ihre lokale Unabhängigkeit zu verlieren.



### D. Die „Laufende Support“-Bürozeiten

* **Zielgruppe**: Alle WFP-Benutzer (aktuelle und potenzielle).

* **Ziel** Bereitstellung einer wiederkehrenden Umgebung mit geringem Aufwand für die Fehlerbehebung und für taktische Hinweise.

* **Die Nachricht**: „Es gibt keine falschen Fragen. Wir sind hier, um Ihnen bei der Lösung Ihrer spezifischen Planungsprobleme in Echtzeit zu helfen.“

* **Ergebnis**: Erhöhtes Anwendervertrauen, schnellere Behebung technischer Probleme und die Identifizierung neuer Muster, die eine globale Standardisierung rechtfertigen könnten.



## &#x200B;9. Personalausstattung in größerem Maßstab: Funktionen und Zuständigkeiten

Um in einem Modell mit verwalteter Skalierung erfolgreich zu sein, ist mehr als nur die Konfiguration von Tools erforderlich. Dafür ist eine klare Verteilung der Rollen auf die Global- und Spoke-Teams erforderlich.



### A. Der Unternehmensarchitekt (zentrale COE/Marketing-Opportunities)

* **Fokus**: Unternehmensintegrität, Systemleistung und **einheitliche Datentaxonomie**.

* **Zuständigkeiten**:

   * Verwaltet die **Globale Taxonomie Workspace**.

   * Erleichtert den **Field Maturity Path** (Förderung lokaler Erfolge nach globalen Standards).

   * Behält die **Primären Workspace**-Ansichten für das Executive-Reporting bei.

   * Führt den monatlichen **semantischen Audit** über Arbeitsbereiche hinweg.



### B. Der Sprecher (Teamprozessinhaber)

* **Focus**: Teamrelevanz und Umsetzungsgeschwindigkeit.

* **Zuständigkeiten**:

   * Fungiert als zentraler Ansprechpartner für das funktionale Team.

   * Sie steuert die Struktur des lokalen Arbeitsbereichs und benutzerdefinierte Feldexperimente.

   * Stellt sicher, dass das Team das **Governed Gateway** (Forms) für die Dateneingabe verwendet.

   * Teilnimmt am **Partizipativen Handshake** während der Harmonisierung teil.



### C. Der Executive Sponsor (Marketing-Führung)

* **Fokus**: Strategische Ausrichtung, OKR-Sichtbarkeit **Portfoliovisualisierung (z. B. globaler Kalender)**.

* **Zuständigkeiten**:

   * Definiert das Unternehmen **Marketing-OKRs** im Arbeitsbereich „Globale Taxonomie“.

   * Setzt sich bei anderen Führungskräften für den Wert von „Schritt 1 für die Sichtbarkeit“ ein.

   * Verstärkt die Ressourcenzuweisung von 80/20 (Wert über Bereinigung).



### D. Der Aktivierungs-Lead (Änderungsverwaltung)

* **Focus**: Kulturwandel und Kompetenzentwicklung.

* **Zuständigkeiten**:

   * hostet wiederkehrende **Office Hours** und **Discovery Workshops**.

   * Verwaltet das interne „Success Story“-Showcase.

   * Identifiziert technische Reibungspunkte, die der Unternehmensarchitekt lösen muss.



## &#x200B;10. Checkliste für die Skalierung des nächsten Teams

* [ ] **Identify the Champion**: Wer ist der „Process Owner“ oder „Champion“ dieses neuen Teams?

* [ ] **Definieren des „Lokalen Deltas“**: Welche 2-3 Felder benötigt dieses Team, die der globale Standard derzeit nicht bereitstellt?

* [ ] **Map to Global Lanes**: Welche bereits vorhandenen globalen Felder können 80% ihres Bedarfs decken?

* [ ] **Globale Sichtbarkeit gewähren**: Gewähren Sie ihnen schreibgeschützten Zugriff auf die relevanten Primären Arbeitsbereiche und den Arbeitsbereich für die globale Taxonomie an Tag 1.

* [ ] **Etablierung des Handoffs**: Wie „speist“ deren Arbeit die relevanten Primären Arbeitsbereiche? (z. B. über einen globalen Datensatztyp oder eine bestimmte Suche).

<!--original content: 

**Version**: 1.0 

**Context**: "We've landed our first use case, and now everyone wants in." 

 

## 1. The "Success Trap" 

Sometimes it can feel like the most dangerous phase of WFP adoption is immediately after the first successful use case or POC. Enthusiasm is high, but the fear of "technical debt" and "administrative sprawl" can lead to two equally damaging responses: 

1.  **Over-Governance**: Locking down the system so tightly that new teams revert to spreadsheets. 

2.  **Zero-Governance**: Letting every team create their own fields and record types, recreating the fragmented metadata sprawl found in legacy environments. 

 

## 2. The Core Philosophy: WFP as the "Reconciliation Engine" 

Instead of trying to stop teams from being different, we position WFP as the place where those differences are **made visible so they can be reconciled**. 

 

*   **Managing Adoption Velocity**: It is natural to feel cautious about expanding into a new tool before "cleaning up" existing environments. While choosing to **Simplify First** provides a highly governed foundation, it can delay time-to-value for teams ready to align. We believe the most effective way to lead through this change is to recognize that **visibility is Step 1**. Momentum toward a shared, enterprise-ready tool (moving away from the sprawl of PPTs and spreadsheets) is what ultimately unblocks long-term goals.  

 

    **Recommendation**: Instead of a "Clean Up First" mandate, we recommend allocating a smaller portion of resources to ongoing maintenance and a significantly larger portion to solving pressing business needs. For example, spending a year solely on "cleaning up" taxonomies yields little incremental value. However, delivering **cross-team visibility** (e.g., through a Unified Enterprise Calendar or a consolidated GTM roadmap) provides the transformative value your stakeholders need, while providing the unified data structure you need to govern the environment over time. 

*   **Acknowledge the Reality**: Independent teams naturally develop their own processes, which often stay hidden in siloed spreadsheets. Transitioning to WFP doesn't create a mess; it shines a light on the one that already exists. By making these processes visible in a shared environment, you put them in the one place where they can finally be addressed and improved. 

*   **The Progress Signal**: When a team asks for their own fields, it's not "sprawl"—it's **Adoption**. It means they see WFP as their workspace. 

*   **Manage Debt, Don't Hide It**: It is natural to be concerned about the effort required to clean up divergent taxonomies later. However, the alternative—forcing strict standards too early—often drives teams back to spreadsheets where their processes (and their debt) remain hidden. By allowing teams to begin in WFP with their current classifications, you are moving that debt into a visible, governed environment. This makes the eventual reconciliation an iterative task rather than a single, overwhelming migration project. 

 

## 3. The "Lanes on a Road" Governance Model 

Scale without debt by defining "Global Lanes" and "Local Playgrounds." 

 

### A. The Global Lanes 

*   **Controlled Objects**: Objects that every team must use for enterprise reporting (e.g., `Strategic Pillar`, `Region`, `Fiscal Quarter`). 

*   **Managed By**: The Central COE/Marketing Ops Admin. 

*   **Rule**: These fields are "Shared" and mandatory. 

 

### B. The Local Playgrounds (Spokes) 

*   **Experimental Objects**: Fields or record types specific to a team's tactical needs (e.g., a Social team's `Influencer Handle` or a Web team's `URL Slug`). 

*   **Managed By**: The Team Lead (with light guidance). 

*   **Rule**: Teams can innovate here. If a "Local" field is adopted by >3 teams, it is "Promoted" to a Global Lane. 

 

## 4. The Governance Paradox: Teams First, Standards Follow 

A common challenge in scaling WFP is deciding which comes first: **Enterprise Governance** or **Team Operational Alignment**.  

 

We believe the most effective way to navigate this is to recognize that enterprise value is built on a two-way street: 

1.  **Teams need relevance**: The enterprise only realizes value when its teams are actively executing. Therefore, governance must **serve the teams** by providing structure that supports their known operational needs. 

2.  **The Enterprise needs visibility**: Leadership can only make informed decisions when data is clean enough to aggregate. Therefore, the teams must **serve the enterprise** by providing the minimum viable metadata required for portfolio visibility. 

 

The goal of "Managed Scaling" is to find the intersection of these two needs—standardizing enough to provide visibility, but not so much that you stall team execution. 

 

### A. Aligning Priorities: Data vs. Visualization 

When scaling, recognize that the definition of "Value" differs between personas: 

*   **The Admin/Product Owner**: Values **unified taxonomies and classifications**. Their goal is a clean data architecture that supports long-term scalability. 

*   **The Stakeholder/Leader**: Values **visualization and insight** (e.g., a Global Calendar or a Portfolio Timeline). Their goal is the "Lightning Moment" that makes the data actionable. 

 

**The Strategy**: Use the stakeholder's need for visualization as the *incentive* for the team's compliance with the admin's need for data standards. You get the unified taxonomy by delivering the "Super Calendar" that leadership demands. 

 

### B. The "Service-Led" Observation Phase 

During early scale-up, the Admin's role is to facilitate this exchange between teams and the enterprise. 

*   **Prioritize Operation over Standardization**: It is better to have teams actively planning in siloed workspaces than to have them stalled by a lack of global definitions. This activity is the "raw data" required to build healthy, real-world standards. 

*   **Identify the "Visibility Minimums"**: Work with leadership to identify the 3-5 fields that *must* be clean for enterprise reporting (e.g., `Strategic Alignment`, `Start Date`, `Budget`). Focus your enforcement energy ONLY here. 

 

### B. Retroactive Harmonization (Governance as a Service) 

Once a pattern of "known needs" emerges across teams, the enterprise can move to consolidate those patterns into a global service. 

1.  **Observe Successful Patterns**: Identify the "winning" taxonomies that teams have already built and adopted. 

2.  **The Collaborative Handshake**: Bring team champions together to refine their local successes into a shared enterprise standard. 

3.  **Deploy as a Service**: Roll out the new global lanes not as a "restriction," but as a way to simplify reporting and cross-team alignment for the people doing the work. 

 

**Key Takeaway**: Governance should be a response to operational success, not a prerequisite for it.  

 

## 5. Scaling Mechanics: The Pattern-Based Growth Model 

Applying this philosophy requires a thoughtful approach to data structure. To avoid "Governance Sprawl," resist the urge to build global fields for every individual request. Instead, use the **Field Maturity Path** to let real-world usage guide your enterprise standards: 

 

1.  **Level 1: Local Experiment**: Team A creates a custom field in their workspace. 

2.  **Level 2: Pattern Recognition**: The Admin notices Teams B and C are using or asking for a similar field. 

3.  **Level 3: Enterprise Standardization**: The Admin creates a single, standardized version of that field as a record type in the **Global Taxonomy Workspace** and syndicates it to teams. 

 

### The Mechanics of "Soft Retirement" 

Because WFP does not currently have a native "Archive" feature for fields, retiring a local field requires a deliberate "Soft Retirement" process to preserve historical data without cluttering the UI: 

 

1.  **Data Migration**: Use a table view (or Fusion) to bulk-copy values from the local "Shadow" field into the new Global Lane field. Ensure the data is validated and cleaned during this move. 

2.  **Rename for Deprecation**: Rename the local field with a prefix like `[DEPRECATED]` or `z_` (e.g., `z_Language (Old)`). This pushes the field to the bottom of field pickers and signals to users that it is no longer the "Source of Truth." 

3.  **Form Removal**: **This is the most critical step.** Remove the deprecated field from all **Record Forms**. This prevents new data from being entered while keeping the old data visible in existing table views or reports if needed. 

4.  **The "Sunset" Period**: Keep the deprecated field (prefixed and off-form) for 30-60 days to ensure no data was missed during migration. After this period, if the data is fully reconciled in the Global Lane, the local field can be deleted from the workspace. 

 

## 6. Avoiding the "Core Drift" (The Abstraction Rule) 

To prevent Planning from becoming as cluttered as Core: 

*   **The Abstraction Layer**: Every field in WFP should answer a **Strategic Question**. If a field is only used for tactical tracking (e.g., "Was this proof approved?"), keep it in Core. 

*   **Consolidation First**: If a team wants a new metadata field, invite them to check the Global Taxonomy first. This requires granting team leads **Read-Only access** to the Global Taxonomy workspace (see Section 7). By mapping their tactical needs to an existing strategic field, you prevent unnecessary duplication and maintain reporting integrity. 

 

## 7. The "Read-Only Access" Visibility Model 

Solve the "Siloed" feeling without the noise of "Siloed" work. 

*   **The Problem**: Teams in spokes feel isolated because they only see their own records. 

*   **The Fix**: Grant teams **Read-Only access to the workspaces designated as 'Primary' for those shared record types**.  

*   **The Result**: They can see the broader enterprise context for inspiration and alignment, but their local workspace remains clean and focused on their specific tasks. 

 

## 8. Managing Growth through Workshops 

Scaling WFP is as much a cultural challenge as a technical one. Use targeted workshops to bridge the "Governance Gap." 

 

### A. The "Necessary Mess" Discovery Workshop 

*   **Audience**: Regional Marketing Leads and Ops Champions. 

*   **Goal**: Document the current "Siloed Reality" (the fragmented operational data). 

*   **The Message**: "We aren't here to delete your fields. We're here to understand how they link to the global strategy." 

*   **Outcome**: A draft mapping of local tactical fields to global strategic lanes. 

 

### B. The "Strategic Visibility" Alignment Session 

*   **Audience**: High-level Marketing Stakeholders (leadership). 

*   **Goal**: Reframe the "Simplify First" anxiety. 

*   **The Message**: "We don't need a perfect taxonomy to start. We are using WFP as the environment to *build* the perfect taxonomy." 

*   **Outcome**: Approval to move forward with WFP as the reconciliation engine while Core remains in its current state. 

 

### C. The "Spoke-to-Global" Showcase 

*   **Audience**: New teams exploring WFP. 

*   **Goal**: Reduce the "siloed" feeling. 

*   **The Message**: "See how Team A's local work automatically feeds the designated Primary Workspace? You can have that same visibility for your work too." 

*   **Outcome**: Opt-in from new departments who see the benefit of being "connected" without losing their local independence. 

 

### D. The "Ongoing Support" Office Hours 

*   **Audience**: All WFP users (current and prospective). 

*   **Goal**: Provide a recurring, low-stakes environment for troubleshooting and tactical guidance. 

*   **The Message**: "There are no wrong questions. We are here to help you solve your specific planning challenges in real-time." 

*   **Outcome**: Increased user confidence, faster resolution of technical friction, and the identification of new patterns that might warrant global standardization. 

 

## 9. Staffing for Scale: Roles and Responsibilities 

Success in a managed scaling model requires more than just tool configuration; it requires a clear distribution of roles across the Global and Spoke teams. 

 

### A. The Enterprise Architect (Central COE/Marketing Ops) 

*   **Focus**: Enterprise integrity, system performance, and **unified data taxonomy**. 

*   **Responsibilities**: 

    *   Manages the **Global Taxonomy Workspace**. 

    *   Facilitates the **Field Maturity Path** (promoting local successes to global standards). 

    *   Maintains the **Primary Workspace** views for executive reporting. 

    *   Leads the monthly **Semantic Audit** across workspaces. 

 

### B. The Spoke Champion (Team Process Owner) 

*   **Focus**: Team relevance and adoption velocity. 

*   **Responsibilities**: 

    *   Acts as the single point of contact for the functional team. 

    *   Owns the local workspace structure and custom field experiments. 

    *   Ensures the team uses the **Governed Gateway** (Forms) for data entry. 

    *   Participates in the **Collaborative Handshake** during harmonization. 

 

### C. The Executive Sponsor (Marketing Leadership) 

*   **Focus**: Strategic alignment, OKR visibility, and **portfolio visualization (e.g., Global Calendaring)**. 

*   **Responsibilities**: 

    *   Defines the enterprise **Marketing OKRs** in the Global Taxonomy workspace. 

    *   Champions the value of "Visibility Step 1" to other leaders. 

    *   Reinforces the 80/20 resource allocation (Value over Cleanup). 

 

### D. The Enablement Lead (Change Management) 

*   **Focus**: Cultural shift and skill development. 

*   **Responsibilities**: 

    *   Hosts recurring **Office Hours** and **Discovery Workshops**. 

    *   Maintains the internal "Success Story" showcase. 

    *   Identifies technical friction points for the Enterprise Architect to resolve. 

 

## 10. Checklist for Scaling the Next Team 

* [ ] **Identify the Champion**: Who is the "Process Owner" or "Champion" of this new team? 

* [ ] **Define the "Local Delta"**: What 2-3 fields does this team need that the Global standard doesn't currently provide? 

* [ ] **Map to Global Lanes**: Which existing Global fields can satisfy 80% of their needs? 

* [ ] **Grant Global Visibility**: Give them Read-Only access to the relevant Primary Workspaces and the Global Taxonomy workspace on Day 1. 

* [ ] **Establish the Handoff**: How does their work "feed" the relevant Primary Workspaces? (e.g., via a Global Record Type or a specific lookup).

-->