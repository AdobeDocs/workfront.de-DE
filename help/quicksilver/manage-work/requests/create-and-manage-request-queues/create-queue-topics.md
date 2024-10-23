---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Erstellen von Warteschlangenthemen
description: Die Themen der Warteschlange funktionieren zusammen mit Routing-Regeln, um eingehende Arbeiten automatisch einem Benutzer, einer Auftragsrolle oder einem Team zuzuweisen oder in einem Projekt zu platzieren. Die Themen der Warteschlange definieren die Bedingungen, die für die Implementierung der Routing-Regel vorhanden sein müssen.
author: Lisa
feature: Work Management, Requests
role: User, Admin
exl-id: 65a74698-011f-4caa-9739-d7510faeb66f
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '845'
ht-degree: 2%

---

# Erstellen von Warteschlangenthemen

<!-- Audited: 12/2023 -->

Die Themen der Warteschlange funktionieren zusammen mit Routing-Regeln, um eingehende Arbeiten automatisch einem Benutzer, einer Auftragsrolle oder einem Team zuzuweisen oder in einem Projekt zu platzieren. Die Themen der Warteschlange definieren die Bedingungen, die für die Implementierung der Routing-Regel vorhanden sein müssen.

Die Anzahl der Warteschlangenthemen, die einer Themengruppe oder einem Projekt zugewiesen werden können, ist unbegrenzt. Die Themen der Warteschlange sind ein berichtspflichtiger Objekttyp.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

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

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
    <p>Neu: Standard</p>
    <p>oder</p>
    <p>Aktuell: Plan</p></td>  
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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen eines Warteschlangenthemas

1. Erstellen Sie eine Routing-Regel, eine Themengruppe und ein benutzerdefiniertes Formular, wenn Sie sie mit Ihrem Warteschlangenthema verknüpfen möchten.\
   Weitere Informationen zum Erstellen von Routing-Regeln, Themengruppen oder benutzerdefinierten Formularen finden Sie in den folgenden Artikeln:

   * [Routing-Regeln erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)
   * [Themengruppen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [Benutzerdefiniertes Formular erstellen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)

1. Wechseln Sie zu dem Projekt, das Sie als Warteschlange für Hilfeanfragen aktiviert haben und in dem Sie ein neues Warteschlangenthema erstellen möchten.\
   Weitere Informationen dazu, wie Sie ein Projekt als Warteschlange für Hilfeanfragen festlegen, finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Sie können verwandte Warteschlangenthemen unter einer Themengruppe organisieren. Dadurch erhalten die Anfragende bei der Anforderung eine Reihe von Dropdown-Menüs.

   Oder

   Sie können die Warteschlangenthemen direkt unter dem Projekt verschachteln, das als Warteschlange für Hilfeanfragen bezeichnet wird, ohne Themengruppe.

   Informationen zum Erstellen von Themengruppen finden Sie unter [Themengruppen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

1. Klicken Sie im linken Bedienfeld auf **Warteschlangenthemen** . Möglicherweise müssen Sie auf **Mehr anzeigen** und dann auf **Warteschlangenthemen** klicken.
1. Klicken Sie auf **Neues Warteschlangenthema**.
1. Geben Sie im Formular **Neues Warteschlangenthema** Folgendes ein:

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
      <td role="rowheader"><strong>Zu Themengruppe hinzufügen</strong> </td> 
      <td> Wenn das Projekt keine Themengruppen enthält, wird der Name des Projekts standardmäßig als Themengruppe verwendet.<br>Wenn Sie von hier aus weitere Themengruppen erstellen möchten, wählen Sie <strong>Neue Themengruppe erstellen</strong> aus dem Dropdownmenü.<br><img src="assets/create-new-topic-group-within-queue-topic-350x203.png" alt="create_new_topic_group_Innerhalb_queue_topic.png" style="width: 350;height: 203;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Benutzerdefinierte Formulare</strong> </td> 
      <td>Wählen Sie alle benutzerdefinierten Formulare aus, die Sie mit dem Warteschlangenthema verknüpfen möchten. Sie müssen benutzerdefinierte Formulare für Probleme erstellen, bevor Sie sie mit Warteschlangenthemen verknüpfen können. Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Entwerfen eines Formulars mit dem Formularentwickler</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standardgenehmigung</strong></td> 
      <td> <p>Verknüpfen Sie einen Genehmigungsprozess mit diesem Warteschlangenthema. In diesem Dropdown-Menü werden nur die Prozesse zur Genehmigung von Problemen angezeigt. Alle an diese Warteschlange gesendeten Probleme werden mit diesem Genehmigungsprozess verknüpft. Ihr Adobe Workfront-Administrator muss Validierungsprozesse auf Systemebene definieren, bevor Sie sie mit Warteschlangenthemen verknüpfen können. <span>Ein Benutzer mit administrativem Zugriff auf Genehmigungsprozesse kann auch gruppenspezifische Validierungsprozesse erstellen.</span> Weitere Informationen zum Erstellen von Genehmigungsprozessen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Erstellen eines Genehmigungsprozesses für Arbeitselemente</a>.<br></p> 
       <div> 
        <p>Wichtig: Wenn sich die Gruppe des Projekts ändert, wird der gruppenspezifische Validierungsprozess, der an bestehende Probleme angehängt ist, zu einem Validierungsprozess für einzelne Anwendungen. Weitere Informationen dazu, wie sich Änderungen an der Gruppe des Projekts oder am Genehmigungsprozess auf die Genehmigungseinstellungen auswirken, finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Auswirkungen von Änderungen am Gruppen- und Genehmigungsprozess auf zugewiesene Genehmigungsprozesse</a>.</p> 
        <p>Beachten Sie beim Hinzufügen von Genehmigungsprozessen zu Warteschlangenthemen Folgendes: </p> 
        <ul style="list-style-type: circle;"> 
         <li>In der Liste werden nur aktive Validierungsprozesse angezeigt. </li> 
         <li> <p>Systemweite und gruppenspezifische Validierungsprozesse werden in der Liste angezeigt. Ein Genehmigungsprozess, der mit einer anderen Gruppe als der des Projekts verknüpft ist, wird nicht in der Liste angezeigt.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standarddauer</strong> </td> 
      <td>Dies ist die Standarddauer der Anforderung, und das geplante Abschlussdatum der Anforderung wird auf Grundlage dieses Werts berechnet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standardroute</strong> </td> 
      <td>Geben Sie die Routing-Regel an, die Sie mit dem Thema Warteschlange verknüpfen möchten. Sie müssen die Routing-Regel erstellen, bevor Sie sie an ein Warteschlangenthema anhängen können. Weitere Informationen finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md">Erstellen von Routing-Regeln</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Anforderungstypen</strong> </td> 
      <td> <p>Wählen Sie, welche Art von Anforderungen dieses Warteschlangen-Thema speichert. Die sichtbaren Optionen werden auf der Registerkarte <strong>Warteschlangendetails</strong> des Projekts festgelegt. Dies ist ein Pflichtfeld. </p>

   <p><b>NOTE</b>:

   Typen werden nur dann als Auswahl im Bereich Anforderungen angezeigt, wenn der Anfragetyp sowohl auf den Seiten Warteschlangendetails als auch Warteschlangenthema ausgewählt ist. Informationen zum Einrichten des Bereichs &quot;Queue Details&quot;eines Projekts finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Erstellen einer Anforderungswarteschlange</a>. </p> <p>Wählen Sie aus den folgenden Typen aus:</p>
   <ul>
   <li>Fehlerbericht</li>
   <li>Änderungsanforderung</li>
   <li>Problem</li>
   <li>Anfrage</li>
   </ul> <p>Möglicherweise hat Ihr Workfront-Administrator einige dieser Optionen umbenannt. </p> </td>
   </tr> 
    </tbody> 
   </table>

   ![Neues Feld für Warteschlangenthema](assets/new-queue-topic-box.png)

1. Klicken Sie auf **Speichern**.\
   Das Thema Warteschlange steht jetzt zur Verwendung zur Verfügung und ist im Bereich Anforderungen von Workfront sichtbar, nachdem eine Anforderungswarteschlange und eine Themengruppe ausgewählt wurden.
