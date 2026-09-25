---
product-area: documents
navigation-topic: approvals
title: Anzeigen von KI-Prüfer-Bewertung und -Feedback
description: Sekunden nach dem Senden der Genehmigungsanfrage können Sie die Punktzahl und das Feedback des KI-Reviewers im Bedienfeld Dokumentzusammenfassung anzeigen.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 838e8f3d-0ea6-4844-a261-ef7b0e78a755
TQID: 'https://experienceleague.adobe.com/iPlcSTaPI-zhmWvRvO81RKFYnIzUoJqzM70mNcxrVbs'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: bc354886dc8c2f1dae24513f1d74e800e19fb3ab
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 3%
---
# Anzeigen von KI-Prüfer-Bewertung und -Feedback

Sekunden nach dem Senden der Prüfungs- und Genehmigungsanfrage können Sie die Punktzahl und das Feedback des KI-Reviewers im Bedienfeld Dokumentzusammenfassung anzeigen.

Der KI-Reviewer ist nicht als Entscheidungsträger im Überprüfungs- und Genehmigungs-Workflow vorgesehen. Es werden nur eine Bewertung und Empfehlungen bereitgestellt, um das Asset an den festgelegten Markenanforderungen auszurichten.

![KI-Reviewer-Feedback](assets/ai-reviewer-output.png)

## Berechnen der Punktzahl

Der KI-Reviewer berechnet die Bewertungen je nach Revisionstyp unterschiedlich:

* Bildüberprüfung: Dieser Wert spiegelt das Verhältnis zwischen übergebenen Richtlinien und fehlgeschlagenen Richtlinien wider.
* Copy-Review: Diese Punktzahl setzt eine ausgewogene Gewichtung subjektiver und objektiver Ergebnisse voraus. Objektive Richtlinien (angezeigt unter „Beheben„) werden dreimal so gewichtet wie subjektive Richtlinien (angezeigt unter „Berücksichtigen„).

Da objektive Richtlinien bei der Rezension von Kopien mehr Gewicht haben, empfehlen wir, konkrete, messbare Richtlinien für Ihre Marke zu schreiben. Weitere Informationen finden Sie im Abschnitt [Best Practices für die Erstellung von Markenrichtlinien](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md#best-practices-for-writing-brand-guidelines) im Artikel Erstellen und Verwalten von Marken für KI-Reviewer .

## Punktzahl und Feedback anzeigen

Sie können die Bewertung und das Feedback des KI-Reviewers im Bedienfeld Dokumentzusammenfassung oder auf der Registerkarte Genehmigungen auf der Seite Dokumentdetails einsehen.

1. Klicken Sie in der Workfront-Benachrichtigungs-E **Mail auf „Zum Überprüfen wechseln**.

   ODER

   Wechseln Sie zum Bereich Dokumente , in den das Dokument hochgeladen wird, und öffnen Sie das Bedienfeld Dokumentzusammenfassung .
1. Klicken Sie auf **Score**.
   ![Dokumentbewertung anzeigen](assets/view-score.png)

Im Fenster Bewertung und Feedback erklärt der KI-Reviewer, warum das Asset nicht den angegebenen Richtlinien entspricht.
![Das Feedback der KI-Prüfer erfordert Aufmerksamkeit](assets/ai-reviewer-needs-attention.png)

## Neue Version hochladen und erneut KI-Reviewer hinzufügen

Wenn Sie das Asset basierend auf dem Feedback des KI-Reviewers anpassen müssen, können Sie eine neue Version hochladen und eine neue Überprüfung starten.

Weitere Informationen finden Sie unter [Neue Dokumentversion hochladen und eine Genehmigung anfordern](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/upload-new-doc-version.md).
