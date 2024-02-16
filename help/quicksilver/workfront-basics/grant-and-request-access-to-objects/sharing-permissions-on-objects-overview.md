---
content-type: overview
navigation-topic: grant-and-request-access-to-objects
title: Übersicht über die Freigabe von Berechtigungen für Objekte
description: Sie können Berechtigungen für ein von Ihnen erstelltes Objekt oder ein für Sie freigegebenes Objekt freigeben oder daraus entfernen.
author: Alina
feature: Get Started with Workfront
exl-id: 7c14702e-ac55-4266-88a7-f31618f84218
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 0%

---

# Übersicht über die Freigabe von Berechtigungen für Objekte

<!-- Audited: 12/2023 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Redundancy here with the article Permissions for shared objects?</p>
-->
Wenn Sie ein Objekt mit einer Person im System teilen, können Sie dem Empfänger eine der folgenden Berechtigungen erteilen: Anzeigen, Beiträge und Verwalten.

Sie müssen kein Adobe Workfront-Administrator sein, um Berechtigungen für Objekte freigeben zu können, auf die Sie Zugriff haben. Ihre Berechtigungen für Objekte funktionieren jedoch innerhalb der Zugriffsebenen, die vom Workfront-Administrator festgelegt wurden.

Sie können Berechtigungen für ein von Ihnen erstelltes Objekt oder ein für Sie freigegebenes Objekt freigeben oder daraus entfernen. Wenn Sie nicht der Ersteller des Objekts sind, müssen Sie zusätzlich zu den Berechtigungen zum Freigeben für das Objekt über Freigabezugriff für das Objekt verfügen, das Sie auf Ihrer Zugriffsebene freigeben möchten. Informationen zu Zugriffsebenen finden Sie unter [Übersicht über die neuen Zugriffsebenen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md) oder [Übersicht über Zugriffsebenen](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!NOTE]
>
>Ein Workfront-Administrator kann allen Elementen im System Berechtigungen hinzufügen oder entfernen, ohne Eigentümer dieser Elemente zu sein.

## In Workfront freigegebene Objekte

Sie können die folgenden Objekte in Workfront für andere Benutzer freigeben:

* **Projekte**: Weitere Informationen finden Sie unter [Freigeben eines Projekts in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

* **Vorlagen**: Weitere Informationen finden Sie unter [Projektvorlagen freigeben](../../manage-work/projects/create-and-manage-templates/share-project-template.md).

* **Portfolios**: Weitere Informationen finden Sie unter [Portfolio freigeben](../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio.md).

* **Programme**: Weitere Informationen finden Sie unter [Programm freigeben](../../workfront-basics/grant-and-request-access-to-objects/share-a-program.md) .

* **Aufgaben**: Weitere Informationen finden Sie unter [Aufgabe freigeben](../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md).

* **Probleme**: Weitere Informationen finden Sie unter [Problem freigeben](../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md).

* **Dokumente**: Weitere Informationen finden Sie unter [Freigeben eines Dokuments](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

* **Dokumentenordner**: Weitere Informationen finden Sie unter [Dokumentordner freigeben](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

* **Testsendungen**: Weitere Informationen finden Sie unter [Freigeben eines Testversands in Workfront](/help/quicksilver/review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

* **Berichte, Dashboards und Kalender**: Weitere Informationen finden Sie unter [Berichte, Dashboards und Kalender freigeben](../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md). Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Bericht in Adobe Workfront freigeben](../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)
   * [Dashboard freigeben](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md)
   * [Kalenderberichte freigeben](../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md)

* **Filter, Ansichten und Gruppierungen**: Weitere Informationen finden Sie unter [Filter, Ansichten oder Gruppierungen freigeben](../../reports-and-dashboards/reports/reporting-elements/share-filter-view-grouping.md).

* **Pläne**: Weitere Informationen finden Sie unter [Plan im Szenario-Planer freigeben](../../scenario-planner/share-a-plan.md).

  Dies erfordert eine zusätzliche Lizenz.

* **Ziele**: Weitere Informationen finden Sie unter [Freigeben eines Ziels in Workfront-Zielen](../../workfront-goals/workfront-goals-settings/share-a-goal.md).

  Dies erfordert eine zusätzliche Lizenz.

## Überlegungen zum Freigeben von Objekten

* Sie können nur die gleiche oder eine niedrigere Berechtigungsstufe für das Objekt freigeben.

  Wenn Sie beispielsweise über Beitragsberechtigungen für das Objekt verfügen, können Sie keinen anderen Benutzer Verwaltungsberechtigungen für dieses Objekt erteilen.

* Sie können ein Objekt nicht mit einer Berechtigungsebene freigeben, die höher ist als die Zugriffsebene eines Benutzers.

  Wenn ein Benutzer beispielsweise auf der Zugriffsebene Zugriff auf Projekte anzeigen hat, können Sie ihm keine Verwaltungsberechtigungen für ein Projekt erteilen.
* Ein Benutzer mit der Berechtigung zum Anzeigen eines Objekts kann dieses Objekt für eine andere Person freigeben.
* Sie können Objekte für aktive Benutzer, Arbeitsplatzrollen, Teams, Gruppen oder Unternehmen freigeben.

  >[!NOTE]
  >
  >Sie können einen Plan oder ein Ziel nur für andere aktive Benutzer freigeben. Dies erfordert zusätzliche Lizenzen.
  >
  >
  >Weitere Informationen:
  >
  >* [Plan im Szenario-Planer freigeben](../../scenario-planner/share-a-plan.md)
  >* [Freigeben eines Ziels in Workfront-Zielen](../../workfront-goals/workfront-goals-settings/share-a-goal.md)

## Freigabebeschränkungen

Sie können ein Objekt für bis zu 100 Entitäten freigeben (Benutzer, Teams, Gruppen, Jobrollen, Unternehmen). Es wird empfohlen, Objekte für Gruppen, Teams oder Unternehmen und nicht für einzelne Benutzer freizugeben, um diese Einschränkung zu vermeiden.

## Berechtigungen für Objekte freigeben

Die folgende Tabelle zeigt die Höhe der Berechtigungen, die Sie beim Freigeben eines Objekts auswählen können. Nicht alle Objekte verfügen über alle diese Einstellungen. Sie können einer anderen Entität Berechtigungen zum Anzeigen oder Verwalten eines Objekts erteilen. Wenn Sie ein Projekt, eine Aufgabe oder ein Problem freigeben, können Sie auch Berechtigungen erteilen, damit Sie dazu beitragen können.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Anzeigen</strong></td> 
   <td> <p>Sie können die folgenden Aktionen für das Objekt ausführen:</p> 
    <ul> 
     <li><p>Anzeigen des Objekts</p></li> 
     <li><p>Hinzufügen von Dokumenten zum Objekt</p></li> 
     <li><p>Anzeigen von Finanzinformationen zum Objekt</p></li> 
     <li> <p>Objekt freigeben<br></p> <p>Wenn Sie das Objekt freigeben, können Sie anderen Benutzern die gleiche Berechtigungsstufe gewähren, die Sie nur für das Objekt und nicht für eine höhere Ebene haben.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Mitwirken</strong></td> 
   <td> <p>Sie können die folgenden Aktionen für das Objekt ausführen:</p> 
    <ul> 
     <li>Alle Aktionen, die mit der Berechtigung Ansicht enthalten sind.</li> 
     <li>Ausgaben hinzufügen</li> 
     <li>Hinzufügen von Problemen (wenn es sich um eine Aufgabe oder ein Projekt handelt)</li> 
     <li>Aufgaben hinzufügen (falls es sich um ein Projekt handelt)</li> 
     <li>Benutzerdefinierte Forms bearbeiten</li> 
     <li>Protokollzeiten für das Objekt</li> 
     <li>Zuweisungen vornehmen</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Verwalten</strong></td> 
   <td> <p>Sie können die folgenden Aktionen für das Objekt ausführen:</p> 
    <ul> 
     <li>Alle Aktionen, die in den Berechtigungen "Anzeigen"und "Beiträge"enthalten sind</li> 
     <li>Löschen</li> 
     <li>Finanzinformationen verwalten</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Veröffentlichen Sie dies für externe Benutzer</strong></td> 
   <td> <p>Jeder ohne Workfront-Konto kann das Objekt anzeigen, indem er auf einen Link zu ihm klickt. Dies ist nicht für alle Objekte verfügbar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Systemweit sichtbar machen.</strong></td> 
   <td> <p>Das Objekt kann in Suchvorgängen gefunden und von jedem mit einem Workfront-Konto angezeigt werden.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Grundlegendes zu geerbten Berechtigungen und zur Hierarchie von Objekten

### Von übergeordneten Objekten geerbte Berechtigungen {#permissions-inherited-from-parent-objects}

Berechtigungen in Workfront werden hierarchisch übernommen. Wenn Sie einem Benutzer Berechtigungen für ein übergeordnetes Objekt erteilen, erhalten diese standardmäßig dieselben Berechtigungen für die ihm zugeordneten untergeordneten Objekte.

Wenn Sie beispielsweise einem Benutzer Berechtigungen zum Beitragen für ein Projekt erteilen, hat der Benutzer Beitragsberechtigungen für alle Aufgaben und Probleme (untergeordnete Objekte), die mit diesem Projekt verbunden sind.

Um mit dem obigen Beispiel fortzufahren, können Sie die Berechtigungen nicht auf untergeordnete Objekte beschränken. Wenn Sie nicht möchten, dass der Benutzer über Beitragsberechtigungen für dem Projekt zugeordnete untergeordnete Objekte verfügt, müssen Sie die geerbten Berechtigungen manuell aus den Objekten entfernen und dann die Berechtigungen für den einzelnen Benutzer anpassen, einschließlich aller erweiterten Einstellungen. 

Weitere Informationen zur Hierarchie und Interdependenz von Objekten in Workfront finden Sie im Abschnitt . [Abhängigkeit und Hierarchie von Objekten](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#interdependency-and-hierarchy-of-objects) im Artikel [Übersicht über Adobe Workfront-Objekte](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

>[!NOTE]
>
>Ihr Workfront-Administrator kann geerbte Berechtigungen für Dokumente in Ihrer Zugriffsebene deaktivieren. Weitere Informationen zum Deaktivieren von geerbten Berechtigungen für Dokumente auf Zugriffsebene finden Sie unter [Benutzerdefinierte Zugriffsebenen erstellen oder ändern](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

### Durch Mitgliedschaften in Unternehmen erworbene Berechtigungen  {#permissions-acquired-through-organizational-memberships}

Wenn Sie einer Benutzergruppe für ein Objekt Verwaltungsberechtigungen erteilen und Sie einem einzelnen Benutzer in dieser Gruppe Ansichtsberechtigungen für dasselbe Objekt erteilen, hat der Benutzer die höchsten Berechtigungen (Verwalten), die durch die Gruppenmitgliedschaft für das Objekt gewährt werden. 

Wenn Sie Benutzern, die bereits Teil einer Organisationseinheit sind (Gruppe, Team, Auftragsrolle oder Firma) mit einer höheren Berechtigungsstufe, niedrigere Berechtigungen erteilen möchten, müssen Sie die Berechtigungen aus der Organisationseinheit entfernen und Benutzer einzeln mit niedrigeren Berechtigungen hinzufügen.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Remove permissions from objects</h2>
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">AL: draft/ hide this div when Becky makes Remove permissions from objects live and replace with the drafted content with the link at the top of this section</p>
<p>You can remove permissions from objects you have access to Share. Removing permissions from objects is identical for all objects that can be shared.&nbsp;</p> <note type="note">
&nbsp;You cannot remove permissions when you share items in bulk. You can remove permissions only when selecting individual items.&nbsp;
</note>
<p>To remove permissions from objects consider the following:&nbsp;</p>
<ul>
<li><a href="#remove-entities-from-the-sharing-list-of-an-object" class="MCXref xref">Remove entities from the sharing list of an object</a> </li>
<li><a href="#remove-inherited-permissions" class="MCXref xref">Remove inherited permissions</a> </li>
<li><a href="#make-an-object-private" class="MCXref xref">Make an object private</a> </li>
</ul>
<p><strong>Remove entities from the sharing list of an object</strong></p>
<p>You can remove entities from the sharing list of an object to remove their permissions from the object.</p>
<p>To remove permissions from objects:&nbsp;</p>
<ol>
<li value="1">Navigate to an object on which you want to modify the permissions.</li>
<li value="2">Click the <strong>Actions</strong> menu, then click <strong>Sharing</strong>.<br>For example, on a project, click <strong>Project Actions</strong>, then <strong>Sharing</strong>.&nbsp;</li>
<li value="3">Click the <strong>x</strong> next to the name of a user, team, group, company, job role to remove them.<br></li>
<li value="4">In the <strong><User Name>'s Workfront access will be removed from this</strong> drop-down menu, select whether you want their access to be removed just from the object you have selected, or from all children objects associated with it.<br>The following scenarios exist:
<ul>
<li>If you remove the entity only from the object, that entity loses their permissions on the object, and their inherited permissions to the children objects. If they are granted permissions to the children items individually, they retain the same permissions on all children objects associated with it when you select this option.&nbsp;</li>
<li>If you remove the entity from the object and all the children objects, that entity loses their permissions to the object as well as all children objects, even when they have been given individual permission on each child object.&nbsp;</li>
</ul></li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
<p> <p><strong>Remove inherited permissions</strong></p> </p>
<p>Inherited permissions can be removed from objects allowing for owners to specifically&nbsp;identify who will get access to children objects regardless of the access of a user to a parent object. Only users with Manage permission are able to remove inherited permissions.</p>
<p>To remove inherited permissions:</p>
<ol>
<li value="1">Navigate to an object to which you have Manage permissions. <br>For example, navigate to a task.</li>
<li value="2">Go to the sharing list as described in the <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> section in this article. </li>
<li value="3">Select the <strong>X</strong>&nbsp;mark next to <strong>Inherited Permission</strong>&nbsp;on the sharing box to remove&nbsp;anyone listed there.<br><br>This ensures that no one who is granted permissions to the parent object (for example, the project) has permissions to this task by default. You must list&nbsp; individual entities in the sharing list of the task to grant permissions on the task.<br><note type="note">
You cannot remove individual entities from the Inherited Permissions list. You can only disable the Inherited Permissions for all entities listed.
</note></li>
<li value="4">Click <strong>Save</strong>.&nbsp;</li>
</ol>
<p><strong>Make an object private</strong></p>
<p>If you have shared an object system-wide, or you have shared it with external uses by making it public, you can make it private again by removing the system-wide or public permissions.&nbsp;</p>
<p>For more information about making an object available system-wide, or publicly, see the section <a href="#Share" class="MCXref xref">Overview of sharing permissions on objects</a> in this article.</p>
<p>To make an object private:</p>
<ol>
<li value="1">Go to the object you want to make private.<br>For example, navigate to a report.</li>
<li value="2">Click <strong>Report Actions</strong>, then <strong>Sharing</strong>.<br><br></li>
<li value="3">Click <strong>Remove public access</strong> to remove the access of external users to viewing the report.</li>
<li value="4">Click <strong>Remove system-wide access</strong> to stop sharing it with all Workfront users.&nbsp;</li>
<li value="5">Click <strong>Save</strong>.</li>
</ol>
</div>
-->

## Objekt freigeben

Informationen zum Freigeben von Objekten finden Sie unter [Objekt freigeben](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

## Berechtigungen aus Objekten entfernen

Informationen zum Entfernen von Berechtigungen von Objekten finden Sie unter [Berechtigungen aus Objekten entfernen](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Anfordern von Berechtigungen für Objekte

Wenn Ihnen ein Benutzer einen Link zu einem Objekt sendet, für das Sie keine Berechtigung zum Anzeigen haben, oder wenn Sie für ein Objekt über niedrigere Berechtigungen verfügen und eine höhere Berechtigungsstufe anfordern möchten, können Sie Berechtigungen für das Objekt anfordern. 

Sie können den Zugriff auf ein Objekt von allen Personen anfordern, die über die Berechtigung &quot;Freigeben&quot;für das Objekt verfügen. 

Weitere Informationen zum Anfordern von Berechtigungen für Objekte finden Sie unter [Zugriff auf Objekte anfordern](../../workfront-basics/grant-and-request-access-to-objects/request-access.md).
