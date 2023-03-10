---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Erstellen von Warteschlangenthemen
description: Die Themen der Warteschlange funktionieren zusammen mit Routing-Regeln, um eingehende Arbeiten automatisch einem Benutzer, einer Auftragsrolle oder einem Team zuzuweisen oder in einem Projekt zu platzieren. Die Themen der Warteschlange definieren die Bedingungen, die für die Implementierung der Routing-Regel vorhanden sein müssen.
author: Alina
feature: Work Management
exl-id: 65a74698-011f-4caa-9739-d7510faeb66f
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 3%

---

# Erstellen von Warteschlangenthemen

Die Themen der Warteschlange funktionieren zusammen mit Routing-Regeln, um eingehende Arbeiten automatisch einem Benutzer, einer Auftragsrolle oder einem Team zuzuweisen oder in einem Projekt zu platzieren. Die Themen der Warteschlange definieren die Bedingungen, die für die Implementierung der Routing-Regel vorhanden sein müssen.

Die Anzahl der Warteschlangenthemen, die einer Themengruppe oder einem Projekt zugewiesen werden können, ist unbegrenzt. Die Themen der Warteschlange sind ein berichtspflichtiger Objekttyp.

## Zugriffsanforderungen

<!--drafted - replace table with P&P:

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
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
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
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p> Berechtigungen für das Projekt verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben

## Erstellen eines Warteschlangenthemas

1. Erstellen Sie eine Routing-Regel, eine Themengruppe und ein benutzerdefiniertes Formular, wenn Sie sie mit Ihrem Warteschlangenthema verknüpfen möchten.\
   Weitere Informationen zum Erstellen von Routing-Regeln, Themengruppen oder benutzerdefinierten Formularen finden Sie in den folgenden Artikeln:

   * [Erstellen von Routing-Regeln](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)
   * [Themengruppen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [Benutzerdefiniertes Formular erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

1. Wechseln Sie zu dem Projekt, das Sie als Warteschlange für Hilfeanfragen aktiviert haben und in dem Sie ein neues Warteschlangenthema erstellen möchten.\
   Weitere Informationen zum Ausweisen eines Projekts als Warteschlange für Hilfeanfragen finden Sie im folgenden Artikel:\
   [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

   Sie können verwandte Warteschlangenthemen unter einer Themengruppe oder direkt unter dem Projekt organisieren, das als Warteschlange für Hilfeanfragen bezeichnet wird. Dadurch erhalten die Anfragende bei der Anforderung eine Reihe von Dropdown-Menüs.\
   Sie können die Warteschlangenthemen direkt unter dem Projekt verschachteln, das als Warteschlange für Hilfeanfragen bezeichnet wird, ohne Themengruppe.

   Informationen zum Erstellen von Themengruppen finden Sie unter [Themengruppen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

1. Klicken **Warteschlangenthemen** im linken Bereich. Möglicherweise müssen Sie auf **Mehr anzeigen**, dann **Warteschlangenthemen**.
1. Klicken **Neues Warteschlangenthema**.
1. Im **Neues Warteschlangenthema** Formular, geben Sie Folgendes an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Name</strong> </td> 
      <td> Name des Warteschlangenthemas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Beschreibung</strong> </td> 
      <td>Beschreiben Sie die Anforderungswarteschlange. Die Beschreibung wird angezeigt, wenn Benutzer das Warteschlangenthema beim Senden einer neuen Anforderung auswählen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Der Themengruppe hinzufügen</strong> </td> 
      <td> Wenn das Projekt keine Themengruppen enthält, wird der Name des Projekts standardmäßig als Themengruppe verwendet.<br>Wenn Sie von hier aus weitere Themengruppen erstellen möchten, wählen Sie <strong>Neue Themengruppe erstellen</strong> aus dem Dropdown-Menü.<br><img src="assets/create-new-topic-group-within-queue-topic-350x203.png" alt="create_new_topic_group_Innerhalb_queue_topic.png" style="width: 350;height: 203;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Benutzerdefinierte Formulare</strong> </td> 
      <td>Wählen Sie alle benutzerdefinierten Formulare aus, die Sie mit dem Warteschlangenthema verknüpfen möchten. Sie müssen benutzerdefinierte Formulare für Probleme erstellen, bevor Sie sie mit Warteschlangenthemen verknüpfen können. Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">Benutzerdefiniertes Formular erstellen oder bearbeiten</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standardgenehmigung</td> 
      <td> <p>Verknüpfen Sie einen Genehmigungsprozess mit diesem Warteschlangenthema. In diesem Dropdown-Menü werden nur die Prozesse zur Genehmigung von Problemen angezeigt. Alle an diese Warteschlange gesendeten Probleme werden mit diesem Genehmigungsprozess verknüpft. Ihr Adobe Workfront-Administrator muss Validierungsprozesse auf Systemebene definieren, bevor Sie sie mit Warteschlangenthemen verknüpfen können. <span>Benutzer mit Administratorzugriff auf Genehmigungsprozesse können auch gruppenspezifische Validierungsprozesse erstellen.</span> Weitere Informationen zum Erstellen von Genehmigungsprozessen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Erstellen eines Genehmigungsprozesses für Arbeitselemente</a>.<br></p> 
       <div> 
        <p>Wichtig: Wenn sich die Gruppe des Projekts ändert, wird der gruppenspezifische Genehmigungsprozess, der an bestehende Probleme angehängt ist, zu einem Genehmigungsprozess für einzelne Anwendungen. Weitere Informationen dazu, wie sich Änderungen an der Projektgruppe oder Änderungen im Genehmigungsprozess auf die Validierungseinstellungen auswirken, finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Auswirkungen von Änderungen am Gruppen- und Genehmigungsprozess auf zugewiesene Genehmigungsprozesse</a>.</p> 
        <p>Beachten Sie beim Hinzufügen von Genehmigungsprozessen zu Warteschlangenthemen Folgendes: </p> 
        <ul style="list-style-type: circle;"> 
         <li>In der Liste werden nur aktive Validierungsprozesse angezeigt. </li> 
         <li> <p>Systemweite und gruppenspezifische Validierungsprozesse werden in der Liste angezeigt. Ein Genehmigungsprozess, der mit einer anderen Gruppe als der des Projekts verknüpft ist, wird nicht in der Liste angezeigt.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standardzeitraum</strong> </td> 
      <td>Dies ist die Standarddauer der Anfrage und das geplante Abschlussdatum der Anfrage wird anhand dieses Werts berechnet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standardroute</strong> </td> 
      <td>Geben Sie die Routing-Regel an, die Sie mit dem Thema Warteschlange verknüpfen möchten. Sie müssen die Routing-Regel erstellen, bevor Sie sie an ein Warteschlangenthema anhängen können.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Anforderungstypen</strong> </td> 
      <td> <p>Wählen Sie, welche Art von Anforderungen dieses Warteschlangen-Thema speichert. Die sichtbaren Optionen werden auf der <strong>Warteschlangendetails</strong> des Projekts. Dies ist ein Pflichtfeld. </p> <p>Hinweis: Anfragetypen werden nur dann als Auswahl im Bereich Anforderungen angezeigt, wenn der Anfragetyp sowohl auf den Seiten Warteschlangendetails als auch Warteschlangenthema ausgewählt ist. Informationen zum Einrichten des Bereichs "Queue Details"eines Projekts finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Erstellen einer Anforderungswarteschlange</a>. </p> <p>Wählen Sie aus den folgenden Typen aus:</p> 
       <ul> 
        <li>Bug-Bericht</li> 
        <li>Änderungsanforderung</li> 
        <li>Anfrage</li> 
        <li>Anfrage</li> 
       </ul> <p>Möglicherweise hat Ihr Workfront-Administrator einige dieser Optionen umbenannt. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/new-queue-topic-box-nwe-350x375.png)

1.  
1. Klicken Sie auf **Speichern**.\
   Das Thema Warteschlange steht jetzt zur Verwendung zur Verfügung und ist im Bereich Anforderungen von Workfront sichtbar, nachdem eine Anforderungswarteschlange und eine Themengruppe ausgewählt wurden.
