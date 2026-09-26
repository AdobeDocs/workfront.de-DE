---
product-area: documents
navigation-topic: approvals
title: Erste Schritte mit dem Workfront AI Reviewer
description: Verwenden Sie den Workfront AI Reviewer, um Inhalte während der Überprüfungs- und Genehmigungs-Workflows anhand von Markenrichtlinien zu bewerten.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/5nwapHAbb8wRWqen7a49QfpsAMLPZNEfJUJ2vm4R7SA'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 3%
---
# Erste Schritte mit dem Workfront AI Reviewer

KI-Reviewer ist ein KI-Mitarbeiter - ein Typ von KI-Agent, der zu Ihren Projekten, Aufgaben und Dokumenten hinzugefügt werden kann. KI-Mitwirkende können im Bereich „Setup“ konfiguriert und genau wie Benutzende zugewiesen werden.

In Workfront hilft AI Reviewer, die Inhaltsgeschwindigkeit zu erhöhen und die Markenkonformität während des gesamten Prüfungs- und Genehmigungsprozesses zu verbessern. Sie können Validierungsverantwortliche für KI zu den Validierungsvorlagen hinzufügen oder sie in individuelle Überprüfungs- und Validierungsanfragen einschließen.

## Zugriffsanforderungen

Um KI-Reviewer in Workfront einzurichten, müssen Sie Systemadministrator sein.

Jeder Benutzer kann den KI-Reviewer zu einer Überprüfungs- und Genehmigungsanfrage hinzufügen.

## Anforderungen

* Für Ihre Workfront-Instanz müssen einheitliche Genehmigungen aktiviert sein.
* Ihr Unternehmen muss über GenStudio Foundation verfügen.
  * KI-Reviewer in Workfront bietet die in GenStudio Foundation verfügbaren Funktionen für Asset-Prüfungs- und Genehmigungs-Workflows. Sie müssen nicht direkt auf GenStudio Foundation zugreifen, um Ihre Arbeit abzuschließen. Ihr Zugriff auf GenStudio Foundation-Funktionen über AI Reviewer fällt unter die Bedingungen Ihres Workfront-Vertrags.
* Adobe muss eine unterzeichnete Adobe Gen AI-Vereinbarung in der Datei haben.
Weitere Informationen zur Unterzeichnung des Abkommens finden Sie unter [Unterzeichnung des Adobe Gen AI-Abkommens](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).
* KI-Reviewer ist in Sandbox-Umgebungen nicht verfügbar.


## Unterstützte Dateitypen {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="Nicht unterstützter Dateityp"
>abstract="Dieser KI-Prüfer unterstützt den ausgewählten Dateityp nicht. Laden Sie einen unterstützten Dateityp hoch oder entfernen Sie den KI-Reviewer, um die Anfrage zu senden."

Der KI-Reviewer kann die folgenden Dateitypen überprüfen:

* PNG (.png)
* JPEG (.jpeg, .jpg)
* WEBP (.webp)
* Nicht animierte GIF (.gif)
* PDF (.pdf)
* PPT (.ppt, .pptx)
* DOC (.doc, .docx)

Wenn Sie einen nicht unterstützten Dateityp hochladen, ist die Option „KI-Reviewer“ beim Erstellen eines Genehmigungs-Workflows nicht verfügbar.

## Einrichten von Markenrichtlinien

Der Workfront AI Reviewer verwendet bei der Überprüfung Ihrer Inhalte die Markenrichtlinien. Workfront-Administratoren können im Bereich &quot;Workfront-Setup“ Markenrichtlinien einrichten. In GenStudio Foundation erstellte Marken sind auch in Workfront verfügbar.

Um Markenrichtlinien einzurichten, müssen Systemadministratoren:

1. [Zugriff auf Markenberechtigungen gewähren](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md)
1. [Erstellen und Verwalten von Marken für den KI-Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).


## Erstellen von KI-Prüfern

Sobald mindestens eine Marke eingerichtet ist, können Workfront-Administratoren im Bereich „Setup“ mit der Erstellung von KI-Reviewern beginnen. Sie können mehrere KI-Reviewer erstellen, die sich auf verschiedene Richtlinien konzentrieren:

* **Bild**: Dieser KI-Reviewer überprüft das Asset anhand der Image-Markenrichtlinien, die Sie in Workfront festgelegt haben. [!BADGE Beta]{type=Positive tooltip="Diese Funktion befindet sich derzeit in der Betaphase."}
  * Systemadministratoren müssen die Beta-Vereinbarung unterzeichnen, um diese Funktion zu aktivieren.
* **Markensprache**: Der KI-Reviewer überprüft das Asset anhand der Markensprachrichtlinien, die Sie in Workfront eingerichtet haben.

KI-Reviewer können dann Validierungsvorlagen und individuellen Überprüfungs- und Validierungsanfragen zugewiesen werden.

Weitere Informationen finden Sie unter [Konfigurieren von KI-Mitwirkenden](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Was KI-Reviewer auswertet {#what-ai-reviewer-evaluates}

Der KI-Reviewer bewertet Inhalte je nach Richtlinientyp unterschiedlich: Bild oder Markensprache.

### Bild

KI-Reviewer wertet aus:

* **Komposition**: Fokus, Hintergrund, Zuschnitt, kreatives Framing
* **Beleuchtung &amp; Stimmung**: Einsatz von Licht, Lebendigkeit, Optimismus
* **Diversität und Inklusion**: Vertretung von Menschen (Rasse, Geschlecht, Alter, Fähigkeit)

KI-Reviewer bewertet nicht:

* **Logo-Nutzung**: Platzierung, freier Platz, Größe, korrekte Logo-Version
* **Farbpalette**: Einhaltung der Markenfarben, Vermeidung nicht genehmigter Farben
* **Typografie**: Schriftfamilie, Gewichtung, Abstand, Ausrichtung
* **Illustrationsstil**: Konsistenz mit dem Illustrationsansatz der Marke
* **Barrierefreiheit**: Kontrasttreue, Lesbarkeit

### Markenstimme

KI-Reviewer wertet aus:

* **Ton der Stimme**: Konversativ, klar, menschlich, mit Markenpersönlichkeit abgestimmt
* **Jargon/Formalität**: Vermeidung von Schlagwörtern, Elitismus oder übermäßiger Formalität
* **Messaging**: Ermutigung, Ehrlichkeit, verantwortungsvolle Positionierung (z. B. für KI-Themen)

KI-Reviewer bewertet nicht:

* **Legal/Compliance**: Markennutzung, Haftungsausschlüsse, Lokalisierungsregeln

Eine Anleitung zum Erstellen von Markenrichtlinien, die den Bewertungen durch den KI-Reviewer entsprechen, finden Sie unter [Erstellen und Verwalten von Marken für den KI-Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).

## Hinzufügen von KI-Reviewern zu Prüfungs- und Genehmigungsanfragen

Benutzer können KI-Reviewer zu vorhandenen Genehmigungsvorlagen oder zu individuellen Prüfungs- und Genehmigungsanfragen hinzufügen.

### Genehmigungsvorlagen

Wenn in Ihrem Unternehmen häufig dieselben Personen an Prüfungs- und Genehmigungsanfragen beteiligt sind, können Benutzer von Standardlizenzen im Bereich &quot;Workfront-Setup“ Genehmigungsvorlagen erstellen.

Benutzer können KI-Reviewer zu Genehmigungsvorlagen hinzufügen, um automatisch die Markenkonformität zu überprüfen, wenn eine Vorlage zum Erstellen einer Anfrage verwendet wird.

Nach der Erstellung können Validierungsvorlagen auf Assets im Dokumentbereich eines Projekts, einer Aufgabe oder eines Problems angewendet werden.

Weitere Informationen finden Sie unter [Erstellen einer Workflow-Vorlage für Genehmigungen für Dokumente](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

![Vorlagenliste mit KI-Reviewern](assets/ai-review-templates.png)

### Individuelle Prüfung und Genehmigung

Wenn Benutzer einzelne Prüfungs- und Genehmigungsanfragen erstellen, können sie einen KI-Reviewer in mit anderen Teilnehmern hinzufügen oder sie können eine einzelne Anfrage mit nur dem KI-Reviewer erstellen, um die Markenkonformität zu überprüfen.

Weitere Informationen finden Sie unter [Erstellen eines Dokumentgenehmigungs-Workflows](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).


![KI-Prüfer wurde der individuellen Genehmigungsanfrage hinzugefügt](assets/new-stage.png)

## Anzeigen von KI-Prüfer-Bewertung und -Feedback

Sekunden nach der Übermittlung der Prüfungs- und Genehmigungsanfrage mit einem KI-Reviewer sind die Punktzahl und das Feedback vom KI-Reviewer im Bedienfeld Dokumentzusammenfassung verfügbar - auch wenn andere Teilnehmer noch immer Prüfungs- und Entscheidungsfindungsprozesse durchführen.

Genehmigungsinhaber erhalten außerdem eine E-Mail, die sie darüber informiert, dass eine Überprüfung des Assets abgeschlossen wurde. Klicken Sie in der E **Mail auf Zum Überprüfen wechseln** die Punktzahl und das Feedback in Workfront anzeigen.

Der KI-Reviewer ist nicht als Entscheidungsträger im Überprüfungs- und Genehmigungs-Workflow vorgesehen. Es werden nur eine Bewertung und Empfehlungen bereitgestellt, um das Asset an den festgelegten Markenanforderungen auszurichten.

Wenn das Asset nicht den Markenrichtlinien entspricht, kann der Kreative eine neue Version hochladen und der Genehmigungsinhaber kann eine zweite Überprüfungs- und Genehmigungsanfrage mit dem KI-Reviewer erstellen.

Weitere Informationen zum Anzeigen von Bewertungen und Feedback finden Sie unter [Anzeigen von Bewertungen und Feedback von KI-Prüfern](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md).

