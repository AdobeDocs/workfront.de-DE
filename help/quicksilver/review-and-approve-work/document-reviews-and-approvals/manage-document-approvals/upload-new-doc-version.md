---
product-area: documents
navigation-topic: approvals
title: Hochladen einer neuen Dokumentversion und Anfordern einer Genehmigung
description: Sie können eine neue Dokumentversion hochladen und die Genehmigung von anderen Benutzern in Adobe Workfront anfordern.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/grwYgMUQc-Ft08jC1Fb1n7y18cLi1HNcXvJ3wPX0URg
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 82530b9b87f6865ec294adcdc601443ee48dcbcf
workflow-type: tm+mt
source-wordcount: 1196
ht-degree: 5%

---

# Hochladen einer neuen Dokumentversion und Anfordern einer Genehmigung

{{highlighted-preview}}

Wenn ein Dokument in einer früheren Überprüfung als „Überarbeitung erforderlich“ gekennzeichnet ist, können Sie eine neue Version in das Originaldokument hochladen und eine weitere Genehmigungsrunde starten. Nachdem Sie eine neue Version des Dokuments hochgeladen haben, werden die vorherigen Versionen gesperrt.

Wenn der Dateiname der neuen Version vom Dateinamen der vorherigen Version abweicht, zeigt Workfront das Dokument mit dem neueren Dateinamen an.

Wenn einem Dokument mit ausstehenden Genehmigungen eine neue Version hinzugefügt wird, wird die Genehmigung für die vorherige Version als „Zurückgezogen“ angezeigt. Der vorherige Genehmigungsprozess wird geschlossen, auch wenn einige Teilnehmer noch keine Entscheidung getroffen haben.

Wenn die neueste Dokumentversion gelöscht wird, bleiben die vorherigen Versionen gesperrt. Wenn Sie eine frühere Version bearbeiten müssen, müssen Sie sie manuell entsperren.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Jedes Workfront-Paket zur Verwaltung von Genehmigungen unter Verwendung des alten Workfront-Speichers</p>
<p>Beliebiges Workflow-Paket zum Verwalten von Genehmigungen mithilfe des Adobe-Cloud-Speichers</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen</td> 
   <td> <p>Anfragende oder höher</p>
   <p>Mitwirkende oder höher</p>
   <p>Wenn Sie die Frame.io-Integration verwenden, benötigen Sie eine Standardlizenz zum Erstellen von Genehmigungs-Workflows.</p>
    </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriffrecht „Bearbeiten“ für Dokumente</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Bearbeitungszugriff auf das mit dem Dokument verknüpfte Objekt</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++



## Verwenden Sie Drag-and-Drop, um im Bereich für veraltete Dokumente in der Produktion eine neue Version hinzuzufügen

Wenn sich Ihr Unternehmen im Workfront-Speicher befindet, wird der Bereich für veraltete Dokumente angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Workfront-Speicher finden Sie unter [Unterschiede zwischen Adobe-Cloud-Speicher und Legacy-Workfront-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>Drag-and-Drop funktioniert nicht mit Internet Explorer.


Wenn Sie eine weitere Runde der Überprüfung und Genehmigung für ein Dokument benötigen, können Sie in Workfront eine neue Dokumentversion erstellen.

Sie können die vorherigen Teilnehmer, neue Teilnehmer oder eine Mischung aus beiden hinzufügen. Informationen zu früheren Versionen und Teilnehmern finden Sie auf der Seite Dokumentdetails .

Hinzufügen einer neuen Version:

1. Navigieren Sie zum Dokument in Workfront.
1. Ziehen Sie die neue Datei auf das vorherige Dokument. Dadurch wird automatisch eine neue Version erstellt.

1. Nachdem das Dokument hochgeladen wurde, wählen Sie das Dokument aus, um das Bedienfeld Dokumentzusammenfassung zu öffnen. Hier sehen Sie die Versionsnummer oben im Bedienfeld.


1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** .

1. Klicken Sie **Workflow erstellen** und geben Sie dann die folgenden Details ein:

   <table>
   <tr>
   <td><strong>Name der Phase</strong></td>
   <td>Einen Namen für das Stadium hinzufügen. Sie können den Namen in einen aussagekräftigeren Namen ändern, z. B<em> „Erstprüfung</em> oder "<em> Genehmigung</em>.</td>
   </tr>
   <tr>
   <td><strong>Namen oder E-Mails hinzufügen</strong></td>
   <td>Beginnen Sie mit der Eingabe eines Benutzer- oder Team-Namens, der als genehmigende Person oder Prüfende Person hinzugefügt werden soll. Wenn Sie nur über Validierungsverantwortliche verfügen, werden diese benachrichtigt und haben die Möglichkeit, die Überprüfung abzuschließen. Es ist jedoch keine Entscheidung erforderlich oder getroffen.</td>
   </tr>
   <tr>
   <td><strong>Eine Entscheidung erforderlich (optional)</strong></td>
   <td>Die erste Person, die eine Entscheidung trifft, schließt die Phase ab.</td>
   </tr>
   <tr>
   <td><strong>Fälligkeitsdatum (optional)</strong></td>
   <td>Legen Sie ein Fälligkeitsdatum für die Genehmigung fest. Benutzer und Teams werden 72 Stunden und dann 24 Stunden vor dem angegebenen Fälligkeitsdatum per E-Mail benachrichtigt.</td>
   </tr>
   </table>

1. (Optional) Wiederholen Sie den vorherigen Schritt, um weitere Schritte nach Bedarf hinzuzufügen.

   >[!NOTE]
   >
   >Wenn Sie mehrere Phasen hinzufügen, wird der Genehmigungs-Workflow in der Reihenfolge fortgesetzt, in der die Phasen aufgelistet sind. Wenn alle erforderlichen Entscheidungen getroffen werden, beginnt die nächste Phase und die vorherige Phase wird gesperrt.



1. (Optional) Um eine vorhandene Genehmigungsvorlage hinzuzufügen, wählen Sie auf der linken Seite des Dialogfelds eine Vorlage aus.

   >[!TIP]
   >
   >   Benutzer mit einer Standardlizenz können wiederverwendbare Genehmigungsvorlagen im Bereich „Setup“ erstellen. Weitere Informationen finden Sie unter [Erstellen einer Workflow-Vorlage für Genehmigungen für Dokumente](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).



1. Nachdem Sie alle erforderlichen Stadien und Teilnehmer hinzugefügt haben, klicken Sie auf **Genehmigung anfordern**.

   Der Genehmigungs-Workflow wird gestartet und die genehmigenden Personen erhalten eine Benachrichtigung, dass ihre Genehmigung für die neue Dokumentversion erforderlich ist. Die vorherige Dokumentversion ist gesperrt und alle ausstehenden Genehmigungen für die vorherige Version werden zurückgezogen.

   !&lbrack;Genehmigung anfordern
   <!--1. To add all previous participants, click **Add all**. You can also add new participants or remove previous participants as needed.-->

<div class="preview">

## Verwenden Sie Drag-and-Drop, um im Bereich für veraltete Dokumente in der Vorschau eine neue Version hinzuzufügen

Wenn sich Ihr Unternehmen im Workfront-Speicher befindet, wird der Bereich für veraltete Dokumente angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Workfront-Speicher finden Sie unter [Unterschiede zwischen Adobe-Cloud-Speicher und Legacy-Workfront-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>Drag-and-Drop funktioniert nicht mit Internet Explorer.

Wenn Sie eine weitere Runde der Überprüfung und Genehmigung für ein Dokument benötigen, können Sie in Workfront eine neue Dokumentversion erstellen. Sie können die vorherigen Teilnehmer, neue Teilnehmer oder eine Mischung aus beiden hinzufügen. Informationen zu früheren Versionen und Teilnehmern finden Sie auf der Seite Dokumentdetails .

Das Dialogfeld Genehmigung anfordern wird standardmäßig im Standardmodus für eine einstufige Genehmigung geöffnet. Wechseln Sie in den erweiterten Modus, um mehrstufige Genehmigungen oder parallele Pfade zu konfigurieren.

So fügen Sie eine neue Version hinzu und fordern die Genehmigung an:

1. Navigieren Sie zum Dokument in Workfront.

1. Ziehen Sie die neue Datei auf das vorherige Dokument. Workfront erstellt automatisch eine neue Version.

1. Nachdem das Dokument hochgeladen wurde, wählen Sie das Dokument aus, um das Bedienfeld Dokumentzusammenfassung zu öffnen. Die Versionsnummer wird oben im Bedienfeld angezeigt.

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** und klicken Sie dann auf **Workflow erstellen**. Das **„Genehmigung anfordern** wird im Standardmodus geöffnet.

1. Konfigurieren des Validierungs-Workflows. Beschreibung der Felder, des erweiterten Modus-Umschalters und der parallelen Flusspfade finden Sie unter [Erstellen eines Workflow für die Dokumentvalidierung](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Klicken Sie **Genehmigung anfordern**.

   Der Genehmigungs-Workflow wird gestartet und die genehmigenden Personen erhalten eine Benachrichtigung, dass ihre Genehmigung für die neue Dokumentversion erforderlich ist. Die vorherige Dokumentversion ist gesperrt und alle ausstehenden Genehmigungen für die vorherige Version werden zurückgezogen.

## Verwenden Sie Drag-and-Drop, um in der Vorschau im Bereich Neue Dokumente eine neue Version hinzuzufügen

Wenn Ihr Unternehmen Adobe Cloud Storage verwendet, wird der Bereich Neue Dokumente angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Adobe Cloud-Speicher finden Sie unter [Übersicht über Adobe Cloud-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md).

>[!NOTE]
>
>Drag-and-Drop funktioniert nicht mit Internet Explorer.

Wenn Sie eine weitere Runde der Überprüfung und Genehmigung für ein Dokument benötigen, können Sie in Workfront eine neue Dokumentversion erstellen. Sie können der neuen Version des Dokuments einen Genehmigungs-Workflow hinzufügen.

<!--
the previous participants, new participants, or a mix of both. You can view information about previous versions and participants on the Document Details page.
-->

Das Dialogfeld Genehmigung anfordern wird standardmäßig im Standardmodus für eine einstufige Genehmigung geöffnet. Wechseln Sie in den erweiterten Modus, um mehrstufige Genehmigungen oder parallele Pfade zu konfigurieren.

So fügen Sie eine neue Version hinzu und fordern die Genehmigung an:

1. Navigieren Sie zum Dokument in Workfront.

1. Ziehen Sie die neue Datei auf das vorherige Dokument. Workfront erstellt automatisch eine neue Version.

1. Nachdem das Dokument hochgeladen wurde, wählen Sie das Dokument aus, um das Bedienfeld Zusammenfassung zu öffnen. Standardmäßig ist die neueste Version des Dokuments ausgewählt.

1. Scrollen Sie nach unten zum Abschnitt **Genehmigungen** und klicken Sie dann auf **Workflow erstellen**. Das **„Genehmigung anfordern** wird im Standardmodus geöffnet.

1. Konfigurieren des Validierungs-Workflows. Beschreibung der Felder, des erweiterten Modus-Umschalters und der parallelen Flusspfade finden Sie unter [Erstellen eines Workflow für die Dokumentvalidierung](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

1. Klicken Sie **Genehmigung anfordern**.

   Der Genehmigungs-Workflow wird gestartet und die genehmigenden Personen erhalten eine Benachrichtigung, dass ihre Genehmigung für die neue Dokumentversion erforderlich ist. Die vorherige Dokumentversion ist gesperrt und alle ausstehenden Genehmigungen für die vorherige Version werden zurückgezogen.

</div>
