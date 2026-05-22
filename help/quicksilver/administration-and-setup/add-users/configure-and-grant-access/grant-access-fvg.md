---
title: Zugriff auf Filter, Ansichten und Gruppierungen gewähren
user-type: administrator
product-area: system-administration
navigation-topic: configure-access-to-workfront
description: Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um den Zugriff eines Benutzers auf die Filter-, Ansicht- und Gruppierungssteuerelemente für Listen und Berichte zu definieren.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4fb6eefd-74dd-4941-91d4-0e5f637febf3
source-git-commit: 14b3bfaf16a4ab8749538b32100ce6363a3a9335
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 11%

---

# Zugriff auf Filter, Ansichten und Gruppierungen gewähren

Als Adobe Workfront-Administrator können Sie eine Zugriffsebene verwenden, um den Zugriff eines Benutzers auf die Filter-, Ansicht- und Gruppierungssteuerelemente für Listen und Berichte zu definieren, wie unter [Zugriffsebenen - Übersicht](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md) beschrieben.

Informationen zu den Steuerelementen „Filter“, „Ansicht“ und „Gruppierung[&#x200B; finden Sie unter „Berichterstellungselemente: Filter, Ansichten und Gruppierungen](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p>
   <p>Abo</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurieren des Benutzerzugriffs auf Filter, Ansichten und Gruppierungen mithilfe einer benutzerdefinierten Zugriffsebene

1. Erstellen oder bearbeiten Sie die Zugriffsebene, wie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen“ &#x200B;](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Klicken Sie auf das Zahnradsymbol ![](assets/gear-icon-settings.png) der Schaltfläche **Anzeigen** oder **Bearbeiten** rechts neben den Filtern und wählen Sie dann unter **Einstellungen optimieren** die Funktionen aus, die Sie gewähren möchten.

   ![](assets/gear-icon-filters-dashboards-groupings.png)

   Standardmäßig haben Benutzer mit einer Standard-, Plan-, Arbeits-, Licht-, Prüfer-, Mitwirkende- oder Anfragelizenz die volle Anzeige- und Bearbeitungsfunktion. Benutzer mit einer Lizenz für externe Benutzer haben keinen Zugriff auf Filter, Ansichten und Gruppierungen.

   <!--
   If this changes, undraft section with table below
   -->

1. (Optional) Um Zugriffseinstellungen für andere Objekte und Bereiche in der Zugriffsebene, an der Sie arbeiten, zu konfigurieren, fahren Sie mit einem der in [Zugriff auf Adobe Workfront konfigurieren](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md) aufgelisteten Artikel fort, z. B. [Zugriff auf Aufgaben gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) und [Zugriff auf Finanzdaten gewähren](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Wenn Sie fertig sind, klicken Sie auf **Speichern**.

   Nachdem die Zugriffsebene erstellt wurde, können Sie sie einem Benutzer zuweisen. Weitere Informationen finden Sie [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Zugriff auf Filter, Ansichten und Gruppierungen nach Lizenztyp

Informationen dazu, was Benutzer in den einzelnen Zugriffsebenen mit Filtern, Ansichten und Gruppierungen tun können, finden Sie im Abschnitt [Filter, Ansichten und Gruppierungen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/functionality-available-for-objects.md#filters-views-and-groupings) im Artikel [Für jeden Objekttyp verfügbare Funktionen](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/functionality-available-for-objects.md).

<!--

Drafting out this section for now because the table is redundant since all four license types can do everything.


This table lists what a Workfront administrator can allow users with each license type to do with filter, views, and groupings. For information about the Workfront license types, see [Adobe Workfront licenses overview](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

<table style="table-layout:auto">
<col>
<col>
<col>
<col>
<col>
<thead>
<tr>
<th> Action </th>
<th> Planner </th>
<th> Worker </th>
<th> Reviewer </th>
<th> Requester </th>
</tr>
</thead>
<tbody>
<tr>
<td>Edit filters, views, and groupings</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Create filters, views, and groupings</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>View filters, views, and groupings</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Delete filters, views, and groupings</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Share filters, views, and groupings</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
<tr>
<td>Share filters, views, and groupings system-wide</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
<td>✓</td>
</tr>
</tbody>
</table>

-->