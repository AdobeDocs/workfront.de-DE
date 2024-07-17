---
title: Freigeben eines Projekts in Adobe Workfront
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Ihr Adobe Workfront-Administrator kann Ihnen beim Zuweisen Ihrer Zugriffsebene Zugriff auf das Anzeigen oder Bearbeiten von Projekten gewähren. Weitere Informationen finden Sie unter Gewähren von Zugriff auf Projekte.
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

Ihr Adobe Workfront-Administrator kann Ihnen beim Zuweisen Ihrer Zugriffsebene Zugriff auf das Anzeigen oder Bearbeiten von Projekten gewähren. Weitere Informationen finden Sie unter [Gewähren des Zugriffs auf Projekte](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

Neben der Zugriffsstufe, die Benutzern zugewiesen wird, können Sie ihnen auch Berechtigungen für die Anzeige, Contribute oder Verwaltung bestimmter Projekte erteilen, auf die Sie Zugriff haben.

Berechtigungen beziehen sich auf ein Element in Workfront und legen fest, welche Aktionen für dieses Element durchgeführt werden können.

## Überlegungen zum Freigeben von Projekten

Weitere Informationen finden Sie unter [Übersicht über die Freigabe von Berechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Standardmäßig ist der Ersteller eines Projekts berechtigt, das Projekt zu verwalten, und ist auch als Projekteigentümer ausgewiesen. Wenn das Projekt einem anderen Eigentümer zugewiesen ist, hat dieser Benutzer auch die Berechtigung zum Verwalten des Projekts. Wenn der Projektersteller (oder -inhaber) das Projekt mit anderen Benutzern teilt, erteilen er diesen Benutzern bestimmte Berechtigungen, um zu steuern, was sie bei der Arbeit am Projekt tun können.

  Wenn ein Projekteigentümer jedoch nicht über eine Planner-Lizenz verfügt, hat er keinen vollen Zugriff auf die Verwaltung des Projekts. Nur Benutzer mit einer Planungslizenz können zur Verwaltung eines Projekts berechtigt sein. Weitere Informationen finden Sie unter [Wie Zugriffsebenen und Berechtigungen zusammenarbeiten](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

* Sie können Projekte einzeln oder mehrere freigeben. Die Freigabe von Projekten ist mit der Freigabe anderer Objekte identisch. Weitere Informationen zum Freigeben von Elementen in Workfront finden Sie unter [Freigeben eines Objekts](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).
* Sie können einem Projekt die folgenden Berechtigungen erteilen:

   * Anzeigen
   * Verwalten
   * Mitwirken

     ![](assets/view-on-projects-190x207.png) ![](assets/contribute-on-projects-159x243.png) ![](assets/manage-on-projects-178x230.png)

* Wenn Sie ein Projekt freigeben, erben alle Aufgaben, Probleme und Dokumente dieselben Berechtigungen, sofern nicht anders angegeben.

  Informationen zum Verwalten des Zugriffs auf Aufgaben und Probleme im Projekt basierend auf den Berechtigungen eines Benutzers für das Projekt finden Sie im Abschnitt [](../../manage-work/projects/manage-projects/edit-projects.md#access) im Artikel [Projekte bearbeiten](../../manage-work/projects/manage-projects/edit-projects.md).

  Der Workfront-Administrator kann angeben, ob Dokumente Berechtigungen von höheren Objekten in der Zugriffsebene des Benutzers erben sollen. Weitere Informationen zum Einschränken von geerbten Berechtigungen auf Dokumente finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Sie können geerbte Berechtigungen aus einem Projekt entfernen, damit die untergeordneten Objekte sie nicht übernehmen. Weitere Informationen zum Entfernen von geerbten Berechtigungen aus Objekten finden Sie unter [Berechtigungen aus Objekten entfernen](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Möglichkeiten zum Freigeben eines Projekts {#ways-to-share-a-project}

Sie können ein Projekt wie folgt freigeben:

* Führen Sie manuell einen der folgenden Schritte aus:

   * Hinzufügen von Benutzern zum Projektteam. Wenn Sie Benutzer zum Projektteam hinzufügen, erhalten sie automatisch Anzeigeberechtigungen für das Projekt.\
     Weitere Informationen zum Hinzufügen von Benutzern zu einem Projektteam finden Sie im Abschnitt &quot;Hinzufügen von Benutzern zu einem Projektteam&quot;in der [Übersicht über das Projektteam](../../manage-work/projects/planning-a-project/project-team-overview.md).
   * Einzelne Freigabe oder Massenweitergabe der Projekte bei Verwendung der Option **Freigabe**.

     Die Freigabe eines Projekts ähnelt der Freigabe aller anderen Objekte in Adobe Workfront.

     Informationen zum Freigeben von Objekten in Workfront finden Sie unter [Freigeben eines Objekts](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Führen Sie automatisch einen der folgenden Schritte aus:

   * Platzieren Sie ein Projekt in ein **Portfolio** oder ein **Programm**, das bereits für andere freigegeben ist. Benutzer erhalten dieselben Berechtigungen für das Projekt, die sie für das Portfolio oder Programm haben.\
     Informationen zum Hinzufügen eines Projekts zu einem **Portfolio** finden Sie unter [Hinzufügen von Projekten zu einem Portfolio](../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).\
     Weitere Informationen zum Hinzufügen eines Projekts zu einem **Programm** finden Sie unter [Hinzufügen eines Projekts zu einem Programm](../../manage-work/portfolios/create-and-manage-programs/add-project-to-program.md).

     Weitere Informationen zum Anzeigen von geerbten Berechtigungen für ein Objekt finden Sie unter [Anzeigen von geerbten Berechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

   * Fügen Sie Entitäten zur Projektfreigabe in einer Vorlage hinzu, die zum Erstellen des Projekts verwendet wird. Informationen zum Freigeben von Projekten aus Vorlagen finden Sie unter [Freigeben einer Vorlage](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).
   * Definieren Sie die Vorlage für den Projektzugriff.

     Informationen zum Definieren der Projektzugriffsvorlage finden Sie unter [Freigeben eines Objekts](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

     >[!TIP]
     >
     >Beim Anhängen oder Speichern einer Vorlage können Sie die Regeln für die Projektfreigabe in Vorlagen löschen.

   * Bearbeiten Sie ein Projekt und definieren Sie die Einstellung &quot;**Wenn jemand Zugriff auf dieses Projekt erhält&quot;** . Weitere Informationen finden Sie unter [Projekte bearbeiten](../../manage-work/projects/manage-projects/edit-projects.md).

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

* Benutzer mit einer Worker-Lizenz verfügen nicht über die Berechtigung zum Verwalten von Projekten. Für Arbeitnehmer ist Contribute die höchste Freigabeberechtigung.
* Benutzer mit einer Anforderungslizenz können Projektinformationen anzeigen, haben jedoch eingeschränkten Projektzugriff.
* Eine Ausnahme bildet die Änderung des Projektstatus, wenn ein Benutzer mit der Berechtigung zum Anzeigen oder Contribute auch in einem Genehmigungsprozess enthalten ist. Sie können das Projekt genehmigen, wodurch der Status des Projekts geändert wird. Der Status ist jedoch der vordefinierte Status für die Genehmigung oder die Ablehnung.
* Um ein Projekt kopieren zu können, muss ein Benutzer auch Zugriff haben, um Projekte in seiner Zugriffsebene zu erstellen.

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

In der folgenden Tabelle sind die Berechtigungen aufgeführt, die Benutzer beim Freigeben eines Projekts gewähren können. Weitere Informationen dazu, welche Zugriffsberechtigungen Benutzer auf der Grundlage ihrer Lizenz erhalten, finden Sie unter [Gewähren des Zugriffs auf Projekte](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

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
   <td> <p>Hinzufügen eines Validierungsprozesses</p> </td> 
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
   <td> <p>Problem(e) hinzufügen</p> </td> 
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
   <td> <p>Geplante Datumswerte ändern</p> </td> 
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
   <td> <p>Grundlinie verwalten</p> </td> 
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
   <td> <p>Verwalten von Finanzverwalten*</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Hinzufügen/Bearbeiten von Ausgaben*</p> </td> 
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
   <td> <p>Geschäftsszenario hinzufügen/bearbeiten</p> </td> 
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
   <td> <p>Bearbeiten von Personal</p> </td> 
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
   <td> <p>Finanz-/Zeitleiste neu berechnen*</p> </td> 
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
   <td> <p>Projekt in einer Liste stapelweise bearbeiten</p> </td> 
   <td> <p>✓</p> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Benutzer ohne Zugriff auf Finanzdaten können Risiken und Finanzen für Projekte nicht verwalten, selbst wenn sie Zugriff auf Projekte bearbeiten haben. Informationen zum Zugriff auf Finanzdaten finden Sie unter [Zugriff auf Finanzdaten gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
