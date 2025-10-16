---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Warteschlangenthemen erstellen
description: Warteschlangenthemen arbeiten mit Routingregeln zusammen, um eingehende Arbeit automatisch einem Benutzer, einem Aufgabengebiet oder Team zuzuweisen oder in einem Projekt zu platzieren. Warteschlangenthemen definieren die Bedingungen, die vorhanden sein müssen, damit die Routingregel implementiert wird.
author: Becky
feature: Work Management, Requests
role: User, Admin
exl-id: 65a74698-011f-4caa-9739-d7510faeb66f
source-git-commit: 4a0cb96f5888819747f63472712f91c685621cf1
workflow-type: tm+mt
source-wordcount: '1013'
ht-degree: 2%

---

# Warteschlangenthemen erstellen

<!-- Audited: 12/2023 -->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Sandbox-Vorschau-Umgebung verfügbar.</span>

Warteschlangenthemen arbeiten mit Routingregeln zusammen, um eingehende Arbeit automatisch einem Benutzer, einem Aufgabengebiet oder Team zuzuweisen oder in einem Projekt zu platzieren. Warteschlangenthemen definieren die Bedingungen, die vorhanden sein müssen, damit die Routingregel implementiert wird.

Die Anzahl der Warteschlangenthemen, die einer Themengruppe oder einem Projekt zugewiesen werden können, ist unbegrenzt. Warteschlangenthemen sind ein berichtspflichtiger Objekttyp.

Sie können Warteschlangenthemen für einzelne Projekte oder für Projektvorlagen erstellen.

Nach der Erstellung können Sie Warteschlangenthemen nicht mehr von einem Projekt oder einer Vorlage in ein anderes verschieben.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
    <p>Standard</p>
    <p>Plan</p></td>  
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

## Warteschlangenthema erstellen

1. Erstellen Sie eine Routingregel, eine Themengruppe und ein benutzerdefiniertes Formular, wenn Sie sie mit Ihrem Warteschlangenthema verknüpfen möchten.\
   Weitere Informationen zum Erstellen von Routing-Regeln, Themengruppen oder benutzerdefinierten Formularen finden Sie in den folgenden Artikeln:

   * [Routing-Regeln erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md)
   * [Themengruppen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md)
   * [Erstellen eines benutzerdefinierten Formulars](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)

1. Gehen Sie zu dem Projekt oder der Vorlage, das bzw. die Sie als Warteschlange für Hilfeanfragen aktivieren möchten, und legen Sie dort ein neues Warteschlangenthema an.\
   Weitere Informationen zum Ausweisen eines Projekts als Warteschlange für Hilfeanfragen finden Sie unter [Erstellen einer Anfragewarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

   Sie können verwandte Warteschlangenthemen unter einer Themengruppe organisieren. Auf diese Weise erhält der Antragsteller bei einer Anfrage eine Reihe von Dropdown-Menüs.

   Oder

   Sie können die Warteschlangenthemen direkt unter dem Projekt verschachteln, das als Warteschlange für Hilfeanfragen bezeichnet wird, ohne dass eine Themengruppe vorhanden ist.

   Informationen zum Erstellen von Themengruppen finden Sie unter [Themengruppen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

1. Klicken Sie **linken Bedienfeld** Warteschlangenthemen“.
1. Klicken Sie **Neues Warteschlangen-Thema**.
1. Geben Sie im **Neues Warteschlangenthema** Folgendes ein:

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
      <td>Beschreiben Sie die Anfrage-Warteschlange. Die Beschreibung wird angezeigt, wenn Benutzer beim Senden einer neuen Anfrage auf das Warteschlangen-Thema klicken. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Zu Themengruppe hinzufügen</strong> </td> 
      <td> Wenn es keine Themengruppen im Projekt gibt, wird der Name des Projekts standardmäßig als Themengruppe verwendet.<br>Wenn Sie von hier aus zusätzliche Themengruppen erstellen möchten, wählen Sie <strong>Neue Themengruppe erstellen</strong> aus dem Dropdown-Menü aus.<br><img src="assets/create-new-topic-group-within-queue-topic-350x203.png" alt="create_new_topic_group_within_queue_topic.png" style="width: 350;height: 203;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Benutzerdefinierte Formulare</strong> </td> 
      <td>Wählen Sie alle benutzerdefinierten Formulare aus, die Sie mit dem Warteschlangenthema verknüpfen möchten. Sie müssen benutzerdefinierte Formulare für Probleme erstellen, bevor Sie sie mit Warteschlangenthemen verknüpfen können. Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Erstellen eines benutzerdefinierten Formulars</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standardgenehmigung</strong></td> 
      <td> <p>Verknüpfen Sie einen Genehmigungsprozess mit diesem Warteschlangenthema. In diesem Dropdown-Menü werden nur Problemgenehmigungsprozesse angezeigt. Alle an diese Warteschlange gesendeten Probleme werden mit diesem Genehmigungsprozess verknüpft. Ihr Adobe Workfront-Administrator muss Genehmigungsprozesse auf Systemebene definieren, bevor Sie sie mit Warteschlangenthemen verknüpfen können. <span>Benutzende mit administrativem Zugriff auf Genehmigungsprozesse können auch gruppenspezifische Genehmigungsprozesse erstellen.</span> Weitere Informationen zum Erstellen von Genehmigungsprozessen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md" class="MCXref xref">Erstellen eines Genehmigungsprozesses für Arbeitselemente</a>.<br></p> 
       <div> 
        <p>Wichtig: Wenn sich die Gruppe des Projekts ändert, wird der gruppenspezifische Genehmigungsprozess, der mit vorhandenen Problemen verbunden ist, zu einem einmaligen Genehmigungsprozess. Weitere Informationen darüber, wie sich Änderungen an der Projektgruppe oder Änderungen im Genehmigungsprozess auf die Genehmigungseinstellungen auswirken, finden Sie unter <a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md" class="MCXref xref">Wie sich Änderungen an Gruppen- und Genehmigungsprozessen auf zugewiesene Genehmigungsprozesse auswirken</a>.</p> 
        <p>Beachten Sie beim Hinzufügen von Genehmigungsprozessen zu Warteschlangenthemen Folgendes: </p> 
        <ul style="list-style-type: circle;"> 
         <li>In der Liste werden nur aktive Genehmigungsprozesse angezeigt. </li> 
         <li> <p>In der Liste werden systemweite und gruppenspezifische Genehmigungsprozesse angezeigt. Ein Genehmigungsprozess, der mit einer anderen Gruppe als der des Projekts verknüpft ist, wird nicht in der Liste angezeigt.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standarddauer</strong> </td> 
      <td>Dies ist die Standarddauer der Anfrage. Anhand dieses Werts wird das geplante Abschlussdatum der Anfrage berechnet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Standardroute</strong> </td> 
      <td>Geben Sie die Routingregel an, die Sie mit dem Warteschlangenthema verknüpfen möchten. Sie müssen die Routingregel erstellen, bevor Sie sie an ein Warteschlangenthema anhängen können. Weitere Informationen finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md">Routing-Regeln erstellen</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Anforderungstypen</strong> </td> 
      <td> <p>Wählen Sie aus, welche Art von Anfragen dieses Warteschlangenthema speichert. Die sichtbaren Optionen werden auf der Registerkarte <strong>Warteschlangendetails</strong> des Projekts festgelegt. Dies ist ein Pflichtfeld. </p> 
       <p><b>HINWEIS</b>:</p>
      <p>Typen werden nur dann als Auswahl im Bereich Anfragen angezeigt, wenn der Anfragetyp sowohl auf den Seiten Warteschlangendetails als auch auf den Seiten Warteschlangenthema ausgewählt ist. Informationen zum Einrichten des Bereichs „Warteschlangendetails“ eines Projekts finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Erstellen einer Anfrage-Warteschlange</a>. </p> <p>Wählen Sie aus den folgenden Typen:</p> 
       <ul> 
        <li>Fehlerbericht</li> 
        <li>Änderungsanforderung</li> 
        <li>Problem</li> 
        <li>Anfrage</li> 
       </ul> <p>Möglicherweise hat Ihr Workfront-Administrator einige dieser Optionen umbenannt. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![Neues Warteschlangenthema-Feld](assets/new-queue-topic-box.png)

1. Klicken Sie auf **Speichern**.\
   Das Warteschlangenthema kann jetzt verwendet werden und wird im Bereich Anfragen von Workfront angezeigt, nachdem eine Anfrage-Warteschlange und eine Themengruppe ausgewählt wurden.

## Warteschlangenthema bearbeiten

So bearbeiten Sie ein vorhandenes Warteschlangenthema:

1. Gehen Sie zu dem Projekt oder der Vorlage, das bzw. die das Warteschlangenthema enthält, das bzw. die Sie bearbeiten möchten.
1. Klicken Sie **linken Bedienfeld** Warteschlangenthemen“.
1. Wählen Sie in der Produktionsumgebung das Warteschlangen-Thema aus, das Sie bearbeiten möchten. Klicken Sie auf der sich öffnenden Detailseite auf **Warteschlangenthema bearbeiten**.
1. <span class="preview">Klicken Sie in der Vorschau-Umgebung auf das Warteschlangen-Thema, das Sie bearbeiten möchten.

Informationen zu den verfügbaren Bearbeitungsoptionen finden Sie unter [Warteschlangenthema erstellen](#create-a-queue-topic) in diesem Artikel.

## Warteschlangenthema löschen

Sie können ein oder mehrere Warteschlangenthemen gleichzeitig löschen.

1. Gehen Sie zu dem Projekt oder der Vorlage, das/die das Warteschlangenthema enthält, das/die Sie löschen möchten.
1. Klicken Sie **linken Bedienfeld** Warteschlangenthemen“.
1. Klicken Sie auf das Kästchen neben dem Namen jedes Warteschlangen-Themas, das Sie löschen möchten. Im Feld wird ein Häkchen angezeigt.
1. Klicken Sie auf **Löschen**-Symbol ![Löschen](assets/delete-icon.png) oben auf der Seite.

