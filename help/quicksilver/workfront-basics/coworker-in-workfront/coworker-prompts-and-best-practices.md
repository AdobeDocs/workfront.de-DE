---
title: CX-Coworker-Eingabeaufforderungen und Best Practices
content-type: reference
description: Erfahren Sie mehr über die Best Practices für die Verwendung von Kollegen in Workfront und sehen Sie sich eine Liste von Beispielen für Eingabeaufforderungen an.
author: Becky
feature: Get Started with Workfront
source-git-commit: 01de260893e5bbf7a228479df2f3fc6a1337d31d
workflow-type: tm+mt
source-wordcount: '2247'
ht-degree: 2%

---

# CX-Coworker-Eingabeaufforderungen und Best Practices

&lt;!—VERWENDEN SIE DIESE NICHT—Verweisen Sie stattdessen auf den Artikel MCP-Beispiel-Eingabeaufforderungen , stellen Sie sicher, dass er mit den neuesten Versionen von MCP aktualisiert wurde—>

>[!IMPORTANT]
>
>CX Coworker steht derzeit Organisationen im Gesundheitswesen, im Finanzwesen oder in einigen anderen Branchen mit sensiblen Daten nicht zur Verfügung. KI-Assistent steht diesen Organisationen zur Verfügung. Weitere Informationen finden Sie unter [Übersicht über den KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).

Mit CX Coworker können Sie natürliche Sprache verwenden, um mit Workfront-Workflows und Workfront-Planung zu interagieren.

Coworker ist Teil von Adobe Experience Cloud Agent Orchestrator.

Weitere Informationen zu Agent Orchestrator finden Sie unter [Adobe Experience Platform Agent Orchestrator ](https://experienceleague.adobe.com/de/docs/experience-cloud-ai/experience-cloud-ai/agents/agent-orchestrator).

## Zugriffsanforderungen

<!--Add info about how to qualify for agent orchestrator stuff-->

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Auswählen von, Prime oder Ultimate </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard oder Light</p>
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td><p>Für alle Funktionen außerhalb der grundlegenden Kenntnisse muss Ihr Unternehmen Adobe Agent Orchestrator erworben haben.</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td><p>Sie müssen über die entsprechenden Berechtigungen verfügen, um über einen Kollegen mit einem beliebigen Objekt interagieren zu können.</p> <p>Um beispielsweise Informationen über ein Projekt über einen Kollegen zu erhalten, müssen Sie mindestens über die Berechtigung Anzeigen für dieses Projekt verfügen.</p></td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Voraussetzungen

* Ihr Workfront-Administrator muss den KI-Assistenten für Ihr Unternehmen aktiviert haben.

  Weitere Informationen finden Sie unter [Voraussetzungen für den KI-](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant)) im Artikel KI-Assistent - Übersicht.
* Ihr Workfront-Administrator muss den KI-Assistenten für Ihre Zugriffsebene aktiviert haben.

  Weitere Informationen finden Sie unter [Aktivieren oder Deaktivieren des KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

## Zu beachten

Beachten Sie die folgenden Einschränkungen bei der Verwendung von CX Coworker:

### Umkehrbarkeit

Einige Aktionen können rückgängig gemacht werden. Wenn beispielsweise ein Objekt erstellt wird, kann diese Erstellung rückgängig gemacht werden.

Einige Aktionen, wie das Löschen von Objekten, können jedoch **nicht** rückgängig gemacht werden. Es wird empfohlen, dies bei der Durchführung von Aktionen mit Ihren Daten über einen Kollegen zu beachten.

### Einschränkungen bei der Daten-/Objektabdeckung

* Die Abfrage von und das Reporting zu benutzerdefinierten Feldern befinden sich in frühen Phasen und einige Fähigkeiten (wie API-basierte Abfrage-Helper) verarbeiten noch keine beliebigen benutzerdefinierten Felder für die Aggregation und Filterung.

### Einschränkungen bei Interaction/UX

* CX Coworker „lernt“ derzeit nicht langfristig aus dem Stil oder den Vorlieben eines einzelnen Benutzers. In jedem Chat wird nur das aktuelle Gespräch und Produktwissen verwendet.
* Der Konversationskontext wird innerhalb einer einzelnen Chat-Sitzung beibehalten. Durch Öffnen einer neuen Seite oder Schließen des Assistenten wird der Unterhaltungsverlauf zurückgesetzt.
* Wenn Genehmigungsverfahren in einem externen Programm wie Confluence oder SharePoint vorhanden sind und nur über URL-Felder verknüpft werden, ruft der Mitarbeiter derzeit keine Inhalte auf diesen Seiten ab und argumentiert nicht darüber.

### Datenspeicher/kundenverwaltete Schlüssel

* Da CX Coworker Teil des Adobe Experience Platform Agent Orchestrator ist, werden Daten aus Ihren Interaktionen mit Coworker in Adobe Experience Platform gespeichert, nicht in Workfront. Daher werden diese Daten nicht von BYOK-Vereinbarungen (Customer Managed Keys) von Workfront abgedeckt.

## Allgemeine grundlegende KI-Kenntnisse

>[!IMPORTANT]
>
>Diese allgemeinen Funktionen stehen allen Benutzenden zur Verfügung, für deren Unternehmen eine unterzeichnete Adobe AI-Vereinbarung vorliegt.

Best Practices und Eingabeaufforderungen für diese allgemeinen Fähigkeiten finden Sie unter [Eingabeaufforderungen und Best Practices für den KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/ai-prompts-best-practices.md).

<!--Follow up with Oznur-->

### Produktkenntnisse

CX Coworker kann Anweisungen oder Referenzinformationen bereitstellen, die aus der Workfront-Dokumentation abgerufen werden.

Weitere Informationen zum Abrufen von Informationen aus der Workfront-Dokumentation finden [ unter „Hilfe vom KI-Assistenten ](/help/quicksilver/workfront-basics/ai-assistant/use-ai-to-retrieve-instructions.md).

Beispiel: Wie ändere ich den Aufgabendauer-Typ?

### Zusammenfassung von Projekten, Aufgaben und Problemen

CX Coworker kann Projekte, Aufgaben oder Probleme <!--, or documents-->, die in Workfront hochgeladen wurden.

Weitere Informationen zu Projekt-, Aufgaben- und Problemzusammenfassungen finden Sie unter [Zusammenfassen mit dem KI-Assistenten](/help/quicksilver/workfront-basics/ai-assistant/summarize-this.md).

Beispiel: Fassen Sie das Projekt Herbstkampagne 2026 zusammen.

<!--

### Locate work items

CX Coworker can find work items like projects, tasks, and issues

Example: Find all tasks assigned to me that are due this week.

For more information on using AI Assistant to locate project, tasks, and issues, see [se AI Assistant to work with projects, tasks, and issues](/help/quicksilver/workfront-basics/ai-assistant/work-with-pti-through-ai-assisant.md).

-->

<!--

Follow up on this to see if it's going away or what

### Catch Me Up 

Catch Me Up summarizes updates, uploaded documents, and other notable changes that have about your projects that have occurred in the last 24 hours, 3 days, or 7 days.  

For more information on Catch me up, see [Catch up on work in Priorities](/help/quicksilver/workfront-basics/priorities/catch-me-up.md).

-->

<!--

### Smart filters

You can use natural language filters in Priorities to replace status, pre-built views to help you filter your work.

For more information on using Smart Filters, see [Filter your work with Smart filters](/help/quicksilver/workfront-basics/priorities/filter-group-work-priorities.md) in the article Filter and group your work with Priorities.

-->

## CX-Mitarbeiter in Workfront

* [Projekt-, Aufgaben- und Probleminformationen](#project-task-and-issue-information)
* [Projekt- und Arbeitsmanagement](#project-and-work-management)
* [Inhalte und Genehmigungen](#content-and-approvals)

### Projekt-, Aufgaben- und Probleminformationen

CX Coworker kann Ihnen Informationen zu Projekten, Aufgaben und Problemen liefern, einschließlich Zusammenfassungen und Projektstatus.

Siehe Beispiel-Eingabeaufforderungen für Dokument- und Asset-Genehmigungen in den folgenden Bereichen:

* [Suchen von Informationen zu Projekten, Aufgaben oder Problemen](#find-information-about-projects-tasks-or-issues)
* [Zusammenfassen von Projekten, Aufgaben oder Problemen](#summarize-projects-tasks-or-issues)
* [Projektstatus für Projekte, Programme oder Portfolios anzeigen](#show-project-health-for-projects-programs-or-portfolios) <!--remove any mention of project health-->

#### Suchen von Informationen zu Projekten, Aufgaben oder Problemen

* Projekte
  * Alle aktiven Projekte für das Marken-Marketing-Team anzeigen
  * benötigt eine Liste von Projekten im Kampagnen-Portfolio des 4. Quartals unter der Kategorie „Digital“.
  * Zeigen Sie mir Projekte, die von Benutzenden in der Creative Services-Firma verwaltet werden, die Projektmanager sind.
* Aufgaben
  * Bring mir alle Aufgaben, die Joan Harris zugewiesen sind.
  * Aufgaben in der Kategorie „Design“ anzeigen, die dem UX-Team zugewiesen sind.
  * Ich benötige Aufgaben, die Copywritern im Holiday Promotions-Programm zugewiesen sind.
* Probleme
  * Alle Ausgaben im Projekt „Website Redesign“ in der Kategorie „Technisch“ anzeigen.
  * Rufen Sie alle ungelösten Probleme ab, die von der QA-Gruppe gemeldet wurden.
  * Ich benötige Anfragen, die Entwicklern im Global Tech-Unternehmen zugewiesen werden.

#### Zusammenfassen von Projekten, Aufgaben oder Problemen

* „Dieses Projekt zusammenfassen“
* „Zusammenfassung der letzten Woche zu diesem Projekt“

#### Projektstatus für Projekte, Programme oder Portfolios anzeigen

>[!NOTE]
>
>Ihre Organisation muss in der Betaversion zur Projektdiagnose registriert sein, um diese Funktion verwenden zu können.

* „Anzeigen des Zustands meiner aktiven Projekte“
* „Zeigen Sie mir den Zustand dieses Programms“

### Projekt- und Arbeitsmanagement

Sie können CX Coworker verwenden, um Projekte zu erstellen und zu verwalten, einschließlich Aufgaben und Zuweisungen.

Siehe Beispielaufforderungen für das Projekt- und Arbeits-Management in den folgenden Bereichen:

* [Erstellen, Aktualisieren oder Löschen von Projekten](#create-update-or-delete-projects)
* [Identifizieren der richtigen Projektvorlage basierend auf der Benutzeraufforderung](#identify-the-right-project-template-based-on-user-prompt)
* [Aufgaben in einem Projekt hinzufügen, bearbeiten oder anpassen](#add-edit-or-customize-tasks-in-a-project)
  <!--* [Create, update, or delete assignments](#create-update-or-delete-assignments)-->
  <!--* [Recommend best matching user assignments for the task based on users' job role and availability](#recommend-best-matching-user-assignments-for-the-task-based-on-users-job-role-and-availability)-->

#### Erstellen, Aktualisieren oder Löschen von Projekten

Sie können Projekte von Grund auf neu oder aus Vorlagen erstellen, aktualisieren und löschen.

* Erstellen Sie ein leeres Projekt mit dem Namen „Q2 Innovation Sandbox“, das am 10. März beginnt und am 30. April endet. Legen Sie mich als Besitzer fest.
* Erstellen Sie ein Projekt mit dem Namen Lucent AI Launch - NA unter Verwendung der Vorlage Integrierte Marketing-Kampagne . Beginnen Sie am 5. Februar und setzen Sie ihn auf Aktuell.
* Erstellen Sie ein Projekt mit dem Namen Website Redesign - EMEA, das am 1. März beginnt und am 15. Juni endet. Seine hohe Priorität, im Besitz von EMEA Marketing, gesponsert von der VP of Marketing, budgetiert auf 250.000 $ mit etwa 1.200 geplanten Stunden, konzentrierte sich auf Europa mit dem Ziel, Konversionen zu verbessern.
* Für das Projekt „Lucent AI Launch - NA“ verschieben Sie es in das zweite Quartal, ändern Sie das Ziel in „Driving Free Trials“, schieben Sie das Ziel bis Mitte April, erhöhen Sie das Budget auf 150.000 Dollar und markieren Sie es als dringend.
* Alle aktuellen, im 2. Quartal abgeschlossenen Marketing-Projekte anzeigen, die hohe oder dringende Priorität haben, sortiert nach frühestem Enddatum.

#### Aufgaben hinzufügen oder bearbeiten

Sie können Aufgaben zu einem Projekt hinzufügen oder bearbeiten und die Aufgabenliste der Vorlage, die Sie zum Erstellen eines Projekts verwenden, anpassen.

* Fügen Sie eine neue Aufgabe mit dem Namen Landingpage-QA zum Projekt hinzu und planen Sie sie vom 22. April bis zum 26. April.
* Aktualisieren Sie die Aufgabe zur Entwurfsüberprüfung so, dass sie am 18. April abgeschlossen ist, und weisen Sie sie dem Kreativ-Team zu.
* Entfernen Sie die Aufgabe „Asset-Produktion drucken“ aus dem Projekt.
* Alle Aufgaben in diesem Projekt anzeigen, die noch nicht abgeschlossen sind und die zwischen dem 1. und 30. April beginnen sollen.
* Legen Sie die Validierung als Vorgänger der Campaign Launch-Aufgabe fest.
* Fügen Sie eine neue Aufgabe mit dem Namen Abgeschlossenes Polnisch kopieren hinzu, die vom 15. bis zum 16. April geplant ist, verschieben Sie die Aufgabe zum Überprüfen kopieren auf den 10. April, entfernen Sie die Aufgabe „Zusätzliche Prüfungsrunde“ und legen Sie „Abgeschlossenes Polnisch kopieren“ als Vorgänger von E-Mail-Build fest.
* Versuchen Sie während des Erstellungsflusses des Projekts, so viele Informationen wie möglich über Ergebnisse bereitzustellen, die idealerweise zu Aufgaben im Rahmen des Projekts werden sollten.

#### Erstellen, Aktualisieren oder Löschen von Zuweisungen

Sie können Benutzer- oder Aufgabenrollenzuweisungen erstellen, aktualisieren und löschen.

* Identifizieren Sie für das Projekt „Landingpage für Produktstart entwerfen“ die entsprechenden Aufgabengebiete und empfohlenen geplanten Stunden für alle derzeit nicht zugewiesenen Aufgaben.
* Ich habe mehrere nicht zugewiesene Aufgaben, einschließlich „GA4-Tracking für Campaign-Site implementieren“, „Konversionsereignisse einrichten“ und „Analytics-Daten validieren“. Können Sie für jedes Aufgabengebiet die richtigen Aufgabengebiete und die richtigen geschätzten Stunden vorschlagen?
* Weisen Sie den Kreativaufgaben „Erstellen von drei Bannervarianten für EMEA-Display-Anzeigen“, „Überarbeitungen anwenden“ und „Fertige Assets exportieren“ die besten Aufgabengebiete zu und schätzen Sie den erforderlichen Aufwand für jede Aufgabe.
* Identifizieren Sie in den Projekten „Produkteinführung im 2. Quartal“, „Website-Neugestaltung - EMEA“ und „Bezahlte Medienkampagne - NA“ alle nicht zugewiesenen Aufgaben und weisen Sie die entsprechenden Aufgabengebiete mit jeweils empfohlenen geplanten Stunden zu.

<!--

#### Identify the right project template based on user prompt

* We're launching a new product feature with a landing page, emails, paid ads, and social posts. Which project template should we use?
* Create a project for a global marketing campaign with multiple channels and regional rollouts. (should suggest a template if provided more info)
* For Website Redesign – EMEA project, recommend and attach the correct project template.

-->

<!--

#### Recommend best matching user assignments for the task based on users' job role and availability

* Who is the best available user to assign to 'Design Landing Page Hero', considering who still has capacity today?
* Who should be assigned to 'Backend API integration for campaign reporting', considering engineering role alignment?
* For all unassigned tasks in this project, recommend the best users based on job role match and daily availability.
* Recommend users for the tasks 'QA testing for website launch' and 'Content review', prioritizing users whose job roles match and who are not over-allocated today.

-->

### Inhalte und Genehmigungen

CX Coworker kann Sie bei der Verwaltung von Dokumenten- und Asset-Genehmigungen in Workfront unterstützen.

Beachten Sie beim Arbeiten mit Dokument- und Asset-Genehmigungen Folgendes:

* Inhaltsgenehmigungen müssen für Ihr Unternehmen aktiviert werden, bevor Sie diese Funktion in Coworker verwenden können.
* KI kann im Namen von Menschen weder genehmigen noch ablehnen. Entscheidungen werden von Benutzern getroffen, mit Ausnahme des Workfront AI Reviewers.

  Weitere Informationen zum Workfront AI Reviewer finden Sie unter [Erste Schritte mit dem Workfront AI Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).
* Diese Funktion ist in Workfront vorhanden und kann nicht für die Interaktion mit externen Tools oder Dokumentanbietern verwendet werden.
* Für ein optimales Erlebnis sollten Sie diese Funktion mit der Erfahrung „Einheitliche Genehmigungen“ verwenden.

  Weitere Informationen zu einheitlichen Genehmigungen finden Sie unter [Übersicht über einheitliche Genehmigungen](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

Siehe Beispiel-Eingabeaufforderungen für Dokument- und Asset-Genehmigungen in den folgenden Bereichen:

* [Genehmigungsteilnehmer hinzufügen oder entfernen](#add-or-remove-approval-participants)
* [Erinnern von Stakeholdern an ein einzelnes Asset, das auf Überprüfung wartet](#remind-stakeholders-of-a-single-asset-waiting-for-review)
* [Hinzufügen, Aktualisieren oder Anwenden von Genehmigungsvorlagen für ein einzelnes Asset](#add-update-or-apply-approval-templates-for-a-single-asset)

#### Genehmigungsteilnehmer hinzufügen oder entfernen

* Fügen Sie Sarah Chen und Miguel Alvarez als genehmigende Personen für das aktuelle Dokument hinzu.
* Entfernen Jennifer Otto von dieser Genehmigung.
* Alle entfernen, die keine Genehmigungsentscheidung getroffen haben.
* Fügen Sie der Datei „spring-campaign.pdf“ einen neuen Schritt namens „Endprüfung“ hinzu.
* Fügen Sie Mark und Sarah als genehmigende Personen und Phil als Prüferin bzw. Prüfer auf der zweiten Stufe der Winterkampagne hinzu.pdf
* Geben Sie für die Winterkampagne.pdf der ersten Phase eine Frist für heute um 17 Uhr und für die abschließende Überprüfung eine Frist für morgen um 17 Uhr
* Fügen Sie der Datei fall-campaign.png eine abschließende Prüfphase mit einer Frist bis Donnerstag um 17 Uhr hinzu und beziehen Sie Jim und Pam als genehmigende Personen sowie Oscar als Prüfer mit ein
* Fügen Sie Mark Jones in der Datei fall-campaign.png zur ersten und letzten Phase als Prüferin bzw. Prüfer hinzu.
* Lassen Sie uns eine mehrstufige Genehmigung für die fall-campaign.png mit 3 Phasen, 1 Design 2 Copywriting und 3 Legal erstellen. Für jede Phase brauche ich nur eine Entscheidung. Mike, Sally, Jane zu Design hinzufügen, Chris, Richard, Mark zu Copywriting und Phil, Tom und Sarah zu Legal.

#### Erinnern von Stakeholdern an ein einzelnes Asset, das auf Überprüfung wartet

* Erinnerung an genehmigende Personen senden, die nicht auf das Asset „Frühlingsvideo zu Kampagnen“ geantwortet haben.
* Erinnern Sie alle Personen, die dieses Asset nicht genehmigt haben, an „Frühlingskampagnenvideo“.
* Wer hat noch keine Entscheidung über das Asset „Markenrichtlinien PDF&quot; getroffen? Erinnern Sie sie.

#### Hinzufügen, Aktualisieren oder Anwenden von Genehmigungsvorlagen für ein einzelnes Asset

* Wenden Sie die Validierungsvorlage „Marketing-Launch“ auf ein Asset mit dem Namen „Frühling-Kampagnen-Video“ an.
* Erstellen Sie eine neue Genehmigungsvorlage mit drei Schritten: Überprüfung durch Creative, rechtliche und endgültige Genehmigung.
* Fügen Sie Julia Santos und Shane Baker zu Stufe 1 hinzu.
* Bearbeiten Sie die Vorlage „Produkteinführung“, um Elizabeth Peterson zur letzten Genehmigungsphase hinzuzufügen.
* Erstellen Sie eine Vorlage namens „Dringende Überprüfung“ mit einem Schritt und weisen Sie sie Olivia Kim zu.
* Aktualisieren Sie die Vorlage &#39;Creative Review&#39;, indem Sie Rick Kuvec entfernen und Karen Sterling zu Schritt 2 hinzufügen.


## CX-Mitarbeiter in der Workfront-Planung

### Arbeiten mit Planungsdatensätzen

* [Erstellen, Löschen, Duplizieren oder Wiederherstellen von Datensätzen](#create-delete-duplicate-or-restore-records)
* [Datensätze mit anderen Datensätzen verknüpfen](#link-records-to-other-records)
* [Bearbeiten, Aktualisieren oder Anhängen eines Felds an einen Datensatz](#edit-update-or-append-a-field-to-a-record)
* [Zugriff auf den Änderungsverlauf des Datensatzes](#access-record-change-history)

#### Erstellen, Löschen, Duplizieren oder Wiederherstellen von Datensätzen

* Erstellen Sie einen neuen Kampagnendatensatz mit dem Namen Summer Sale 2026
* Neuen Produkteintrag mit Namen Widget Pro und Preis $299 hinzufügen
* Können Sie einen neuen Lead-Eintrag für John Smith erstellen?
* Löschen Sie den Kampagnendatensatz mit dem Namen „Alte Promotion“.
* Entfernen Sie den soeben erstellten Testdatensatz.
* Kann die Datensatz-ID Rc123abc456 gelöscht werden?
* Duplizieren des Kampagnendatensatzes für Q1
* Können Sie diese Kampagne kopieren, um eine neue zu erstellen?
* Erstellen einer Kopie der Kampagne zur Weihnachtsaktion
* Die versehentlich gelöschte Kampagne wiederherstellen
* Können Sie den gelöschten Projektdatensatz wiederherstellen?
* Wenn ich einen Datensatz versehentlich gelöscht habe, können Sie ihn wiederherstellen?

#### Datensätze mit anderen Datensätzen verknüpfen

* Verknüpfen des Datensatzes der Sommerkampagne mit der Initiative für das zweite Quartal
* Können Sie dieses Produkt mit den zugehörigen Marketing-Kampagnen verbinden?
* Ich muss diese drei Leads mit dem Datensatz des Unternehmenskontos verknüpfen

#### Bearbeiten, Aktualisieren oder Anhängen eines Felds an einen Datensatz

* Budgetfeld in der Sommerkampagne auf 75.000 $ aktualisieren
* Kann der Status dieses Projektdatensatzes in „Abgeschlossen“ geändert werden?
* John Doe zum Feld „Team-Mitglieder“ für diese Initiative hinzufügen

#### Zugriff auf den Änderungsverlauf des Datensatzes

* Änderungsverlauf für den Datensatz der Sommerkampagne anzeigen
* Können Sie anzeigen, wer dieses Projekt geändert hat und was sie geändert haben?
* Ich muss alle Aktualisierungen sehen, die in der letzten Woche an diesem Datensatz vorgenommen wurden

### Verwenden von System Designer in Workfront Planning

* [Erstellen und Konfigurieren von Arbeitsbereichen](#create-and-configure-workspaces)
* [Datensatztypen definieren](#define-record-types)
* [Designfelder und Formelfelder](#design-fields-and-formula-fields)
* [Erstellen benutzerdefinierter Ansichten](#build-custom-views)


#### Erstellen und Konfigurieren von Arbeitsbereichen

* Erstellen Sie einen neuen Planungsarbeitsbereich mit dem Namen Marketing-Kampagnen 2026
* Aktualisieren Sie meinen Arbeitsbereich Produktplanung , um die Farbe in Blau zu ändern und eine Beschreibung hinzuzufügen
* Alle Planungsarbeitsplätze anzeigen, auf die ich Zugriff habe

#### Datensatztypen definieren

* Einen neuen Datensatztyp mit dem Namen Kampagnen in meinem Arbeitsbereich Planung erstellen
* Aktualisieren Sie den Datensatztyp Initiativen , um das Symbol und die Beschreibung zu ändern
* Alle Datensatztypen in meinem Arbeitsbereich für Marketing-Planung anzeigen

#### Designfelder und Formelfelder

* Ein Budgetfeld zum Datensatztyp „Meine Planungskampagnen“ mit dem Währungstyp hinzufügen
* Erstellen Sie ein Formelfeld in Planning, das die verbleibenden Tage bis zum Enddatum der Kampagne berechnet
* Aktualisieren Sie das Feld Priorität in Mein Arbeitsbereich Planung , um weitere Dropdown-Optionen hinzuzufügen

#### Erstellen benutzerdefinierter Ansichten

* Erstellen Sie eine Zeitleisten -Ansicht in Planning, um meinen Kampagnenkalender nach Start- und Enddatum anzuzeigen
* Meinen Planungsinitiativen eine neue Tabellenansicht hinzufügen, die nur den aktiven Status filtert
* Duplizieren Sie meine aktiven Planning-Kampagnen und ändern Sie die Sortierung.
