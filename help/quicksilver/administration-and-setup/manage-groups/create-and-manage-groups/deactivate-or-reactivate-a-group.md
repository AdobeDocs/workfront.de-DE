---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: Deaktivieren oder Reaktivieren einer Gruppe
description: Sie können eine von Ihnen verwaltete Gruppe, die Sie nicht mehr verwenden, deaktivieren.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 99b81090-8d09-4130-a746-44ed1d76f971
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 0%

---

# Deaktivieren oder Reaktivieren einer Gruppe

<!--
If Callisto adds the <b>Is active</b> checkbox to the Details page for groups you view, add that info to Manage groups/Create and manage groups/manage-a-group and to Manage groups/Create and manage groups/view-and-manage-a-groups-details
-->

Sie können eine von Ihnen verwaltete Gruppe, die Sie nicht mehr verwenden, deaktivieren.

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

## Deaktivieren oder Reaktivieren einer Gruppe

>[!IMPORTANT]
>
>Wenn Sie eine Gruppe deaktivieren, werden auch alle Untergruppen unterhalb dieser Gruppe deaktiviert.
>
>Wenn Sie einen dieser Vorgänge reaktivieren müssen, haben Sie folgende Möglichkeiten:
>
>* Entfernen Sie sie aus der übergeordneten Gruppe. Weitere Informationen finden Sie im Abschnitt [Entfernen einer Untergruppe aus der übergeordneten Gruppe und Festlegen als Gruppe der obersten Ebene](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) im Artikel [Verwalten einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
>
>* Verschieben Sie sie unter eine aktive Gruppe. Weitere Informationen finden Sie im Abschnitt [Erstellen, Verschieben, Anzeigen, Bearbeiten, Kopieren, Umbenennen, Exportieren oder Löschen einer ](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#create)) im Artikel [Verwalten einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).

{{step-1-to-setup}}

1. Wählen Sie im linken Bereich die Option **Gruppen** aus.

   In der angezeigten Liste werden die von Ihnen verwalteten Gruppen sowie alle zugehörigen Untergruppen angezeigt. Adobe Workfront-Administratoren können alle Gruppen anzeigen.

1. Klicken Sie auf den Namen der Gruppe, um deren Seite zu öffnen.

1. Klicken Sie auf das Menü ![Mehr](assets/more-icon.png) neben dem Namen der Gruppe und dann auf **Deaktivieren** oder **Reaktivieren**.

   >[!NOTE]
   >
   >Die Option Ist aktiv (Option Reaktivieren in der Vorschau) ist nicht verfügbar, wenn die Gruppe eine Untergruppe einer deaktivierten Gruppe ist. Bevor Sie sie reaktivieren können, müssen Sie sie aus der übergeordneten Gruppe entfernen oder in eine aktive Gruppe verschieben, wie in dem wichtigen Hinweis oben beschrieben.

1. (Bedingt) Wenn Sie die Gruppe deaktivieren möchten, klicken Sie im daraufhin angezeigten Feld **Gruppe deaktivieren** auf **Deaktivieren**.

## Überlegungen zu inaktiven Gruppen

Beachten Sie Folgendes zu einer Gruppe, die Sie deaktivieren, indem Sie die Option Ist aktiv deaktivieren, die im Abschnitt [Deaktivieren oder Reaktivieren einer Gruppe](#View) in diesem Artikel erläutert wird.

* Durch Deaktivieren einer Gruppe werden auch alle darunter liegenden Untergruppen deaktiviert. Dazu gehören Untergruppen, die Sie hinzufügen, nachdem Sie sie deaktiviert haben.

  Informationen zur Reaktivierung einer Untergruppe in dieser Situation finden Sie unter [Informationen zur Reaktivierung einer Untergruppe unterhalb einer inaktiven übergeordneten Gruppe](#about-reactivating-a-subgroup-below-an-inactive-parent-group) in diesem Artikel.

* Wenn Sie im Setup zum Bereich Gruppen gehen, werden nur aktive Gruppen in der Liste angezeigt, da Active der Standardfilter (![) ](assets/filter-nwepng.png). Wenn Sie alle von Ihnen verwalteten Gruppen anzeigen möchten, einschließlich der inaktiven, können Sie den Filter Alle verwenden. Oder verwenden Sie den Filter Inaktiv , um nur die inaktiven aufzulisten.

  Weitere Informationen zu Filtern in Listen finden Sie unter [Filter - Übersicht](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* Das Deaktivieren einer Gruppe ändert nichts an Folgendem:

   * Die Zuordnungen der Gruppe zu Objekten. Zugeordnete Objekte funktionieren weiterhin wie zuvor, ohne Änderungen.

     Wenn beispielsweise ein Projekt mit einer Gruppe verknüpft ist, die Sie deaktivieren, verwendet das Projekt weiterhin die Voreinstellungen und Status der Gruppe, ohne Änderungen vorzunehmen.

   * Ihre Möglichkeit, ein neues Objekt, z. B. eine Genehmigung, ein Team oder eine Firma, innerhalb der Einrichtungsseite der Gruppe zu erstellen. Standardmäßig ist das neue Objekt mit der inaktiven Gruppe verknüpft.
   * Ihre Fähigkeit als Administrator, die Gruppe in Filtern und Berichten zu finden.

     Sie finden ihn auch in Feldern für Gruppentypvoraussetzung, in denen Sie die Gruppeneinstellungen im Bereich „Setup“ verwalten können. Dazu gehören die Bereiche Voreinstellungen, Ereignisbenachrichtigungen und Systemlizenzen.

     Wenn Sie beispielsweise zu Einrichtung > Projektvoreinstellung > Projekte gehen und das Feld für die automatische Textvervollständigung über den Optionen dort löschen, können Sie weiterhin eine inaktive Gruppe finden und ihre Projektvoreinstellungen konfigurieren.

## Informationen zum Reaktivieren einer Untergruppe unterhalb einer inaktiven übergeordneten Gruppe {#about-reactivating-a-subgroup-below-an-inactive-parent-group}

Durch Deaktivieren einer Gruppe werden auch alle darunter liegenden Untergruppen deaktiviert. Wenn Sie eine der Untergruppen unter einer inaktiven Gruppe reaktivieren müssen, haben Sie zwei Möglichkeiten:

* Verschieben Sie die Untergruppe unter eine aktive Gruppe. Aktivieren Sie dann die Option Ist aktiv für die verschobene Gruppe, wie im Abschnitt [Deaktivieren oder Reaktivieren einer Gruppe](#View) in diesem Artikel beschrieben.

  Anweisungen zum Verschieben einer Gruppe finden Sie unter [Verschieben einer Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

* Entfernen Sie die Untergruppe aus der übergeordneten Gruppe (wodurch die Untergruppe eine Gruppe der obersten Ebene wird). Aktivieren Sie dann die Option Ist aktiv für die verschobene Gruppe, wie im Abschnitt [Deaktivieren oder Reaktivieren einer Gruppe](#View) in diesem Artikel beschrieben.

  Anweisungen zum Entfernen einer Untergruppe aus der übergeordneten Gruppe finden Sie im Abschnitt [Entfernen einer Untergruppe aus der übergeordneten Gruppe und Festlegen als Gruppe auf oberster Ebene](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) im Artikel [Verwalten einer ](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
