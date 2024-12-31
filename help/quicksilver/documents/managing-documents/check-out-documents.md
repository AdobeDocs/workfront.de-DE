---
product-area: documents
navigation-topic: manage-documents
title: Dokumente auschecken
description: Sie können ein Dokument auschecken, um zu verhindern, dass andere Benutzer es löschen oder eine neue Version hochladen. Ein Dokument kann jeweils nur von einem Benutzer ausgecheckt werden. Sie können alle in Adobe Workfront hochgeladenen Dokumente sowie Dokumente auschecken, die mit Drittanbietern von Dokumenten verknüpft sind (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint oder einem anderen benutzerdefinierten Anbieter).
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: 9aa6822c9c1ecade776d4c71b113c1afd997f40c
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 0%

---

# Dokumente auschecken

Sie können ein Dokument auschecken, um zu verhindern, dass andere Benutzer es löschen oder eine neue Version hochladen. Ein Dokument kann jeweils nur von einem Benutzer ausgecheckt werden. Sie können alle in Adobe Workfront hochgeladenen Dokumente sowie Dokumente auschecken, die mit Drittanbietern von Dokumenten verknüpft sind (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint oder einem anderen benutzerdefinierten Anbieter). 

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf das Dokument verwalten</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

## Zulässige Aktionen für ausgecheckte Dokumente

Benutzer mit Verwaltungszugriff auf das Dokument haben folgende Möglichkeiten:

* Dokument bearbeiten (Dokumentname, Beschreibung, benutzerdefinierte Daten)
* Dokument verschieben
* Dokument freigeben
* Vorschau des Dokuments
* Dokument herunterladen

  >[!TIP]
  >
  > Obwohl ein Benutzer ein Dokument herunterladen kann, wenn es von einem anderen Benutzer ausgecheckt wird, empfehlen wir, dass Benutzer warten, bis das Dokument wieder eingecheckt wurde, bevor sie es herunterladen. Wenn ein Dokument ausgecheckt wird, deutet dies oft darauf hin, dass noch an dem Dokument gearbeitet wird. Durch das Warten, bis ein Dokument zum Herunterladen wieder eingecheckt wurde, wird sichergestellt, dass der Benutzer über die neueste Version verfügt.

* Genehmigen eines Dokuments oder Anwenden einer Genehmigung auf das Dokument.
* Überprüfen des Dokuments im Proofing Viewer

  Weitere Informationen zu Proofing finden Sie unter [Proofing](../../review-and-approve-work/proofing/proofing.md)

## Auschecken eines Dokuments

Wenn Sie über Verwaltungsberechtigungen für ein Dokument verfügen, können Sie es auschecken, um bestimmte Aktionen für das Dokument zu verbieten. 

1. Wechseln Sie zu dem Bereich, in dem Ihr Dokument gespeichert ist, und wählen Sie das Dokument aus. 

   Informationen zum Hinzufügen von Dokumenten finden Sie unter [Hinzufügen von Dokumenten zu Adobe Workfront aus Ihrem Dateisystem](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

1. Klicken Sie auf **Symbol** Auschecken![](assets/check-out-25x23.png).

1. Rechts neben dem Dokumentnamen wird ein Sperrsymbol ![](assets/lock-icon-locked-qs.png). Das Dokument bleibt nach der Abmeldung von Workfront ausgecheckt.
1. Nur der Benutzer, der das Dokument ausgecheckt hat, oder der Workfront-Administrator können das Dokument einchecken.

## Ausgecheckte Dokumente verwalten

Beachten Sie Folgendes zu ausgecheckten Dokumenten:

* Bevor Sie ein Objekt löschen können, in dem ein ausgechecktes Dokument gespeichert ist, müssen Sie das Dokument zunächst wieder einchecken. 
* Wenn der Workfront-Administrator eine Person löscht, die ein Dokument ausgecheckt hat, dessen Inhaber sie nicht war, checkt Workfront das Dokument automatisch ein.
* Wenn der Workfront-Administrator eine Person löscht, die ein Dokument in ihrem Besitz ausgecheckt hat, und das Dokument in ein Objekt hochgeladen wird, bleibt das Dokument ausgecheckt. Nur ein Workfront-Administrator kann es wieder einchecken.
* Wenn der Workfront-Administrator eine Benutzerin oder einen Benutzer löscht, die bzw. der ein Dokument in ihrem Besitz ausgecheckt hat, und das Dokument nur im Bereich Dokumente (nicht auf einem Objekt) hochgeladen wird, wird das Dokument mit der Benutzerin bzw. dem Benutzer gelöscht.

  Informationen zum Löschen von Benutzern finden Sie unter [Löschen von Benutzern](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

* Wenn der Workfront-Administrator einen Benutzer deaktiviert, bleiben alle Dokumente, die er ausgecheckt hat, ausgecheckt. Nur ein Workfront-Administrator kann sie wieder einchecken. 

## Dokument einchecken in

Sie müssen ein Dokument erneut einchecken, bevor Sie eine neue Version hochladen oder löschen können. 

Einchecken eines Dokuments:

1. Wechseln Sie zum Bereich, in dem Ihr Dokument gespeichert ist, und wählen Sie das Dokument aus. 

   Rechts neben dem Dokumentnamen wird ein Sperrsymbol ![](assets/lock-icon-locked-qs.png).

1. Klicken Sie auf **Symbol** Einchecken![](assets/check-in-25x22.png).
