---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: Erstellen einer Untergruppe
description: Sie können eine Untergruppe unter einer Gruppe erstellen, die Sie verwalten, um Benutzende und Projekte zu organisieren und Zugriffsrechte innerhalb von Adobe Workfront zuzuweisen. In der Regel verwalten Gruppenadministratoren Gruppen und Untergruppen. Sie können die Seite Gruppen verwenden, um ihre Gruppen und Untergruppen an einem Ort zu verwalten.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 3%

---

# Erstellen einer Untergruppe

Sie können eine Untergruppe unter einer Gruppe erstellen, die Sie verwalten, um Benutzende und Projekte zu organisieren und Zugriffsrechte innerhalb von Adobe Workfront zuzuweisen.

Wenn es Gruppen oberhalb der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

In der Regel verwalten Gruppenadministratoren jedoch Gruppen und Untergruppen. Sie können die Seite Gruppen verwenden, um ihre Gruppen und Untergruppen an einem Ort zu verwalten. Informationen zur Funktionsweise von Gruppen und Untergruppen in Workfront finden Sie unter [Gruppen - Übersicht](../../../administration-and-setup/manage-groups/groups-overview/groups.md) und [Untergruppen - Übersicht](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hinzufügen einer Untergruppe

{{step-1-to-setup}}

1. Klicken Sie **Gruppen**.

   In der angezeigten Liste werden die von Ihnen verwalteten Gruppen sowie alle zugehörigen Untergruppen angezeigt. Adobe Workfront-Administratoren können alle Gruppen anzeigen.

1. Wählen Sie die bestehende Gruppe oder Untergruppe aus, der/der Sie eine neue Untergruppe hinzufügen möchten.
1. Klicken Sie **Neue Untergruppe**.
1. Geben Sie in das **Neue Untergruppe** angezeigte Feld einen **Gruppennamen** für die Untergruppe ein.
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
      <td> <p>(Standardmäßig aktiviert) Aktiviert die Gruppe in Ihrer Workfront-Instanz.</p> <p>Wenn in Feldern mit automatischer Textvervollständigung wie dem unten gezeigten reguläre Benutzer nach einer Gruppe suchen, um sie an ein Objekt anzuhängen oder ein Objekt für sie freizugeben, werden in der Liste nur aktive Gruppen angezeigt.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Um dies für Ihre Benutzerinnen und Benutzer zu optimieren, können Sie die Option Ist aktiv für Gruppen deaktivieren, die derzeit nicht verwendet werden.</p> <p>In diesem Feld können Sie die Gruppenliste einfach nach dem Status Aktiv oder Inaktiv anzeigen, filtern und gruppieren. Informationen zur Verwendung von Ansichten, Filtern und Gruppierungen in Listen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Berichterstellungselemente: Filter, Ansichten und Gruppierungen</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Diese Gruppe und ihre Untergruppen öffentlich machen</td> 
      <td> <p>(Nur verfügbar, wenn Details für eine Gruppe der obersten Ebene und nicht für eine Untergruppe angezeigt werden.) Aktivieren Sie diese Option, damit Benutzende in der Untergruppe mit edit-user-access (die keine Administratoren der Gruppe sind) diese Gruppe und ihre Untergruppen zum Benutzerprofil anderer Benutzender hinzufügen können.</p> <p>Für eine öffentliche Gruppe kann jeder Benutzer (innerhalb oder außerhalb der Gruppe), der über Bearbeitungsbenutzerzugriff verfügt, die Gruppe zum Profil anderer Benutzer hinzufügen. Sie können das nicht für eine private Gruppe tun.</p> <p>Sie können diese Option nur für die oberste übergeordnete Gruppe in einer Gruppenhierarchie bearbeiten, die mehr als eine Ebene hat. Alle Untergruppen der übergeordneten Gruppe übernehmen diese Einstellung.</p> <p><b>HINWEIS</b>:  
        <ul> 
         <li>Sie können eine Untergruppe nicht selbst öffentlich machen, aber Sie können sie zu einer übergeordneten Gruppe auf oberster Ebene machen, wodurch auch alle Untergruppen der übergeordneten Gruppe öffentlich werden.</li> 
         <li>Eine Untergruppe, die zu einer öffentlichen Gruppe gehört, ist standardmäßig öffentlich, sodass jeder Benutzer mit Bearbeitungsbenutzerzugriff die Untergruppe auch anderen Benutzern hinzufügen kann.</li> 
        </ul> </p> <p>Informationen zum Zugriff, der zum Bearbeiten von Benutzern benötigt wird, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Gewähren des Zugriffs für Benutzer</a>. Informationen zum Bearbeiten von Benutzern finden Sie <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Bearbeiten des Benutzerprofils</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Business Leader </td> 
      <td> <p>Sie können einen Benutzer als Business Leader für eine von Ihnen verwaltete Untergruppe zuweisen. Ein Business Leader ist jemand, der geschäftliche Entscheidungen für die Untergruppe trifft. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Business Leader - Übersicht</a><span>.</span></p> <p>Wenn die Person nicht bereits Mitglied der Untergruppe ist, werden sie durch Hinzufügen ihres Namens zu diesem Feld auch zur Gruppe hinzugefügt.</p> <p><b>HINWEIS</b>:  
        <ul> 
         <li>Bevor Sie einen Business Leader aus einer Untergruppe entfernen können, müssen Sie dessen Namen aus dem Feld Business Leader entfernen.</li> 
         <li>Wenn Sie den Namen aus dem Feld „Business Leader“ entfernen, bleibt dieser Benutzer Mitglied der Untergruppe, es sei denn, Sie entfernen ihn daraus. Anweisungen zum Entfernen einer Person aus einer Gruppe finden Sie im Abschnitt <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Verwalten der Gruppenmitgliedschaften</a> im Artikel <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Verwalten einer Gruppe</a>.</li> 
        </ul> </p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Business Leader - Übersicht</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppenmitglieder und Gruppenadministratoren</td> 
      <td> 
       <ul> 
        <li> <p>Gruppenmitglieder: Um Benutzer und Gruppen zur Untergruppe hinzuzufügen, fangen Sie an, den Namen eines vorhandenen Benutzers oder einer vorhandenen Gruppe, den/die Sie hinzufügen möchten, einzugeben, und wählen Sie dann den Namen aus, wenn er angezeigt wird.</p> <p>Die Benutzer und Gruppen, die Sie hinzufügen, haben Zugriff auf alle Objekte, die für die Gruppe freigegeben sind.</p> </li> 
        <li> <p data-mc-conditions="SnippetConditions-wf-groups.subgroups">Gruppenadministratoren: Eine Untergruppe übernimmt die Gruppenadministratoren der Gruppe, die sich darüber befindet. Die Angabe eines Benutzers als Gruppenadministrator für eine Untergruppe ist daher optional. Über das Dropdown-Menü rechts neben dem Benutzernamen können Sie ein Gruppenmitglied als Administrator für die Gruppe zuweisen.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Personen und Gruppen in der Liste durchsuchen</td> 
      <td> Wenn Sie einen Benutzer oder eine Gruppe suchen müssen, der bzw. die dieser Untergruppe bereits zugewiesen ist, können Sie den Namen hier eingeben und ihn bzw. sie auswählen, wenn er/sie angezeigt wird.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Speichern.**
