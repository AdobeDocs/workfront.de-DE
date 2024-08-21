---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: Erstellen einer Untergruppe
description: Sie können eine Untergruppe unter einer Gruppe erstellen, die Sie verwalten, um Benutzer und Projekte zu organisieren und Zugriffsberechtigungen in Adobe Workfront zuzuweisen. In der Regel verwalten Gruppenadministratoren Gruppen und Untergruppen. Sie können die Seite Gruppen verwenden, um ihre Gruppen und Untergruppen an einem Ort zu verwalten.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 3%

---

# Erstellen einer Untergruppe

Sie können eine Untergruppe unter einer Gruppe erstellen, die Sie verwalten, um Benutzer und Projekte zu organisieren und Zugriffsberechtigungen in Adobe Workfront zuzuweisen.

Wenn es Gruppen über der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

In der Regel verwalten Gruppenadministratoren jedoch Gruppen und Untergruppen. Sie können die Seite Gruppen verwenden, um ihre Gruppen und Untergruppen an einem Ort zu verwalten. Informationen dazu, wie Gruppen und Untergruppen in Workfront funktionieren, finden Sie unter [Gruppenübersicht](../../../administration-and-setup/manage-groups/groups-overview/groups.md) und [Übersicht über Untergruppen](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Plan*</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs für Benutzer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben.

+++

## Hinzufügen einer Untergruppe

{{step-1-to-setup}}

1. Klicken Sie auf **Gruppen**.

   In der angezeigten Liste können Sie die von Ihnen verwalteten Gruppen sowie die darin enthaltenen Untergruppen sehen. Adobe Workfront-Administratoren können alle Gruppen sehen.

1. Wählen Sie die vorhandene Gruppe oder Untergruppe aus, der Sie eine neue Untergruppe hinzufügen möchten.
1. Klicken Sie auf **Neue Untergruppe**.
1. Geben Sie im angezeigten Feld **Neue Untergruppe** einen **Gruppennamen** für die Untergruppe ein.
1. (Optional) Geben Sie eine der folgenden Informationen an:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Gruppenname</td> 
      <td>Ändern Sie den Namen der Gruppe.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td>Geben Sie eine Beschreibung für die Untergruppe ein. Sie können bis zu 512 Zeichen eingeben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ist aktiv</td> 
      <td> <p>(Standardmäßig aktiviert) Macht die Gruppe in Ihrer Workfront-Instanz aktiv.</p> <p>Wenn normale Benutzer in vorgelagerten Feldern wie dem unten gezeigten nach einer Gruppe suchen, um sie an ein Objekt anzuhängen oder für dieses freizugeben, werden nur aktive Gruppen in der Liste angezeigt.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Um dies für Ihre Benutzer zu optimieren, können Sie die Option Ist aktiv für aktuell nicht verwendete Gruppen deaktivieren.</p> <p>Mithilfe dieses Felds können Sie die Gruppenliste einfach anhand des aktiven oder inaktiven Status anzeigen, filtern und gruppieren. Informationen zur Verwendung von Ansichten, Filtern und Gruppierungen in Listen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Berichterstellungselemente: Filter, Ansichten und Gruppierungen</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Diese Gruppe und ihre Untergruppen öffentlich machen</td> 
      <td> <p>(Nur verfügbar, wenn Sie Details für eine Gruppe der obersten Ebene und keine Untergruppe anzeigen.) Aktivieren Sie diese Option, damit Benutzer in der Untergruppe mit Zugriff auf die Bearbeitung und den Benutzer (die keine Administratoren der Gruppe sind) diese Gruppe und ihre Untergruppen zum Benutzerprofil anderer Benutzer hinzufügen können.</p> <p>Für eine öffentliche Gruppe kann jeder Benutzer (in oder außerhalb der Gruppe), der über Bearbeitungs-Benutzerzugriff verfügt, die Gruppe zum Profil anderer Benutzer hinzufügen. Sie können dies nicht für eine private Gruppe tun.</p> <p>Sie können diese Option nur auf der obersten übergeordneten Gruppe in einer Hierarchie von Gruppen mit mehr als einer Ebene bearbeiten. Alle Untergruppen der übergeordneten Gruppe übernehmen ihre Einstellung.</p> <p><b>NOTE</b>:  
        <ul> 
         <li>Sie können eine Untergruppe nicht allein öffentlich machen, aber Sie können sie als übergeordnete Gruppe der obersten Ebene veröffentlichen, wodurch auch alle Untergruppen der übergeordneten Gruppe öffentlich gemacht werden.</li> 
         <li>Eine Untergruppe, die zu einer öffentlichen Gruppe gehört, ist standardmäßig öffentlich, sodass alle Benutzer mit Bearbeitungszugriff die Untergruppe auch anderen Benutzern hinzufügen können.</li> 
        </ul> </p> <p>Wenn Sie Informationen über den für die Bearbeitung von Benutzern benötigten Zugriff benötigen, finden Sie weitere Informationen unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Gewähren des Zugriffs für Benutzer</a>. Weitere Informationen zum Bearbeiten von Benutzern finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Profil eines Benutzers bearbeiten</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Business Leader </td> 
      <td> <p>Sie können einen Benutzer als Business Leader für eine von Ihnen verwaltete Untergruppe zuweisen. Ein Business Leader ist jemand, der Geschäftsentscheidungen für die Untergruppe trifft. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Übersicht über den Business Leader</a><span>.</span></p> <p>Wenn die Person noch nicht Mitglied der Untergruppe ist, werden sie durch Hinzufügen ihres Namens zu diesem Feld auch zur Gruppe hinzugefügt.</p> <p><b>NOTE</b>:  
        <ul> 
         <li>Bevor Sie den Business Leader aus einer Untergruppe entfernen können, müssen Sie dessen Namen aus dem Feld Business Leader entfernen.</li> 
         <li>Wenn Sie den Namen aus dem Feld "Business Leader"entfernen, bleibt dieser Benutzer Mitglied der Untergruppe, es sei denn, Sie entfernen ihn daraus. Anweisungen zum Entfernen einer Person aus einer Gruppe finden Sie im Abschnitt <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Verwalten der Gruppenmitgliedschaften</a> im Artikel <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Verwalten einer Gruppe</a>.</li> 
        </ul> </p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Übersicht über den Business Leader</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppenmitglieder und Gruppenadministratoren</td> 
      <td> 
       <ul> 
        <li> <p>Gruppenmitglieder: Um Benutzer und Gruppen zur Untergruppe hinzuzufügen, geben Sie den Namen eines vorhandenen Benutzers oder einer vorhandenen Gruppe ein, den/die Sie hinzufügen möchten, und wählen Sie dann den Namen aus, wenn er angezeigt wird.</p> <p>Die Benutzer und Gruppen, die Sie hinzufügen, haben Zugriff auf alle Objekte, die für die Gruppe freigegeben sind.</p> </li> 
        <li> <p data-mc-conditions="SnippetConditions-wf-groups.subgroups">Gruppenadministratoren: Eine Untergruppe erbt die Gruppenadministratoren der übergeordneten Gruppe. Die Angabe eines Benutzers als Gruppenadministrator für eine Untergruppe ist daher optional. Über das Dropdown-Menü rechts neben dem Benutzernamen können Sie ein Gruppenmitglied als Administrator für die Gruppe zuweisen.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Personen und Gruppen in der Liste durchsuchen</td> 
      <td> Wenn Sie einen Benutzer oder eine Gruppe finden möchten, der bzw. die dieser Untergruppe bereits zugewiesen ist, können Sie hier seinen Namen eingeben und ihn bzw. diese Gruppe auswählen, sobald sie angezeigt wird.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern.**
