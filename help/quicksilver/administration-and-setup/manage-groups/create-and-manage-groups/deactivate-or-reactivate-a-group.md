---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Deaktivieren oder Reaktivieren einer Gruppe
description: Sie können eine Gruppe, die Sie verwalten und die Sie nicht mehr verwenden, deaktivieren.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '766'
ht-degree: 0%

---

# Gruppe deaktivieren oder reaktivieren

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

Sie können eine Gruppe, die Sie verwalten und die Sie nicht mehr verwenden, deaktivieren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
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
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gruppe deaktivieren oder reaktivieren

>[!IMPORTANT]
>
>Wenn Sie eine Gruppe deaktivieren, werden auch alle Untergruppen darunter deaktiviert.
>
>Wenn Sie eine dieser Optionen reaktivieren müssen, können Sie dies tun, nachdem Sie einen der folgenden Schritte ausgeführt haben:
>
>* Entfernen Sie sie aus der übergeordneten Gruppe. Weitere Informationen finden Sie im Abschnitt [Eine Untergruppe aus ihrer übergeordneten Gruppe entfernen und daraus eine Gruppe der obersten Ebene machen](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) im Artikel [Verwalten einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md) .
>
>* Verschieben Sie sie unter eine aktive Gruppe. Weitere Informationen finden Sie im Abschnitt [Erstellen, Verschieben, Anzeigen, Bearbeiten, Kopieren, Umbenennen, Exportieren oder Löschen einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create) im Artikel [Verwalten einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).

{{step-1-to-setup}}

1. Wählen Sie im linken Bereich **Gruppen** aus.

   In der angezeigten Liste können Sie die von Ihnen verwalteten Gruppen sowie die darin enthaltenen Untergruppen sehen. Adobe Workfront-Administratoren können alle Gruppen sehen.

1. Klicken Sie auf den Namen der Gruppe, um die zugehörige Seite zu öffnen.

1. Klicken Sie auf das Menü Mehr neben dem Namen der Gruppe und dann auf **Deaktivieren** oder **Reaktivieren**.![](assets/more-icon.png)

   >[!NOTE]
   >
   >Die Option Ist aktiv (Option Reaktivieren in der Vorschau) ist nicht verfügbar, wenn es sich bei der Gruppe um eine Untergruppe einer deaktivierten Gruppe handelt. Bevor Sie sie reaktivieren können, müssen Sie sie aus der übergeordneten Gruppe entfernen oder unter eine aktive Gruppe verschieben, wie im obigen wichtigen Hinweis beschrieben.

1. (Bedingt) Wenn Sie die Gruppe deaktivieren, klicken Sie im angezeigten Feld **Gruppe deaktivieren** auf **Deaktivieren** .

## Überlegungen zu inaktiven Gruppen

Beachten Sie Folgendes zu einer Gruppe, die Sie deaktivieren, indem Sie die Option Ist aktiv deaktivieren, die im Abschnitt [Deaktivieren oder reaktivieren einer Gruppe](#View) in diesem Artikel erläutert wird.

* Durch Deaktivieren einer Gruppe werden auch alle Untergruppen darunter deaktiviert. Dies umfasst Untergruppen, die Sie nach der Deaktivierung hinzufügen.

  Informationen zum erneuten Aktivieren einer Untergruppe in dieser Situation finden Sie unter [Über die Reaktivierung einer Untergruppe unterhalb einer inaktiven übergeordneten Gruppe](#about-reactivating-a-subgroup-below-an-inactive-parent-group) in diesem Artikel.

* Wenn Sie in der Einrichtung zum Bereich Gruppen navigieren, sehen Sie nur aktive Gruppen in der Liste, da &quot;Aktiv&quot;der Standardfilter ![](assets/filter-nwepng.png) dafür ist. Wenn Sie alle von Ihnen verwalteten Gruppen sehen möchten, einschließlich der inaktiven Gruppen, können Sie den Filter Alle verwenden. Oder verwenden Sie den Filter Inaktiv , um nur die inaktiven aufzulisten.

  Weitere Informationen zu Filtern in Listen finden Sie unter [Filterübersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Durch das Deaktivieren einer Gruppe wird Folgendes nicht geändert:

   * Die Verbindungen der Gruppe zu Objekten. Zugeordnete Objekte funktionieren weiterhin wie zuvor, ohne dass Änderungen vorgenommen werden.

     Wenn beispielsweise ein Projekt mit einer Gruppe verknüpft ist, die Sie deaktivieren, verwendet das Projekt weiterhin die Voreinstellungen und Status der Gruppe ohne Änderungen.

   * Ihre Fähigkeit, ein neues Objekt, wie z. B. eine Genehmigung, ein Team oder ein Unternehmen, innerhalb der Seite der Gruppe zu erstellen. Standardmäßig ist das neue Objekt mit der inaktiven Gruppe verknüpft.
   * Ihre Fähigkeit als Administrator, die Gruppe in Filtern und Berichten zu finden.

     Sie finden sie auch in Gruppentypvorlagenfeldern, in denen Sie die Gruppeneinstellungen im Bereich Einrichtung verwalten möchten. Dazu gehören die Bereiche Voreinstellungen, Ereignisbenachrichtigungen und Systemlizenzen .

     Wenn Sie beispielsweise &quot;Einrichtung&quot;> &quot;Projektpräferenz&quot;> &quot;Projekte&quot;aufrufen und das Feld &quot;type-ahead&quot;über den Optionen dort löschen, können Sie weiterhin eine inaktive Gruppe finden und deren Projekteigenschaften konfigurieren.

## Über die Reaktivierung einer Untergruppe unterhalb einer inaktiven übergeordneten Gruppe {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

Durch Deaktivieren einer Gruppe werden auch alle Untergruppen darunter deaktiviert. Wenn Sie eine der Untergruppen unter einer inaktiven Gruppe reaktivieren müssen, haben Sie zwei Möglichkeiten:

* Verschieben Sie die Untergruppe unter eine aktive Gruppe. Aktivieren Sie dann die Option Ist aktiv für die verschobene Gruppe, wie im Abschnitt [Deaktivieren oder reaktivieren Sie eine Gruppe](#View) in diesem Artikel beschrieben.

  Anweisungen zum Verschieben einer Gruppe finden Sie unter [Verschieben einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* Entfernen Sie die Untergruppe aus ihrer übergeordneten Gruppe (wodurch die Untergruppe zu einer Gruppe der obersten Ebene wird). Aktivieren Sie dann die Option Ist aktiv für die verschobene Gruppe, wie im Abschnitt [Deaktivieren oder reaktivieren Sie eine Gruppe](#View) in diesem Artikel beschrieben.

  Anweisungen zum Entfernen einer Untergruppe aus ihrer übergeordneten Gruppe finden Sie im Abschnitt [Entfernen einer Untergruppe aus ihrer übergeordneten Gruppe und Einrichten einer Gruppe der obersten Ebene](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) im Artikel [Verwalten einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md) .
