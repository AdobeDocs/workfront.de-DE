---
product-area: documents
navigation-topic: manage-documents
title: Verwalten von Dokumentversionen
description: You can manage multiple versions of a document in Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 8%

---

# Verwalten von Dokumentversionen

<!-- Audited: 5/2025 -->

You can manage multiple versions of a document in Workfront.

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
   <td role="rowheader">Adobe Workfront-Lizenzen</td> 
   <td> 
   <p>Mitwirkende oder höher</p>
   <p>Anfragende oder höher </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Dokumente anzeigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>View access to the Document</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

* This article assumes that the document has multiple versions.

  If you need information about uploading new versions of a document to Workfront, see [Upload a new version of a document](../../documents/managing-documents/upload-new-document-version.md).

## View a list of all versions of a document

{{step1-to-documents}}

1. On the **Documents** page, select a document in the list.

1. In the upper-right corner of the page, click the **Open Summary** icon ![Open Summary icon](assets/qs-summary-in-new-toolbar-small.png). The **Document Summary** side panel opens.

1. Scroll down to the **Versions** section to view all the document versions.

## View and manage details for a previous document version

{{step1-to-documents}}

1. Hover over the document, then click **Document Details**.

1. Near the top of the **Document Details** page, click the drop-down menu next to the name, then click the name of the version you want to view and manage.

   ![Version drop-down on the Document Details page](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   Along with viewing the version&#39;s details, you can make changes to the version, such as its name, metadata, and proofing settings (if it&#39;s a document proof).

## Download a single document version

{{step1-to-documents}}

1. On the **Documents** page, select a document in the list.

1. In the upper-right corner of the page, click the **Open Summary** icon ![Open Summary icon](assets/qs-summary-in-new-toolbar-small.png). The **Document Summary** side panel opens.

1. In the **Versions** section, click the click the **More** menu ![More menu](assets/more-icon.png) to the right of the version, then click **Download** in the drop-down list that appears.

   ![Download a single document](assets/more-versions-350x143.png)

## Download all versions of a document

{{step1-to-documents}}

1. Wählen Sie auf **Seite** Dokumente“ ein Dokument in der Liste aus.

1. Klicken Sie oben rechts auf der Seite auf das Symbol **Zusammenfassung öffnen** (![ Zusammenfassung öffnen](assets/qs-summary-in-new-toolbar-small.png). Das Seitenbedienfeld **Dokumentzusammenfassung** wird geöffnet.

1. Scrollen Sie nach unten zum Abschnitt **Versionen** und klicken Sie dann auf **Alle herunterladen**.

## Dokumentversion löschen

Wenn Sie versehentlich eine Version eines Dokuments hochladen oder eine Version nicht mehr benötigt wird, können Sie die Version löschen und das Originaldokument beibehalten.

>[!IMPORTANT]
>
>Sie können eine Dokumentversion, die Sie einzeln löschen, nicht wiederherstellen.

Beachten Sie beim Löschen einer Dokumentversion Folgendes:

* Es kann jeweils nur eine Version gelöscht werden. Wenn eine Version gelöscht wird, wird diese Aktion im Abschnitt Aktualisierungen des Dokuments angezeigt.
* Wenn Sie nach dem Löschen einer Version eine neue Version hochladen, erhält die neue Version die nächste sequenzielle Nummer. Wenn es beispielsweise drei Versionen eines Dokuments gibt und Sie Version 3 löschen, wird als nächstes Dokument Version 4 hochgeladen.
* Systemaktualisierungen und Kommentare zu einer Version werden nach dem Löschen der Version in Workfront beibehalten.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

Löschen einer Dokumentversion:

{{step1-to-documents}}

1. Wählen Sie auf **Seite** Dokumente“ das Dokument aus der Liste aus.

1. Klicken Sie oben rechts auf der Seite auf das Symbol **Zusammenfassung öffnen** (![ Zusammenfassung öffnen](assets/qs-summary-in-new-toolbar-small.png). Das Seitenbedienfeld **Dokumentzusammenfassung** wird geöffnet.

1. Scrollen Sie nach unten zum Abschnitt **Versionen**, um alle Dokumentversionen anzuzeigen.
1. Klicken Sie **Abschnitt** Versionen“ auf das Menü **Mehr** ![Mehr](assets/more-icon.png) rechts von der Version und klicken Sie dann in der angezeigten Dropdown-Liste auf **Löschen**.

   >[!NOTE]
   >
   >* Die **Löschen**-Option ist nur sichtbar, wenn mindestens zwei Versionen vorhanden sind.
   >* Wenn das Dokument mit einer externen Quelle verknüpft ist, wird dieser Link gelöscht und das Dokument ist nicht mehr über Workfront zugänglich.

   ![Löschen Sie die Dokumentversion](assets/more-versions-350x143.png)
