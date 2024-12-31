---
user-type: administrator
product-area: system-administration;user-management
keywords: erstellen,Gruppe,Untergruppe,neu
navigation-topic: create-and-manage-groups
title: Erstellen einer Gruppe
description: Als Adobe Workfront-Administrator können Sie Gruppen erstellen, um Benutzende und Projekte zu organisieren und Zugriffsrechte in Workfront zuzuweisen.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 4a039619-0943-4b5b-ba7a-1ad9b5c11df0
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '1652'
ht-degree: 3%

---

# Erstellen einer Gruppe

<!--
DON'T DELETE, DRAFT, OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT-SENSITIVE HELP LINKS.
-->

Als Adobe Workfront-Administrator können Sie Gruppen erstellen, um Benutzende und Projekte zu organisieren und Zugriffsrechte in Workfront zuzuweisen. Weitere Informationen finden Sie unter [Gruppen - Übersicht](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Jede Untergruppe benötigt mindestens einen Gruppenadministrator. Gruppenadministratoren können die Seite „Gruppen“ verwenden, um ihre Gruppen an einem Ort zu verwalten.

Wenn Sie Gruppenadministrator oder Workfront-Administrator sind, können Sie auch Untergruppen unter einer Gruppe erstellen. Anweisungen finden Sie unter [Erstellen einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

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

## Erstellen einer neuen Gruppe der obersten Ebene

In diesen Schritten wird beschrieben, wie Sie eine neue Gruppe von Grund auf neu erstellen. Informationen zum Erstellen einer Gruppe oder Untergruppe durch Kopieren einer vorhandenen Gruppe finden Sie unter [Erstellen einer Gruppe auf oberster Ebene durch Kopieren einer vorhandenen Gruppe oder Untergruppe](#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) in diesem Artikel.

Sie müssen ein Workfront-Administrator sein, um eine Gruppe der obersten Ebene zu erstellen.

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Gruppen** ![](assets/groups-icon.png).

1. Klicken Sie über der Gruppenliste auf **Neue Gruppe**.

   >[!TIP]
   >
   >Unten in der Gruppenliste können Sie auch auf &quot;**Gruppen hinzufügen** klicken, um eine Gruppe inline hinzuzufügen, und dann auf **Eingabetaste** wenn Sie mit dem Hinzufügen der Gruppeninformationen fertig sind.

1. Geben Sie in das **Neue Gruppe** angezeigte Feld einen Namen für die Gruppe ein.
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
      <td> <p>(Standardmäßig aktiviert) Aktiviert die Gruppe in Ihrer Workfront-Instanz.</p> <p>Wenn in Feldern mit automatischer Textvervollständigung wie dem unten gezeigten reguläre Benutzer nach einer Gruppe suchen, um sie an ein Objekt anzuhängen oder ein Objekt für sie freizugeben, werden in der Liste nur aktive Gruppen angezeigt.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Um dies für Ihre Benutzerinnen und Benutzer zu optimieren, können Sie die Option Ist aktiv für Gruppen deaktivieren, die derzeit nicht verwendet werden.</p> <p>In diesem Feld können Sie die Gruppenliste einfach nach dem Status Aktiv oder Inaktiv anzeigen, filtern und gruppieren. Informationen zur Verwendung von Ansichten, Filtern und Gruppierungen in Listen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref">Berichterstellungselemente: Filter, Ansichten und Gruppierungen</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Diese Gruppe und ihre Untergruppen öffentlich machen</td> 
      <td> <p>(Nur verfügbar, wenn Details für eine Gruppe der obersten Ebene und nicht für eine Untergruppe angezeigt werden.) Aktivieren Sie diese Option, damit Benutzer in der Gruppe mit edit-user-access (die keine Administratoren der Gruppe sind) diese Gruppe und ihre Untergruppen zum Benutzerprofil anderer Benutzer hinzufügen können.</p> <p>Für eine öffentliche Gruppe kann jeder Benutzer (innerhalb oder außerhalb der Gruppe), der über Bearbeitungsbenutzerzugriff verfügt, die Gruppe zum Profil anderer Benutzer hinzufügen. Sie können das nicht für eine private Gruppe tun.</p> <p>Sie können diese Option nur für die oberste übergeordnete Gruppe in einer Gruppenhierarchie bearbeiten, die mehr als eine Ebene hat. Alle Untergruppen der übergeordneten Gruppe übernehmen diese Einstellung.</p> <p><b>HINWEIS</b>:  
        <ul> 
         <li>Sie können eine Untergruppe nicht selbst öffentlich machen, aber Sie können ihre übergeordnete Gruppe auf der obersten Ebene öffentlich machen, wodurch auch alle Untergruppen der übergeordneten Gruppe öffentlich werden.</li> 
         <li>Eine Untergruppe, die zu einer öffentlichen Gruppe gehört, ist standardmäßig öffentlich, sodass jeder Benutzer mit Bearbeitungsbenutzerzugriff die Untergruppe auch anderen Benutzern hinzufügen kann.</li> 
        </ul> </p> <p>Informationen zum Zugriff, der zum Bearbeiten von Benutzern benötigt wird, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>. Informationen zum Bearbeiten von Benutzern finden Sie <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Bearbeiten des Benutzerprofils</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Business Leader </td> 
      <td> <p>Sie können einen Benutzer als Business Leader für eine von Ihnen verwaltete Gruppe zuweisen. Ein Business Leader ist jemand, der geschäftliche Entscheidungen für die Gruppe trifft. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Business Leader - Übersicht</a><span>.</span></p> <p>Wenn die Person noch nicht Mitglied der Gruppe ist, werden sie, wenn Sie ihren Namen diesem Feld hinzufügen, auch der Gruppe hinzugefügt.</p> <p><b>HINWEIS</b>:  
        <ul> 
         <li>Bevor Sie einen Business Leader aus einer Gruppe entfernen können, müssen Sie dessen Namen aus dem Feld Business Leader entfernen.</li> 
         <li>Wenn Sie den Namen aus dem Feld Business Leader entfernen, bleibt dieser Benutzer Mitglied der Gruppe, es sei denn, Sie entfernen ihn daraus. Anweisungen zum Entfernen einer Person aus einer Gruppe finden Sie im Abschnitt <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref">Verwalten der Gruppenmitgliedschaften</a> im Artikel <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref">Verwalten einer Gruppe</a>.</li> 
        </ul> </p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref">Business Leader - Übersicht</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppenmitglieder und Gruppenadministratoren</td> 
      <td>
        <p>Um Gruppenmitglieder hinzuzufügen, fangen Sie an, den Namen eines vorhandenen Benutzers oder einer vorhandenen Gruppe einzugeben, den/die Sie hinzufügen möchten, und wählen Sie dann den Namen aus, wenn er angezeigt wird.</p> 
        <p>Benutzer und Gruppen, die Sie hinzufügen, haben Zugriff auf alle Objekte, die für die Gruppe freigegeben sind.</p>
        <p>Eine Gruppe der obersten Ebene muss mindestens einen Gruppenadministrator haben. </p>
     </tr> 
     <tr> 
      <td role="rowheader">Personen und Gruppen in der Liste durchsuchen</td> 
      <td> Wenn Sie einen Benutzer oder eine Gruppe suchen müssen, der bzw. die dieser Gruppe bereits zugewiesen ist, können Sie seinen/ihren Namen hier eingeben und ihn/sie auswählen, wenn er/sie angezeigt wird.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **Gruppe erstellen**.

## Erstellen Sie eine Gruppe der obersten Ebene durch Kopieren einer vorhandenen Gruppe oder Untergruppe {#create-a-top-level-group-by-copying-an-existing-group-or-subgroup}

Als Workfront-Administrator können Sie eine neue Gruppe auf oberster Ebene erstellen, indem Sie eine bestehende Gruppe oder Untergruppe kopieren.

Beachten Sie dabei Folgendes:

* Alle Mitglieder und alle Untergruppen, die zur vorhandenen Gruppe gehören, werden in die neue Gruppe der obersten Ebene kopiert.
* Die Mitglieder der kopierten Gruppe behalten die Arbeitsaufträge bei, die sie in der ursprünglichen Gruppe hatten. Daher werden die Gruppenadministratoren der ursprünglichen Gruppe auch als Gruppenadministratoren in der kopierten Gruppe bezeichnet.

So erstellen Sie eine neue Gruppe der obersten Ebene durch Kopieren einer Gruppe oder Untergruppe:

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Gruppen** ![](assets/groups-icon.png).

   In der angezeigten Liste werden die von Ihnen verwalteten Gruppen sowie alle zugehörigen Untergruppen angezeigt. Adobe Workfront-Administratoren können alle Gruppen anzeigen.

1. Wählen Sie die Gruppe aus, die Sie kopieren möchten, und klicken Sie dann auf das Symbol Kopieren ![](assets/copy-icon.png).
1. Geben Sie **Feld „Gruppe kopieren** einen **Gruppennamen** für die kopierte Gruppe ein.

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
      <td> <p>(Standardmäßig aktiviert) Aktiviert die Gruppe in Ihrer Workfront-Instanz.</p> <p>Wenn in Feldern mit automatischer Textvervollständigung wie dem unten gezeigten reguläre Benutzer nach einer Gruppe suchen, um sie an ein Objekt anzuhängen oder ein Objekt für sie freizugeben, werden in der Liste nur aktive Gruppen angezeigt.</p> <p> <img src="assets/group-type-aheads.jpg"> </p> <p>Um dies für Ihre Benutzerinnen und Benutzer zu optimieren, können Sie die Option Ist aktiv für Gruppen deaktivieren, die derzeit nicht verwendet werden.</p> <p>In diesem Feld können Sie die Gruppenliste einfach nach dem Status Aktiv oder Inaktiv anzeigen, filtern und gruppieren. Informationen zur Verwendung von Ansichten, Filtern und Gruppierungen in Listen finden Sie unter <a href="../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md" class="MCXref xref" data-mc-variable-override="">Berichterstellungselemente: Filter, Ansichten und Gruppierungen</a>.</p>  </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Diese Gruppe und ihre Untergruppen öffentlich machen</td> 
      <td> <p>(Nur verfügbar, wenn Details für eine Gruppe der obersten Ebene und nicht für eine Untergruppe angezeigt werden.) Aktivieren Sie diese Option, damit Benutzer in der Gruppe mit edit-user-access (die keine Administratoren der Gruppe sind) diese Gruppe und ihre Untergruppen zum Benutzerprofil anderer Benutzer hinzufügen können.</p> <p>Für eine öffentliche Gruppe kann jeder Benutzer (innerhalb oder außerhalb der Gruppe), der über Bearbeitungsbenutzerzugriff verfügt, die Gruppe zum Profil anderer Benutzer hinzufügen. Sie können das nicht für eine private Gruppe tun.</p> <p>Sie können diese Option nur für die oberste übergeordnete Gruppe in einer Gruppenhierarchie bearbeiten, die mehr als eine Ebene hat. Alle Untergruppen der übergeordneten Gruppe übernehmen diese Einstellung.</p> <p><b>HINWEIS</b>:  
        <ul> 
         <li>Sie können eine Untergruppe nicht selbst öffentlich machen, aber Sie können sie zu einer übergeordneten Gruppe auf oberster Ebene machen, wodurch auch alle Untergruppen der übergeordneten Gruppe öffentlich werden.</li> 
         <li>Eine Untergruppe, die zu einer öffentlichen Gruppe gehört, ist standardmäßig öffentlich, sodass jeder Benutzer mit Bearbeitungsbenutzerzugriff die Untergruppe auch anderen Benutzern hinzufügen kann.</li> 
        </ul> </p> <p>Informationen zum Zugriff, der zum Bearbeiten von Benutzern benötigt wird, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref" data-mc-variable-override="">Gewähren des Zugriffs für Benutzer</a>. Informationen zum Bearbeiten von Benutzern finden Sie <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref" data-mc-variable-override="">Bearbeiten des Benutzerprofils</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Business Leader </td> 
      <td> <p>Sie können einen Benutzer als Business Leader für eine von Ihnen verwaltete Gruppe zuweisen. Ein Business Leader ist jemand, der geschäftliche Entscheidungen für die Gruppe trifft. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Business Leader - Übersicht</a><span>.</span></p> <p>Wenn die Person noch nicht Mitglied der Gruppe ist, werden sie, wenn Sie ihren Namen diesem Feld hinzufügen, auch der Gruppe hinzugefügt.</p> <p><b>HINWEIS</b>:  
        <ul> 
         <li>Bevor Sie einen Business Leader aus einer Gruppe entfernen können, müssen Sie dessen Namen aus dem Feld Business Leader entfernen.</li> 
         <li>Wenn Sie den Namen aus dem Feld Business Leader entfernen, bleibt dieser Benutzer Mitglied der Gruppe, es sei denn, Sie entfernen ihn daraus. Anweisungen zum Entfernen einer Person aus einer Gruppe finden Sie im Abschnitt <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md#manage" class="MCXref xref" data-mc-variable-override="">Verwalten der Gruppenmitgliedschaften</a> im Artikel <a href="../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md" class="MCXref xref" data-mc-variable-override="">Verwalten einer Gruppe</a>.</li> 
        </ul> </p> <p>Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md" class="MCXref xref" data-mc-variable-override="">Business Leader - Übersicht</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gruppenmitglieder und Gruppenadministratoren</td> 
      <td> 
       <ul> 
        <li> <p>Gruppenmitglieder: Um der Gruppe Benutzer und Gruppen hinzuzufügen, fangen Sie an, den Namen eines vorhandenen Benutzers oder einer vorhandenen Gruppe, den/die Sie hinzufügen möchten, einzugeben, und wählen Sie dann den Namen aus, wenn er angezeigt wird.</p> <p>Die Benutzer und Gruppen, die Sie hinzufügen, haben Zugriff auf alle Objekte, die für die Gruppe freigegeben sind.</p> </li> 
        <li> <p>Gruppenadministratoren: Alle Gruppenadministratoren der ursprünglichen Gruppe werden ebenfalls als Gruppenadministratoren in der kopierten Gruppe bezeichnet. Über das Dropdown-Menü rechts neben dem Benutzernamen können Sie ein Gruppenmitglied als Administrator für die Gruppe zuweisen.</p> <p>Eine Gruppe der obersten Ebene muss mindestens einen Gruppenadministrator haben.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Personen und Gruppen in der Liste durchsuchen</td> 
      <td> Wenn Sie einen Benutzer oder eine Gruppe suchen müssen, der bzw. die dieser Gruppe bereits zugewiesen ist, können Sie seinen/ihren Namen hier eingeben und ihn/sie auswählen, wenn er/sie angezeigt wird.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >* Wenn die ursprüngliche Gruppe Untergruppen hat, werden die Untergruppen der neuen Gruppe hinzugefügt, und ihre Namen lauten standardmäßig „Name der ursprünglichen Untergruppe (Kopieren)“.
   >* Sie können jeden Benutzer bzw. jede Untergruppe aus der ursprünglichen Gruppe entfernen, indem Sie auf das X rechts neben dem Namen des Benutzers bzw. der Untergruppe klicken.

1. Klicken Sie **Gruppe erstellen**.
