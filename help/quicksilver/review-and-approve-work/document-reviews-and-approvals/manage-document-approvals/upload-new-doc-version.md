---
product-area: documents
navigation-topic: approvals
title: Hochladen einer neuen Dokumentversion und Anfordern einer Genehmigung
description: Sie können eine neue Dokumentversion hochladen und die Genehmigung von anderen Benutzern in Adobe Workfront anfordern.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: 3fd4d18e1be14cc27b3b39d4abf399ec26ddcd51
workflow-type: tm+mt
source-wordcount: '902'
ht-degree: 7%

---

# Hochladen einer neuen Dokumentversion und Anfordern einer Genehmigung

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Sandbox-Vorschau-Umgebung verfügbar.</span>

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
   <td> <p>Beliebig</p> </td> 
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


## Verwenden Sie Drag &amp; Drop, um eine neue Version in Ihrer Produktionsumgebung hinzuzufügen

>[!NOTE]
>
>Drag-and-Drop funktioniert nicht mit Internet Explorer.


Wenn Sie eine weitere Runde der Überprüfung und Genehmigung für ein Dokument benötigen, können Sie in Workfront eine neue Dokumentversion erstellen.

Sie können die vorherigen Teilnehmer, neue Teilnehmer oder eine Mischung aus beiden hinzufügen. Informationen zu früheren Versionen und Teilnehmern finden Sie auf der Seite Dokumentdetails .

Hinzufügen einer neuen Version:

1. Navigieren Sie zum Dokument in Workfront.
1. Ziehen Sie die neue Datei auf das vorherige Dokument. Dadurch wird automatisch eine neue Version erstellt.

1. Nachdem das Dokument hochgeladen wurde, wählen Sie das Dokument aus und klicken Sie auf **Dokumentdetails**.
   ![Öffnen Sie die Dokumentdetailseite](assets/open-doc-details.png)


1. Klicken Sie im linken Bereich auf **Genehmigungen** und dann auf **Hinzufügen**.

1. Um alle vorherigen Teilnehmer hinzuzufügen, klicken Sie auf **Alle hinzufügen**. Bei Bedarf können Sie auch neue Teilnehmer hinzufügen oder frühere Teilnehmer entfernen.


1. Um eine vorhandene Validierungsvorlage hinzuzufügen, klicken Sie auf die Schaltfläche Vorlage und geben Sie einen Vorlagennamen ein.

   >[!TIP]
   >
   >   Benutzer mit einer Standardlizenz können wiederverwendbare Genehmigungsvorlagen im Bereich „Setup“ erstellen. Weitere Informationen finden Sie unter [Erstellen einer Workflow-Vorlage für Genehmigungen für Dokumente](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).


1. (Optional) Legen Sie eine Frist für die Genehmigung fest. Benutzer und Teams werden 72 Stunden und dann 24 Stunden vor dem angegebenen Termin per E-Mail benachrichtigt.

1. Nachdem Sie alle validierungsverantwortlichen Personen und genehmigenden Personen hinzugefügt haben, klicken Sie auf **Senden**. Die Teilnehmer werden per E-Mail benachrichtigt.

   ![Neue Version zur Genehmigung einreichen](assets/add-previous-participants.png)





<div class="preview">

## Verwenden Sie Drag-and-Drop, um eine neue Version in Ihrer Vorschauumgebung im Bereich für veraltete Dokumente hinzuzufügen

Wenn sich Ihr Unternehmen im Workfront-Speicher befindet, wird der Bereich für veraltete Dokumente angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Workfront-Speicher finden Sie unter [Workfront-Speicher im Vergleich zu Adobe Enterprise-Speicher](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

>[!NOTE]
>
>Drag-and-Drop funktioniert nicht mit Internet Explorer.


Wenn Sie eine weitere Runde der Überprüfung und Genehmigung für ein Dokument benötigen, können Sie in Workfront eine neue Dokumentversion erstellen.

Sie können die vorherigen Teilnehmer, neue Teilnehmer oder eine Mischung aus beiden hinzufügen. Informationen zu früheren Versionen und Teilnehmern finden Sie auf der Seite Dokumentdetails .

Hinzufügen einer neuen Version:

1. Navigieren Sie zum Dokument in Workfront.
1. Ziehen Sie die neue Datei auf das vorherige Dokument. Dadurch wird automatisch eine neue Version erstellt.

1. Nachdem das Dokument hochgeladen wurde, wählen Sie das Dokument aus, um das Bedienfeld Dokumentzusammenfassung zu öffnen. Hier sehen Sie die Versionsnummer oben im Bedienfeld.
   ![Öffnen Sie die Dokumentdetailseite](assets/open-doc-details.png)


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

   ![Genehmigung anfordern](assets/request-approval.png)
   <!--1. To add all previous participants, click **Add all**. You can also add new participants or remove previous participants as needed.-->



</div>

