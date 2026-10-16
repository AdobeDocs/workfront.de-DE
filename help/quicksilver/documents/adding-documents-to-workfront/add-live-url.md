---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Weblink als Dokument hinzufügen
description: Sie können eine Website zu Adobe Workfront als Weblink hinzufügen und eine Genehmigung dafür anfordern.
author: Courtney
feature: Digital Content and Documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
source-git-commit: 87fa240bc7d5694d475072b9787dca6f05702c3c
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 9%
---
# Weblink als Dokument hinzufügen

Sie können eine Website zu Adobe Workfront als Weblink aus dem Bereich Neue Dokumente hinzufügen. Nachdem Sie sie hinzugefügt haben, können Sie auf der Live-Web-Seite eine Genehmigung anfordern, genauso wie Sie die Genehmigung für eine hochgeladene Datei anfordern.

Wenn Ihr Unternehmen Adobe Cloud Storage verwendet, wird der Bereich Neue Dokumente angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Adobe Cloud-Speicher finden Sie unter [Übersicht über Adobe Cloud-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Jedes Workfront-Paket zum Verwalten von Dokumenten unter Verwendung des alten Workfront-Speichers</p>
<p>Beliebiges Workflow-Paket zum Verwalten von Dokumenten mit dem Adobe Cloud-Speicher</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen</td> 
   <td> 
   <p>Mitwirkende oder höher</p> 
   <p>Anfragende oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Legacy Workfront-Speicher: Zugriff auf Dokumente bearbeiten</p> 
   <p>Adobe Cloud-Speicher: Der Bearbeitungszugriff auf Dokumente ist standardmäßig aktiviert und kann nicht geändert werden</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Weblink als Dokument hinzufügen

Sie können eine HTML-Webseite als Weblink in Workfront hochladen. Nachdem Sie sie hinzugefügt haben, können Sie auf der Live-Web-Seite eine Genehmigung anfordern, genauso wie Sie die Genehmigung für eine hochgeladene Datei anfordern. Weitere Informationen zum Umgang mit Weblinks mit Frame.io finden Sie unter [Frame.io-Weblinks](https://help.frame.io/en/articles/12893213-html-review-for-frame-io).

<!--
>[!IMPORTANT]
>
>A web page behind single sign-on or a login page can't be displayed for review.
-->

So fügen Sie einen Weblink hinzu:

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, dem bzw. dem Sie die Website hinzufügen möchten, und wählen Sie **Dokumente** im linken Bereich aus.
1. Klicken Sie **Neu** und wählen Sie dann **Weblink**.
1. Geben Sie in das Feld **Dokumentname** einen Namen ein und geben Sie dann die Adresse der Website in das Feld **URL** ein.
1. Klicken Sie auf **Hinzufügen**.
   ![Weblink als Dokument hinzufügen](assets/web-url.png)

Informationen zum Anfordern der Genehmigung für den Weblink finden Sie unter [Erstellen eines Workflow für die Dokumentgenehmigung](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

## Bekannte Einschränkungen

* Es gibt ein temporäres Problem mit Weblink-Dokumenten, die in Frame.io erstellt wurden. Wenn Sie in Frame.io einen Weblink erstellen und anschließend in Workfront eine Genehmigung dafür erstellen, wird das Dokument nicht in Frame.io geöffnet. In Workfront erstellte Web-Links sind davon nicht betroffen. Bis dies behoben ist, müssen Sie Weblink-Dokumente in Workfront erstellen, bevor Sie mit der Genehmigung beginnen.
* Sie können derzeit keine neuen Versionen von Weblink-Dokumenten in Frame.io erstellen. Wenn Sie eine neue Version eines Weblink-Dokuments erstellen müssen, erstellen Sie die neue Version in Workfront.