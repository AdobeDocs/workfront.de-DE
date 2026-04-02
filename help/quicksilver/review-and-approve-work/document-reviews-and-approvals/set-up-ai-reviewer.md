---
product-area: documents
navigation-topic: approvals
title: Erstellen von Inhaltsvalidierern
description: Sobald Sie mindestens eine Marke in Workfront eingerichtet haben, können Sie mehrere Content Reviewer erstellen, die Sie dann Genehmigungsvorlagen und einzelnen Prüfungs- und Genehmigungsanfragen zuweisen können.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
hide: true
hidefromtoc: true
exl-id: 4673049e-119e-4315-95f0-f10d8b286856
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 2b3e2ac00126facab9cc45ba8fb193d8951a37ec
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 15%

---

# Erstellen von Inhaltsvalidierern

>[!NOTE]
>
>Diese Funktion befindet sich derzeit in der Betaphase.

Sobald Sie mindestens eine Marke in Workfront eingerichtet haben, können Sie mehrere Content Reviewer erstellen, die Sie dann Genehmigungsvorlagen und einzelnen Prüfungs- und Genehmigungsanfragen zuweisen können.


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

## Hinzufügen eines Inhalts-Reviewers

>[!NOTE]
>
>Der Content Reviewer ist nicht als Entscheidungsträger im Überprüfungs- und Genehmigungs-Workflow vorgesehen. Es werden nur eine Bewertung und Empfehlungen bereitgestellt, um das Asset an den festgelegten Markenanforderungen auszurichten.

So fügen Sie einen Content Reviewer hinzu:

{{step-1-to-setup}}

1. Navigieren Sie im linken Bedienfeld zu **Überprüfen und** > **Inhaltsvalidierer**.
1. Klicken Sie **Neu hinzufügen**.
1. Geben Sie dem Validierungsverantwortlichen Namen.
1. Wählen Sie eine **Marke** aus.
1. Wählen Sie im Dropdown-Menü **Richtlinientyp** eine der folgenden Optionen:
   * **Bild**: Der Content Reviewer überprüft das Asset anhand der Image-Markenrichtlinien, die Sie in Workfront festgelegt haben.
   * **Markensprache**: Die Inhaltsvalidierungsverantwortliche überprüft das Asset anhand der Markensprachrichtlinien, die Sie in Workfront eingerichtet haben.
1. Klicken Sie auf **Erstellen**.

   Nachdem der Content Reviewer erstellt wurde, können Benutzer den Content Reviewer zu Genehmigungsvorlagen oder einzelnen Genehmigungen hinzufügen.

   Weitere Informationen finden Sie unter 

   * [Erstellen einer Validierungs-Workflow-Vorlage für Dokumente](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md)
   * [Erstellen eines Workflows für die Dokumentvalidierung](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)
