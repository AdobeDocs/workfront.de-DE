---
user-type: administrator
product-area: system-administration;user-management
keywords: create,group,subgroup,new
navigation-topic: create-and-manage-groups
title: Gruppe erstellen
description: Als Adobe Workfront-Administrator können Sie Gruppen erstellen, um Benutzer und Projekte zu organisieren und Zugriffsberechtigungen in Workfront zuzuweisen.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4a039619-0943-4b5b-ba7a-1ad9b5c11df0
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 3%

---

# Gruppe erstellen

<!--
DON'T DELETE, DRAFT, OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT-SENSITIVE HELP LINKS.
-->

Als Adobe Workfront-Administrator können Sie Gruppen erstellen, um Benutzer und Projekte zu organisieren und Zugriffsberechtigungen in Workfront zuzuweisen. Weitere Informationen finden Sie unter [Gruppenübersicht](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Jede Untergruppe benötigt mindestens einen Gruppenadministrator. Gruppenadministratoren können die Seite Gruppen verwenden, um ihre Gruppen an einem Ort zu verwalten.

Wenn Sie Gruppenadministrator oder Workfront-Administrator sind, können Sie auch Untergruppen unter einer Gruppe erstellen. Anweisungen finden Sie unter [Erstellen einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Plan*</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben, wenden Sie sich an Ihren Workfront-Administrator.

## Erstellen einer Gruppe der obersten Ebene von Grund auf neu

In diesen Schritten wird beschrieben, wie Sie eine neue Gruppe von Grund auf neu erstellen. Informationen zum Erstellen einer Gruppe oder Untergruppe durch Kopieren einer vorhandenen Gruppe finden Sie unter [Erstellen einer Gruppe der obersten Ebene durch Kopieren einer vorhandenen Gruppe oder Untergruppe](#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) in diesem Artikel.

Sie müssen ein Workfront-Administrator sein, um eine Gruppe der obersten Ebene zu erstellen.

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png).

1. Klicken Sie über der Gruppenliste auf **Neue Gruppe**.

   >[!TIP]
   >
   >Am unteren Rand der Gruppenliste können Sie auch auf **Weitere Gruppen hinzufügen** Um eine Gruppe in Zeilen hinzuzufügen, klicken Sie auf **Eingabe** wenn Sie mit dem Hinzufügen der Gruppeninformationen fertig sind.

1. Im **Neue Gruppe** ein, das angezeigt wird, geben Sie einen Namen für die Gruppe ein.
1. Geben Sie die folgenden Informationen an:

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
      <td>Geben Sie eine Beschreibung für die Gruppe ein. Sie können bis zu 512 Zeichen eingeben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ist aktiv</td> 
      <td> <p>(Standardmäßig aktiviert) Macht die Gruppe in Ihrer Workfront-Instanz aktiv.</p> <p>Wenn normale Benutzer in vorgelagerten Feldern wie dem unten gezeigten nach einer Gruppe suchen, um sie an ein Objekt anzuhängen oder für dieses freizugeben, werden nur aktive Gruppen in der Liste angezeigt.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Um dies für Ihre Benutzer zu optimieren, können Sie die Option Ist aktiv für aktuell nicht verwendete Gruppen deaktivieren.</p> <p>Mithilfe dieses Felds können Sie die Gruppenliste einfach anhand des aktiven oder inaktiven Status anzeigen, filtern und gruppieren. Informationen zur Verwendung von Ansichten, Filtern und Gruppierungen in Listen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Berichterstellungselemente: Filter, Ansichten und Gruppierungen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Diese Gruppe und ihre Untergruppen öffentlich machen</td> 
      <td> <p>(Nur verfügbar, wenn Sie Details für eine Gruppe der obersten Ebene und keine Untergruppe anzeigen.) Aktivieren Sie diese Option, damit Benutzer in der Gruppe mit Zugriff auf Benutzer mit Bearbeitungszugriff (die keine Administratoren der Gruppe sind) diese Gruppe und ihre Untergruppen zum Benutzerprofil anderer Benutzer hinzufügen können.</p> <p>Für eine öffentliche Gruppe kann jeder Benutzer (in oder außerhalb der Gruppe), der über Bearbeitungs-Benutzerzugriff verfügt, die Gruppe zum Profil anderer Benutzer hinzufügen. Sie können dies nicht für eine private Gruppe tun.</p> <p>Sie können diese Option nur auf der obersten übergeordneten Gruppe in einer Hierarchie von Gruppen mit mehr als einer Ebene bearbeiten. Alle Untergruppen der übergeordneten Gruppe übernehmen ihre Einstellung.</p> <p><b>NOTIZ</b>:  
        <ul> 
         <li>Sie können eine Untergruppe nicht allein öffentlich machen, aber Sie können sie als übergeordnete Gruppe der obersten Ebene veröffentlichen, wodurch auch alle Untergruppen der übergeordneten Gruppe öffentlich gemacht werden.</li> 
         <li>Eine Untergruppe, die zu einer öffentlichen Gruppe gehört, ist standardmäßig öffentlich, sodass alle Benutzer mit Bearbeitungszugriff die Untergruppe auch anderen Benutzern hinzufügen können.</li> 
        </ul> </p> <p>Informationen zum Zugriff, der für die Bearbeitung von Benutzern erforderlich ist, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>. Informationen zum Bearbeiten von Benutzern finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Benutzerprofil bearbeiten</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Business Leader </td> 
      <td> <p>Sie können einen Benutzer für eine von Ihnen verwaltete Gruppe als Business Leader zuweisen. Ein Business Leader ist jemand, der Geschäftsentscheidungen für die Gruppe trifft. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Übersicht über Business Leader</a><span>.</span></p> <p>Wenn die Person noch nicht Mitglied der Gruppe ist, werden sie durch Hinzufügen ihres Namens zu diesem Feld auch zur Gruppe hinzugefügt.</p> <p><b>NOTIZ</b>:  
        <ul> 
         <li>Bevor Sie den Business Leader aus einer Gruppe entfernen können, müssen Sie dessen Namen aus dem Feld Business Leader entfernen.</li> 
         <li>Wenn Sie den Namen aus dem Feld "Business Leader"entfernen, bleibt dieser Benutzer Mitglied der Gruppe, es sei denn, Sie entfernen ihn daraus. Anweisungen zum Entfernen einer Person aus einer Gruppe finden Sie im Abschnitt <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">Gruppenmitgliedschaften verwalten</a> im Artikel <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">Verwalten einer Gruppe</a>.</li> 
        </ul> </p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Übersicht über Business Leader</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppenmitglieder und Gruppenadministratoren</td> 
      <td> 
       <ul> 
        <p>Um Gruppenmitglieder hinzuzufügen, geben Sie den Namen eines vorhandenen Benutzers oder einer vorhandenen Gruppe ein, den/die Sie hinzufügen möchten, und wählen Sie dann den Namen aus, wenn er angezeigt wird.</p> 
        <p>Benutzer und Gruppen, die Sie hinzufügen, haben Zugriff auf alle Objekte, die für die Gruppe freigegeben sind.</p>
        <p>Eine Gruppe der obersten Ebene muss über mindestens einen Gruppenadministrator verfügen. </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Personen und Gruppen in der Liste durchsuchen</td> 
      <td> Wenn Sie einen dieser Gruppe bereits zugewiesenen Benutzer oder eine Gruppe suchen möchten, können Sie hier seinen Namen eingeben und ihn auswählen, sobald er angezeigt wird.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **Gruppe erstellen**.

## Erstellen einer Gruppe der obersten Ebene durch Kopieren einer vorhandenen Gruppe oder Untergruppe {#create-a-top-level-group-by-copying-an-existing-group-or-subgroup}

Als Workfront-Administrator können Sie eine neue Gruppe der obersten Ebene erstellen, indem Sie eine bestehende Gruppe oder Untergruppe kopieren.

Beachten Sie Folgendes, wenn Sie dies tun möchten:

* Alle Mitglieder und Untergruppen, die zur vorhandenen Gruppe gehören, werden in die neue Gruppe der obersten Ebene kopiert.
* Die Mitglieder der kopierten Gruppe behalten die Zuweisungen in der ursprünglichen Gruppe bei. Daher werden die Gruppenadministratoren der ursprünglichen Gruppe auch als Gruppenadministratoren in der kopierten Gruppe bezeichnet.

So erstellen Sie eine neue Gruppe der obersten Ebene durch Kopieren einer Gruppe oder Untergruppe:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png).

   In der angezeigten Liste können Sie die von Ihnen verwalteten Gruppen sowie die darin enthaltenen Untergruppen sehen. Adobe Workfront-Administratoren können alle Gruppen sehen.

1. Wählen Sie die Gruppe aus, die Sie kopieren möchten, und klicken Sie dann auf das Symbol Kopieren . ![](assets/copy-icon.png).
1. Im **Gruppe kopieren** ein, das angezeigt wird, geben Sie einen **Gruppenname** für die kopierte Gruppe.

1. Geben Sie die folgenden Informationen an:

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
      <td>Geben Sie eine Beschreibung für die Gruppe ein. Sie können bis zu 512 Zeichen eingeben.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ist aktiv</td> 
      <td> <p>(Standardmäßig aktiviert) Macht die Gruppe in Ihrer Workfront-Instanz aktiv.</p> <p>Wenn normale Benutzer in vorgelagerten Feldern wie dem unten gezeigten nach einer Gruppe suchen, um sie an ein Objekt anzuhängen oder für dieses freizugeben, werden nur aktive Gruppen in der Liste angezeigt.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Um dies für Ihre Benutzer zu optimieren, können Sie die Option Ist aktiv für aktuell nicht verwendete Gruppen deaktivieren.</p> <p>Mithilfe dieses Felds können Sie die Gruppenliste einfach anhand des aktiven oder inaktiven Status anzeigen, filtern und gruppieren. Informationen zur Verwendung von Ansichten, Filtern und Gruppierungen in Listen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Berichterstellungselemente: Filter, Ansichten und Gruppierungen</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Diese Gruppe und ihre Untergruppen öffentlich machen</td> 
      <td> <p>(Nur verfügbar, wenn Sie Details für eine Gruppe der obersten Ebene und keine Untergruppe anzeigen.) Aktivieren Sie diese Option, damit Benutzer in der Gruppe mit Zugriff auf Benutzer mit Bearbeitungszugriff (die keine Administratoren der Gruppe sind) diese Gruppe und ihre Untergruppen zum Benutzerprofil anderer Benutzer hinzufügen können.</p> <p>Für eine öffentliche Gruppe kann jeder Benutzer (in oder außerhalb der Gruppe), der über Bearbeitungs-Benutzerzugriff verfügt, die Gruppe zum Profil anderer Benutzer hinzufügen. Sie können dies nicht für eine private Gruppe tun.</p> <p>Sie können diese Option nur auf der obersten übergeordneten Gruppe in einer Hierarchie von Gruppen mit mehr als einer Ebene bearbeiten. Alle Untergruppen der übergeordneten Gruppe übernehmen ihre Einstellung.</p> <p><b>NOTIZ</b>:  
        <ul> 
         <li>Sie können eine Untergruppe nicht allein öffentlich machen, aber Sie können sie als übergeordnete Gruppe der obersten Ebene veröffentlichen, wodurch auch alle Untergruppen der übergeordneten Gruppe öffentlich gemacht werden.</li> 
         <li>Eine Untergruppe, die zu einer öffentlichen Gruppe gehört, ist standardmäßig öffentlich, sodass alle Benutzer mit Bearbeitungszugriff die Untergruppe auch anderen Benutzern hinzufügen können.</li> 
        </ul> </p> <p>Informationen zum Zugriff, der für die Bearbeitung von Benutzern erforderlich ist, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Benutzern Zugriff gewähren</a>. Informationen zum Bearbeiten von Benutzern finden Sie unter <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Benutzerprofil bearbeiten</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Business Leader </td> 
      <td> <p>Sie können einen Benutzer für eine von Ihnen verwaltete Gruppe als Business Leader zuweisen. Ein Business Leader ist jemand, der Geschäftsentscheidungen für die Gruppe trifft. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Übersicht über Business Leader</a><span>.</span></p> <p>Wenn die Person noch nicht Mitglied der Gruppe ist, werden sie durch Hinzufügen ihres Namens zu diesem Feld auch zur Gruppe hinzugefügt.</p> <p><b>NOTIZ</b>:  
        <ul> 
         <li>Bevor Sie den Business Leader aus einer Gruppe entfernen können, müssen Sie dessen Namen aus dem Feld Business Leader entfernen.</li> 
         <li>Wenn Sie den Namen aus dem Feld "Business Leader"entfernen, bleibt dieser Benutzer Mitglied der Gruppe, es sei denn, Sie entfernen ihn daraus. Anweisungen zum Entfernen einer Person aus einer Gruppe finden Sie im Abschnitt <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Gruppenmitgliedschaften verwalten</a> im Artikel <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Verwalten einer Gruppe</a>.</li> 
        </ul> </p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Übersicht über Business Leader</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppenmitglieder und Gruppenadministratoren</td> 
      <td> 
       <ul> 
        <li> <p>Gruppenmitglieder: Um Benutzer und Gruppen zur Gruppe hinzuzufügen, geben Sie den Namen eines vorhandenen Benutzers oder einer vorhandenen Gruppe ein, den/die Sie hinzufügen möchten, und wählen Sie dann den Namen aus, wenn er angezeigt wird.</p> <p>Die Benutzer und Gruppen, die Sie hinzufügen, haben Zugriff auf alle Objekte, die für die Gruppe freigegeben sind.</p> </li> 
        <li> <p data-mc-conditions="SnippetConditions-wf-groups.copied groups">Gruppenadministratoren: Alle Gruppenadministratoren der ursprünglichen Gruppe werden auch als Gruppenadministratoren in der kopierten Gruppe bezeichnet. Über das Dropdown-Menü rechts neben dem Benutzernamen können Sie ein Gruppenmitglied als Administrator für die Gruppe zuweisen.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Eine Gruppe der obersten Ebene muss über mindestens 1 Gruppenadministrator verfügen.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Personen und Gruppen in der Liste durchsuchen</td> 
      <td> Wenn Sie einen dieser Gruppe bereits zugewiesenen Benutzer oder eine Gruppe suchen möchten, können Sie hier seinen Namen eingeben und ihn auswählen, sobald er angezeigt wird.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >* Wenn die ursprüngliche Gruppe Untergruppen enthält, werden die Untergruppen der neuen Gruppe hinzugefügt und ihre Namen lauten standardmäßig &quot;Der ursprüngliche Untergruppenname (Kopie)&quot;.
   >* Sie können alle Benutzer oder Untergruppen aus der ursprünglichen Gruppe entfernen, indem Sie auf das X rechts neben dem Namen des Benutzers oder der Untergruppe klicken.


1. Klicken **Gruppe erstellen**.
