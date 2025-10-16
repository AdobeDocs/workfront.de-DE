---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Routingregeln erstellen
description: Routing-Regeln steuern, was Adobe Workfront bei Problemen tut, wenn sie an eine Anfrage-Warteschlange gesendet werden.
author: Becky
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 9cdf3d78e1d19f3d581f8d527919a608c5cc0ddc
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 1%

---

# Routingregeln erstellen

<!-- Audited: 12/2023 -->

Routing-Regeln steuern, was Adobe Workfront bei Problemen tut, wenn sie an eine Anfrage-Warteschlange gesendet werden. Weitere Informationen zum Erstellen von Anfrage-Warteschlangen finden Sie unter [Erstellen einer Anfrage-Warteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Routing-Regeln senden Probleme an bestimmte Benutzer oder Aufgabengebiete, die am besten zur Lösung des gesendeten Problems oder der gesendeten Anfrage geeignet sind. Routingregeln sind in der Regel mit Warteschlangenthemen verknüpft, die steuern, welche Routingregel auf das Problem oder die Anfrage angewendet wird.

Nach der Erstellung können Sie Routing-Regeln nicht mehr von einem Projekt in ein anderes verschieben.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Pakete</p></td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p> Verwalten von Berechtigungen für das Projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen einer Routingregel

1. Gehen Sie zu dem Projekt, dem Sie Routing-Regeln für Ihre Anfragen hinzufügen möchten.
1. Klicken Sie **linken** auf „Routing-Regeln“.
1. Klicken Sie **Neue Routingregel**, um die neue Regel hinzuzufügen. Das Feld **Neue Routingregel** wird geöffnet.

   ![Neues Routingregel-Feld](assets/new-routing-rule-box.png)
1. Geben Sie folgende Informationen für die Routingregel ein:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td>Der Name der Routingregel. Die Routingregel wird angezeigt, wenn Sie Zugriff haben, um diese Informationen für das Projekt anzuzeigen.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beschreibung</strong> </td> 
      <td>Fügen Sie eine Beschreibung für die Routingregel hinzu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standardbevollmächtigter*</strong> </td> 
      <td>Fügen Sie einen aktiven Benutzer oder ein aktives Aufgabengebiet hinzu, dem die neuen Probleme zugewiesen werden sollen. In diesem Feld kann nur ein Standardbenutzer angegeben werden. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standardteam*</strong> </td> 
      <td>Aktives Team hinzufügen, dem das neue Problem zugewiesen werden soll. In diesem Feld kann nur ein Standard-Team vorhanden sein.

   <p><b>NOTIZ</b></p>

   Nachdem das Problem gesendet wurde, können Sie seine Zuweisungen bearbeiten und andere Benutzer, Rollen oder Teams zuweisen. Weitere Informationen finden Sie unter <a href="../../../manage-work/issues/manage-issues/assign-issues.md">Probleme zuweisen</a>.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Zu Projekt weiterleiten</strong> </td> 
      <td>Dies ist das Projekt, in dem das Problem hinzugefügt wird.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >*Wenn ein(e) Benutzende(r), ein Aufgabengebiet oder ein Team deaktiviert wird, nachdem er/sie mit einer Routing-Regel verknüpft wurde, werden die Anfragen weiterhin an ihn/sie weitergeleitet. Sie müssen regelmäßig eine Bestandsaufnahme aller Routingregeln durchführen und deaktivierte Zuweisungen durch aktive ersetzen.

   Wenn Sie ein Problem an ein Projekt weiterleiten, erhalten Benutzende mit Berechtigungen für das Problem die für dieses Projekt festgelegten Berechtigungen. Informationen zum Festlegen von Berechtigungen für Projekte finden Sie unter [Freigeben eines Projekts in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

1. Klicken Sie auf **Speichern**.

   Dieser Prozess definiert nur die Routingregel. Um sicherzustellen, dass das Problem beim Senden an die Anfrage-Warteschlange weitergeleitet wird, müssen Sie die Routing-Regel auf der Registerkarte **Warteschlangendetails** unter **Standardroute** auswählen.

   Informationen zum Hinzufügen einer Standardroute zu einer Anfrage-Warteschlange finden Sie unter [Erstellen einer Anfrage-Warteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Wenn Sie mehrere Routing-Regeln mit der Anfrage-Warteschlange verknüpfen möchten, müssen Sie mehrere Warteschlangenthemen erstellen und jedes mit einer separaten Routing-Regel verknüpfen. Weitere Informationen zum Erstellen eines Warteschlangenthemas finden Sie unter [Warteschlangenthemen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
