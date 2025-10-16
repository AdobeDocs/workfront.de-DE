---
product-area: documents
navigation-topic: approvals
title: Hochladen einer neuen Dokumentversion und Anfordern einer Genehmigung
description: Sie können eine neue Dokumentversion hochladen und die Genehmigung von anderen Benutzern in Adobe Workfront anfordern.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: b615236d2666ebcc6db0d1f796fb0baaf362e0f2
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 0%

---

# Hochladen einer neuen Dokumentversion und Anfordern einer Genehmigung

Wenn ein Dokument als für eine vorherige Überprüfung erforderlich gekennzeichnet ist, können Sie eine neue Version in das Originaldokument hochladen und eine weitere Genehmigungsrunde starten. Nachdem Sie eine neue Version des Dokuments hochgeladen haben, werden die vorherigen Versionen gesperrt.

Wenn der Dateiname der neuen Version vom Dateinamen der vorherigen Version abweicht, zeigt Workfront das Dokument mit dem neueren Dateinamen an.

Wenn einem Dokument mit ausstehenden Genehmigungen eine neue Version hinzugefügt wird, wird die Genehmigung für die vorherige Version als „Zurückgezogen“ angezeigt. Der vorherige Genehmigungsprozess wird geschlossen, auch wenn einige Teilnehmer noch keine Entscheidung getroffen haben.

Wenn die neueste Dokumentversion gelöscht wird, bleiben die vorherigen Versionen gesperrt. Wenn Sie eine frühere Version bearbeiten müssen, müssen Sie sie manuell entsperren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p> Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen</td> 
   <td> <p>Anfrage oder höher</p>
   <p>Mitwirkender oder höher</p>
   <p>Wenn Sie die Frame.io-Integration verwenden, benötigen Sie eine Standardlizenz zum Erstellen von Genehmigungs-Workflows.</p>
    </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Bearbeitungszugriff auf das mit dem Dokument verknüpfte Objekt</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Verwenden von Drag-and-Drop, um eine neue Version hinzuzufügen

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
   >   Benutzer mit einer Standardlizenz können im Bereich „Setup“ wiederverwendbare Genehmigungsvorlagen erstellen. Weitere Informationen finden Sie unter [Erstellen einer Genehmigungsvorlage für Assets und Dokumente](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).


1. (Optional) Legen Sie eine Frist für die Genehmigung fest. Benutzer und Teams werden 72 Stunden und dann 24 Stunden vor dem angegebenen Termin per E-Mail benachrichtigt.

1. Nachdem Sie alle validierungsverantwortlichen Personen und genehmigenden Personen hinzugefügt haben, klicken Sie auf **Senden**. Die Teilnehmer werden per E-Mail benachrichtigt.

   ![Neue Version zur Genehmigung einreichen](assets/add-previous-participants.png)


