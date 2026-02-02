---
title: 'Playbook: Managed Scaling, nach dem ersten Sieg'
description: Erfahren Sie, wie Sie Adobe Workfront Planning nach Ihrer ersten erfolgreichen Implementierung einführen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 28913661935d5a030cb33dd204fcb3c08daf0b26
workflow-type: tm+mt
source-wordcount: '2025'
ht-degree: 0%

---


# Playbook: gemanagte Skalierung, nach dem ersten Sieg

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