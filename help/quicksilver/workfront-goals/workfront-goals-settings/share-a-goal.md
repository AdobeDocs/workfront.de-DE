---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Ziel in Workfront Goals teilen
description: Wenn Sie ein Ziel freigeben, erteilen Sie jemandem, der es nicht erstellt hat, Verwaltungsberechtigungen für ein Ziel.
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '737'
ht-degree: 7%

---

# Ziel in Adobe Workfront Goals teilen

Wenn Sie ein Ziel freigeben, erteilen Sie jemandem, der es nicht erstellt hat, Verwaltungsberechtigungen für ein Ziel.

## Zugriffsanforderungen

>[!NOTE]
>
>Ihr Unternehmen könnte sich dafür entscheiden, weiterhin Adobe Workfront Goals zu verwenden, wenn es dieses Paket in der Vergangenheit gekauft hat. Weitere Informationen erhalten Sie von Ihrem Kundenbetreuer.
>
>Adobe Workfront Goals ist nicht mehr erhältlich.

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Adobe Workfront-Paket</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-Lizenz</td>
 <td>
 <p>Mitwirkender oder höher</p>
<p>Anfrage oder höher</p></td>
 </tr>
  <tr>
 <td role="rowheader">Konfiguration der Zugriffsebene</td>
 <td> <p>Zugriff auf Ziele bearbeiten</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektberechtigungen</td>
 <td>
  <div>
  <p>Anzeigen von oder höheren Berechtigungen für das Ziel, um es anzuzeigen</p>
  <p>Verwalten von Berechtigungen für das Ziel, um es zu bearbeiten</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Systemadministratoren, muss eine Layout-Vorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
</tbody>
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--Old:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
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
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Überlegungen zur Freigabe von Zielen

* Benutzer können über die folgenden Berechtigungen für ein Ziel verfügen:

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
      <td role="rowheader"><p>Ansicht</p></td> 
      <td>
      <p>Benutzer sind berechtigt, das Ziel anzuzeigen, können jedoch keine Informationen für das Ziel bearbeiten oder Informationen für Ergebnisse oder Aktivitäten hinzufügen oder bearbeiten, den Status aktualisieren oder das Ziel löschen.</p>      
      <p>Standardmäßig können alle Benutzer mit Zugriff auf Ziele alle Ziele im System anzeigen. Benutzende können das Ziel kopieren, wenn sie Bearbeitungszugriff auf Ziele in ihrer Zugriffsebene haben.</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Verwalten</p></td> 
      <td> <p>Benutzer können alle Informationen für das Ziel bearbeiten, einschließlich der Ergebnisse oder Aktivitäten, einschließlich löschen.</p> 
      <p>Nur Ersteller von Zielen oder Benutzer, denen spezifische Berechtigungen zum Verwalten eines Ziels erteilt wurden, können ein Ziel verwalten.</p> 
      Nur Benutzer mit der Berechtigung Verwalten für ein Ziel können das Ziel für andere freigeben, um ihnen die Berechtigung Verwalten für das Ziel zu erteilen. </p> </td> 
   </tr> 
   </tbody> 
   </table>

* Sie können die folgenden Arten von Zielen für andere freigeben:

   * Ein Ziel, das Sie erstellt haben
   * Ein von einer anderen Person erstelltes Ziel, dem Sie die Berechtigung zum Verwalten erteilt haben.

* Wenn Sie über Verwaltungsberechtigungen für ein Ziel verfügen, können Sie die Berechtigungen für das Ziel für den Ersteller des Ziels ändern. Standardmäßig verfügen sie beim Erstellen des Ziels über die Berechtigung Verwalten , Sie können jedoch ihre Berechtigungen in Anzeigen ändern.

## Teilen eines Ziels

1. Klicken Sie auf **Hauptmenü**-Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) > **Ziele** in der oberen rechten Ecke.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../workfront-goals-settings/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   Die Liste „Ziel“ wird angezeigt.

1. Klicken Sie auf den Namen eines Ziels in der Liste. Die Zielseite wird geöffnet.

1. Klicken Sie auf **Mehr** neben dem Zielnamen und dann auf **Freigeben**.

   ![Menü „Mehr“](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   Das Feld Zielzugriff wird angezeigt.

   ![Zielzugriff](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. Führen Sie einen der folgenden Schritte aus:

   * Wählen Sie **Einstellung „Systemweit verwalten** aus, um allen im System Benutzern, die Bearbeitungszugriff auf Ziele in ihrer Zugriffsebene haben, Verwaltungsberechtigungen zu erteilen. Diese Option ist für alle neuen Ziele standardmäßig deaktiviert.
   * Geben Sie den Namen eines Benutzers, dem Sie Verwaltungsberechtigungen erteilen möchten, in das Feld **Verwaltungszugriff erteilen für** ein. Wählen Sie den Namen aus, wenn er in der Liste angezeigt wird.

     >[!TIP]
     >
     >Sie können ein Ziel nur für andere Benutzer freigeben. Sie können keine Ziele für Gruppen, Teams oder Ihr Unternehmen freigeben.

1. Klicken Sie auf **Freigabe**.

   Das Ziel wird für die von Ihnen angegebenen Benutzer freigegeben. Eine „systemweite“ Beschriftung oder der Name der Benutzer, die Verwaltungsberechtigungen für das Ziel haben, wird im Feld Zugriff auf Verwaltung im Bedienfeld „Zieldetails“ angezeigt.

## Optionen für Zielberechtigungen

In der folgenden Tabelle sind die Berechtigungen aufgeführt, die Sie bei der Freigabe eines Ziels gewähren können. Weitere Informationen dazu, welchen Zugriff Benutzerinnen und Benutzer auf der Grundlage ihrer Lizenz erhalten, finden Sie unter [Zugriff auf Adobe Workfront-Ziele gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

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
   <td>Projekte anzeigen, die als Aktivitäten hinzugefügt wurden** </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Ziel bearbeiten</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ergebnisse oder Aktivitäten bearbeiten</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Fügen Sie Ergebnisse oder Aktivitäten für das Ziel hinzu</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Verknüpfen Sie ein Projekt als Aktivität mit dem Ziel**</td> 
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

* Sie müssen in Ihrer Zugriffsebene über Bearbeitungszugriff auf Ziele verfügen, um Ergebnisse und Aktivitäten in Ziele konvertieren zu können.

**Sie müssen Zugriff auf die Anzeige von Projekten haben und über die Berechtigung Anzeigen für die hinzugefügten Projekte verfügen oder die Sie zum Ziel hinzufügen möchten, um sie anzuzeigen.

Informationen zur Zugriffsebene von Projekten finden Sie unter [Zugriff auf Projekte gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Informationen zu Projektberechtigungen finden Sie unter [Freigeben eines Projekts in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

 
