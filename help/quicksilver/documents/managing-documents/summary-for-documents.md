---
content-type: reference
product-area: documents
navigation-topic: manage-documents
title: Zusammenfassung für Dokumente – Überblick
description: Die Zusammenfassung ermöglicht die direkte Interaktion mit wichtigen Informationen aus der Dokumentenliste.
author: Courtney
feature: Digital Content and Documents
exl-id: 7a4a4bd3-ad60-4d84-b4b0-332c2a4eb8fb
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '719'
ht-degree: 12%

---

# Zusammenfassung für Dokumente – Überblick

<!--Audited: April, 2024-->

Sie können das Bedienfeld Zusammenfassung verwenden, um direkt über die Liste Dokumente auf wichtige Informationen zuzugreifen und diese zu aktualisieren.


+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.


## Zugriffsanforderungen

Sie benötigen die folgenden Zugriffsrechte, um die Schritte in diesem Artikel auszuführen:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Jedes Workfront-Paket zum Verwalten von Dokumenten unter Verwendung des alten Workfront-Speichers</p>
<p>Beliebiges Workflow-Paket zum Verwalten von Dokumenten mit Adobe Enterprise Storage</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen</td> 
   <td> <p>Mitwirkende oder höher</p> 
   <p>Anfragende oder höher</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriffrecht „Bearbeiten“ für Dokumente</p>  </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen des Zugriffs auf das mit dem Dokument verknüpfte Objekt</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Zusammenfassung für Dokumente im alten Dokumentenerlebnis

Wenn sich Ihr Unternehmen im alten Workfront-Speicher befindet, wird der Bereich für ältere Dokumente angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zum alten Workfront-Speicher finden Sie unter [Unterschiede zwischen dem alten Workfront-Speicher und dem Adobe Enterprise-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md).

### Öffnen Sie die Zusammenfassungsansicht in der Legacy-Dokumenterfahrung

{{step1-to-documents}}

1. Wählen Sie auf **Seite** Dokumente“ ein Dokument in der Liste aus.

1. Klicken Sie oben rechts auf der Seite auf das Symbol **Zusammenfassung öffnen** (![ Zusammenfassung öffnen](assets/qs-summary-in-new-toolbar-small.png). Das Seitenbedienfeld **Dokumentzusammenfassung** wird geöffnet.

   ![Zusammenfassungsdetails](assets/document-summary-panel.png)

   Nachdem Sie die Zusammenfassung geöffnet haben, bleibt sie auf dieser Seite geöffnet (auch wenn Sie auf andere Dokumente klicken), bis Sie sie manuell schließen.


### Details

Verwenden Sie den Abschnitt Details , um allgemeine Übersichtsinformationen anzuzeigen und mit benutzerdefinierten Formularen zu interagieren. Klicken Sie oben im Abschnitt auf Details , um zur Seite mit den vollständigen Dokumentdetails zu gelangen.

* [Übersicht](#overview)
* [Benutzerdefinierte Formulare](#custom-forms)

#### Übersicht {#overview}

Erweitern Sie den Abschnitt Überblick , um eine Miniaturansicht anzuzeigen oder herunterzuladen, einen Korrekturabzug zu öffnen, die allgemeine Beschreibung zu aktualisieren, das Dokument zu überprüfen und vieles mehr.

![Dokumentzusammenfassung - Übersicht](assets/details-section.png)

#### Benutzerdefinierte Formulare {#custom-forms}

Verwenden Sie den Abschnitt Benutzerdefinierte Forms , um benutzerdefinierte Formulare, die mit dem Dokument verknüpft sind, hinzuzufügen, zu bearbeiten oder anzuzeigen. Beginnen Sie mit der Eingabe des Namens des benutzerdefinierten Formulars, um es dem Dokument hinzuzufügen. Weitere Informationen finden Sie unter [Hinzufügen oder Bearbeiten eines benutzerdefinierten Formulars zu einem Dokument](../../documents/managing-documents/add-custom-form-documents.md).

![Hinzufügen eines benutzerdefinierten Formulars in der Dokumentzusammenfassung](assets/custom-forms-section.png)

### Updates

Verwenden Sie den Abschnitt Aktualisierungen , um eine Aktualisierung anzuzeigen, die jemand für das Dokument oder den Korrekturabzug vorgenommen hat. Die Zusammenfassung zeigt die ersten zwei Kommentare an. Weitere Informationen zu Aktualisierungen finden Sie unter [Kommentar zu einem Korrekturabzug](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/comment-on-proof.md).

![Updates section in Summary panel](assets/updates-section.png)

### Genehmigungen

Use the Approvals section to ask for a document approval. You can also remind someone about an approval, resubmit the approval and cancel the previous decision, or delete the approval. Document approvers can use the Summary to make a decision.

Proof approvals must be added in the Proof Workflow. For more information on approvals, see

* [Approving work](../../review-and-approve-work/manage-approvals/approving-work.md)
* [Dokumentgenehmigungen anfordern](../../review-and-approve-work/manage-approvals/request-document-approvals.md)

![Document summary approvals](assets/approvals-section.png)

### Versionen

Use the Versions section to view the number of versions created for a specific document. Click the More icon ![More icon](assets/more-icon.png) to do the following:

* Open a proof.
* Download a proof or document.
* Preview a browser-supported document.
* Go to the Document Details.
* Delete a proof or document.

![Document summary versions](assets/versions-section.png)

## Summary for documents in the new documents experience

Wenn Ihr Unternehmen Enterprise-Speicher verwendet, wird der Bereich „Neue Dokumente“ angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Massenspeicher für Unternehmen finden Sie unter [Übersicht über Speicher für Unternehmen in Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

### Details

Verwenden Sie den Abschnitt Details , um allgemeine Übersichtsinformationen anzuzeigen und mit benutzerdefinierten Formularen zu interagieren.

![Document summary details in new documents experience](assets/summary-details.png)

### Genehmigungen

Use the Approvals section to create an approval workflow. You can also remind participants about an approval or delete the approval. Document approvers can access the Frame.io viewer or use the Summary to make a decision.

For more information about approvals and Frame.io, see

* [Get started with unified review and approval](/help/quicksilver/review-and-approve-work/get-started-with-unified-approvals.md)
* [Create a document review or approval request](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

![Document summary approvals in new documents experience](assets/summary-approvals.png)


<!-- resubmit the approval and cancel the previous decision, or delete the approval. Document approvers can use the Summary to make a decision.-->


### Versionen

Use the Versions section to view the number of versions created for a specific document. Click the More icon to do the following:

* Rename a version
* View document details
* Request approval on a specific version
* In Frame.io öffnen
* Download the version
* Share the version
* Delete the version

![Document summary versions in new documents experience](assets/summary-versions.png)

### Verlauf

Use the History section to view a list of all activities related to the document.

![Document summary history in new documents experience](assets/summary-history.png)