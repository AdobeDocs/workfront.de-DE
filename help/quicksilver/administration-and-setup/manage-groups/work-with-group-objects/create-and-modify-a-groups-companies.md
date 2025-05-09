---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Erstellen und Ändern der Unternehmen einer Gruppe
description: Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie mit Unternehmen arbeiten, die mit der Gruppe und ihren Untergruppen verknüpft sind.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 407f6631-ecc1-4ed8-bfec-6d726ae87a3d
source-git-commit: 485f2985c70b1bb095e31323b7b4698bcb7a04cf
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 0%

---

# Erstellen und Ändern der Unternehmen einer Gruppe

Wenn Sie eine Gruppe anzeigen, die Sie im Bereich Gruppen verwalten, können Sie mit Unternehmen arbeiten, die mit der Gruppe und ihren Untergruppen verknüpft sind.

Wenn es Gruppen oberhalb Ihrer Gruppe gibt, können deren Administratoren diese Dinge auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

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
   <td role="rowheader">Adobe Workfront-Lizenz</td>
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Im Bereich Gruppen können Sie Unternehmen für Ihre Gruppe anzeigen, mit ihnen arbeiten und sie erstellen

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![Gruppen](assets/groups-icon.png).

1. Klicken Sie auf den Namen der Gruppe, für die Sie Firmen erstellen oder ändern möchten.
1. Klicken Sie im linken Bereich auf **Firmen**, um die mit der Gruppe verbundenen Unternehmen und etwaigen Untergruppen aufzulisten.
1. (Optional) Um eine Firma hinzuzufügen, klicken Sie auf **Firma hinzufügen** und konfigurieren Sie dann die Firma mithilfe der unten aufgeführten Optionen. Wenn Sie fertig sind, klicken Sie auf **Firma erstellen**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Abschnitt „Grundlegende Informationen“</td> 
      <td> 
       <ul> 
        <li> <p><b>Firmenname</b>: Geben Sie einen Namen für das Unternehmen ein.</p> </li> 
        <li> <p><b>Ist Aktiv</b>: Wenn diese Option aktiviert ist, können Benutzer das Unternehmen finden und es an Projekte anhängen, die sie erstellen und bearbeiten. Eine inaktive Firma kann nicht mit Projekten verknüpft werden. Diese Option ist standardmäßig aktiviert.</p> </li> 
        <li> <p><b>Dies ist die Primäre Firma</b>: Weist die Firma als die primäre Firma Ihrer Organisation zu. Die Primärfirma stellt in der Regel Ihr Workfront-Konto dar, in dem die meisten Ihrer Benutzenden arbeiten.</p> <p>Durch Ändern ihrer Zugriffsebenen können Sie Benutzer darauf beschränken, andere Benutzer anzuzeigen:</p> 
         <ul> 
          <li>Nur in der Primärfirma</li> 
          <li> <p>In der zugehörigen Firma und der primären Firma</p> <p>Informationen zur primären Unternehmensfunktion in den Zugriffsebenen der Benutzer finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> <p>Es kann nur eine oder keine Firma als Primärfirma angegeben werden, aber es können nicht mehrere Firmen als Primärfirmen angegeben werden. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </li> 
         </ul> </li> 
        <li> <p><b>Gruppe</b>: Wenn es eine Gruppe gibt, die mit der Firma Geschäfte macht, können Sie den Namen der Gruppe hier hinzufügen. Dies ist für Gruppenadministratoren nützlich, die Berichte über alle Unternehmen erstellen und diese verwalten müssen, mit denen ihre Gruppen Geschäfte machen.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Das System füllt das Feld <strong>Gruppe</strong> für die neue Firma mit der Gruppe aus, die Sie anzeigen.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Wenn Sie administrativen Zugriff auf Unternehmen in Ihrer Zugriffsebene haben, können Sie die Gruppe aus der Firma entfernen und eine andere zuweisen oder die Firma ohne Gruppe verlassen.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Wenn Sie keinen administrativen Zugriff auf Unternehmen haben, ist das Feld <strong>Gruppe</strong> erforderlich, und Sie können nur die von Ihnen verwalteten Gruppen oder alle Untergruppen unter diesen Gruppen auswählen.</p> <p data-mc-conditions="SnippetConditions-wf-groups.groups">Informationen zum administrativen Zugriff für Unternehmen finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Gewähren von administrativem Zugriff für Benutzer auf bestimmte Bereiche</a>.</p> </li> 
        <li> <p><b>Firmenmitglieder</b>: Fügen Sie dem Unternehmen vorhandene Benutzer hinzu. Auf diese Weise verknüpfen Sie diese Benutzer mit dieser Firma.</p> <p>Es gibt keine Begrenzung dafür, wie viele Benutzer Sie mit einer Firma verknüpfen. Ein Benutzer kann jedoch nicht mit mehr als einer Firma verknüpft werden.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">Benutzerdefinierter Forms-Abschnitt</td> 
      <td> <p>Wenn es Felder gibt, die Sie Ihrem Unternehmen hinzufügen möchten und die in Workfront nicht verfügbar sind, können Sie ein benutzerdefiniertes Formular erstellen und es mit Ihrem Unternehmen verknüpfen. Sie können dieses Formular an Ihr Unternehmen anhängen, indem Sie es aus dem Dropdown-Menü auswählen. Im Dropdown-Menü werden nur aktive Unternehmen aufgelistet. Informationen zum Erstellen benutzerdefinierter Formulare finden Sie unter <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Erstellen eines benutzerdefinierten Formulars</a>. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Wenn Sie administrativen Zugriff auf Unternehmen in Ihrer Zugriffsebene haben, können Sie auch unten in der Liste auf Weitere Unternehmen hinzufügen klicken. Dadurch wird eine Zeile hinzugefügt, in der Sie das neue Unternehmen schnell konfigurieren können.

1. (Optional) Um Unternehmen zu bearbeiten oder zu löschen, wählen Sie mindestens ein Unternehmen aus und verwenden Sie dann die Schaltflächen in der Symbolleiste, um es zu bearbeiten ![Symbol „Bearbeiten](assets/edit-icon.png) oder zu löschen ![Symbol „Löschen](assets/delete.png).

   Informationen zum Bearbeiten eines Unternehmens finden Sie im Abschnitt [Erstellen oder Bearbeiten eines Unternehmens in Workfront](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md#adding-a-company-to-workfront) im Artikel [Erstellen und Bearbeiten von Unternehmen](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

1. (Optional) Klicken Sie zum Exportieren der Unternehmensliste auf das Symbol „Exportieren![ und wählen ](assets/export.png) das gewünschte Dateiformat für die exportierte Liste aus.
