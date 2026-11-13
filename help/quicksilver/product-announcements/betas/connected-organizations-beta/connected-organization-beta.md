---
product-area: betas
title: Beta-Programm für Connected Organisations-Funktionen
description:
author: Alina
feature: Product Announcements
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: 8f8f4e7962bfde525470842caecd49f03b758b29
workflow-type: tm+mt
source-wordcount: '2241'
ht-degree: 1%
---
# Beta-Programm zur Funktion für verbundene Organisationen

>[!IMPORTANT]
>
>Die Funktion „Connected Organizations“ befindet sich derzeit in der geschlossenen Beta-Phase und steht einer kleinen Anzahl von Kunden offen.
>
>Die Beta-Version läuft bis Ende 2026.
>
>Wenden Sie sich bei Fragen an Ihren Adobe Beta-Programmmanager.

Die Funktion „Connected Organisations“ ermöglicht es einem Unternehmen und seinen Partnern, gemeinsam an der Arbeit zu arbeiten, wenn beide Unternehmen Adobe Workfront erworben haben.

Beispielsweise kann ein Kundenunternehmen eine Anfrage an sein Anbieterunternehmen senden, damit Arbeiten erledigt werden.

Jedes Unternehmen kann weiterhin in seiner eigenen Workfront-Instanz mit eigenen Benutzenden, Berechtigungen und Workflows arbeiten.

Arbeitsobjekte werden zwischen den beiden Instanzen gespiegelt, und nur die Daten, die beide Seiten gemeinsam nutzen, werden synchronisiert.

Das Ergebnis ist eine freigegebene Ansicht von Anfragen, Status und Entscheidungen ohne zusätzliche Gastanmeldungen, doppelte Lizenzen oder lange E-Mail-Threads.

## Überblick über den heutigen Workflow für mehrere Organisationen

Wenn zwei Unternehmen beide in Workfront investierten, sollten sie zusammenarbeiten können, ohne dass eines zweimal zahlt oder in das System des anderen wechselt.

Wenn die beiden Unternehmen heutzutage in zwei separaten Systemen arbeiten, kann ihre Zusammenarbeit einige der folgenden Workflows umfassen:

* Anfragen und Briefings durchlaufen E-Mail-Threads, denen schwer zu folgen ist.

* Übergaben erfolgen manuell und sind kaum überprüfbar.

* Die Arbeit im System eines anderen Unternehmens bedeutet Gastanmeldungen, zusätzliche Lizenzen oder beides.

* Mehrere Kopien von Dateien zirkulieren, und niemand ist sicher, welche die Quelle der Wahrheit ist.

* Der Status ist schwer einzuhalten, sodass Account Manager Zeit mit dem Erstellen von Decks und dem Planen von Aktualisierungsbesprechungen verbringen.

## Überblick über die Lösung für vernetzte Organisationen

Wenn Sie die Funktion „Verbundene Organisation“ verwenden, arbeiten die beiden Unternehmen weiterhin in zwei separaten Systemen. Ihre Zusammenarbeit umfasst einige der folgenden Workflows:

* Keine Organisation greift auf ein Objekt in der Instanz der anderen zu.
* Ein Objekt wie eine Anfrage der Client-Organisation wird dupliziert und in der Instanz des Anbieters veröffentlicht.
* Nur die für die Synchronisierung konfigurierten Metadaten werden zwischen den beiden Kopien auf dem neuesten Stand gehalten.
* Jedes Unternehmen verwaltet über dieses Objekt hinaus seine eigenen Benutzer, Berechtigungen und Workflows.

Das Leitprinzip ist, das Minimum für die Erledigung der Arbeit zu teilen und alles andere vertraulich zu behandeln.

<table>
<tbody>
<tr class="odd">
<td><strong>Freigegebene Elemente</strong></td>
<td><strong>Was bleibt privat?</strong></td>
</tr>
<tr class="even">
<td><ul>
<li><p>Briefs und Anfragedetails</p></li>
<li><p>Vereinbarte Fristen und Meilensteine</p></li>
<li><p>Kommentare prüfen</p></li>
<li><p>Genehmigungsentscheidungen</p></li>
<li><p>Endgültige genehmigte Assets</p></li>
</ul></td>
<td><ul>
<li><p>Beziehungen zu anderen Kunden oder anderen Agenturen</p></li>
<li><p>Finanzen, Tarife und was dem Kunden in Rechnung gestellt wird</p></li>
<li><p>Ressourcenplanung und -kapazität</p></li>
<li><p>Interne Projektstruktur, Aufgaben und Felder, die nicht für die Freigabe ausgewählt wurden</p></li>
</ul></td>
</tr>
</tbody>
</table>

## In der Beta-Version verfügbare Funktionen

Die erste Phase des Beta-Programms ermöglicht es Ihnen, die beiden Instanzen zu verbinden und Ihre Arbeit zu starten.

|                                   |                                                                                                                                                                                                                                                                                                                                       |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Funktion** | **Was tut sie** |
| **Verbundene Organisationen** | Verknüpft die beiden Workfront-Instanzen zwischen den beiden Organisationen. Während der Beta-Phase konfiguriert Adobe die Verbindung. Ein Self-Service-Setup befindet sich derzeit in der Entwicklung. |
| **Anfrageformulare** | Die Client-Firma erstellt ein Anfrageformular, veröffentlicht es und gibt es über die Freigabeeinstellungen des Formulars für eine Anbieter-Firma frei. |
| **KI-gestützter Anforderungseingang** | Der Auftraggeber des Clients kann die Funktion zum Ausfüllen eines KI-Formulars verwenden, um eine Eingabeaufforderung einzugeben und Dateien anzuhängen, anstatt ein langes Formular auszufüllen. Das System ordnet diesen Inhalt den Formularfeldern zu und zeigt die Zuordnung zur Überprüfung an. Der Antragsteller akzeptiert das Ergebnis und übermittelt das Formular. |
| **Gespiegelte Anfragen** | Die gesendete Anfrage wird im Bereich Anfragen des Anbieterunternehmens als schreibgeschützte Kopie angezeigt, einschließlich benutzerdefinierter Feldwerte. |
| **Konvertierung von Anfrage zu Projekt** | Der Dienstleister wandelt die Anfrage in ein Projekt um und wählt das Portfolio, das Programm und die Vorlage aus, um die Arbeit zu starten. Das neue -Objekt in der Instanz des Anbieters ist mit der ursprünglichen Anfrage des Clients verknüpft. Die Details der eigentlichen Arbeit auf Anbieterseite sind für das anfragende Unternehmen nicht sichtbar. |
| **Zwei-Wege-Kommentare** | Kommentare zum Antrag sind auf beiden Seiten sichtbar und kommen fast sofort an, sodass beide Parteien an einem Ort auf eine Einigung hinarbeiten können. |
| **Anfordern der Annahme** | Sobald sich beide Seiten einig sind, akzeptiert der Provider die Anfrage und der Client kann sehen, dass sie akzeptiert wurde. |
| **Von KI entworfene Statusaktualisierungen** | Wenn ein Anfragender in einem Kommentar nach dem Status fragt, kann der Anbieter mithilfe von KI-Befehlen schnell und konsistent einen Antwortentwurf erstellen. <br> Der Entwurf enthält Informationen aus den mit der Anfrage verbundenen Objekten, z. B. geplantes Abschlussdatum, Bedingung und Stunden, die für die geplanten Stunden protokolliert wurden. <br> Es handelt sich dabei um eine Zusammenfassung der wichtigsten Informationen, nicht um einen Export nach Feld. Eine Person prüft und bearbeitet sie, bevor sie eine Antwort an den Client sendet. |

## Beta-Version verwenden

Sprechen Sie mit Ihrem Adobe Beta-Programm-Manager, um an der Beta-Version teilzunehmen.

### Was wir von den Teilnehmern verlangen

* Nehmen Sie an einem wöchentlichen Feedback-Aufruf teil.

* Nehmen Sie sich etwa eine Stunde pro Woche Zeit, um selbst praktische Tests durchzuführen. Live-Arbeitssitzungen zum Anruf sind eine Option.

* Bringen Sie, soweit möglich, die Perspektiven beider Partner zu den Treffen mit.

* Identifizieren Sie die zu verbindenden Workfront-Umgebungen und stellen Sie Administratorkonten für eine geringe Anzahl von Adobe-Technikern bereit, damit diese die Verbindung validieren können.

### Was wir lernen wollen

* Ist das Spiegeln eines Objekts und das Synchronisieren nur ausgewählter Daten das richtige Freigabemodell? Ist es flexibel genug für jede Seite?

* Ist die Phasenfolge richtig oder sollte eine spätere Funktion früher kommen?

* Welche Touchpoints fehlen bei der Zusammenarbeit?

* Wie sollten Feldbenennung und -zuordnung zwischen den beiden Instanzen funktionieren?

  Heute gehören das Formular und die Anfrage dem Client. Der Anbieter sieht sie schreibgeschützt mit den Feldnamen des Clients.

* Was benötigt die IT, um eine Verbindung zu genehmigen und zu verwalten?

## End-to-End-Workflow

In diesem Abschnitt wird der Arbeitsablauf für zwei an dieser Integration beteiligten Parteien beschrieben.

Als Beispiele verwenden wir einen Client- und Provider-Workflow.

Der Workflow umfasst die folgenden Schritte:

1. [Erstellen einer Instanzverbindung](#1-create-an-instance-connection)
1. [Verbindung quittieren](#2-acknowledge-the-connection)
1. [Freigeben eines Anfrageformulars für die verbundene Organisation](#3-share-a-request-form-with-the-connected-organization)
1. [Senden Sie eine Anfrage](#4-submit-a-request)
1. [Überprüfen der Anfrage und Erstellen eines Projekts](#5-review-the-request-and-create-a-project)
1. [Mitwirken am unternehmensübergreifenden Gespräch](#6-collaborate-in-the-cross-company-conversation)

### Voraussetzungen

* Sie müssen Systemadministrator sein und in beiden Fällen uneingeschränkten Zugriff auf den Bereich **Setup** haben.
* Die anfragende Instanz benötigt die eindeutige Kunden **GUID** der empfangenden Instanz.
* Das Formular, das Sie freigeben möchten, muss veröffentlicht werden.

### &#x200B;1. Erstellen einer Instanzverbindung

Richten Sie in der anfordernden Instanz (dem Client) Folgendes ein:

1. Melden Sie sich bei der Client-Umgebung an und gehen Sie zu **Setup** > **Instanzverbindungen**. Die Seite listet alle Verbindungen auf und ist leer, wenn noch keine vorhanden sind.
1. Klicken Sie **Verbindung erstellen**.
1. Fügen Sie im Feld **Verbindung erstellen** die **Empfangsinstanz-GUID“**. Dies ist ein Pflichtfeld.
1. (Optional) Legen Sie ein **Ablaufdatum** fest. Die Verbindung funktioniert nach diesem Datum nicht mehr.
1. Klicken Sie **Verbindung erstellen**.

   Die neue Verbindung wird in der Liste der Verbindungen mit dem Status **Ausstehend** angezeigt.
1. Wählen Sie die neue Verbindung aus, um deren Details anzuzeigen.

   >[!TIP]
   >
   >Eine ausstehende Verbindung hat keine Freigabe. Die empfangende Instanz muss sie zuerst bestätigen.


### &#x200B;2. Verbindung quittieren

Richten Sie in der empfangenden Instanz (dem Anbieter) Folgendes ein:

1. Melden Sie sich bei der Instanz des Anbieters an und gehen Sie zu **Hauptmenü** > **Setup** > **Verbindungen**.
1. Klicken Sie auf den Namen, um die Verbindung von der empfangenden Instanz aus zu öffnen. In einem Banner wird die folgende Meldung angezeigt: **Eine Instanz möchte eine Verbindung zu Ihrer Instanz herstellen. Wählen Sie mindestens einen geeigneten Empfänger aus und bestätigen Sie dann die Verbindung. Es wird nichts freigegeben, bis Sie dies tun.**
1. Öffnen **unter &quot;** Empfänger“ die Liste **Suchgruppen und Benutzer** und wählen Sie aus, wer Arbeit von der anfordernden Instanz erhalten kann. Sie können Gruppen und einzelne Benutzer auswählen. <!--asking Anna K if this should be teams and users, instead of groups; it's groups in the UI-->
1. Klicken Sie **Bestätigen**, um die Verbindung zu akzeptieren, oder klicken Sie auf eine der folgenden Optionen:

   * **Ablehnen**, um die Verbindung abzulehnen.
   * **Schließen**, um sie ausstehend zu lassen.

   Die Meldung „Changes saved“ (Änderungen gespeichert) wird angezeigt, und der Verbindungsstatus ändert sich in **Active**. Die Liste zeigt jetzt die zulässigen Empfänger, das Erstellungsdatum und das Ablaufdatum an.

   >[!TIP]
   >
   >**Bestätigen** bleibt abgeblendet, bis Sie mindestens einen geeigneten Empfänger auswählen.

### &#x200B;3. Freigeben eines Anfrageformulars von der anfragenden Organisation

In der Workfront-Instanz des Clients:

1. Wechseln Sie **Hauptmenü** > **Anfragen** und klicken Sie auf **Formulare anfordern**.
1. Öffnen Sie das veröffentlichte Formular, das Sie freigeben möchten.
1. Klicken Sie auf **Freigabe**.

   Beachten Sie die folgenden Registerkarten im Feld **Freigeben**:

   * **Interne Freigabe**
   * **Öffentliche Freigabe**
   * **Verbundene Organisationen**
1. Öffnen Sie die **Verbundene Organisationen** .
1. Wählen **Feld** Organisation“ die Instanz des verbundenen Anbieters aus.
1. Wählen Sie im Feld **Benutzer und Gruppen** aus, wer in dieser Organisation das Formular verwenden kann. Benutzer und Gruppen hinzufügen.
1. Klicken Sie auf **Speichern**.

Eine **Ihre Änderungen wurden erfolgreich gespeichert** Meldung bestätigt die Freigabe. <!--need to submit a UI text change - remove "successfully"-->

### &#x200B;4. Senden Sie eine Anfrage

Senden Sie als Benutzer in der Client-Instanz eine Anfrage wie folgt:

1. Melden Sie sich bei der Workfront-Instanz des Clients an und gehen Sie zu **Hauptmenü** > **Anfragen**.

   Auf **Seite „Neue Anfrage senden** werden die neuesten Formulare aufgelistet, einschließlich des soeben freigegebenen.

   Oben wird ein Hinweis angezeigt **Firmenübergreifende Anforderung: Mit diesem Formular gesendete Anfragen sind für die verbundene Organisation sichtbar.**
1. Füllen Sie das Formular manuell aus oder verwenden Sie **Formular ausfüllen**, damit KI es für Sie erledigt.
1. (Optional) Gehen Sie wie folgt vor, um das Formular „Ausfüllen“ zu verwenden:

   1. Klicken Sie **Formular ausfüllen**.
   1. Beschreiben Sie Ihre Anfrage, fügen Sie eine zugehörige E-Mail ein oder klicken Sie auf **Dateien anhängen**, um eine Datei hochzuladen. AI findet die relevanten Details und wendet sie auf das Formular an.
   1. Klicken Sie **Auf Formular anwenden**. In einer Fortschrittsleiste wird **Formular ausfüllen** angezeigt, während Feldwerte generiert werden.
   1. Um den KI-Schritt zu überspringen, klicken Sie auf **Überspringen**.
1. Überprüfen Sie die generierten Werte und bearbeiten Sie alle Elemente, die geändert werden müssen.
1. Klicken Sie **Senden** um die Anfrage zu senden.

   Eine **Anfrage erfolgreich gesendet** wird mit dem Link **Ihre Anfrage anzeigen** angezeigt.

   Die neue Anfrage wird der Anfrageliste mit dem Formularnamen und dem Status **Neu** sowohl in der Client- als auch in der Anbieterinstanz hinzugefügt.

   >[!TIP]
   >
   >KI-Antworten können ungenau sein. Überprüfen Sie die ausgefüllten Werte immer, bevor Sie den Vorgang starten.

   Die erstellte Anfrage ist in der Instanz des Anbieters schreibgeschützt.

### &#x200B;5. Überprüfen der Anfrage und Erstellen eines Projekts

1. Melden Sie sich bei der Workfront-Instanz des Anbieters an und gehen Sie zu **Hauptmenü** > **Anfragen**.

Die eingehende Anfrage wird in der Liste angezeigt.

Der **Typ** der Anfrage wird als &quot;**: &lt; Name der Client-Instanz >** markiert, wodurch er als von der verbundenen Organisation stammend markiert wird.

1. Öffnen Sie die Anfrage. Neben dem Titel wird ein **Freigegeben für: &lt; Name der Client-Instanz >**-Badge angezeigt, und das Bedienfeld „Kommentare“ zeigt die folgende **Firmenübergreifende Konversation** Hinweis: **Diese Diskussion ist für &lt; Name der Organisation des Kunden > sichtbar.**
1. Überprüfen Sie die Anfrageinformationen und die Formularantworten.
1. Klicken Sie auf das **Mehr**-Menü rechts neben dem Anfragenamen und dann auf **Objekt erstellen**.
1. Aktualisieren Sie **Dialogfeld &quot;** erstellen“ die folgenden Felder:
   * **Aktion**: Wählen Sie eine Aktion aus dem Menü aus. Beispiel: **Ein einzelnes Projekt erstellen**
   * **Projektvorlage**: Eine verfügbare Vorlage auswählen.
   * **Projektinhaber**: Fügen Sie einen Projektinhaber hinzu.
   * **Modul**: Wählen Sie ein Produkt aus, in dem das Objekt angezeigt werden soll. Wenn Sie **Workflow** auswählen, wird ein Projekt in der Instanz des Anbieters von Workfront erstellt.
   * **Benutzerdefinierte Formulare**: Fügen Sie bei Bedarf benutzerdefinierte Formulare an.
   * **Portfolio** und **Program**: Fügen Sie Portfolios oder Programme für das neue Projekt hinzu.
1. Klicken Sie auf **Erstellen**.

   Die Anfrage in der Instanz des Anbieters ist jetzt mit dem neuen Projekt verknüpft, und der Status der Anfrage ändert sich in **In Bearbeitung**, wenn das Projekt den Status „Aktuell“ hat. Die anfragende Instanz des Clients sieht die Statusänderung in der eigenen Kopie der Anfrage.

### &#x200B;6. Mitwirken am unternehmensübergreifenden Gespräch

Benutzer in beiden Organisationen können zu ihren jeweiligen Anfragen Stellung nehmen. Das Banner **Firmenübergreifende Konversation** erinnert daran, dass alles, was hier geschrieben ist, für die andere Organisation sichtbar ist.

Führen Sie einen der folgenden Schritte aus:

1. So fordern Sie eine Aktualisierung von der Client-Instanz an:

   1. Öffnen Sie die Anfrage und navigieren Sie zum Bedienfeld **Kommentare**.
   1. Klicken Sie auf **Neuer Kommentar**, geben Sie Ihre Nachricht ein und klicken Sie auf **Senden**.

1. So aktualisieren Sie die Anfrage aus der Instanz des Anbieters:

   1. Öffnen Sie die Anfrage. Der neue Kommentar wird mit einer Beschriftung **Neu** hervorgehoben.
   1. Klicken Sie **Antwort** schreiben Sie die Antwort und klicken Sie auf **Senden**.

1. Folgenachricht für die Client-Instanz:

   1. Öffnen Sie die Anfrage. Die Antwort des Anbieters erscheint unter dem ursprünglichen Kommentar.
   1. Klicken Sie auf **Gefällt mir**, um es zu bestätigen, oder **Antwort hinzufügen**, um die Diskussion fortzusetzen.




<!--
### Client's workflow

As a requestor in the client's organization, you can do the following:  

1. Create or ask an administrator to create a request form, publish it, and share it with the connected provider's organization.

2. Open the published form from the Requests area, enter a prompt, and attach any files.

3. Review how the content maps to the form fields, accept, and submit.

### Provider's workflow

As a work manager in the provider's organization, do the following: 

1. Receive the request in your Requests area as a read-only copy.

2. Discuss the request through comments until both sides are aligned, then accept it.

3. Convert the request into a project, choosing the portfolio, program, and template, if needed.

4. Choose which project fields are mirrored back to the client's request. 

5. Answer status questions in comments, or generate a draft status update, review it, and publish to your request. It will also display on the client's original request. 

    From that point on, the request on the provider's side acts as a replica of the client's original request, so comments and agreed-upon data stay in sync.
-->

## Sicherheit und Governance

Der Schutz der Daten jedes Unternehmens ist eine zentrale Anforderung an das Design.

Eine der Grundlagen, die wir für die Beta-Version festlegen möchten, besteht darin, wie einfach IT- und Sicherheits-Teams eine Verbindung zwischen Instanzen genehmigen und verwalten können.

Der Workflow für verbundene Organisationen bietet folgende Vorteile:

* **Kein instanzenübergreifender Zugriff**: In Ihrer Instanz sind keine Benutzer aus der Partnerorganisation erforderlich, sodass keine Gastanmeldungen und keine zusätzlichen Lizenzen vorhanden sind.

* **Mindest erforderliche Freigabe**: Es werden nur die für die Synchronisierung konfigurierten Daten freigegeben. Alles andere verbleibt in der ursprünglichen Instanz.

* **Unabhängige Kontrollen**: Jede Organisation verfügt über eigene Benutzer, Berechtigungen und Workflows.

* **Umfang auf Teamebene**: Anfragen richten sich nur an die Agenturteams, die mithilfe der bestehenden Zugriffssteuerungen von Workfront für die Zusammenarbeit mit diesem Client eingerichtet wurden.

## Roadmap-Ausblick

In den folgenden Phasen wird unser aktueller Entwicklungs- und Veröffentlichungsplan beschrieben. Die Sequenzierung kann sich je nachdem, was wir während der Beta-Phase lernen, ändern. Spätere Phasen sind keine Verpflichtungen.

<table>
<tbody>
<tr class="odd">
<td><strong>Phase</strong></td>
<td><strong>Fokus und geplante Funktionen</strong></td>
<td><strong>Status</strong></td>
</tr>
<tr class="even">
<td><strong>Phase 1</strong></td>
<td>Verbinden von Instanzen und Beginn der Arbeit: Anfrageformulare, KI-gestützte Erfassung, gespiegelte Anfragen, Projektkonvertierung, Kommentare und Statuserstellung.</td>
<td>In Beta</td>
</tr>
<tr class="odd">
<td><strong>Phase 2</strong></td>
<td><ul>
<li><p>Überprüfung und Genehmigung mithilfe von Frame und dem einheitlichen Prüf- und Genehmigungserlebnis</p></li>
<li><p>Ausstehende Überprüfungen werden in Workfront oder Frame angezeigt, wo immer der Stakeholder arbeitet</p></li>
<li><p>Anmerkungen bleiben an die Arbeitsdatei gebunden, sodass Kreativ-Teams Feedback an einer Stelle sehen</p></li>
</ul></td>
<td>Geplant</td>
</tr>
<tr class="even">
<td><strong>Phase 3</strong></td>
<td><ul>
<li><p>Aufgabenbasierte Arbeitszuweisung zusätzlich zu Anfragen</p></li>
<li><p>Mehr automatisierter Status, informiert durch freigegebene oder nicht freigegebene Felder</p></li>
<li><p>Ein neuer Objekttyp mit Arbeitsergebnissen, bei dem die Metadaten während des Briefings definiert werden und vom endgültig genehmigten Asset übernommen werden</p></li>
<li><p>Direkte Bereitstellung genehmigter endgültiger Assets in der AEM der Marke, wodurch die manuelle Eingabe von Metadaten reduziert wird</p></li>
</ul></td>
<td>Geplant</td>
</tr>
<tr class="odd">
<td><strong>Phase 4</strong></td>
<td><ul>
<li><p>Gemeinsamer Kontext zwischen Partnern</p></li>
<li><p>Verwendung von Adobe Brand Intelligence-<!--by the agency--> vor der Überprüfung, wobei der Zugriff vom Team gesteuert wird</p></li>
<li><p>Kontextbezogene Funktionen wie Schätzung</p></li>
</ul></td>
<td>Langfristig</td>
</tr>
</tbody>
</table>






<!--

Original pdf from team:

**ADOBE WORKFRONT | BETA PROGRAM**

**Agency Brand Connectors**

Product overview for beta participants

# **Overview**

Agency Brand Connectors lets a brand and its agency collaborate on work when both organizations run Adobe Workfront. Each side keeps working in its own Workfront instance, with its own users, permissions, and workflows. Work objects are mirrored between the two instances, and only the data both sides agree to share is synchronized.

The result is a shared view of requests, status, and decisions without guest logins, duplicate licenses, or long email threads.

# **The challenge this addresses**

When a brand and an agency are both invested in Workfront, they should be able to work together without either one paying twice or moving into the other's system. Today the collaboration usually looks like this:

  - Requests and briefs travel through email threads that are hard to follow.

  - Handoffs are manual, with little auditability.

  - Working inside a partner's system means guest logins, extra licenses, or both.

  - Multiple copies of files circulate, and no one is sure which is the source of truth.

  - Status is hard to see, so producers and account managers spend time building decks and scheduling update meetings.

# **How it works: the sharing model**

Neither organization accesses an object in the other's instance. Instead, an object such as a request is duplicated and published into the partner's instance, and only the metadata configured for sync is kept up to date between the two copies. Each side manages its own users, permissions, and workflows downstream of that object.

The guiding principle is to share the minimum needed to get the work done, and to keep everything else confidential.

<table>
<tbody>
<tr class="odd">
<td><strong>What is shared</strong></td>
<td><strong>What stays private</strong></td>
</tr>
<tr class="even">
<td><ul>
<li><p>Briefs and request details</p></li>
<li><p>Agreed deadlines and milestones</p></li>
<li><p>Review comments</p></li>
<li><p>Approval decisions</p></li>
<li><p>Final approved assets</p></li>
</ul></td>
<td><ul>
<li><p>Relationships with other clients or other agencies</p></li>
<li><p>Financials, rates, and what is charged to the client</p></li>
<li><p>Resource planning and capacity</p></li>
<li><p>Internal project structure, tasks, and any fields not selected for sharing</p></li>
</ul></td>
</tr>
</tbody>
</table>

# **Features available in the beta**

The first phase of the beta covers connecting two instances and kicking off work.

|                                   |                                                                                                                                                                                                                                                                                                                                       |
| --------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Feature**                       | **What it does**                                                                                                                                                                                                                                                                                                                      |
| **Connected organizations**       | Links a brand instance and an agency instance. During the beta, Adobe configures the connection. A self-serve setup is being worked on.                                                                                                                                                                                               |
| **Request forms**                 | The brand creates a request form, publishes it, and shares it with a connected organization from the form's Share settings.                                                                                                                                                                                                           |
| **AI-assisted request intake**    | The requester types a prompt and attaches files instead of filling out a long form. The system maps that content to the form fields and shows the mapping for review. The requester accepts the result and submits. This uses Workfront's existing form-filling technology.                                                           |
| **Mirrored requests**             | The submitted request appears in the agency's request area as a read-only copy, including custom field values.                                                                                                                                                                                                                        |
| **Request-to-project conversion** | The agency converts the request into a project and selects the portfolio, program, and template. The new object is linked back to the request. Downstream work on the agency side is not visible to the brand.                                                                                                                        |
| **Two-way comments**              | Comments on the request are visible on both sides and arrive almost immediately, so both parties can work toward agreement in one place.                                                                                                                                                                                              |
| **Request acceptance**            | Once both sides agree, the agency accepts the request and the brand sees that it has been accepted.                                                                                                                                                                                                                                   |
| **AI-drafted status updates**     | When a brand asks for status in a comment, the agency can use a slash command to generate a draft reply. The draft draws on connected objects, such as planned completion date, condition, and hours logged against hours planned. It is a summary, not a field-by-field export, and a person reviews and edits it before publishing. |

# **End-to-end workflow**

## **Brand side**

1.  Create a request form, publish it, and share it with the connected agency.

2.  Open the published form, enter a prompt, and attach any files.

3.  Review how the content maps to the form fields, accept, and submit.

## **Agency side**

1.  Receive the request in the request area as a read-only copy.

2.  Discuss the request through comments until both sides are aligned, then accept it.

3.  Convert the request into a project, choosing the portfolio, program, and template.

4.  Choose which project data is mirrored back to the brand.

5.  Answer status questions in comments, or generate a draft status update, review it, and publish.

From that point on, the request on the agency side acts as a replica of the request on the brand side, so comments and agreed data stay in step.

# **Security and governance**

Keeping each organization's data protected is a core design requirement, and one of the baselines we want the beta to establish is how easily IT and security teams can approve and administer a connection between instances.

  - **No cross-instance access.** No users from the partner organization are needed in your instance, so there are no guest logins and no additional licenses.

  - **Minimum necessary sharing.** Only the data configured for sync is shared. Everything else stays in the originating instance.

  - **Independent controls.** Each organization keeps its own users, permissions, and workflows.

  - **Team-level scoping.** Requests are intended to reach only the agency teams set up to work on that brand, using existing Workfront access controls.

# **Roadmap**

The phases below describe our current plan. Sequencing may change based on what we learn in the beta, and later phases are not commitments.

<table>
<tbody>
<tr class="odd">
<td><strong>Phase</strong></td>
<td><strong>Focus and planned capabilities</strong></td>
<td><strong>Status</strong></td>
</tr>
<tr class="even">
<td><strong>Phase 1</strong></td>
<td>Connect instances and kick off work: request forms, AI-assisted intake, mirrored requests, project conversion, comments, and status drafting.</td>
<td>In beta</td>
</tr>
<tr class="odd">
<td><strong>Phase 2</strong></td>
<td><ul>
<li><p>Review and approval using Frame and the unified review and approval experience</p></li>
<li><p>Pending reviews appear in Workfront or Frame, wherever the stakeholder works</p></li>
<li><p>Annotations stay tied to the working file so creative teams see feedback in one place</p></li>
</ul></td>
<td>Planned, next</td>
</tr>
<tr class="even">
<td><strong>Phase 3</strong></td>
<td><ul>
<li><p>Task-based work assignment in addition to requests</p></li>
<li><p>More automated status, informed by shared or unshared fields</p></li>
<li><p>A new deliverable object type, with metadata defined during briefing and inherited by the final approved asset</p></li>
<li><p>Direct delivery of approved final assets into the brand's AEM, reducing manual metadata entry</p></li>
</ul></td>
<td>Planned, next</td>
</tr>
<tr class="odd">
<td><strong>Phase 4</strong></td>
<td><ul>
<li><p>Shared context between brand and agency</p></li>
<li><p>Use of Adobe Brand Intelligence by the agency before review, with access controlled by team</p></li>
<li><p>Context-informed capabilities such as estimating</p></li>
</ul></td>
<td>Longer term</td>
</tr>
</tbody>
</table>

# **Participating in the beta**

## **What we ask of participants**

  - Join a weekly feedback call.

  - Set aside about one hour per week for hands-on testing. Live working sessions on the call are an option if time is tight.

  - Bring both the brand and the agency perspective where possible.

  - Identify the Workfront environments to connect, and provision admin accounts for a small number of Adobe engineers so they can validate the connection.

## **What we want to learn**

  - Is mirroring an object and syncing only selected data the right sharing model, and is it flexible enough for each side?

  - Is the phase sequencing right, or should a later capability come sooner?

  - What touchpoints are missing from the collaboration?

  - How should field naming and mapping work between brand and agency instances? Today, the form and request are owned by the brand, and the agency sees them read-only with the brand's field names.

  - What does IT need to approve and administer a connection?

The beta runs through the end of the year. For questions or blockers, contact your Adobe beta program manager.


-->