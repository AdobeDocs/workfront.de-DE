---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Gruppe deaktivieren oder reaktivieren
description: Sie können eine Gruppe, die Sie verwalten und die Sie nicht mehr verwenden, deaktivieren.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 0%

---

# Gruppe deaktivieren oder reaktivieren

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

Sie können eine Gruppe, die Sie verwalten und die Sie nicht mehr verwenden, deaktivieren.

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

## Gruppe deaktivieren oder reaktivieren

>[!IMPORTANT]
>
>Wenn Sie eine Gruppe deaktivieren, werden auch alle Untergruppen darunter deaktiviert.
>
>Wenn Sie eine dieser Optionen reaktivieren müssen, können Sie dies tun, nachdem Sie einen der folgenden Schritte ausgeführt haben:
>
>* Entfernen Sie sie aus der übergeordneten Gruppe. Weitere Informationen finden Sie im Abschnitt . [Entfernen Sie eine Untergruppe aus ihrer übergeordneten Gruppe und machen Sie sie zu einer Gruppe der obersten Ebene](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) im Artikel [Verwalten einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* Verschieben Sie sie unter eine aktive Gruppe. Weitere Informationen finden Sie im Abschnitt . [Erstellen, Verschieben, Anzeigen, Bearbeiten, Kopieren, Umbenennen, Exportieren oder Löschen einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) im Artikel [Verwalten einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>


1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Wählen Sie im linken Bereich die Option **Gruppen**.

   In der angezeigten Liste können Sie die von Ihnen verwalteten Gruppen sowie die darin enthaltenen Untergruppen sehen. Adobe Workfront-Administratoren können alle Gruppen sehen.

1. Klicken Sie auf den Namen der Gruppe, um die zugehörige Seite zu öffnen.

1. Klicken Sie auf das Menü Mehr . ![](assets/more-icon.png) neben dem Namen der Gruppe klicken Sie auf **Deaktivieren** oder **Reaktivieren**.

   >[!NOTE]
   >
   >Die Option Ist aktiv (Option Reaktivieren in der Vorschau) ist nicht verfügbar, wenn es sich bei der Gruppe um eine Untergruppe einer deaktivierten Gruppe handelt. Bevor Sie sie reaktivieren können, müssen Sie sie aus der übergeordneten Gruppe entfernen oder unter eine aktive Gruppe verschieben, wie im obigen wichtigen Hinweis beschrieben.

1. (Bedingt) Wenn Sie die Gruppe deaktivieren, klicken Sie auf **Deaktivieren** im **Gruppe deaktivieren** angezeigt.

## Überlegungen zu inaktiven Gruppen

Beachten Sie Folgendes zu einer Gruppe, die Sie deaktivieren, indem Sie die Option Ist aktiv deaktivieren, wie im Abschnitt beschrieben [Gruppe deaktivieren oder reaktivieren](#View) in diesem Artikel.

* Durch Deaktivieren einer Gruppe werden auch alle Untergruppen darunter deaktiviert. Dies umfasst Untergruppen, die Sie nach der Deaktivierung hinzufügen.

   Informationen zum erneuten Aktivieren einer Untergruppe finden Sie in dieser Situation unter [Über die Reaktivierung einer Untergruppe unterhalb einer inaktiven übergeordneten Gruppe](#about-reactivating-a-subgroup-below-an-inactive-parent-group) in diesem Artikel.

* Wenn Sie in der Einrichtung zum Bereich &quot;Gruppen&quot;gehen, werden in der Liste nur aktive Gruppen angezeigt, da &quot;Aktiv&quot;der Standardfilter ist ![](assets/filter-nwepng.png) verwendet werden. Wenn Sie alle von Ihnen verwalteten Gruppen sehen möchten, einschließlich der inaktiven Gruppen, können Sie den Filter Alle verwenden. Oder verwenden Sie den Filter Inaktiv , um nur die inaktiven aufzulisten.

   Weitere Informationen zu Filtern in Listen finden Sie unter [Filterübersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Durch das Deaktivieren einer Gruppe wird Folgendes nicht geändert:

   * Die Verbindungen der Gruppe zu Objekten. Zugeordnete Objekte funktionieren weiterhin wie zuvor, ohne dass Änderungen vorgenommen werden.

      Wenn beispielsweise ein Projekt mit einer Gruppe verknüpft ist, die Sie deaktivieren, verwendet das Projekt weiterhin die Voreinstellungen und Status der Gruppe ohne Änderungen.

   * Ihre Fähigkeit, ein neues Objekt, wie z. B. eine Genehmigung, ein Team oder ein Unternehmen, innerhalb der Seite der Gruppe zu erstellen. Standardmäßig ist das neue Objekt mit der inaktiven Gruppe verknüpft.
   * Ihre Fähigkeit als Administrator, die Gruppe in Filtern und Berichten zu finden.

      Sie finden sie auch in Gruppentypvorlagenfeldern, in denen Sie die Gruppeneinstellungen im Bereich Einrichtung verwalten möchten. Dazu gehören die Bereiche Voreinstellungen, Ereignisbenachrichtigungen und Systemlizenzen .

      Wenn Sie beispielsweise &quot;Einrichtung&quot;> &quot;Projektpräferenz&quot;> &quot;Projekte&quot;aufrufen und das Feld &quot;type-ahead&quot;über den Optionen dort löschen, können Sie weiterhin eine inaktive Gruppe finden und deren Projekteigenschaften konfigurieren.

## Über die Reaktivierung einer Untergruppe unterhalb einer inaktiven übergeordneten Gruppe {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

Durch Deaktivieren einer Gruppe werden auch alle Untergruppen darunter deaktiviert. Wenn Sie eine der Untergruppen unter einer inaktiven Gruppe reaktivieren müssen, haben Sie zwei Möglichkeiten:

* Verschieben Sie die Untergruppe unter eine aktive Gruppe. Aktivieren Sie dann die Option Ist aktiv für die verschobene Gruppe, wie im Abschnitt beschrieben [Gruppe deaktivieren oder reaktivieren](#View) in diesem Artikel.

   Anweisungen zum Verschieben einer Gruppe finden Sie unter [Gruppe verschieben](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* Entfernen Sie die Untergruppe aus ihrer übergeordneten Gruppe (wodurch die Untergruppe zu einer Gruppe der obersten Ebene wird). Aktivieren Sie dann die Option Ist aktiv für die verschobene Gruppe, wie im Abschnitt beschrieben [Gruppe deaktivieren oder reaktivieren](#View) in diesem Artikel.

   Anweisungen zum Entfernen einer Untergruppe aus ihrer übergeordneten Gruppe finden Sie im Abschnitt [Entfernen Sie eine Untergruppe aus ihrer übergeordneten Gruppe und machen Sie sie zu einer Gruppe der obersten Ebene](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) im Artikel [Verwalten einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
