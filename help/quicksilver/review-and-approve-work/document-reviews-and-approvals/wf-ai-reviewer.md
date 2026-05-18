---
product-area: documents
navigation-topic: approvals
title: Erste Schritte mit dem Workfront Content Reviewer
description: Verwenden Sie den Workfront Content Reviewer AI Collaborator , um Inhalte während Prüfungs- und Genehmigungs-Workflows anhand der Markenrichtlinien zu bewerten.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 0f4fd3a7-9578-4fda-b10f-9b4be147f1de
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 9e217d36d5aeb36761a9a433b84e73ac2b7a114b
workflow-type: tm+mt
source-wordcount: '789'
ht-degree: 4%

---

# Erste Schritte mit dem Workfront Content Reviewer

Content Reviewer ist ein KI-Mitwirkender - eine Art von KI-Agent, der zu Ihren Projekten, Aufgaben und Dokumenten hinzugefügt werden kann. KI-Mitwirkende können im Bereich „Setup“ konfiguriert und genau wie Benutzende zugewiesen werden.

In Workfront hilft Content Reviewer, die Inhaltsgeschwindigkeit zu erhöhen und die Markenkonformität während des gesamten Prüfungs- und Genehmigungsprozesses zu verbessern. Sie können Inhaltsvalidierer zu Validierungsvorlagen hinzufügen oder sie in individuelle Überprüfungs- und Validierungsanfragen einschließen.

## Zugriffsanforderungen

Um Content Reviewers in Workfront einzurichten, müssen Sie Systemadministrator sein.

Jeder Benutzer kann den Content Reviewer zu einer Überprüfungs- und Genehmigungsanfrage hinzufügen.

## Anforderungen

* Für Ihre Workfront-Instanz müssen einheitliche Genehmigungen aktiviert sein.
* Ihr Unternehmen muss über GenStudio Foundation verfügen.
   * Content Reviewer in Workfront bietet die in GenStudio Foundation verfügbaren Funktionen für Asset-Prüfungs- und Genehmigungs-Workflows. Sie müssen nicht direkt auf GenStudio Foundation zugreifen, um Ihre Arbeit abzuschließen. Ihr Zugriff auf GenStudio Foundation-Funktionen über Content Reviewer fällt unter die Bedingungen Ihres Workfront-Vertrags.
* Adobe muss eine unterzeichnete Adobe Gen AI-Vereinbarung in der Datei haben.
Weitere Informationen zur Unterzeichnung des Abkommens finden Sie unter [Unterzeichnung des Adobe Gen AI-Abkommens](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).
* Content Reviewer ist in Sandbox-Umgebungen nicht verfügbar.


## Unterstützte Dateitypen {#supported-file-types-ai-reviewer}

>[!CONTEXTUALHELP]
>id="wf_document_approvals_ai_supported_files"
>title="Nicht unterstützter Dateityp"
>abstract="Dieser Inhaltsprüfer unterstützt den ausgewählten Dateityp nicht. Laden Sie einen unterstützten Dateityp hoch oder entfernen Sie den Inhaltsprüfer, um die Anfrage zu senden."

Der Content Reviewer kann die folgenden Dateitypen überprüfen:

* PNG (.png)
* JPEG (.jpeg, .jpg)
* WEBP (.webp)
* Nicht animierte GIF (.gif)
* PDF (.pdf)
* PPT (.ppt, .pptx)
* DOC (.doc, .docx)

Wenn Sie einen nicht unterstützten Dateityp hochladen, ist die Option „Inhalts-Reviewer“ beim Erstellen eines Genehmigungs-Workflows nicht verfügbar.

## Einrichten von Markenrichtlinien

Workfront Content Reviewer verwendet bei der Überprüfung Ihrer Inhalte die Markenrichtlinien. Workfront-Administratoren können im Bereich &quot;Workfront-Setup“ Markenrichtlinien einrichten. In GenStudio Foundation erstellte Marken sind auch in Workfront verfügbar.

Um Markenrichtlinien einzurichten, müssen Systemadministratoren:

1. [Zugriff auf Markenberechtigungen gewähren](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-access-brands.md)
1. [Erstellen und Verwalten von Marken für den Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).


## Erstellen von Inhaltsvalidierern

Sobald mindestens eine Marke eingerichtet ist, können Workfront-Administratoren im Bereich „Setup“ mit der Erstellung von Content Reviewern beginnen. Sie können mehrere Content Reviewer erstellen, die sich auf verschiedene Richtlinien konzentrieren:

* **Bild**: Dieser Content Reviewer überprüft das Asset anhand der Image-Markenrichtlinien, die Sie in Workfront festgelegt haben. [!BADGE Beta]{type=Positive tooltip="Diese Funktion befindet sich derzeit in der Betaphase."}
   * Systemadministratoren müssen die Beta-Vereinbarung unterzeichnen, um diese Funktion zu aktivieren.
* **Markensprache**: Die Inhaltsvalidierungsverantwortliche überprüft das Asset anhand der Markensprachrichtlinien, die Sie in Workfront eingerichtet haben.

Inhaltsvalidierer können dann Validierungsvorlagen und einzelnen Überprüfungs- und Validierungsanfragen zugewiesen werden.

Weitere Informationen finden Sie unter [Konfigurieren von KI-Mitwirkenden](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Hinzufügen von Content Reviewern zu Prüfungs- und Genehmigungsanfragen

Benutzer können Inhaltsvalidierer zu vorhandenen Validierungsvorlagen oder zu einzelnen Überprüfungs- und Validierungsanfragen hinzufügen.

### Genehmigungsvorlagen

Wenn in Ihrem Unternehmen häufig dieselben Personen an Prüfungs- und Genehmigungsanfragen beteiligt sind, können Benutzer von Standardlizenzen im Bereich &quot;Workfront-Setup“ Genehmigungsvorlagen erstellen.

Benutzer können Inhaltsvalidierer zu Validierungsvorlagen hinzufügen, um automatisch die Markenkonformität zu überprüfen, wenn eine Vorlage zum Erstellen einer Anfrage verwendet wird.

Nach der Erstellung können Validierungsvorlagen auf Assets im Dokumentbereich eines Projekts, einer Aufgabe oder eines Problems angewendet werden.

Weitere Informationen finden Sie unter [Erstellen einer Workflow-Vorlage für Genehmigungen für Dokumente](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).

![Vorlagenliste mit KI-Reviewern](assets/ai-review-templates.png)

### Individuelle Prüfung und Genehmigung

Wenn Benutzer einzelne Prüfungs- und Genehmigungsanfragen erstellen, können sie einen Content Reviewer in mit anderen Teilnehmern hinzufügen oder sie können eine einzige Anfrage mit nur dem Content Reviewer erstellen, um die Markenkonformität zu überprüfen.

Weitere Informationen finden Sie unter [Erstellen eines Dokumentgenehmigungs-Workflows](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).


![Inhaltsvalidierer wurde zur individuellen Validierungsanfrage hinzugefügt](assets/new-stage.png)

## Anzeigen der Punktzahl und des Feedbacks von Inhaltsvalidierern

Sekunden nach der Übermittlung der Prüfungs- und Genehmigungsanfrage mit einem Inhaltsvalidierer sind die Punktzahl und das Feedback des Inhaltsvalidierers im Bedienfeld Dokumentzusammenfassung verfügbar, selbst wenn andere Teilnehmer noch immer ihre Entscheidungen prüfen und treffen.

Genehmigungsinhaber erhalten außerdem eine E-Mail, die sie darüber informiert, dass eine Überprüfung des Assets abgeschlossen wurde. Klicken Sie in der E **Mail auf Zum Überprüfen wechseln** die Punktzahl und das Feedback in Workfront anzeigen.

Der Content Reviewer ist nicht als Entscheidungsträger im Überprüfungs- und Genehmigungs-Workflow vorgesehen. Es werden nur eine Bewertung und Empfehlungen bereitgestellt, um das Asset an den festgelegten Markenanforderungen auszurichten.

Wenn das Asset nicht den Markenrichtlinien entspricht, kann der Kreative eine neue Version hochladen und der Genehmigungsinhaber kann eine zweite Überprüfungs- und Genehmigungsanfrage mit dem Inhaltsvalidierer erstellen.

Weitere Informationen zum Anzeigen von Bewertungen und Feedback finden Sie unter [Anzeigen der Punktzahl und des Feedbacks von Inhaltsreviewern](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/view-ai-reviewer-feedback.md).

