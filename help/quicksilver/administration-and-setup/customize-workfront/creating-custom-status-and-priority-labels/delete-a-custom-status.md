---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Benutzerdefinierten Status löschen
description: Sie können einen benutzerdefinierten Systemstatus löschen, wenn dieser für Ihre Organisation nicht mehr nützlich ist.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: c3bfaf666fb0ceb43bcabda13949b27b567b5d08
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 1%

---

# Benutzerdefinierten Status löschen

Sie können einen benutzerdefinierten Systemstatus löschen, wenn dieser für Ihre Organisation nicht mehr nützlich ist.

Ob der Status gesperrt oder entsperrt ist, bestimmt, ob der Status für alle Gruppen im System gelöscht wird:

* Wenn Sie einen Systemstatus löschen, der derzeit gesperrt ist, wird der Status für alle Gruppen im System entfernt, unabhängig davon, ob die Gruppe ihn umbenannt hat.
* Wenn Sie dagegen einen Systemstatus löschen, der derzeit entsperrt ist, bleibt der Status für alle Gruppen im System erhalten.


>[!NOTE]
>
>Folgendes kann nicht gelöscht werden:
>
>* Ein gesperrter oder entsperrter Systemstatus, der in einem Systemgenehmigungsprozess verwendet wird, der derzeit auf Genehmigung für mindestens ein Objekt in Ihrem System wartet.
>
>  Sie können jedoch einen entsperrten Systemstatus löschen, der in einem Genehmigungsprozess auf Einzelnutzung oder Gruppenebene verwendet wird, der derzeit noch nicht genehmigt wird.
>
>  Sie können einen Bericht ausführen, um die Objekte zu suchen und die ausstehenden Genehmigungen zu lösen, und dann erneut versuchen, den Status zu löschen. Anweisungen finden Sie unter [Auflisten von Objekten mit ausstehenden Genehmigungsprozessen mit einem bestimmten Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md).
>
>* Status, die in Genehmigungsprozessen verwendet werden, bei denen die Genehmigung für mindestens ein Objekt in Ihrem System aussteht.

Anweisungen zum Löschen eines Gruppenstatus finden Sie unter [Löschen eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Benutzerdefinierten Systemstatus löschen

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Projekteinstellungen** > **Status**.

1. Um den Status im gesamten System zu löschen (auch für einzelne Gruppen), bewegen Sie den Mauszeiger über den Status, klicken Sie auf **Bearbeiten** und stellen Sie sicher, dass **Für alle Gruppen sperren** ausgewählt ist. Klicken Sie auf **Speichern**.

   Oder

   Um den Systemstatus zu löschen, ihn jedoch für einzelne Gruppen beizubehalten, bewegen Sie den Mauszeiger über den Status, klicken Sie auf **Bearbeiten** und stellen Sie sicher, dass die Option **Sperren für alle Gruppen** deaktiviert ist. Klicken Sie auf **Speichern**.

1. Bewegen Sie den Mauszeiger über den Status, den Sie löschen möchten, und klicken Sie dann auf **Löschen**.
1. Klicken Sie in der angezeigten Meldung auf **Status löschen**.
1. Wählen Sie im angezeigten Feld **Löschstatus** einen Status in dem Feld mit der Bezeichnung **Alle Projekte, die diesen Status aufweisen, auf**.

   Projekte, die den Status verwenden, den Sie löschen, werden auf den von Ihnen ausgewählten Status gesetzt.

   Status sind nur dann in der Dropdownliste verfügbar, wenn sie mit dem Status übereinstimmen, den Sie löschen.

   Wenn Sie beispielsweise einen Status löschen, der dem aktuellen Status entspricht, können nur Status ausgewählt werden, die auch dem aktuellen Status entsprechen.

1. Klicken Sie auf **Status löschen**.
