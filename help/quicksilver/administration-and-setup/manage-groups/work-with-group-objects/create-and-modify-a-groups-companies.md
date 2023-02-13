---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Erstellen und Ändern von Unternehmen einer Gruppe
description: Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie Unternehmen, die mit der Gruppe und ihren Untergruppen verbunden sind, anzeigen und mit ihnen arbeiten.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 0%

---

# Erstellen und Ändern von Unternehmen einer Gruppe

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie Unternehmen, die mit der Gruppe und ihren Untergruppen verbunden sind, anzeigen und mit ihnen arbeiten.

Wenn es Gruppen über Ihrer Gruppe gibt, können ihre Administratoren diese Dinge auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

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
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben, wenden Sie sich an Ihren Workfront-Administrator.

## Anzeigen, Arbeiten mit und Erstellen von Unternehmen für Ihre Gruppe über den Bereich &quot;Gruppen&quot;

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe, für die Sie Unternehmen erstellen oder ändern möchten.
1. Klicken Sie im linken Bereich auf **Unternehmen** die mit der Gruppe verbundenen Unternehmen und gegebenenfalls die ihr gegebenenfalls untergeordneten Gruppen aufzulisten.
1. (Optional) Um ein Unternehmen hinzuzufügen, klicken Sie auf **Firma hinzufügen** und konfigurieren Sie dann das Unternehmen mithilfe der unten aufgeführten Optionen. Wenn Sie fertig sind, klicken Sie auf **Unternehmen erstellen**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Grundlegender Informationsabschnitt</td> 
      <td> 
       <ul> 
        <li> <p><b>Firmenname</b>: Geben Sie einen Namen für das Unternehmen ein.</p> </li> 
        <li> <p><b>Ist aktiv</b>: Wenn diese Option aktiviert ist, können Benutzer das Unternehmen suchen und es an Projekte anhängen, die sie erstellen und bearbeiten. Ein inaktives Unternehmen kann nicht an Projekte angehängt werden. Diese Option ist standardmäßig aktiviert.</p> </li> 
        <li> <p><b>Dies ist das Primäre Unternehmen</b>: Weist das Unternehmen als Hauptunternehmen Ihrer Organisation zu. Das primäre Unternehmen stellt normalerweise Ihr Workfront-Konto dar, in dem die meisten Ihrer Benutzer arbeiten.</p> <p>Durch Ändern der Zugriffsebene können Sie Benutzer auf andere Benutzer beschränken:</p> 
         <ul> 
          <li>Nur in ihrer Hauptfirma</li> 
          <li> <p>In der verbundenen Firma und dem Primärunternehmen</p> <p>Informationen zur primären Unternehmensfunktionalität in den Zugriffsebenen der Benutzer finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> <p>Sie können nur ein Unternehmen oder kein Unternehmen als Hauptunternehmen festlegen, aber Sie können nicht mehrere Unternehmen als Primärunternehmen bestimmen lassen. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>Gruppe</b>: Wenn es eine Gruppe gibt, die Geschäfte mit dem Unternehmen führt, können Sie hier den Namen der Gruppe hinzufügen. Dies ist nützlich für Gruppenadministratoren, die über alle Unternehmen berichten und diese verwalten müssen, mit denen ihre Gruppen Geschäfte tätigen.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Das System füllt die <strong>Gruppe</strong> für das neue Unternehmen mit der Gruppe, die Sie anzeigen.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Wenn Sie administrativen Zugriff auf Unternehmen in Ihrer Zugriffsebene haben, können Sie die Gruppe aus dem Unternehmen entfernen und eine andere zuweisen oder das Unternehmen ohne Gruppe lassen.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Wenn Sie keinen Administratorzugriff auf Unternehmen haben, wird die <strong>Gruppe</strong> -Feld erforderlich ist und Sie können nur die von Ihnen verwalteten Gruppen oder Untergruppen unter diesen Gruppen auswählen.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Informationen über den administrativen Zugriff auf Unternehmen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren</a>.</p> </li> 
        <li> <p><b>Firmenmitglieder</b>: Fügen Sie dem Unternehmen vorhandene Benutzer hinzu. Dadurch verknüpfen Sie diese Benutzer mit diesem Unternehmen.</p> <p>Es gibt keine Beschränkung dafür, wie viele Benutzer Sie mit einem Unternehmen verknüpfen, aber ein Benutzer kann nicht mit mehr als einem Unternehmen verknüpft werden.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bereich "Abrechnungssätze"</td> 
      <td> <p>Sie können die mit Ihren Auftragsrollen auf Unternehmensebene verbundenen Abrechnungsraten überschreiben. Informationen zum Erstellen von Auftrags-Rollen und deren Zuordnung zu Abrechnungsraten finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref" data-mc-variable-override="">Erstellen und Verwalten von Vorgangsrollen</a>.</p> <p>Weitere Informationen über das Außerkraftsetzen der Abrechnungssätze auf Unternehmensebene finden Sie unter <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md" class="MCXref xref" data-mc-variable-override="">Außerkraftsetzen der Abrechnungssätze für Stellenangebote auf Unternehmensebene</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Benutzerspezifischer Forms-Abschnitt</td> 
      <td> <p>Wenn Sie Ihrem Unternehmen Felder hinzufügen möchten, die nicht in Workfront verfügbar sind, können Sie ein benutzerdefiniertes Formular erstellen und es mit Ihrem Unternehmen verknüpfen. Sie können dieses Formular an Ihr Unternehmen anhängen, indem Sie es aus dem Dropdown-Menü auswählen. Im Dropdown-Menü werden nur aktive Unternehmen aufgeführt. Informationen zum Erstellen von benutzerdefinierten Forms finden Sie unter <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" data-mc-variable-override="">Benutzerdefiniertes Formular erstellen oder bearbeiten</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Wenn Sie Administratorzugriff auf Unternehmen in Ihrer Zugriffsebene haben, können Sie auch unten in der Liste auf Weitere Unternehmen hinzufügen klicken. Dadurch wird eine Zeile hinzugefügt, in der Sie das neue Unternehmen schnell konfigurieren können.

1. (Optional) Um Unternehmen zu bearbeiten oder zu löschen, wählen Sie mindestens ein Unternehmen aus und bearbeiten Sie dann über die Schaltflächen der Symbolleiste ![](assets/edit-icon.png) oder löschen ![](assets/delete.png) es.

   Informationen zum Bearbeiten eines Unternehmens finden Sie im Abschnitt . [Erstellen oder Bearbeiten eines Unternehmens in Workfront](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) im Artikel [Erstellen und Bearbeiten von Unternehmen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (Optional) Um die Liste der Unternehmen zu exportieren, klicken Sie auf das Symbol Exportieren . ![](assets/export.png)und wählen Sie dann das Dateiformat für die exportierte Liste aus.
