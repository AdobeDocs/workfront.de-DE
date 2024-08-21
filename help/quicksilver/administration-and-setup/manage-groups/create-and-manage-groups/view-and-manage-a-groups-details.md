---
title: Details einer Gruppe anzeigen und verwalten
description: Sie können die Seite Gruppendetails für eine von Ihnen verwaltete Gruppe oder Untergruppe anzeigen und bearbeiten.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: edd2c58a-f912-4638-b6a3-ff3b1b622f48
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 1%

---

# Details einer Gruppe anzeigen und verwalten

Sie können die Seite Gruppendetails für eine von Ihnen verwaltete Gruppe oder Untergruppe anzeigen und bearbeiten. Diese Seite enthält:

* Beschreibung der Gruppe
* Die Namen des Business Leaders und der Gruppenadministratoren
* Eine Option, mit der Sie die Gruppe und ihre Untergruppen öffentlich oder privat machen können

  <!--
  <li>An option that allows you to deactivate or reactivate a group and its subgroups.
  DRAFTED IN FLARE:
  Make this change when Callisto adds the
  <b>Is active</b>
   option to the Details pag
  </li>
  -->

Weitere Informationen zu anderen Methoden zum Verwalten einer Gruppe finden Sie unter [Erstellen einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Informationen dazu, wie Sie eine Gruppe deaktivieren oder reaktivieren können, finden Sie unter [Deaktivieren oder Reaktivieren einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

<!--
DRAFTED IN FLARE:
Delete this paragraph when Callisto adds the
<b>Is active</b>
 option to the Details pag
-->

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

## Details einer Gruppe anzeigen und verwalten

{{step-1-to-setup}}

1. Klicken Sie auf **Gruppen**.

   In der angezeigten Liste können Sie die von Ihnen verwalteten Gruppen sowie die darin enthaltenen Untergruppen sehen. Adobe Workfront-Administratoren können alle Gruppen sehen.

1. Klicken Sie auf den Namen der Gruppe der obersten Ebene, die Sie bearbeiten möchten.
1. Wenn Sie die Gruppe deaktivieren oder reaktivieren möchten,
1. Klicken Sie im linken Menü auf **Gruppendetails** und führen Sie dann einen der folgenden Schritte aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td> <p>Sie können bis zu 512 Zeichen eingeben.</p> <p>Wenn das Feld leer ist, klicken Sie auf <strong>Hinzufügen</strong> , um eine Beschreibung einzugeben.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Ist aktiv</td> 
      <td> <p>(Standardmäßig aktiviert) Macht die Gruppe in Ihrer Workfront-Instanz aktiv.</p> <p>Wenn normale Benutzer in vorgelagerten Feldern wie dem unten gezeigten nach einer Gruppe suchen, um sie an ein Objekt anzuhängen oder für dieses freizugeben, werden nur aktive Gruppen in der Liste angezeigt.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Um dies für Ihre Benutzer zu optimieren, können Sie die Option Ist aktiv für aktuell nicht verwendete Gruppen deaktivieren.</p> <p>Mithilfe dieses Felds können Sie die Gruppenliste einfach anhand des aktiven oder inaktiven Status anzeigen, filtern und gruppieren. Informationen zur Verwendung von Ansichten, Filtern und Gruppierungen in Listen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Berichterstellungselemente: Filter, Ansichten und Gruppierungen</a>.</p> <p>Informationen zu inaktiven Gruppen finden Sie im Abschnitt <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md#inactive" class="MCXref xref">Überlegungen zu inaktiven Gruppen</a> im Artikel <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md" class="MCXref xref">Löschen oder Deaktivieren eines benutzerdefinierten Formulars</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppenzugriff</td> 
      <td> <p>(Nur verfügbar, wenn Sie Details für eine Gruppe und keine Untergruppe anzeigen.) Aktivieren oder deaktivieren Sie die Option <strong>Diese Gruppe und Untergruppen privat machen</strong>.</p> <p>Für eine öffentliche Gruppe kann jeder Benutzer (in oder außerhalb der Gruppe), der über Bearbeitungs-Benutzerzugriff verfügt, die Gruppe zum Profil anderer Benutzer hinzufügen. Sie können dies nicht für eine private Gruppe tun.</p> <p>Sie können diese Option nur auf der obersten übergeordneten Gruppe in einer Hierarchie von Gruppen mit mehr als einer Ebene bearbeiten. Alle Untergruppen der übergeordneten Gruppe übernehmen ihre Einstellung.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppen-Stakeholder</td> 
      <td> 
       <ul> 
        <li><strong>Gruppenadministratoren</strong>: Fügen Sie Benutzer mit einer Planner-Lizenz als Gruppenadministratoren für die Gruppe hinzu oder entfernen Sie sie. Beginnen Sie mit der Eingabe des Benutzernamens und klicken Sie dann auf den Namen, wenn er im Dropdown-Menü angezeigt wird.</li> 
        <li><strong>Business Leader</strong>: Führen Sie einen der folgenden Schritte aus:
         <ul>
          <li>Wenn Sie der Gruppe noch keinen Business Leader zugewiesen haben, klicken Sie auf <strong>Hinzufügen</strong>, geben Sie den Namen des Benutzers ein, den Sie zuweisen möchten, und klicken Sie dann auf den Namen der Person, wenn dieser angezeigt wird.</li>
          <li>Wenn die Gruppe bereits über einen Business Leader verfügt und Sie ihn ändern möchten, doppelklicken Sie auf den Namen des vorhandenen Business Leaders. Löschen Sie den Namen, geben Sie den Namen des Benutzers ein, den Sie zuweisen möchten, und klicken Sie dann auf den Namen der Person, wenn dieser angezeigt wird.</li>
         </ul></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefiniertes Formular hinzufügen</td> 
      <td>Wenn Sie über Ihre Zugriffsebene benutzerdefinierte Formulare verwalten können, fügen Sie der Gruppe ein benutzerdefiniertes Formular hinzu. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Benutzerdefinierte Formulare</a>.</td> 
     </tr> 
    </tbody> 
   </table>
