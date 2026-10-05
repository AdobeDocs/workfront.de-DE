---
product-area: documents;workfront-integrations
navigation-topic: adobe-creative-cloud-projects
title: Verwenden von Workfront-Dokumenten in Creative Cloud-Apps
description: Öffnen, Bearbeiten und Speichern von Workfront-Dokumenten aus Photoshop, Illustrator und InDesign und Anfordern von Genehmigungen dafür.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: e8e94a483c700dc00466ce7fa37f9ddaf3e86004
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 3%
---
# Verwenden von Workfront-Dokumenten in Creative Cloud-Apps

Sobald ein Workfront-Projekt im Bedienfeld Creative Cloud-Projekte verfügbar ist, können Sie mit seinen Dokumenten direkt in Photoshop, Illustrator oder InDesign arbeiten.

## Voraussetzungen

* Ihr Unternehmen muss über eine Version von Workfront verfügen, die die Adobe-Cloud-Datenspeicherung unterstützt.
* Workfront und Photoshop, Illustrator oder InDesign müssen Berechtigungen in derselben Adobe Identity Management System (IMS)-Organisation haben.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Version</td> 
   <td>Workflow-Ultimate mit aktiviertem Adobe-Cloud-Speicher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td>
      <p>Anzeigen des Zugriffs auf ein Projekt, um es im Bedienfeld "Creative Cloud-Projekte“ anzuzeigen</p>
      <p>Zugriff auf ein Projekt bearbeiten, um es hinzuzufügen, zu bearbeiten oder zu löschen</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Zugriff auf ein Workfront-Projekt

Die Ordnerstruktur Dokumente in einem Workfront-Projekt wird im Bedienfeld Projekte gespiegelt. Wenn Sie ein Dokument in einem Projektordner öffnen, bearbeiten und speichern, werden Ihre Änderungen in Workfront angezeigt.

>[!NOTE]
>
>Ältere Workfront-Speicherprojekte werden im Bedienfeld „Projekte“ nicht unterstützt - nur Adobe-Cloud-Speicherprojekte.


So greifen Sie auf ein Workfront-Projekt in Photoshop, Illustrator oder InDesign zu:

1. Öffnen Sie Photoshop, Illustrator oder InDesign.
1. Wählen **im Bedienfeld** Projekte“ auf der linken Seite der App das Workfront-Projekt aus, das Sie öffnen möchten.

   ![Workfront-Projekte im Bedienfeld „Projekte“](assets/cc-projects.png)

1. Öffnen Sie ein Dokument im Projekt, um es zu bearbeiten. Nachdem Sie Ihre Änderungen gespeichert haben, werden sie automatisch wieder im Workfront-Projekt gespeichert.


>[!TIP]
>
>Verwenden Sie stattdessen Adobe Cloud Drive, um einen Dateityp zu bearbeiten, den Photoshop, Illustrator oder InDesign nicht öffnen können, z. B. ein Word- oder Excel-Dokument. Weitere Informationen finden Sie unter [Übersicht über Adobe Cloud Drive](/help/quicksilver/documents/adobe-cloud-drive/adobe-cloud-drive-overview.md).

## Speichern eines neuen Dokuments in Workfront aus einer Creative Cloud-App

1. Öffnen Sie Photoshop, Illustrator oder InDesign und erstellen Sie eine neue Datei.
1. Wählen Sie im oberen Menü die Option **Datei > Speichern unter**.
1. Wählen Sie im Dialogfeld **Speichern unter** die Option **In Cloud-Dokumenten speichern** und wählen Sie dann das benötigte Workfront-Projekt aus.

   >[!NOTE]
   >
   >Beim Speichern eines Dokuments, das sich bereits im Workfront-Projekt befindet, wird das Dialogfeld „Speichern unter“ nicht geöffnet. Sie können ein Workfront-Projekt auswählen, in einem anderen Ordner speichern oder ein anderes Workfront-Projekt auswählen.


   ![Neues Dokument in Workfront speichern](assets/save-new-to-wf.png)

1. Wählen Sie einen Dokumentordner aus und klicken Sie dann auf **Speichern**. Wenn Sie keinen Ordner auswählen, wird das Dokument im Stammordner des Projekts gespeichert.

   ![Ordner zum Speichern eines neuen Dokuments in Workfront auswählen](assets/save-to-folder.png)

## Genehmigung für ein Dokument anfordern

Sie können wie bei jedem anderen Dokument zu jedem Dokument, das Sie aus Photoshop, Illustrator oder InDesign oder aus Adobe Cloud Drive hochgeladen haben, eine Dokumentgenehmigung in Workfront hinzufügen. Weitere Informationen finden Sie unter [Erstellen eines Dokumentgenehmigungs-Workflows](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).



## Verwalten von Dokumentversionen in Workfront über eine Creative Cloud-App

Wenn Sie ein Dokument aus Photoshop, Illustrator oder InDesign in Workfront speichern, werden die Änderungen, die Sie speichern, in der aktuellen Datei auf der Registerkarte Versionen angezeigt und mit dem Badge „Neue Änderungen“ gekennzeichnet.

Sie können eine Genehmigung für die aktuelle Datei anfordern, anstatt eine neue Version des Dokuments hochzuladen. Weitere Informationen finden Sie unter [Anfordern einer Genehmigung für die aktuelle Datei](#request-approval-on-the-current-file).

![Aktuelle Datei mit Abzeichen für neue Änderungen](assets/current-file.png)

### Genehmigung der aktuellen Datei anfordern

So fordern Sie eine Genehmigung für die aktuelle Datei eines Dokuments in Workfront an:

1. Gehen Sie zu dem Projekt in Workfront, das das Dokument enthält, für das Sie eine Genehmigung anfordern möchten.
1. Öffnen Sie das Dokument und wechseln Sie zur Registerkarte **Versionen** .
1. Klicken Sie in der aktuellen Datei auf das Menü **Mehr** und dann auf **Genehmigung anfordern**.
1. Führen Sie im Dialogfeld **Genehmigung anfordern** die Schritte unter [Erstellen eines Workflow für &#x200B;](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md) Dokumentvalidierung“ aus, um die Validierung zu erstellen.

   ![Genehmigung für aktuelle Datei anfordern](assets/request-update-on-current-file.png)

