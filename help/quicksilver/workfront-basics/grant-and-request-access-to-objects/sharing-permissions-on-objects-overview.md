---
content-type: overview
navigation-topic: grant-and-request-access-to-objects
title: Übersicht über Freigabeberechtigungen für Objekte
description: Sie können Berechtigungen für ein von Ihnen erstelltes Objekt oder ein für Sie freigegebenes Objekt freigeben oder entfernen.
author: Courtney
feature: Get Started with Workfront
exl-id: 7c14702e-ac55-4266-88a7-f31618f84218
source-git-commit: 97f5adc8811a3be7be23137a82d10d45b76ec605
workflow-type: tm+mt
source-wordcount: '1332'
ht-degree: 1%

---

# Übersicht über Freigabeberechtigungen für Objekte

<!-- Audited: 12/2023 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Redundancy here with the article Permissions for shared objects?</p>
-->
Wenn Sie ein Objekt für eine Person im System freigeben, können Sie der Empfängerin bzw. dem Empfänger eine der folgenden Berechtigungen erteilen: Anzeigen, Mitwirken und Verwalten.

Sie müssen kein Adobe Workfront-Administrator sein, um Berechtigungen für Objekte freizugeben, auf die Sie Zugriff haben, aber Ihre Berechtigungen für Objekte funktionieren innerhalb der Zugriffsebenen, die vom Workfront-Administrator festgelegt wurden.

Sie können Berechtigungen für ein von Ihnen erstelltes Objekt oder ein für Sie freigegebenes Objekt freigeben oder entfernen. Wenn Sie nicht der Ersteller des -Objekts sind, müssen Sie zusätzlich zu den Freigabeberechtigungen für das -Objekt über Freigabeberechtigungen für das -Objekt verfügen, das Sie auf Ihrer Zugriffsebene freigeben möchten. Weitere Informationen zu Zugriffsebenen finden Sie unter [Übersicht über neue Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) oder [Übersicht über Zugriffsebenen](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!NOTE]
>
>Ein Workfront-Administrator kann für alle Benutzenden Berechtigungen zu Elementen im System hinzufügen oder entfernen, ohne Besitzer dieser Elemente zu sein.

## Objekte, die Sie in Workfront freigeben können

Sie können die folgenden Objekte in Workfront für andere Benutzer freigeben:

* **Projekte**: Weitere Informationen finden Sie unter [Freigeben eines Projekts in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* **Vorlagen**: Weitere Informationen finden Sie unter &quot;[&#x200B; von Projektvorlagen](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* **Portfolios**: Weitere Informationen finden Sie unter [Freigeben eines Portfolios](../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio.md).

* **Programme**: Weitere Informationen finden Sie unter [Freigeben eines Programms](../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md) .

* **Aufgaben**: Weitere Informationen finden Sie unter [Freigeben einer Aufgabe](../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

* **Probleme**: Weitere Informationen finden Sie unter [Freigeben eines Problems](../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

* **Dokumente**: Weitere Informationen finden Sie unter [Freigeben eines Dokuments](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

* **Dokumentordner**: Weitere Informationen finden Sie unter [Freigeben eines Dokumentordners](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

* **Korrekturabzüge**: Weitere Informationen finden Sie unter [Freigeben eines Korrekturabzugs in Workfront](/help/quicksilver/review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* **Berichte, Dashboards und Kalender**: Weitere Informationen finden Sie unter [Freigeben von Berichten, Dashboards und Kalendern](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).  Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Freigeben eines Berichts in Adobe Workfront](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [Dashboard freigeben](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [Kalenderbericht freigeben](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* **Filter, Ansichten und Gruppierungen**: Weitere Informationen finden Sie unter [Freigeben von Filtern, Ansichten oder Gruppierungen](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

* **Pläne**: Weitere Informationen finden Sie unter [Freigeben eines Plans im Szenario-Planer](../../scenario-planner/share-a-plan.md).

  Dies erfordert eine zusätzliche Lizenz.

* **Ziele**: Weitere Informationen finden Sie unter [Freigeben eines Ziels in Workfront Goals](../../workfront-goals/workfront-goals-settings/share-a-goal.md).

  Dies erfordert eine zusätzliche Lizenz.

## Überlegungen zur Freigabe von Objekten

* Sie können nur die gleiche oder eine niedrigere Berechtigungsstufe für das Objekt freigeben.

  Wenn Sie beispielsweise über Beitragsberechtigungen für das Objekt verfügen, können Sie keinem anderen Benutzer Berechtigungen zum Verwalten für dieses Objekt erteilen.

* Sie können kein Objekt mit einer Berechtigungsstufe freigeben, die höher ist als die Zugriffsebene eines Benutzers.

  Wenn ein(e) Benutzende(r) beispielsweise auf der Zugriffsebene Ansichtszugriff auf Projekte hat, können Sie ihm/ihr keine Verwaltungsberechtigungen für ein Projekt erteilen.
* Ein Benutzer mit der Berechtigung Anzeigen kann dieses Objekt zumindest für eine andere Person freigeben.
* Sie können Objekte für aktive Benutzer, Aufgabengebiete, Teams, Gruppen oder Unternehmen freigeben.

  >[!NOTE]
  >
  >Sie können einen Plan oder ein Ziel nur für andere aktive Benutzende freigeben. Dies erfordert zusätzliche Lizenzen.
  >
  >
  >Weitere Informationen finden Sie unter:
  >
  >* [Plan im Szenario-Planer freigeben](../../scenario-planner/share-a-plan.md)
  >* [Teilen Sie ein Ziel in Workfront Goals](../../workfront-goals/workfront-goals-settings/share-a-goal.md)

* Workfront sendet Benachrichtigungen an Benutzer, wenn Sie ein Objekt für sie freigeben. Benachrichtigungen werden gesendet, wenn beide Einstellungen aktiviert sind:

   * Die E **Mail-Benachrichtigungen &quot;** für Benutzer“ und **Objektfreigabe für Team** werden im Bereich „Setup“ von einem System- oder Gruppenadministrator aktiviert. Weitere Informationen finden Sie unter [Konfigurieren von Ereignisbenachrichtigungen für alle Personen im System](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
   * Die **Jemand gibt ein Objekt für mich frei** und **Jemand gibt ein Objekt für mein Team frei** werden Benachrichtigungen auf der Profilseite des Benutzers aktiviert. Weitere Informationen finden Sie unter [Eigene E-Mail-Benachrichtigungen ändern](/help/quicksilver/workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  Die Einstellungen auf System- oder Gruppenebene müssen zuerst aktiviert werden, bevor Sie die Benachrichtigungseinstellungen für den Benutzer aktivieren können.

## Freigabebeschränkungen

* Sie können ein Objekt für bis zu 100 Entitäten (Benutzer, Teams, Gruppen, Aufgabengebiete, Unternehmen) freigeben. Es wird empfohlen, Objekte für Gruppen, Teams oder Unternehmen freizugeben, anstatt sie für einzelne Benutzer freizugeben, um diese Einschränkung zu vermeiden.
* Ein Benutzer, dessen Zugriffsebene keinen Zugriff auf Finanzdaten zulässt, kann keinen Zugriff gewähren, der es anderen ermöglicht, Finanzdaten anzuzeigen. Dazu gehört der Zugriff auf Projekte, die Finanzdaten anzeigen, oder die Änderung einer Zugriffsebene, um die Anzeige von Finanzdaten zu ermöglichen.


## Freigeben von Berechtigungen für Objekte

Die folgende Tabelle zeigt die Berechtigungsstufe, die Sie bei der Freigabe eines Objekts auswählen können. Nicht für alle Objekte sind diese Einstellungen verfügbar. Sie können einer anderen Entität Berechtigungen zum Anzeigen oder Verwalten eines Objekts erteilen. Wenn Sie ein Projekt, eine Aufgabe oder ein Problem freigeben, können Sie auch Berechtigungen zum Mitwirken erteilen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Ansicht</strong></td> 
   <td> <p>Sie können die folgenden Aktionen für das Objekt ausführen:</p> 
    <ul> 
     <li><p>Objekt anzeigen</p></li> 
     <li><p>Hinzufügen von Dokumenten zum Objekt</p></li> 
     <li><p>Probleme zum Objekt hinzufügen (wenn es sich um eine Aufgabe oder ein Projekt handelt)</p></li> 
     <li><p>Finanzinformationen zum Objekt anzeigen</p></li> 
     <li> <p>Objekt freigeben<br></p> <p>Wenn Sie das -Objekt freigeben, können Sie anderen Benutzern dieselbe Berechtigungsstufe gewähren, die Sie nur für das -Objekt haben, keine höhere Ebene.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Mitwirken</strong></td> 
   <td> <p>Sie können die folgenden Aktionen für das Objekt ausführen:</p> 
    <ul> 
     <li>Alle Aktionen, die in der Berechtigung Anzeigen enthalten sind.</li> 
     <li>Kosten hinzufügen</li> 
     <li>Aufgaben hinzufügen (wenn es sich um ein Projekt handelt)</li> 
     <li>Benutzerdefinierte Forms darauf bearbeiten</li> 
     <li>Stunden für das Objekt protokollieren</li> 
     <li>Zuweisungen daran vornehmen</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Verwalten</strong></td> 
   <td> <p>Sie können die folgenden Aktionen für das Objekt ausführen:</p> 
    <ul> 
     <li>Alle Aktionen, die mit den Berechtigungen „Anzeigen“ und „Beitragen“ enthalten sind</li> 
     <li>Löschen</li> 
     <li>Finanzinformationen in IT verwalten</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Für externe Benutzende öffentlich machen</strong></td> 
   <td> <p>Jeder ohne Workfront-Konto kann das Objekt durch Klicken auf einen Link anzeigen. Dies ist nicht für alle Objekte verfügbar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Systemweit sichtbar machen.</strong></td> 
   <td> <p>Das -Objekt kann bei Suchvorgängen gefunden und von Benutzenden mit einem Workfront-Konto angezeigt werden.</p><p><b>Hinweis</b>: Benutzer mit einer Beitragenden - oder Anfordererlizenz können Projekte nicht sehen, selbst wenn diese Einstellung aktiviert ist. </td> 
  </tr> 
 </tbody> 
</table>

## Grundlegendes zu geerbten Berechtigungen und der Hierarchie von Objekten

### Berechtigungen geerbt von übergeordneten Objekten {#permissions-inherited-from-parent-objects}

Berechtigungen werden in Workfront hierarchisch vererbt. Wenn Sie also einem Benutzer Berechtigungen für ein übergeordnetes Objekt erteilen, erhält er standardmäßig dieselben Berechtigungen für die untergeordneten Objekte, die ihm zugeordnet sind.

Wenn Sie beispielsweise einem Benutzer die Berechtigung Beitragen für ein Projekt erteilen, verfügt der Benutzer über die Berechtigung Beitragen für alle Aufgaben und Probleme (untergeordnete Objekte), die mit diesem Projekt verknüpft sind.

Um mit dem obigen Beispiel fortzufahren, können Sie Berechtigungen nicht auf untergeordnete Objekte beschränken. Wenn Sie nicht möchten, dass der Benutzer über Beitragsberechtigungen für untergeordnete Objekte verfügt, die mit dem Projekt verknüpft sind, müssen Sie die geerbten Berechtigungen manuell aus den Objekten entfernen und dann die Berechtigungen für einzelne Benutzer anpassen, einschließlich aller erweiterten Einstellungen.

Weitere Informationen zur Hierarchie und Interdependenz von Objekten in Workfront finden Sie im Abschnitt [Interdependenz und Hierarchie der Objekte](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#interdependency-and-hierarchy-of-objects) im Artikel [Übersicht über Adobe Workfront-Objekte](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Ihr Workfront-Administrator kann geerbte Berechtigungen für Dokumente auf Ihrer Zugriffsebene deaktivieren.  Weitere Informationen zum Deaktivieren von geerbten Berechtigungen für Dokumente in der Zugriffsebene finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### Durch Organisationsmitgliedschaften erworbene Berechtigungen   {#permissions-acquired-through-organizational-memberships}

Wenn Sie einer Benutzergruppe für ein Objekt Verwaltungsberechtigungen erteilen und einem einzelnen Benutzer in dieser Gruppe für dasselbe Objekt Ansichtsberechtigungen erteilen, verfügt der Benutzer über die höchste Berechtigungsstufe (Verwalten), die über die Gruppenmitgliedschaft für das Objekt gewährt wurde.

Wenn Sie einem Benutzer, der bereits Teil einer Organisationseinheit (Gruppe, Team, Aufgabengebiet oder Unternehmen) mit einer höheren Berechtigungsstufe ist, niedrigere Berechtigungen erteilen möchten, müssen Sie die Berechtigungen aus der Organisationseinheit entfernen und Benutzer einzeln mit einer niedrigeren Berechtigungsstufe hinzufügen.


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Remove permissions from objects</h2>
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">AL: draft/ hide this div when Becky makes Remove permissions from objects live and replace with the drafted content with the link at the top of this section</p>
<p>You can remove permissions from objects you have access to Share. Removing permissions from objects is identical for all objects that can be shared.  </p> <note type="note">
  You cannot remove permissions when you share items in bulk. You can remove permissions only when selecting individual items.  
</note>
<p>To remove permissions from objects consider the following:  </p>
<ul>
<li><a href="#remove-entities-from-the-sharing-list-of-an-object" class="MCXref xref">Remove entities from the sharing list of an object</a> </li>
<li><a href="#remove-inherited-permissions" class="MCXref xref">Remove inherited permissions</a> </li>
<li><a href="#make-an-object-private" class="MCXref xref">Make an object private</a> </li>
</ul>
<p><strong>Remove entities from the sharing list of an object</strong></p>
<p>You can remove entities from the sharing list of an object to remove their permissions from the object.</p>
<p>To remove permissions from objects:  </p>
<ol>
<li value="1">Navigate to an object on which you want to modify the permissions.</li>
<li value="2">Click the <strong>Actions</strong> menu, then click <strong>Sharing</strong>.<br>For example, on a project, click <strong>Project Actions</strong>, then <strong>Sharing</strong>.  </li>
<li value="3">Click the <strong>x</strong> next to the name of a user, team, group, company, job role to remove them.<br></li>
<li value="4">In the <strong><User Name>'s Workfront access will be removed from this</strong> drop-down menu, select whether you want their access to be removed just from the object you have selected, or from all children objects associated with it.<br>The following scenarios exist:
<ul>
<li>If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they are granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.  </li>
<li>If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they have been given individual permission on each child object.  </li>
</ul></li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<p> <p><strong>Remove inherited permissions</strong></p> </p>
<p>Inherited permissions can be removed from objects allowing for owners to specifically  identify who will get access to children objects regardless of the access of a user to a parent object. Only users with Manage permission are able to remove inherited permissions.</p>
<p>To remove inherited permissions:</p>
<ol>
<li value="1">Navigate to an object to which you have Manage permissions. <br>For example, navigate to a task.</li>
<li value="2">Go to the sharing list as described in the <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> section in this article. </li>
<li value="3">Select the <strong>X</strong>  mark next to <strong>Inherited Permission</strong>  on the sharing box to remove  anyone listed there.<br><br>This ensures that no one who is granted permissions to the parent object (for example, the project) has permissions to this task by default. You must list   individual entities in the sharing list of the task to grant permissions on the task.<br><note type="note">
You cannot remove individual entities from the Inherited Permissions list. You can only disable the Inherited Permissions for all entities listed.
</note></li>
<li value="4">Click <strong>Save</strong>.  </li>
</ol>
<p><strong>Make an object private</strong></p>
<p>If you have shared an object system-wide, or you have shared it with external uses by making it public, you can make it private again by removing the system-wide or public permissions.  </p>
<p>For more information about making an object available system-wide, or publicly, see the section <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> in this article.</p>
<p>To make an object private:</p>
<ol>
<li value="1">Go to the object you want to make private.<br>For example, navigate to a report.</li>
<li value="2">Click <strong>Report Actions</strong>, then <strong>Sharing</strong>.<br><br></li>
<li value="3">Click <strong>Remove public access</strong> to remove the access of external users to viewing the report.</li>
<li value="4">Click <strong>Remove system-wide access</strong> to stop sharing it with all Workfront users.  </li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Freigeben eines Objekts

Informationen zum Freigeben von Objekten finden Sie unter [Freigeben eines Objekts](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

## Entfernen von Berechtigungen aus Objekten

Informationen zum Entfernen von Berechtigungen aus Objekten finden Sie unter [Entfernen von Berechtigungen aus Objekten](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Anfordern von Berechtigungen für Objekte

Wenn Ihnen jemand einen Link zu einem Objekt sendet, für das Sie keine Anzeigeberechtigungen haben, oder wenn Sie niedrigere Berechtigungen für ein Objekt haben und eine höhere Berechtigungsstufe anfordern möchten, können Sie Berechtigungen für das Objekt anfordern.

Sie können von jeder Person Zugriff auf ein Objekt anfordern, die über Freigabeberechtigungen für das Objekt verfügt.

Weitere Informationen zum Anfordern von Berechtigungen für Objekte finden Sie unter [Anfordern von Zugriff auf Objekte](../../workfront-basics/grant-and-request-access-to-objects/request-access.md).
