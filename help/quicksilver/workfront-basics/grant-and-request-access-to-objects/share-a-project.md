---
title: Freigeben eines Projekts in Adobe Workfront
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Ihr Adobe Workfront-Administrator kann Ihnen bei der Zuweisung Ihrer Zugriffsebene Zugriff zum Anzeigen oder Bearbeiten von Projekten gewähren. Weitere Informationen finden Sie unter Gewähren des Zugriffs auf Projekte.
author: Alina
feature: Get Started with Workfront
exl-id: eaeedff8-9114-40d9-8cd4-56996edc7dad
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 2%

---

# Freigeben eines Projekts in Adobe Workfront

<!-- Audited: 1/2024 -->

Ihr Adobe Workfront-Administrator kann Ihnen bei der Zuweisung Ihrer Zugriffsebene Zugriff zum Anzeigen oder Bearbeiten von Projekten gewähren. Weitere Informationen finden Sie unter [Zugriff auf Projekte ](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Neben der Zugriffsebene, die Benutzern gewährt wird, können Sie ihnen auch Berechtigungen zum Anzeigen, Contribute oder Verwalten bestimmter Projekte erteilen, auf die Sie Zugriff haben, um sie freizugeben.

Berechtigungen sind für ein Element in Workfront spezifisch und definieren, welche Aktionen man für dieses Element ausführen kann.

## Überlegungen zur Freigabe von Projekten

Zusätzlich zu den unten stehenden Überlegungen finden Sie weitere Informationen unter [Übersicht über Freigabeberechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Standardmäßig verfügt der Ersteller eines Projekts über Berechtigungen zum Verwalten des Projekts und wird auch als Projektbesitzer bezeichnet. Wenn das Projekt einem anderen Eigentümer zugewiesen ist, verfügt dieser Benutzer auch über Berechtigungen zum Verwalten des Projekts. Wenn der Projektersteller (oder -eigentümer) das Projekt für andere Benutzer freigibt, gewähren sie diesen Benutzern bestimmte Berechtigungen, um zu steuern, was sie bei der Arbeit am Projekt tun können.

  Wenn ein Projekteigentümer jedoch nicht über eine Planner-Lizenz verfügt, hat er nicht den vollen Zugriff, um das Projekt zu verwalten. Nur Benutzer mit einer Planlizenz können über Berechtigungen zum Verwalten eines Projekts verfügen. Weitere Informationen finden Sie unter [ der Zusammenarbeit von Zugriffsebenen und Berechtigungen](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

* Sie können Projekte einzeln oder gemeinsam nutzen. Die Freigabe von Projekten ist mit der Freigabe anderer Objekte identisch. Weitere Informationen zum Freigeben von Elementen in Workfront finden Sie unter [Freigeben eines Objekts](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Sie können einem Projekt die folgenden Berechtigungen erteilen:

   * Anzeigen
   * Verwalten
   * Mitwirken

     ![](assets/view-on-projects-190x207.png) ![](assets/contribute-on-projects-159x243.png) ![](assets/manage-on-projects-178x230.png)

* Wenn Sie ein Projekt freigeben, erben alle Aufgaben, Probleme und Dokumente dieselben Berechtigungen, sofern nicht anders angegeben.

  Informationen zur Verwaltung des Zugriffs auf Aufgaben und Probleme im Projekt auf der Grundlage der Berechtigungen eines Benutzers für das Projekt finden Sie im [](../../manage-work/projects/manage-projects/edit-projects.md#access) Abschnitt im Artikel [Projekte bearbeiten](../../manage-work/projects/manage-projects/edit-projects.md).

  Der Workfront-Administrator kann angeben, ob Dokumente Berechtigungen von höheren Objekten auf der Zugriffsebene der Benutzenden erben sollen. Weitere Informationen zum Beschränken von geerbten Berechtigungen für Dokumente finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Sie können geerbte Berechtigungen aus einem Projekt entfernen, sodass die untergeordneten Objekte sie nicht erben. Weitere Informationen zum Entfernen geerbter Berechtigungen aus Objekten finden Sie unter [Entfernen von Berechtigungen aus Objekten](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Möglichkeiten zum Freigeben eines Projekts {#ways-to-share-a-project}

Sie können ein Projekt wie folgt freigeben:

* Führen Sie dazu manuell einen der folgenden Schritte aus:

   * Hinzufügen von Benutzern zum Projektteam. Wenn Sie Benutzer zum Projekt-Team hinzufügen, erhalten diese automatisch Ansichtsberechtigungen für das Projekt.\
     Weitere Informationen zum Hinzufügen von Benutzern zu einem Projektteam finden Sie im Abschnitt „Hinzufügen von Benutzern zu einem Projektteam“ in [Übersicht über das Projektteam](../../manage-work/projects/planning-a-project/project-team-overview.md).
   * Einzeln oder für die Massenfreigabe der Projekte bei Verwendung der Option **Freigabe**.

     Die Freigabe eines Projekts ähnelt der Freigabe aller anderen Objekte in Adobe Workfront.

     Informationen zum Freigeben von Objekten in Workfront finden Sie unter [Freigeben eines Objekts](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Führen Sie automatisch einen der folgenden Schritte aus:

   * Platzieren Sie ein Projekt in einem **Portfolio** oder **Programm**, das bereits für andere freigegeben ist. Benutzer erhalten für das Projekt dieselben Berechtigungen wie für das Portfolio oder Programm.\
     Informationen zum Hinzufügen eines Projekts zu einem **Portfolio** Sie unter [Hinzufügen von Projekten zu einem Portfolio](../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).\
     Informationen zum Hinzufügen eines Projekts zu einem **Programm** finden Sie unter [Hinzufügen eines Projekts zu einem Programm](../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).

     Weitere Informationen zum Anzeigen geerbter Berechtigungen für ein Objekt finden Sie unter [Anzeigen geerbter Berechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

   * Entitäten zur Projektfreigabe einer Vorlage hinzufügen, mit der das Projekt erstellt wurde. Informationen zum Freigeben von Projekten aus Vorlagen finden Sie unter [Freigeben einer Vorlage](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).
   * Definieren Sie die Projektzugriffsvorlage.

     Informationen zum Definieren der Projektzugriffsvorlage finden Sie unter [Freigeben eines Objekts](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

     >[!TIP]
     >
     >Beim Anhängen oder Speichern einer Vorlage können Sie die Regeln zur Projektfreigabe in der Vorlage löschen.

   * Bearbeiten Sie ein Projekt und definieren Sie die Einstellung **Wenn jemand Zugriff auf dieses Projekt erhält** . Weitere Informationen finden Sie unter [Projekte bearbeiten](../../manage-work/projects/manage-projects/edit-projects.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: drafted because I created new article and linked it above) </p>
<p>To view what users have inherited the access on the project from a portfolio or a program, do the following:</p>
<ol style="list-style-type: lower-alpha;">
<li value="1">Go to a project whose sharing permissions you want to view. </li>
<li value="2"> Click the <strong>More</strong> menu <img src="assets/more-icon.png">, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>Expand the <strong>Inherited Permissions</strong> list. </p> <p>This list displays the names of users that have access to either the portfolio or the program that the project belongs to and also have permissions to the project. </p>  </li>
</ol>
</div>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a project whose sharing permissions you want for all projects you create from scratch. (NOTE: drafted because linked above)&nbsp;</li>
<li value="2"> Click the More menu, then click <strong>Sharing</strong>. </li>
<li value="3"> <p>In the Project Access box that displays, near the upper-right corner, click the gear icon <img src="assets/gear-icon-settings.png">, then click <strong>Set as my project access template</strong>.</p> <p>The entities that are granted permissions on the selected project have the same permissions for all the projects you create from scratch in the future.</p> <p> The project access template overrides the sharing defaults granted to you by the Workfront administrator in your Access Level.<br>For more information about specifying sharing defaults for projects in the Access Level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>.</p> </li>
<li value="4">Click <strong>Save</strong>.</li>
</ol>
-->

## Einschränkungen für verschiedene Lizenztypen

* Benutzer mit einer Worker-Lizenz sind nicht berechtigt, Projekte zu verwalten. Für Worker lautet die höchste Freigabeberechtigung Contribute.
* Benutzer mit einer Anfragelizenz können Projektinformationen anzeigen, haben jedoch eingeschränkten Projektzugriff.
* Eine Ausnahme vom Ändern des Status eines Projekts tritt auf, wenn ein(e) Benutzende(r) mit der Berechtigung Anzeigen oder Contribute ebenfalls in einen Genehmigungsprozess eingeschlossen ist. Sie können das Projekt genehmigen, was den Status des Projekts ändert, aber der Status ist der vordefinierte Status für die Genehmigung oder Ablehnung.
* Um ein Projekt kopieren zu können, muss ein Benutzer auch Zugriff zum Erstellen von Projekten auf seiner Zugriffsebene haben.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Configure default permissions for a project</h2>
<p>(NOTE: drafted because I added one more way to automatically share the project above in the bullet list and linked it to Edit Projects) </p>
<p>As a project owner, you can configure the default permissions for View, Manage, and Contribute access that are used when sharing&nbsp;the project with others. When users share a project, the default permissions are used. Users can then adjust the default permissions when sharing the project, as described in <a title="Project Permissions" href="#ways-to-share-a-project" class="MCXref xref">Ways to share a project</a>. </p>
<p>To configure the default permissions that are included with each access level:</p>
<ol>
<li value="1">Go to the project where you want to set the default permissions.</li>
<li value="2"> <p>Click the More menu <img src="assets/more-icon.png">, then click <strong>Edit</strong>. <img src="assets/edit-icon.png"></p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> </p> </li>
<li value="3">Click <strong>Access</strong> in the list on the left.</li>
<li value="4"> <p>In the <strong>When someone is given access to this PROJECT</strong> section, select permissions that you want to be available when users are given access to the project via sharing.</p> <p>Ensure that any permissions that you want to include in the selected access level are selected and deselect any permissions that you do not want to include in the selected permissions level.</p> <p>To view which permissions are available for each level, see&nbsp;<a title="Project Permissions" href="#Understanding_Project_Permissions" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <note type="note">
The
<strong>Delete</strong> access in the
<strong>Manage</strong> permission level determines whether users can&nbsp;delete the project itself. Users with
<strong>Manage</strong> access to the project can delete tasks and issues within the project regardless of whether this option is selected, if they have
<strong>Manage</strong> permissions to the tasks and issues.&nbsp;
</note> </li>
<li value="5">Click <strong>Save Changes</strong>.</li>
</ol>
</div>
-->

## Optionen für Projektberechtigungen

In der folgenden Tabelle sind die Berechtigungen aufgeführt, die Benutzer bei der Freigabe eines Projekts erteilen können. Weitere Informationen dazu, welchen Zugriff Benutzer auf ihrer Lizenz erhalten, finden Sie unter [Zugriff auf Projekte gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Aktionen</strong> </p> </th> 
   <th> <p><strong>Verwalten</strong> </p> </th> 
   <th> <p><strong>Contribute</strong> </p> </th> 
   <th> <p><strong>Anzeigen</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Benutzerdefiniertes Formular hinzufügen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Benutzerdefinierte Felder aktualisieren</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Genehmigungsprozess hinzufügen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Genehmigen eines Projekts</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Stunden genehmigen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓ </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Erstellen eines Projekts</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Dokument(e) hinzufügen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Anfrage(n) hinzufügen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aufgabe(n) hinzufügen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt kopieren</p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt löschen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Geplante Daten ändern</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt freigeben</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Systemweit teilen</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt anzeigen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktualisierungen/Kommentare</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Status ändern</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Stunden protokollieren</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Zuweisungen bearbeiten</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Baseline verwalten</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Risiken verwalten*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Finanzen verwalten*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Kosten hinzufügen/bearbeiten*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Finanzen anzeigen*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Vorlage anfügen</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Als Vorlage speichern</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Business Case hinzufügen/bearbeiten</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projektdetails bearbeiten</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Personal bearbeiten</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>In MS Project exportieren</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Neuberechnen der Finanzen/des Zeitplans*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Festlegen von Warteschlangeneigenschaften</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p>  </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt stapelweise in einer Liste bearbeiten</p> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Benutzende ohne Zugriff auf Finanzdaten können Risiken und Finanzen für Projekte nicht verwalten, auch wenn sie Bearbeitungszugriff auf Projekte haben. Informationen zum Zugriff auf Finanzdaten finden Sie unter [Zugriff auf Finanzdaten gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
