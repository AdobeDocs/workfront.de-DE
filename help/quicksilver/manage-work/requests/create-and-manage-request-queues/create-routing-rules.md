---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Erstellen von Routing-Regeln
description: Routing-Regeln steuern, was Adobe Workfront mit Problemen macht, wenn sie an eine Anforderungswarteschlange gesendet werden.
author: Alina
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 640f9054-f2f8-4594-9311-e93518f58453
source-git-commit: 8ec279ece400c10a37e67664b77b1e0df6639724
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 1%

---

# Erstellen von Routing-Regeln

<!-- Audited: 12/2023 -->

Routing-Regeln steuern, was Adobe Workfront mit Problemen unternimmt, wenn sie an eine Anforderungswarteschlange gesendet werden. Weitere Informationen zum Erstellen von Anforderungswarteschlangen finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Routing-Regeln senden Probleme an bestimmte Benutzer oder Auftragsrollen, die am besten für die Lösung des gesendeten Problems oder der Anfrage geeignet sind. Routing-Regeln sind normalerweise mit Warteschlangenthemen verknüpft, mit denen gesteuert wird, welche Routing-Regel auf das Problem oder die Anfrage angewendet wird.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Abo</p></td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neue Lizenz: Standard </p> 
   Oder
   <p>Aktuelle Lizenz: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p> Berechtigungen für das Projekt verwalten</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen einer Routing-Regel

1. Gehen Sie zu dem Projekt, in dem Sie Routing-Regeln für Ihre Anforderungen hinzufügen möchten.
1. Klicken Sie im linken Bereich auf **Routing-Regeln** . Möglicherweise müssen Sie auf **Mehr anzeigen** und dann auf **Routing-Regeln** klicken.
1. Klicken Sie auf **Neue Routing-Regel** , um die neue Regel hinzuzufügen. Das Feld **Neue Routing-Regel** wird geöffnet.

   ![Feld für neue Routing-Regel](assets/new-routing-rule-box.png)
1. Geben Sie die folgenden Informationen für die Routing-Regel ein:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td>Der Name der Routing-Regel. Sie können die Routing-Regel sehen, wenn Sie Zugriff auf diese Informationen zum Projekt haben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beschreibung</strong> </td> 
      <td>Fügen Sie eine Beschreibung für die Routing-Regel hinzu.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standardzuweisung*</strong> </td> 
      <td>Fügen Sie einen aktiven Benutzer oder eine aktive Auftragsrolle hinzu, denen die neuen Probleme zugewiesen werden sollen. In diesem Feld darf nur ein Standardverantwortlicher enthalten sein. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standardteam*</strong> </td> 
      <td>Fügen Sie ein aktives Team hinzu, dem das neue Problem zugewiesen werden soll. In diesem Feld darf nur ein Standardteam vorhanden sein.

   <p><b>NOTIZ</b></p>

   Nachdem das Problem gesendet wurde, können Sie seine Zuweisungen bearbeiten und andere Benutzer, Rollen oder Teams zuweisen. Weitere Informationen finden Sie unter <a href="../../../manage-work/issues/manage-issues/assign-issues.md">Zuweisen von Problemen</a>.

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Route zum Projekt</strong> </td> 
      <td>Dies ist das Projekt, in dem das Problem hinzugefügt wird.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >*Wenn ein Benutzer, eine Auftragsrolle oder ein Team deaktiviert wird, nachdem sie mit einer Routing-Regel verknüpft sind, werden die Anforderungen weiterhin an ihn weitergeleitet. Sie müssen regelmäßig eine Bestandsaufnahme aller Routing-Regeln vornehmen und deaktivierte Zuweisungen durch aktive ersetzen.

   Wenn Sie ein Problem an ein Projekt weiterleiten, erhalten Benutzer mit Berechtigungen für das Problem die für dieses Projekt festgelegten Berechtigungen. Weitere Informationen zum Festlegen von Berechtigungen für Projekte finden Sie unter [Freigeben eines Projekts in Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

1. Klicken Sie auf **Speichern**.

   Dieser Prozess definiert nur die Routing-Regel. Um sicherzustellen, dass das Problem beim Senden an die Anforderungswarteschlange weitergeleitet wird, müssen Sie die Routing-Regel auf der Registerkarte **Warteschlangendetails** unter **Standardroute** auswählen.

   Informationen zum Hinzufügen einer Standardroute zu einer Anforderungswarteschlange finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Wenn Sie mehrere Routing-Regeln mit der Anforderungswarteschlange verknüpfen möchten, müssen Sie mehrere Warteschlangenthemen erstellen und jede einzelne mit einer separaten Routing-Regel verknüpfen. Weitere Informationen zum Erstellen eines Warteschlangenthemas finden Sie unter [Themen für Warteschlangen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).
