---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Erstellen von Routing-Regeln
description: Routing-Regeln steuern, was Adobe Workfront mit Problemen macht, wenn sie an eine Anforderungswarteschlange gesendet werden. Weitere Informationen zum Erstellen von Anforderungswarteschlangen finden Sie unter Anforderungswarteschlangen erstellen .
author: Alina
feature: Work Management
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 2%

---

# Erstellen von Routing-Regeln

Routing-Regeln steuern, was Adobe Workfront mit Problemen unternimmt, wenn sie an eine Anforderungswarteschlange gesendet werden. Weitere Informationen zum Erstellen von Anforderungswarteschlangen finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Routing-Regeln senden Probleme an bestimmte Benutzer oder Auftragsrollen, die am besten für die Lösung des gesendeten Problems oder der Anfrage geeignet sind. Routing-Regeln sind normalerweise mit Warteschlangenthemen verknüpft, mit denen gesteuert wird, welche Routing-Regel auf das Problem oder die Anfrage angewendet wird.

## Zugriffsanforderungen

<!--drafted - replace the table at P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p> Berechtigungen für das Projekt verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen einer Routing-Regel

1. Gehen Sie zu dem Projekt, dem Sie die Routing-Regeln für Ihre Anforderungen hinzufügen möchten.
1. Klicken **Routing-Regeln** im linken Bereich. Möglicherweise müssen Sie auf **Mehr anzeigen**, dann **Routing-Regeln**.
1. Klicken **Neue Routing-Regeln** , um die neue Regel hinzuzufügen.
1. Geben Sie die folgenden Informationen für die Routing-Regel an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td> <p>Der Name der Routing-Regel. Sie können die Routing-Regel sehen, wenn Sie Zugriff auf diese Informationen zum Projekt haben.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beschreibung</strong> </td> 
      <td>Fügen Sie eine Beschreibung für die Routing-Regel hinzu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standard-Bevollmächtigter*</strong> </td> 
      <td>Fügen Sie einen aktiven Benutzer oder eine aktive Auftragsrolle hinzu, denen die neuen Probleme zugewiesen werden sollen. In diesem Feld darf nur ein Standardverantwortlicher enthalten sein. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standardteam*</strong> </td> 
      <td>Fügen Sie ein aktives Team hinzu, dem das neue Problem zugewiesen werden soll. In diesem Feld darf nur ein Standardteam vorhanden sein.

   <p><b>NOTIZ</b></p>

   Nachdem das Problem gesendet wurde, können Sie seine Zuweisungen bearbeiten und andere Benutzer, Rollen oder Teams zuweisen. Weitere Informationen finden Sie unter  <a href="../../../manage-work/issues/manage-issues/assign-issues.md">Zuweisen von Problemen </a>.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Dem Projekt zuführen</strong> </td> 
      <td>Dies ist das Projekt, in dem das Problem hinzugefügt wird.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >*Wenn ein Benutzer, eine Auftragsrolle oder ein Team deaktiviert wird, nachdem sie mit einer Routing-Regel verknüpft sind, werden die Anforderungen weiterhin an ihn weitergeleitet. Sie müssen regelmäßig eine Bestandsaufnahme aller Routing-Regeln vornehmen und deaktivierte Zuweisungen durch aktive ersetzen.

   Wenn Sie ein Problem an ein Projekt weiterleiten, erhalten Benutzer mit Berechtigungen für das Problem die für dieses Projekt festgelegten Berechtigungen. Informationen zum Festlegen von Berechtigungen für Projekte finden Sie unter [Freigeben eines Projekts in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   ![](assets/new-routing-rule-box-nwe-350x419.png)

1. Klicken Sie auf **Speichern**.

   Dieser Prozess definiert nur die Routing-Regel. Um sicherzustellen, dass das Problem weitergeleitet wird, wenn es an die Anforderungswarteschlange gesendet wird, müssen Sie die Routing-Regel für **Warteschlangendetails** Registerkarte unter **Standardroute**.

   Informationen zum Hinzufügen einer Standardroute zu einer Anforderungswarteschlange finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Wenn Sie mehrere Routing-Regeln mit der Anforderungswarteschlange verknüpfen möchten, müssen Sie mehrere Warteschlangenthemen erstellen und jede einzelne mit einer separaten Routing-Regel verknüpfen. Weitere Informationen zum Erstellen eines Warteschlangenthemas finden Sie unter [Erstellen von Warteschlangenthemen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
