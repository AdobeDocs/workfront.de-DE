---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Freigeben eines Ziels in Workfront-Zielen
description: Wenn Sie ein Ziel freigeben, gewähren Sie "Verwalten"Berechtigungen für ein Ziel für eine Person, die es nicht erstellt hat.
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '754'
ht-degree: 2%

---

# Freigeben eines Ziels in Adobe Workfront-Zielen

Wenn Sie ein Ziel freigeben, gewähren Sie &quot;Verwalten&quot;Berechtigungen für ein Ziel für eine Person, die es nicht erstellt hat.

## Zugriffsanforderungen

<!--drafted - replace the table below with this one when P&P releases: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
  </tr>
  <tr data-mc-conditions="">
   <td role="rowheader">Object permissions</td>
   <td>
    <div>
     <p>View or higher permissions to the goal to view it</p>
     <p>Manage permissions to the goal to edit it</p>
     <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
    </div> </td>
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
   <td> <p>Pro oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung oder höher</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td> <p>Sie müssen eine zusätzliche Lizenz für die Adobe Workfront Goals erwerben, um auf die in diesem Artikel beschriebene Funktion zugreifen zu können. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Voraussetzungen für die Verwendung von Workfront-Zielen</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Ziele oder höher bearbeiten</p> <p><b>NOTIZ</b><p>Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter:</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Zugriff auf Adobe Workfront-Ziele gewähren</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> 
    <div> 
     <p>Berechtigungen für das Ziel verwalten</p> 
     <p>Informationen zum Freigeben von Zielen finden Sie unter <a href="#" class="MCXref xref selected">Freigeben eines Ziels in Workfront-Zielen</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie über Folgendes verfügen:

* Eine Layout-Vorlage, die den Bereich Ziele im Hauptmenü enthält.

## Überlegungen zur Freigabe von Zielen

* Benutzer können die folgenden Berechtigungen für ein Ziel haben:

   <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Zielberechtigungen</b></p></td> 
      <td>
      <p><b>Beschreibung</b></p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Anzeigen</p></td> 
      <td>
      <p>Benutzer sind berechtigt, das Ziel anzuzeigen, können jedoch keine Informationen für das Ziel bearbeiten, keine Informationen für Ergebnisse oder Aktivitäten hinzufügen oder bearbeiten, den Status nicht aktualisieren oder das Ziel löschen.</p>      
      <p>Standardmäßig können alle Benutzer mit Zugriff auf Ziele alle Ziele im System anzeigen. Benutzer können das Ziel kopieren, wenn sie in ihrer Zugriffsebene Zugriff auf Ziele bearbeiten haben.</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Verwalten</p></td> 
      <td> <p>Benutzer können alle Informationen für das Ziel bearbeiten, einschließlich der Ergebnisse oder Aktivitäten, einschließlich Löschen.</p> 
      <p>Nur Zielersteller oder Benutzer, denen ausdrücklich die Berechtigung zum Verwalten eines Ziels erteilt wurde, können ein Ziel verwalten.</p> 
      Nur Benutzer mit Verwaltungsberechtigungen für ein Ziel können das Ziel für andere freigeben, um ihnen Berechtigungen zum Ziel zu erteilen. </p> </td> 
   </tr> 
   </tbody> 
   </table>

* Sie können die folgenden Arten von Zielen für andere freigeben:

   * Ein von Ihnen erstelltes Ziel
   * Ein Ziel, das von einer anderen Person erstellt wurde, der Sie die Berechtigung zum Verwalten erteilt haben.

* Wenn Sie über Verwaltungsberechtigungen für ein Ziel verfügen, können Sie die Berechtigungen für das Ziel für den Ersteller ändern. Standardmäßig verfügen sie über Verwaltungsberechtigungen, wenn sie das Ziel erstellen. Sie können ihre Berechtigungen jedoch ändern, um sie anzuzeigen.

## Ziel freigeben

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) > **Ziele** in der oberen rechten Ecke.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../workfront-goals-settings/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Die Zielliste wird angezeigt.

1. Klicken Sie auf den Namen eines Ziels in der Liste. Die Zielseite wird geöffnet.

1. Klicken Sie auf **Weitere Symbole** neben dem Zielnamen klicken Sie dann auf **Freigeben**.

   ![](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   Das Feld &quot;Zielzugriff&quot;wird angezeigt.

   ![](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie die **Systemweit verwalten** -Einstellung, um allen Benutzern im System, die in ihrer Zugriffsebene Zugriff auf Ziele bearbeiten haben, Verwaltungsberechtigungen zu erteilen. Diese Option ist standardmäßig für alle neuen Ziele deaktiviert.
   * Beginnen Sie mit der Eingabe des Namens eines Benutzers, dem Sie &quot;Manage-Berechtigungen&quot;im **Zugriff gewähren an** ankreuzen. Wählen Sie den Namen aus, wenn er in der Liste angezeigt wird.

      >[!TIP]
      >
      >Sie können ein Ziel nur für andere Benutzer freigeben. Sie können keine Ziele für Gruppen, Teams oder Ihr Unternehmen freigeben.

1. Klicken **Freigeben**.

   Das Ziel wird für die von Ihnen angegebenen Benutzer freigegeben. Eine systemweite Beschriftung oder der Name der Benutzer, die über Verwaltungsberechtigungen für das Ziel verfügen, wird im Feld Zugriff auf Verwalten im Bereich Zieldetails angezeigt.

## Optionen für Zielberechtigungen

In der folgenden Tabelle sind die Berechtigungen aufgeführt, die Sie beim Freigeben eines Ziels gewähren können. Weitere Informationen über den Zugriff, den Benutzer auf der Grundlage ihrer Lizenz erhalten, finden Sie unter [Zugriff auf Adobe Workfront-Ziele gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p><strong>Aktionen</strong> </p> </th> 
   <th> <p><strong>Verwalten</strong> </p> </th> 
   <th> <p><strong>Anzeigen</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Ziel anzeigen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ergebnisse oder Aktivitäten anzeigen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Ziel kopieren* </td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Konvertieren von Ergebnissen oder Aktivitäten in andere Ziele*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Als Aktivitäten hinzugefügte Projekte anzeigen* </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Ziel bearbeiten</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Bearbeiten von Ergebnissen oder Aktivitäten</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Hinzufügen von Ergebnissen oder Aktivitäten für das Ziel</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Projekt als Aktivität dem Ziel zuordnen**</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Ziel löschen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Ergebnisse oder Aktivitäten löschen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Projekte vom Ziel trennen</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

*Sie müssen Zugriff auf Ziele bearbeiten in Ihrer Zugriffsebene haben, um Ergebnisse und Aktivitäten in Ziele konvertieren zu können.

**Sie müssen Zugriff auf die Berechtigungen Projekte anzeigen und anzeigen haben, die hinzugefügt wurden oder die Sie zum Ziel hinzufügen möchten, um sie anzuzeigen.

Informationen zur Zugriffsebene von Projekten finden Sie unter [Projektzugriff gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Weitere Informationen zu Projektberechtigungen finden Sie unter [Freigeben eines Projekts in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

 
