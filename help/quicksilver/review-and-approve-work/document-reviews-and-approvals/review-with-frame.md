---
product-area: documents
navigation-topic: approvals
title: Überprüfen und Genehmigen mit dem Frame.io-Viewer
description: Erfahren Sie, wie Sie Dokumente mit dem Frame.io-Viewer überprüfen und genehmigen können.
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 3190ad18-180e-42e5-aa10-bdad74303d3d
source-git-commit: a5041aecad22d3e576d7f0e9a4388a3e5bc69565
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# Überprüfen und Genehmigen mit dem Frame.io-Viewer

Sie können Dokumente in Workfront mit dem Frame.io-Viewer überprüfen und genehmigen.

Durch die Überprüfung von Workfront-Dokumenten mit dem Frame.io-Viewer können Sie Kommentare hinterlassen oder bestimmte Abschnitte eines Dokuments, Bildes oder Videos markieren, um effizient mit Ihrem Team zusammenzuarbeiten und sicherzustellen, dass das Feedback klar und umsetzbar ist.

Weitere Informationen zur Integration von Frame.io in Workfront finden Sie unter [Übersicht über die Frame.io-Integration](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md).


<!--## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p> Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses</td> 
   <td> <p>Request or higher</p>
   <p>Contributor or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Documents</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Edit access to the object associated with the document</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ -->

## Voraussetzungen

* Die Integration von Workfront und Frame.io muss in Ihrer Workfront-Instanz eingerichtet sein. Weitere Informationen finden Sie unter [Übersicht über die Frame.io-Integration](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/frame-int-overview.md#integration-requirements).

## Überprüfen eines Dokuments

Als Reviewer können Sie Assets mit Kommentaren versehen und mit Markierungen versehen. Nach Abschluss des Vorgangs können Sie Ihre Überprüfung in Workfront als abgeschlossen markieren. Das Markieren der Überprüfung als abgeschlossen ist nicht erforderlich, damit das Asset im Genehmigungsprozess fortfahren kann.

1. Navigieren Sie zu Ihrer E-Mail-Benachrichtigung zur Überprüfung und klicken Sie auf **Zum Überprüfen wechseln**.
oder
Gehen Sie zur Workfront-Startseite, suchen Sie das Widget Meine Genehmigungen und klicken Sie dann auf **Überprüfung öffnen**.

   >[!NOTE]
   > 
   >Möglicherweise müssen Sie das Widget Meine Genehmigungen zu Ihrer Startseite hinzufügen. Weitere Informationen finden Sie unter [Widgets auf der Startseite hinzufügen, bearbeiten oder &#x200B;](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md).

1. Verwenden Sie in Frame.io die Kommentar-Tools, um Feedback zu hinterlassen oder Fragen zu stellen.
Kommentare und Asset-Markup sind nur im Frame.io-Viewer sichtbar. Kommentare werden in Workfront nicht angezeigt. Weitere Informationen zur Verwendung des Frame.io-Viewers finden Sie unter [Kommentieren von Medien](https://help.frame.io/en/articles/9105251-commenting-on-your-media).
1. Wenn Sie mit dem Dokument zufrieden sind, navigieren Sie zurück zur Seite Dokumentdetails in Workfront und markieren Sie Ihre Überprüfung als abgeschlossen.

   ![Review als abgeschlossen markieren](assets/mark-review-complete.png)

## Dokument genehmigen

Als genehmigende Person können Sie Kommentare hinzufügen und Assets markieren. Sie müssen eine Entscheidung treffen, um den Genehmigungsprozess voranzubringen.

Das Dokument wechselt erst dann in den Status Genehmigt , wenn alle zugewiesenen genehmigenden Personen „Genehmigt“ auswählen.

So treffen Sie eine Entscheidung über ein Dokument:

1. Navigieren Sie zu Ihrer E-Mail-Benachrichtigung zur Überprüfung und klicken Sie auf **Zum Überprüfen wechseln**.
oder
Gehen Sie zur Workfront-Startseite, suchen Sie das Widget Meine Genehmigungen und klicken Sie dann auf **Überprüfung öffnen**.

   >[!NOTE]
   > 
   >Möglicherweise müssen Sie das Widget Meine Genehmigungen zu Ihrer Startseite hinzufügen. Weitere Informationen finden Sie unter [Widgets auf der Startseite hinzufügen, bearbeiten oder &#x200B;](/help/quicksilver/workfront-basics/using-home/using-the-home-area/add-edit-remove-widgets-in-new-home.md).


1. Verwenden Sie in Frame.io die Kommentar-Tools, um Feedback zu hinterlassen oder Fragen zu stellen. Kommentare und Asset-Markup sind nur im Frame.io-Viewer sichtbar. Weitere Informationen zur Verwendung des Frame.io-Viewers finden Sie unter [Kommentieren von Medien](https://help.frame.io/en/articles/9105251-commenting-on-your-media).
1. Wenn Sie mit dem Dokument zufrieden sind, können Sie eine der folgenden Entscheidungen im Frame.io-Viewer auswählen:

   * **Genehmigen**: Das Asset benötigt keine Änderungen und ist einsatzbereit.
   * **Muss bearbeitet**: Das Asset muss geändert werden und ist nicht einsatzbereit. Sobald die angegebenen Änderungen vorgenommen wurden, muss das Asset als neue Version hochgeladen werden und eine weitere Genehmigungsrunde durchlaufen. Weitere Informationen finden Sie unter [Neue Dokumentversion hochladen und eine Genehmigung anfordern](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/upload-new-doc-version.md). <!--do they need to tell someone it was uploaded via comment tagging?-->

   Sobald Sie eine Entscheidung treffen, wird der Dokumentverantwortliche per E-Mail benachrichtigt.

   Weitere Informationen zu Entscheidungen in Workfront finden Sie unter [Übersicht über den &#x200B;](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/document-approval-status.md).

   ![Frame-Viewer und Entscheidung](assets/make-decision-frame.png)



<!--is document owner the correct term?-->
