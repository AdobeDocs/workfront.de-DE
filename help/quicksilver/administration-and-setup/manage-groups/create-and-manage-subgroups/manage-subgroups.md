---
user-type: administrator
product-area: system-administration;user-management
keywords: verwalten,Untergruppe,bearbeiten
navigation-topic: create-and-manage-subgroups
title: Verwalten einer Untergruppe
description: Als Gruppenadministrator einer Untergruppe können Sie die Untergruppe erstellen, verschieben, anzeigen, bearbeiten, kopieren, umbenennen, exportieren und löschen. Sie können eine Untergruppe auch zu einer Gruppe der obersten Ebene machen, indem Sie sie aus der übergeordneten Gruppe entfernen.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5186d266-fa9f-445d-9dcc-bc07eb147b60
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '1386'
ht-degree: 0%

---

# Verwalten einer Untergruppe

Als Gruppenadministrator einer Untergruppe können Sie die Untergruppe erstellen, verschieben, anzeigen, bearbeiten, kopieren, umbenennen, exportieren und löschen.

Sie können eine Untergruppe auch zu einer Gruppe der obersten Ebene machen, indem Sie sie aus der übergeordneten Gruppe entfernen.

Wenn es Gruppen oberhalb Ihrer Gruppe gibt, können deren Administratoren diese Dinge auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

Weitere Informationen zu Untergruppen finden Sie unter [Untergruppen - Übersicht](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

>[!TIP]
>
>Wenn Sie eine Gruppe verwalten, die Untergruppen enthält, ist es hilfreich, Daten über die gesamte Gruppe und alle zugehörigen Untergruppen identifizieren und filtern zu können. Verwenden Sie dazu das Feld ID des obersten übergeordneten Elements in einem Bericht oder einer Liste.
>
>Angenommen, Sie verwalten eine große Marketing-Abteilung und möchten eine Liste aller Projekte anzeigen, an denen die gesamte Abteilung arbeitet.
>
>In Workfront wird diese Marketing-Abteilung durch eine Gruppe namens Marketing mit drei Untergruppen namens Field Marketing, Product Marketing und Digital Marketing repräsentiert. Um die Projekte aufzulisten, die zur gesamten Marketing-Abteilung gehören (alle 4 Gruppen), können Sie mit der folgenden Filterregel einen Filter für den Bereich „Projekte“ erstellen:
>
>`Group: Top Parent ID > Equal > Marketing`
>
>Sie können auch das Feld Name des obersten übergeordneten Elements verwenden, um Daten zu identifizieren, die mit einer Gruppe der obersten Ebene verknüpft sind, jedoch nur in Ansichten, nicht in Filtern oder Gruppierungen.

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

## Erstellen einer Untergruppe

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![Gruppen](assets/groups-icon.png).

   In der angezeigten Liste werden die von Ihnen verwalteten Gruppen sowie alle zugehörigen Untergruppen angezeigt. Adobe Workfront-Administratoren können alle Gruppen anzeigen.

1. Klicken Sie auf den Namen der Gruppe, der Sie eine Untergruppe hinzufügen möchten.
1. Klicken Sie im linken Menü auf **Untergruppen**.
1. Um eine neue Untergruppe eine Ebene unterhalb der angezeigten Gruppe zu erstellen, klicken Sie auf **Untergruppe hinzufügen**.

   Oder, wenn Sie die neue Untergruppe unter einer anderen Untergruppe in der Liste erstellen möchten, wählen Sie diese Untergruppe aus und klicken Sie dann auf **Untergruppe hinzufügen**.

   Informationen zu den Optionen, mit denen Sie die Untergruppe konfigurieren können, finden Sie unter [Erstellen einer Untergruppe](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

   Eine Gruppenhierarchie kann nicht mehr als 15 Ebenen umfassen, aber eine einzelne Ebene kann eine unbegrenzte Anzahl paralleler Gruppen aufweisen.

## Verschieben einer Untergruppe

Sie können bestehende Untergruppen unter eine andere Gruppe verschieben, die Sie verwalten.

Eine Gruppenhierarchie kann nicht mehr als 15 Ebenen umfassen, aber eine einzelne Ebene kann eine unbegrenzte Anzahl paralleler Gruppen aufweisen.

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![Gruppen](assets/groups-icon.png).

   In der angezeigten Liste werden die von Ihnen verwalteten Gruppen sowie alle zugehörigen Untergruppen angezeigt. Adobe Workfront-Administratoren können alle Gruppen anzeigen.

1. Klicken Sie auf den Namen der Zielgruppe (Sie geben in einem späteren Schritt an, welche Untergruppen verschoben werden sollen).
1. Klicken Sie im linken Menü auf **Untergruppen**.
1. (Optional) Wählen Sie eine Untergruppe aus, um sie zur Zielgruppe zu machen.

   Wenn Sie diesen Schritt überspringen, ist die in Schritt 3 ausgewählte Gruppe die Zielgruppe.

1. Klicken Sie **Untergruppe hinzufügen > Vorhandene Gruppe**.
1. Geben **im angezeigten** „Vorhandene Gruppe“ den Namen einer Untergruppe ein, die Sie verschieben möchten.

   Die angezeigten Ergebnisse enthalten keine Gruppen oberhalb der Zielgruppe.

   Sie können sicherstellen, dass Sie die richtige Gruppe auswählen, indem Sie den Mauszeiger darüber bewegen und auf das Informationssymbol ![Informationssymbol](assets/info-icon.png) klicken, das daneben angezeigt wird. Dadurch wird eine QuickInfo angezeigt, die Informationen über die Gruppe auflistet, wie z. B. die Hierarchie der darüber liegenden Gruppen und deren Administratoren.

1. Wählen Sie den Namen der Untergruppe aus, die verschoben werden soll, wenn Sie sie in der Liste finden.
1. Wiederholen Sie die Schritte 7-8 für alle anderen Untergruppen, die Sie in die Zielgruppe verschieben möchten.
1. Klicken Sie auf **Speichern**.

## Bearbeiten einer Untergruppe

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![Gruppen](assets/groups-icon.png).

   In der angezeigten Liste werden die von Ihnen verwalteten Gruppen sowie alle zugehörigen Untergruppen angezeigt. Adobe Workfront-Administratoren können alle Gruppen anzeigen.

1. Klicken Sie auf den Namen der Gruppe, die die zu bearbeitende Untergruppe enthält.
1. Klicken Sie im linken Menü auf **Untergruppen**.
1. Wählen Sie die zu bearbeitende Untergruppe aus und klicken Sie dann auf das **Bearbeiten**-Symbol ![Bearbeiten](assets/edit-icon.png).

   Informationen zu den Optionen, mit denen Sie die Untergruppe konfigurieren können, finden Sie unter [Erstellen einer Untergruppe](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Kopieren einer Untergruppe

>[!NOTE]
>
>Nur ein Systemadministrator kann eine Untergruppe kopieren.

Wenn Sie eine Untergruppe kopieren, wird sie zu einer übergeordneten Gruppe. Alle Gruppenmitglieder und Untergruppen werden damit kopiert. Die Mitglieder der Gruppe behalten alle Arbeitsaufträge bei, die sie in der ursprünglichen Gruppe hatten.

Beachten Sie beim Kopieren einer Untergruppe Folgendes:

* Wenn eine kopierte Untergruppe über eigene Untergruppen verfügt, sind diese in der Kopie enthalten und ihre Namen sind wie folgt formatiert:

  `Original subgroup name (Copy)`

* Jede Untergruppe, die zu einer öffentlichen Gruppe gehört, ist ebenfalls öffentlich, sodass jeder Benutzer mit Zugriff zum Bearbeiten von Benutzern, unabhängig davon, ob er in der Gruppe ist oder nicht, Benutzer zur Untergruppe hinzufügen kann.

So kopieren Sie eine Untergruppe:

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![Gruppen](assets/groups-icon.png).

   In der angezeigten Liste werden die von Ihnen verwalteten Gruppen sowie alle zugehörigen Untergruppen angezeigt. Adobe Workfront-Administratoren können alle Gruppen anzeigen.

1. Klicken Sie auf den Namen der Gruppe, die die zu kopierende Untergruppe enthält.
1. Klicken Sie im linken Menü auf **Untergruppen**.
1. Wählen Sie eine Untergruppe aus und klicken Sie dann auf **Kopieren**-Symbol ![Kopieren-Symbol](assets/copy-icon.png), um eine neue Gruppe der obersten Ebene basierend auf der ausgewählten Gruppe zu erstellen.
1. Konfigurieren Sie die Einstellungen der neuen Gruppe.

   Hilfe zu diesen Einstellungen finden Sie unter [Erstellen einer Gruppe der obersten Ebene durch Kopieren einer vorhandenen Gruppe oder Untergruppe](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#create-a-top-level-group-by-copying-an-existing-group-or-subgroup) im Artikel [Erstellen einer Gruppe](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

1. Klicken Sie **Gruppe erstellen**.

## Exportieren einer Untergruppe

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![Gruppen](assets/groups-icon.png).

   In der angezeigten Liste werden die von Ihnen verwalteten Gruppen sowie alle zugehörigen Untergruppen angezeigt. Adobe Workfront-Administratoren können alle Gruppen anzeigen.

1. Klicken Sie auf den Namen der Gruppe, die die zu exportierende Untergruppe enthält.
1. Klicken Sie im linken Menü auf **Untergruppen**.
1. Wählen Sie die zu exportierende Untergruppe bzw. die zu exportierenden Untergruppen aus.
1. Klicken Sie auf **Export**-Symbol ![Export-Symbol](assets/export.png) und wählen Sie dann das gewünschte Dateiformat aus.

## Entfernen Sie eine Untergruppe aus der übergeordneten Gruppe und machen Sie sie zu einer Gruppe der obersten Ebene.

Sie können eine Untergruppe zu einer Gruppe der obersten Ebene machen, indem Sie sie aus der übergeordneten Gruppe entfernen.

>[!TIP]
>
>Wenn Sie eine Gruppe deaktivieren, die Untergruppen enthält, werden diese Untergruppen ebenfalls inaktiv. Wenn Sie möchten, dass eine der Gruppen aktiv ist, können Sie sie mithilfe dieser Anweisungen aus der übergeordneten Gruppe entfernen und dann reaktivieren.
>&#x200B;>Anweisungen zum Deaktivieren und Reaktivieren von Gruppen finden Sie unter [Deaktivieren oder Reaktivieren einer Gruppe](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![Gruppen](assets/groups-icon.png).
1. Wählen Sie die übergeordnete Gruppe der Untergruppe aus, die Sie zu einer Gruppe der obersten Ebene machen möchten, und klicken Sie dann auf das Symbol **Bearbeiten** ![Symbol Bearbeiten](assets/edit-icon.png).
1. Geben Sie im angezeigten Feld **Gruppe bearbeiten** den Namen der Untergruppe, die Sie zu einer Gruppe der obersten Ebene machen möchten, in das Feld **Suche** (unter **Gruppenmitglieder und Gruppenadministratoren**) ein. Klicken Sie dann rechts neben dem Namen auf das X, wenn es angezeigt wird.
1. Klicken Sie auf **Speichern**.

## Löschen einer Untergruppe

>[!IMPORTANT]
>
>Wenn Sie eine Gruppe oder Untergruppe löschen, müssen Sie die Benutzenden, Arbeitselemente und alle Untergruppen beibehalten, die ihr derzeit zugewiesen sind. Um sicherzustellen, dass sie erhalten bleiben, müssen Sie bei einer Eingabeaufforderung die Objekte der Gruppe einer anderen Gruppe zuweisen.

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![Gruppen](assets/groups-icon.png).

   In der angezeigten Liste werden die von Ihnen verwalteten Gruppen sowie alle zugehörigen Untergruppen angezeigt. Adobe Workfront-Administratoren können alle Gruppen anzeigen.

1. Klicken Sie auf den Namen der Gruppe, die die zu löschende Untergruppe enthält.
1. Klicken Sie im linken Menü auf **Untergruppen**.
1. Wählen Sie die Untergruppe aus und klicken Sie dann auf das **Löschen**-Symbol ![Löschen](assets/delete.png).

   Beginnen Sie im angezeigten **Gruppe löschen** mit der Eingabe und wählen Sie dann den Namen der Gruppe aus, in die Sie die Mitglieder, Arbeitselemente und Untergruppen der zu löschenden Gruppe verschieben möchten.

1. Klicken Sie **Löschen**.

## Anzeigen und Verwalten der Untergruppenmitglieder einer Gruppe

Wenn Sie die Hauptseite einer von Ihnen verwalteten Gruppe anzeigen, können Sie alle Benutzenden in den Untergruppen der Gruppe anzeigen und verwalten. Anweisungen finden Sie unter [Anzeigen und Verwalten von Untergruppenmitgliedern](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

