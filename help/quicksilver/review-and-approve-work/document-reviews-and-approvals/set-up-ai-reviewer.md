---
product-area: documents
navigation-topic: approvals
title: Erstellen von KI-Prüfern
description: Nachdem Sie mindestens eine Marke in Workfront eingerichtet haben, können Sie mehrere KI-Reviewer erstellen, die Sie dann Genehmigungsvorlagen und einzelnen Prüfungs- und Genehmigungsanfragen zuweisen können.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
exl-id: 4673049e-119e-4315-95f0-f10d8b286856
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/sfM3OtA-DVqywr3Up8VGjcycLRs5WtF22dcpXzRlnvQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: c10f2e93-7a58-4212-aa24-684c265ebe76
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 290
ht-degree: 17%

---

# Erstellen von KI-Prüfern

>[!NOTE]
>
>Diese Funktion befindet sich derzeit in der Betaphase.

Nachdem Sie mindestens eine Marke in Workfront eingerichtet haben, können Sie mehrere KI-Reviewer erstellen, die Sie dann Genehmigungsvorlagen und einzelnen Prüfungs- und Genehmigungsanfragen zuweisen können.


## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen Systemadministrator sein.</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie beginnen, müssen Sie in Workfront Richtlinien für die Bild-Markendarstellung einrichten. Weitere Informationen finden Sie unter [Erstellen und Verwalten von Marken für den Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).

## Hinzufügen eines KI-Reviewers

>[!NOTE]
>
>Der KI-Reviewer ist nicht als Entscheidungsträger im Überprüfungs- und Genehmigungs-Workflow vorgesehen. Es werden nur eine Bewertung und Empfehlungen bereitgestellt, um das Asset an den festgelegten Markenanforderungen auszurichten.

So fügen Sie einen Content Reviewer hinzu:

{{step-1-to-setup}}

1. Navigieren Sie im linken Bedienfeld zu **Überprüfen und** > **KI-Prüfer**.
1. Klicken Sie **Neu hinzufügen**.
1. Geben Sie dem Validierungsverantwortlichen Namen.
1. Wählen Sie eine **Marke** aus.
1. Wählen Sie im Dropdown-Menü **Richtlinientyp** eine der folgenden Optionen:
   * **Bild**: Der KI-Reviewer überprüft das Asset anhand der Image-Markenrichtlinien, die Sie in Workfront festgelegt haben.
   * **Markensprache**: Der KI-Reviewer überprüft das Asset anhand der Markensprachrichtlinien, die Sie in Workfront eingerichtet haben.
1. Klicken Sie auf **Erstellen**.

   Nachdem der KI-Reviewer erstellt wurde, können Benutzer den KI-Reviewer zu Genehmigungsvorlagen oder Einzelgenehmigungen hinzufügen.

   Weitere Informationen finden Sie unter

   * [Erstellen einer Validierungs-Workflow-Vorlage für Dokumente](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
   * [Erstellen eines Workflows für die Dokumentvalidierung](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)
