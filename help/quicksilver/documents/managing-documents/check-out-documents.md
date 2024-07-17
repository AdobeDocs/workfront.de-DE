---
product-area: documents
navigation-topic: manage-documents
title: Dokumente auschecken
description: Sie können ein Dokument auschecken, um zu verhindern, dass andere Benutzer es löschen oder eine neue Version hochladen. Es kann jeweils nur ein Benutzer ein Dokument auschecken. Sie können alle Dokumente auschecken, die in Adobe Workfront hochgeladen wurden, sowie Dokumente, die mit Dokumentanbietern von Drittanbietern verknüpft sind (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint oder andere benutzerdefinierte Anbieter).
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Dokumente auschecken

Sie können ein Dokument auschecken, um zu verhindern, dass andere Benutzer es löschen oder eine neue Version hochladen. Es kann jeweils nur ein Benutzer ein Dokument auschecken. Sie können alle Dokumente auschecken, die in Adobe Workfront hochgeladen wurden, sowie Dokumente, die mit Dokumentanbietern von Drittanbietern verknüpft sind (Box, Dropbox, Google Drive, Webdam, Workfront DAM, SharePoint oder andere benutzerdefinierte Anbieter). 

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf das Dokument verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Aktionen, die bei ausgecheckten Dokumenten zulässig sind

Benutzer mit verwaltetem Zugriff auf das Dokument können Folgendes tun:

* Bearbeiten des Dokuments (Dokumentname, Beschreibung, benutzerdefinierte Daten)
* Dokument verschieben
* Dokument freigeben
* Dokumentvorschau
* Dokument herunterladen

  >[!TIP]
  >
  > Obwohl ein Benutzer ein Dokument herunterladen kann, wenn es von einem anderen Benutzer ausgecheckt wird, wird empfohlen, dass Benutzer warten, bis das Dokument wieder eingecheckt wurde, bevor sie es herunterladen. Wenn ein Dokument ausgecheckt wird, deutet dies oft darauf hin, dass noch an dem Dokument gearbeitet wird. Wenn Sie warten, bis ein Dokument wieder eingecheckt ist, um es herunterzuladen, wird sichergestellt, dass der Benutzer über die neueste Version verfügt.

* Validieren Sie ein Dokument oder wenden Sie eine Validierung auf das Dokument an.
* Überprüfen Sie das Dokument im Testversand-Viewer.

  Weitere Informationen zum Testen finden Sie unter [Testversand](../../review-and-approve-work/proofing/proofing.md)

## Auschecken eines Dokuments

Wenn Sie über Verwaltungsberechtigungen für ein Dokument verfügen, können Sie es auschecken, um bestimmte Aktionen für das Dokument zu verbieten. 

1. Markieren Sie den Bereich, in dem das Dokument gespeichert ist, und wählen Sie das Dokument aus. 

   Informationen zum Hinzufügen von Dokumenten finden Sie unter [Hinzufügen von Dokumenten zu Adobe Workfront aus Ihrem Dateisystem](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

1. Klicken Sie auf das Symbol **Auschecken** ![](assets/check-out-25x23.png).

1. Rechts neben dem Dokumentnamen wird ein Sperrsymbol ![](assets/lock-icon-locked-qs.png) angezeigt. Das Dokument bleibt nach der Abmeldung von Workfront ausgecheckt.
1. Nur der Benutzer, der das Dokument ausgecheckt hat, oder der Workfront-Administrator können das Dokument einchecken.

## Ausgecheckte Dokumente verwalten

Beachten Sie Folgendes zu ausgecheckten Dokumenten:

* Bevor Sie ein Objekt löschen können, in dem ein ausgechecktes Dokument gespeichert ist, müssen Sie zunächst das Dokument wieder einchecken. 
* Wenn der Workfront-Administrator einen Benutzer löscht, der ein Dokument ausgecheckt hat, dessen Inhaber er nicht war, checkt Workfront das Dokument automatisch ein.
* Wenn der Workfront-Administrator einen Benutzer löscht, der ein Dokument ausgecheckt hat, dessen Eigentümer er ist, und das Dokument auf ein Objekt hochgeladen wird, bleibt das Dokument ausgecheckt. Nur ein Workfront-Administrator kann sie wieder einchecken.
* Wenn der Workfront-Administrator einen Benutzer löscht, der ein Dokument ausgecheckt hat, dessen Eigentümer er ist, und das Dokument nur im Bereich &quot;Dokumente&quot;(nicht in einem Objekt) hochgeladen wird, wird das Dokument mit dem Benutzer gelöscht.

  Informationen zum Löschen von Benutzern finden Sie unter [Benutzer löschen](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

* Wenn der Workfront-Administrator einen Benutzer deaktiviert, bleiben alle ausgecheckten Dokumente ausgecheckt. Nur ein Workfront-Administrator kann sie wieder einchecken. 

## Einchecken eines Dokuments in

Sie müssen ein Dokument erneut einchecken, bevor Sie eine neue Version hochladen oder löschen können. 

So checken Sie ein Dokument ein:

1. Markieren Sie im entsprechenden Bereich das Dokument und wählen Sie es aus. 

   Rechts neben dem Dokumentnamen wird ein Sperrsymbol ![](assets/lock-icon-locked-qs.png) angezeigt.

1. Klicken Sie auf das Symbol **Einchecken** ![](assets/check-in-25x22.png).
