---
title: Anzeigen und Verwalten der Details einer Gruppe
description: Sie können die Seite „Gruppendetails“ für eine von Ihnen verwaltete Gruppe oder Untergruppe anzeigen und bearbeiten.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: edd2c58a-f912-4638-b6a3-ff3b1b622f48
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 2%

---

# Anzeigen und Verwalten der Details einer Gruppe

Sie können die Seite „Gruppendetails“ für eine von Ihnen verwaltete Gruppe oder Untergruppe anzeigen und bearbeiten. Diese Seite enthält:

* Eine Beschreibung der Gruppe
* Die Namen des Business Leaders und der Gruppenadministratoren
* Eine Option, mit der Sie die Gruppe und ihre Untergruppen öffentlich oder privat machen können

Informationen zu anderen Möglichkeiten zum Verwalten einer Gruppe finden Sie unter [Erstellen einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Informationen dazu, wie Sie eine Gruppe deaktivieren oder reaktivieren können, finden Sie unter [Deaktivieren oder Reaktivieren einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr>
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr>
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anzeigen und Verwalten der Details einer Gruppe

{{step-1-to-setup}}

1. Klicken Sie **Gruppen**.

   In der angezeigten Liste werden die von Ihnen verwalteten Gruppen sowie alle zugehörigen Untergruppen angezeigt. Adobe Workfront-Administratoren können alle Gruppen anzeigen.

1. Klicken Sie auf den Namen der Gruppe der obersten Ebene, die Sie bearbeiten möchten.
1. Wenn Sie die Gruppe deaktivieren oder reaktivieren möchten,
1. Klicken Sie im linken Menü auf **Gruppendetails** und führen Sie dann einen der folgenden Schritte aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Beschreibung</td> 
      <td> <p>Sie können bis zu 512 Zeichen eingeben.</p> <p>Wenn das Feld leer ist, klicken Sie auf <strong>Hinzufügen</strong>, um eine Beschreibung einzugeben.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Ist aktiv</td> 
      <td> <p>(Standardmäßig aktiviert) Aktiviert die Gruppe in Ihrer Workfront-Instanz.</p> <p>Wenn in Feldern mit automatischer Textvervollständigung wie dem unten gezeigten reguläre Benutzer nach einer Gruppe suchen, um sie an ein Objekt anzuhängen oder ein Objekt für sie freizugeben, werden in der Liste nur aktive Gruppen angezeigt.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Um dies für Ihre Benutzerinnen und Benutzer zu optimieren, können Sie die Option Ist aktiv für Gruppen deaktivieren, die derzeit nicht verwendet werden.</p> <p>In diesem Feld können Sie die Gruppenliste einfach nach dem Status Aktiv oder Inaktiv anzeigen, filtern und gruppieren. Informationen zur Verwendung von Ansichten, Filtern und Gruppierungen in Listen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Berichterstellungselemente: Filter, Ansichten und Gruppierungen</a>.</p> <p>Informationen zu inaktiven Gruppen finden Sie im Abschnitt <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md#inactive" class="MCXref xref">Überlegungen zu inaktiven Gruppen</a> im Artikel <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md" class="MCXref xref">Löschen oder Deaktivieren eines benutzerdefinierten Formulars</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppenzugriff</td> 
      <td> <p>(Nur verfügbar, wenn Details für eine Gruppe, nicht für eine Untergruppe angezeigt werden.) Aktivieren oder deaktivieren Sie die Option <strong>Diese Gruppe und Untergruppen privat machen</strong>.</p> <p>Für eine öffentliche Gruppe kann jeder Benutzer (innerhalb oder außerhalb der Gruppe), der über Bearbeitungsbenutzerzugriff verfügt, die Gruppe zum Profil anderer Benutzer hinzufügen. Sie können das nicht für eine private Gruppe tun.</p> <p>Sie können diese Option nur für die oberste übergeordnete Gruppe in einer Gruppenhierarchie bearbeiten, die mehr als eine Ebene hat. Alle Untergruppen der übergeordneten Gruppe übernehmen diese Einstellung.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppen-Stakeholder</td> 
      <td> 
       <ul> 
        <li><strong>Gruppenadministratoren</strong>: Fügen Sie Benutzer mit einer Planner-Lizenz als Gruppenadministratoren für die Gruppe hinzu oder entfernen Sie sie. Geben Sie den Namen eines Benutzers ein und klicken Sie auf den Namen, wenn er im Dropdown-Menü angezeigt wird.</li> 
        <li><strong>Business Leader</strong>: Führen Sie einen der folgenden Schritte aus:
         <ul>
          <li>Wenn Sie noch keinen Business Leader für die Gruppe zugewiesen haben, klicken Sie auf <strong>Hinzufügen</strong>, geben Sie den Namen des Benutzers ein, den Sie zuweisen möchten, und klicken Sie dann auf den Namen der Person, wenn er angezeigt wird.</li>
          <li>Wenn die Gruppe bereits über einen Business Leader verfügt und Sie ihn ändern möchten, doppelklicken Sie auf den Namen des vorhandenen Business Leaders. Löschen Sie den Namen, geben Sie den Namen des Benutzers ein, den Sie zuweisen möchten, und klicken Sie dann auf den Namen der Person, wenn er angezeigt wird.</li>
         </ul></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerdefiniertes Formular hinzufügen</td> 
      <td>Wenn Sie mit Ihrer Zugriffsebene benutzerdefinierte Formulare verwalten können, fügen Sie der Gruppe ein benutzerdefiniertes Formular hinzu. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md" class="MCXref xref">Benutzerdefinierte Formulare</a>.</td> 
     </tr> 
    </tbody> 
   </table>
