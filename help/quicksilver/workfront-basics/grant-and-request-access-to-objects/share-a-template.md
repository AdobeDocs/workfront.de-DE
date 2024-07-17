---
title: Vorlage freigeben
product-area: templates
navigation-topic: grant-and-request-access-to-objects
description: Als Adobe Workfront-Administrator können Sie Benutzern Zugriff auf das Anzeigen oder Bearbeiten von Vorlagen gewähren, wenn Sie ihre Zugriffsebene zuweisen. Ein Benutzer muss über eine Planungslizenz verfügen, um Zugriff auf Vorlagen bearbeiten zu haben.
author: Alina
feature: Get Started with Workfront
exl-id: 19fb0de5-7db5-42a9-9f33-a4570acfeef8
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 2%

---

# Vorlage freigeben

Als Adobe Workfront-Administrator können Sie Benutzern Zugriff auf das Anzeigen oder Bearbeiten von Vorlagen gewähren, wenn Sie ihre Zugriffsebene zuweisen. Ein Benutzer muss über eine Planungslizenz verfügen, um Zugriff auf Vorlagen bearbeiten zu haben.

Weitere Informationen zur Gewährung des Zugriffs auf Vorlagen finden Sie unter [Gewähren des Zugriffs auf Vorlagen](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md).

Neben der Zugriffsstufe, die Sie gewähren, können Benutzer auch von anderen Benutzern, die sie teilen, Berechtigungen zum Anzeigen oder Verwalten bestimmter Vorlagen erhalten.

>[!NOTE]
>
>Berechtigungsstufen funktionieren innerhalb der Zugriffsebenen. Beispielsweise kann ein Benutzer keine Berechtigungen zum Verwalten einer Vorlage erhalten, wenn seine Zugriffsebene es ihm nur ermöglicht, Vorlagen anzuzeigen.

Berechtigungen beziehen sich auf ein Element in Workfront und legen fest, welche Aktionen für dieses Element durchgeführt werden können.

## Überlegungen zum Freigeben einer Vorlage

* Weitere Informationen finden Sie unter [Übersicht über die Freigabe von Berechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).
* Der Ersteller einer Vorlage sowie der Vorlageneigentümer haben standardmäßig die Berechtigung &quot;Verwalten&quot;für die Vorlage. Weitere Informationen zum Benennen eines Benutzers als Vorlageninhaber finden Sie unter [Bearbeiten von Projektvorlagen](../../manage-work/projects/create-and-manage-templates/edit-templates.md).
* Beim Freigeben einer Vorlage können Sie Folgendes freigeben:

   * Die Vorlage

     Weitere Informationen zum Freigeben einer Vorlage finden Sie unter [Projektvorlagen freigeben](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

     Sie können einer Vorlage die folgenden Berechtigungen erteilen:

      * Anzeigen

        ![](assets/view-on-template-262x221.png)

      * Verwalten

        ![](assets/manage-on-template-225x280.png)

   * Die künftigen Projekte, die mithilfe der Vorlage erstellt werden. Sie können für Projekte, die aus einer Vorlage erstellt wurden, dieselben Berechtigungen erteilen wie für einzelne Projekte. 

     Informationen zum Freigeben eines Projekts aus einer Vorlage auf Vorlagenebene finden Sie unter [Projektvorlagen freigeben](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* Wenn Sie eine Vorlage oder ein Projekt freigeben, das aus der Vorlage erstellt wird, erben Benutzer standardmäßig dieselben Berechtigungen für alle untergeordneten Objekte, die mit der Vorlage oder dem Projekt verknüpft sind.

  Weitere Informationen zur Hierarchie von Objekten in Workfront finden Sie unter  [Objekte in Adobe Workfront verstehen](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* Wenn Sie eine Vorlage freigeben, erben alle Vorlagenaufgaben und -dokumente sowie die Probleme im zukünftigen Projekt, die aus der Vorlage erstellt werden, dieselben Berechtigungen, sofern nicht anders angegeben.

  Informationen zum Verwalten des Zugriffs auf Vorlagenaufgaben und Probleme im Projekt basierend auf den Berechtigungen eines Benutzers für das Projekt finden Sie im Abschnitt [Zugriff](../../manage-work/projects/create-and-manage-templates/edit-templates.md#access) im Artikel [Bearbeiten von Projektvorlagen](../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* Der Workfront-Administrator kann angeben, ob Dokumente Berechtigungen von höheren Objekten in der Zugriffsebene des Benutzers erben sollen. Weitere Informationen zum Einschränken von geerbten Berechtigungen auf Dokumente finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Share a template</h2>
<p>(NOTE: drafted because this is also linked above: Share project templates >> which is an article in the Manage Work section>> Templates)&nbsp;</p>
<ol>
<li value="1"> <p>Go to the template you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Template Sharing</strong>.<br>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Template</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing the name of a user, group, team, job role, or company that you want to share the template with in the <strong>Give template access to</strong> or <strong>Edit template access for</strong> fields.</p> <p>Select them when they appear in the list.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant:<br>
<ul>
<li><p><strong>View it</strong>: Users with these permissions are able to view the template and create a project using it, or attach it to an existing project.</p><p><img src="assets/template-permissions-350x197.png" alt="template_permissions.png" style="width: 350;height: 197;"></p></li>
<li><strong>Manage it</strong>: Users with these permissions are able to edit or delete the template.</li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions.</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<h2>Share a project at the template level</h2>
<p>You can share the future projects that are created using a template with users at the template level.</p>
<ol>
<li value="1"> <p>Go to the template whose future projects you want to share with other entities, click <strong>Template Actions</strong>, then <strong>Project Sharing</strong>.</p> <p>Or</p> <p>Navigate to a list of templates, and select multiple templates from the list, then click <strong>Share Project</strong>.</p> <note type="note">
If you select multiple templates, you cannot view who already has project permissions to the individual templates.
</note> </li>
<li value="2"> <p>Start typing and then select the name of a user, group, team, job role, or company with whom you want to share future projects created from the template in the <strong>Give project access to</strong> or <strong>Edit template access for</strong> fields.</p> <note type="tip">
You can share an object only with active users, teams,
<span>roles,</span> or companies.
</note> </li>
<li value="3">From the drop-down menu, select which level of permissions you want to grant.<br>Select from the following:<br>
<ul>
<li><strong>No access</strong>: You can specify which users will not have any access to the template.<br>This option is available only when bulk sharing projects from templates.&nbsp;</li>
<li><strong>View</strong>: Users with these permissions can view projects created from the template.</li>
<li><strong>Contribute</strong>: Users with these permissions can contribute to projects created from the template&nbsp;</li>
<li><strong>Manage</strong>: Users with these permissions can manage or delete projects created from this template.<br><img src="assets/share-project-from-template-350x268.png" alt="share_project_from_template.png" style="width: 350;height: 268;"></li>
</ul></li>
<li value="4">(Optional) Click <strong>Advanced Settings</strong> to fine-tune your settings for each level of permissions. </li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Erweiterte Einstellungen für die Vorlagenfreigabe

Die folgende Tabelle zeigt, welche Berechtigungen Sie Benutzern gewähren können, wenn sie eine Vorlage anzeigen oder verwalten können. Anweisungen zum Freigeben einer Vorlage finden Sie im Abschnitt [Vorlage freigeben](../../manage-work/projects/create-and-manage-templates/share-project-template.md#share) im Artikel [Projektvorlagen freigeben](../../manage-work/projects/create-and-manage-templates/share-project-template.md) .

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Aktionen</th> 
   <th>Verwalten</th> 
   <th>Anzeigen</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Kopieren</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Löschen</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Vorlagendetails bearbeiten</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Vorlage anzeigen</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Freigeben</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Systemweit teilen</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Dokumente hinzufügen</p> <p>Tipp: Manchmal fügen Personen Dokumente zu einer Projektvorlage hinzu, weil sie glauben, sie würden zu einem Projekt hinzugefügt. Sie können dies für Ihre Empfänger verhindern, indem Sie diese Einstellung deaktivieren.</p> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

Informationen zu den Berechtigungen, die Sie Benutzern für Projekte gewähren, die aus einer Vorlage erstellt wurden, finden Sie unter [Freigeben eines Projekts in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
