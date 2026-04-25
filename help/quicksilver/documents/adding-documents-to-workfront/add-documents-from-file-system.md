---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Hinzufügen von Dokumenten zu Adobe Workfront aus Ihrem Dateisystem
description: You can add documents to projects, tasks, or issues in multiple areas in Adobe Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 0a5f82b2-f86e-4ffa-b3a6-18221dd0e158
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '1271'
ht-degree: 5%

---

# Hinzufügen von Dokumenten zu Adobe Workfront aus Ihrem Dateisystem

Workfront verfügt derzeit über zwei Versionen des Dokumentbereichs: den alten Dokumentbereich und den neuen Dokumentbereich. Welche Version Ihr Unternehmen verwendet, hängt davon ab, ob sich Ihr Unternehmen auf ältere Workfront-Speicher oder Unternehmensspeicher stützt. Weitere Informationen zu diesen Speichertypen finden Sie unter [Übersicht über Adobe Enterprise-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md).

Adding documents to Workfront differs depending on which version of the documents area your organization uses.

* [Add documents to from your file system in the legacy documents area](#add-documents-from-your-file-system-in-the-legacy-documents-area)
* [Add documents to Workfront in the new documents area](#add-documents-to-workfront-in-the-new-documents-area)



## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Jedes Workfront-Paket zum Verwalten von Dokumenten unter Verwendung des alten Workfront-Speichers</p>
<p>Beliebiges Workflow-Paket zum Verwalten von Dokumenten mit Adobe Enterprise Storage</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen*</td> 
   <td> 
   <p>Mitwirkende oder höher</p> 
   <p>Anfragende oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Legacy Workfront Storage: Edit access to Documents</p> 
   <p>Enterprise storage: Edit access to Documents is enabled by default and cannot be changed</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Add documents from your file system in the legacy documents area

If your organization is on legacy Workfront Storage, you will see the legacy documents area when you access documents in Workfront. For more information about Workfront Storage, see [Differences between Adobe enterprise storage and legacy Workfront storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-enterprise-storage-and-legacy-workfront-storage).

You can add documents to projects, tasks, or issues in the following areas in Adobe Workfront:

* The global Documents area
* The Documents area for a Workfront object
* A connected card on a Workfront board

You can also upload new versions of documents and add links to documents from third-party cloud vendors, such as Google Drive, Dropbox, and Microsoft OneDrive. For information about adding new versions of documents, see [Upload a new version of a document](../../documents/managing-documents/upload-new-document-version.md). For information about adding documents from third-party cloud vendors, see [Link documents from external applications](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

There are no restrictions on the types and sizes of files that you can upload to Workfront. However, in order to be successful, the upload must be completed within five minutes and you must have adequate storage space available.

If you need information about uploading new versions of a document to Workfront, see [Upload a new version of a document](../../documents/managing-documents/upload-new-document-version.md).


### Add documents to Workfront in the legacy documents area

Sie können Workfront neue Dokumente aus dem Dateisystem auf Ihrer Workstation hinzufügen. Sie können auch Dokumente von Drittanbieterprogrammen wie Google Drive und SharePoint verknüpfen.

>[!IMPORTANT]
>
>* Sie können bis zu 150 Dokumente gleichzeitig hochladen.
>* Die Dateigröße ist nicht beschränkt.
>* Dokument-Downloads sind auf 4 GB beschränkt.

Hinzufügen eines Dokuments:

1. Navigieren Sie zum Projekt, zur Aufgabe oder zum Problem, dem bzw. dem Sie ein neues Dokument hinzufügen möchten.
1. Klicken Sie auf **Registerkarte** Dokumente“ und dann auf das **Neu hinzufügen** Dropdown-Menü.

   ![Neues Dokument hinzufügen](assets/add-new-doc.png)

1. Führen Sie je nach dem hinzuzufügenden Dokumenttyp einen der folgenden Schritte aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Hochladen von Dokumenten aus Ihrem Dateisystem auf Ihre Workstation</td> 
      <td> 
       <ol> 
        <li value="1">Wählen Sie <strong> Dropdown-Menü </strong>Neu hinzufügen“ <strong>Dokument.</strong></li> 
        <li value="2"> <p>Navigieren Sie zu dem Dokument, das Sie aus dem Dateisystem auf Ihrer Workstation hinzufügen möchten, und wählen Sie es aus.<br></p> <p>Sie können mehrere Dokumente auswählen, indem Sie die Umschalttaste gedrückt halten, während Sie zusätzliche Dateien auswählen.</p> </li> 
        <li value="3">Klicken Sie auf <strong>Öffnen</strong>.</li> 
       </ol> 
       <p><b>HINWEIS</b>: Sie können Dateien auch direkt aus Ihrem Datei-Manager per Drag-and-Drop in die Dokumentliste ziehen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hochladen von Dokumenten aus einer Drittanbieteranwendung wie Google Drive oder SharePoint</td> 
      <td> 
       <ol> 
        <li value="1"> <p>Wählen Sie <strong> Dropdown-Menü </strong>Neu hinzufügen“ die Option <strong>Von &lt;Name_der_Drittanbieteranwendung&gt;</strong> aus.</p> <p>Um beispielsweise ein Dokument von Google Drive hochzuladen, klicken Sie auf <strong>Von Google Drive</strong>.</p> </li> 
        <li value="2"> <p>Befolgen Sie die Anweisungen, um das Dokument im Drittanbieterprogramm auszuwählen.<br></p> <p>Weitere Informationen zu verknüpften Dokumenten finden Sie unter <a href="../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md" class="MCXref xref">Verknüpfen von Dokumenten aus externen Anwendungen</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dokument von einem anderen Workfront-Benutzer anfordern</td> 
      <td> 
       <ol> 
        <li value="1">Wählen Sie <strong> Dropdown-Menü </strong>Neu hinzufügen“ die Option <strong>Dokument anfordern</strong>.</li> 
        <li value="2">Geben <strong> in das Feld „Von wem wird </strong> angefordert?“ den Namen des Benutzers ein, von dem aus Sie das Dokument anfordern.</li> 
        <li value="3">Geben <strong> in das Feld „Geben Sie an, was Sie </strong> möchten“ den Namen des Dokuments ein.</li> 
        <li value="4"> <p>Klicken Sie <strong>Anfrage senden</strong>.</p> <p>Your request displays on your Documents tab.</p> <p>For more information about requesting documents, see <a href="../../documents/adding-documents-to-workfront/request-a-document.md" class="MCXref xref">Request a Document</a>.</p> </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>


## Add documents to Workfront in the new documents area

You can add documents to projects, tasks, or issues using the enterprise storage model. Weitere Informationen zu Massenspeicher für Unternehmen finden Sie unter [Übersicht über Speicher für Unternehmen in Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Functionality not currently supported in the new documents area:

* Uploading documents to the global Documents area
* Adding links to documents from third-party cloud vendors, such as Google Drive, Dropbox, and Microsoft OneDrive.
* Requesting documents
* Copying a link to a folder
* Checking out documents
* Pasting images from the clipboard
* Adding Smart folders


### Add documents to Workfront in the new documents area

Wenn Ihr Unternehmen Enterprise-Speicher verwendet, wird der Bereich „Neue Dokumente“ angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Massenspeicher für Unternehmen finden Sie unter [Übersicht über Speicher für Unternehmen in Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

<!--
>[!IMPORTANT]
>
>* You can upload up to 150 documents at one time.
>* There is no limit on the file size. 
>* Document downloads are limited to 4GB.
-->

Hinzufügen eines Dokuments:

1. Navigieren Sie zum Projekt, zur Aufgabe oder zum Problem, dem bzw. dem Sie ein neues Dokument hinzufügen möchten.
1. Click the **Documents** in the left panel.
1. Click **New** on the right side of the page or drag and drop the file into the drop zone that appears. You can add multiple documents at one time.

   ![Add a new document](assets/add-new-doc-new-doc.png)

If you need information about uploading new versions of a document to Workfront, see [Upload a new version of a document](../../documents/managing-documents/upload-new-document-version.md).

## Document security for enterprise storage

Workfront prevents viruses and other malicious content from entering the site via documents in the following ways:

**So erkennt Workfront beschädigte Dateien**

Das Scannen von Dokumenten wird automatisch für Objekte aktiviert, die das Unternehmensspeichermodell verwenden.

Alle Dateien mit weniger als 500 MB werden beim Hochladen gescannt. Dateien über 500 MB werden nicht gescannt. Wenn Workfront ein beschädigtes Dokument erkennt, wird es automatisch entfernt.

**Dateinamenbeschränkungen**

Da diese Integration mit Adobe Enterprise Storage erstellt wird, müssen beim Verwalten von Projekten und Dokumenten einige erzwungene Struktur- und Benennungskonventionen beachtet werden.

* Objektnamen müssen eindeutig sein und können nicht dupliziert werden
* Der Adobe Enterprise-Speicher erfordert eindeutige Namen für Peer-Objekte mit demselben übergeordneten Element in der Hierarchiestruktur
* Dokumente können nicht denselben Namen haben, wenn sie zum selben Projekt gehören
* Dokumentnamen dürfen keines der folgenden Sonderzeichen enthalten: `\ / : * ? " | < >`
* Dokumentnamen sind auf maximal 255 Zeichen beschränkt

Unter Berücksichtigung dieser Einschränkungen benennt Workfront Objekte oder Dokumente automatisch nach Bedarf um, um Konflikte zu vermeiden.


## Dokumentensicherheit für alten Workfront-Speicher

Workfront Site verhindert auf folgende Weise, dass Viren und andere schädliche Inhalte über Dokumente auf die Site gelangen:

**So erkennt Workfront beschädigte Dateien**

Die Dokumentüberprüfung ist für Ihr Unternehmen nur auf Anfrage aktiviert.

Wenn die Dokumentüberprüfung aktiviert ist, werden Dateien mit einer Größe von unter 25 MB beim Hochladen überprüft. Dateien über 25 MB werden nicht gescannt.

Wenn Workfront ein beschädigtes Dokument entdeckt, wird eine Meldung angezeigt, die angibt, dass die Datei beschädigt ist. Sie erhalten auch eine E-Mail-Benachrichtigung, wenn Workfront potenziell schadhaften Inhalt entdeckt und die Datei entfernt werden soll.

Beschädigte Dateien werden innerhalb von 24 Stunden nach Erkennung entfernt, es sei denn, Sie entfernen sie manuell. Wenn Sie eine beschädigte Datei löschen, verfolgt Workfront diese Aktion als Aktualisierung. Wenn Sie Workfront erlauben, es zu entfernen, werden keine Aktualisierungen aufgezeichnet.

**Dateinamenbeschränkungen**

Dateien, die in Workfront hochgeladen werden, dürfen bestimmte Zeichen in Dateinamen nicht enthalten. Wenn eine Datei eines der folgenden Zeichen im Dateinamen enthält, werden die Zeichen beim Hochladen der Datei aus dem Dateinamen entfernt: `! # % * \ | ' " / ? < > { } [ ]`.
