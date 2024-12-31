---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: Löschen eines benutzerdefinierten Status
description: Sie können einen benutzerdefinierten Systemstatus löschen, wenn er für Ihr Unternehmen nicht mehr nützlich ist.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 1%

---

# Benutzerdefinierten Status löschen

Sie können einen benutzerdefinierten Systemstatus löschen, wenn er für Ihr Unternehmen nicht mehr nützlich ist.

Ob der Status gesperrt oder entsperrt ist, bestimmt, ob der Status für alle Gruppen im System gelöscht wird:

* Wenn Sie einen derzeit gesperrten Systemstatus löschen, wird der Status für alle Gruppen im System entfernt, unabhängig davon, ob die Gruppe ihn umbenannt hat oder nicht.
* Wenn Sie dagegen einen aktuell entsperrten Systemstatus löschen, bleibt der Status für alle Gruppen im System erhalten.


>[!NOTE]
>
>Folgendes kann nicht gelöscht werden:
>
>* Ein gesperrter oder entsperrter Systemstatus, der in einem Systemgenehmigungsprozess verwendet wird, der derzeit für mindestens ein Objekt in Ihrem System noch nicht genehmigt wurde.
>
>  Sie können jedoch einen entsperrten Systemstatus löschen, der in einem Genehmigungsprozess auf Einzelnutzungs- oder Gruppenebene verwendet wird, der derzeit noch nicht genehmigt wurde.
>
>  Sie können einen Bericht ausführen, um die Objekte zu finden und die ausstehenden Genehmigungen aufzulösen, und dann erneut versuchen, den Status zu löschen. Anweisungen finden Sie unter [Objekte mit ausstehenden Genehmigungsprozessen mit einem bestimmten Status auflisten](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md).
>
>* Status, die in Genehmigungsprozessen verwendet werden, deren Genehmigung für mindestens ein Objekt in Ihrem System derzeit aussteht.

Anweisungen zum Löschen eines Gruppenstatus finden Sie unter [Löschen eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
     <p>Neu: Standard</p>
     <p>oder</p>
     <p>Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Löschen eines benutzerdefinierten Systemstatus

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Projektvoreinstellungen** > **Status**.

1. Um den Status im gesamten System zu löschen (einschließlich für einzelne Gruppen), bewegen Sie den Mauszeiger über den Status, klicken Sie auf **Bearbeiten** und stellen Sie sicher, dass **Für alle Gruppen sperren** ausgewählt ist. Klicken Sie auf **Speichern**.

   Oder

   Um den Systemstatus zu löschen, ihn aber für einzelne Gruppen beizubehalten, bewegen Sie den Mauszeiger über den Status, klicken Sie auf **Bearbeiten** und stellen Sie dann sicher, dass **Für alle Gruppen sperren** deaktiviert ist. Klicken Sie auf **Speichern**.

1. Bewegen Sie den Mauszeiger über den Status, den Sie löschen möchten, und klicken Sie dann auf **Löschen**.
1. Klicken Sie in der angezeigten Meldung auf **Status löschen**.
1. Wählen Sie im angezeigten **Löschstatus** einen Status im Feld mit der Bezeichnung **Alle Projekte, die aktuell diesen Status aufweisen, auf**.

   Projekte, die den Status verwendet haben, den Sie löschen möchten, werden auf den ausgewählten Status gesetzt.

   Status sind in der Dropdown-Liste nur verfügbar, wenn sie mit dem Status übereinstimmen, den Sie löschen möchten.

   Wenn Sie beispielsweise einen Status löschen, der dem aktuellen entspricht, können nur Status ausgewählt werden, die auch dem aktuellen entsprechen.

1. Klicken Sie **Status löschen**.
