---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-groups
title: Verschieben einer Gruppe
description: Sie können eine Gruppe unter eine andere Gruppe verschieben, die Sie verwalten.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f5227454-457d-40d3-865c-c2551471d83e
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 1%

---

# Gruppe verschieben

Sie können eine Gruppe unter eine andere Gruppe verschieben, die Sie verwalten.

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

## Verschieben einer Gruppe unter einer anderen Gruppe

>[!NOTE]
>
>Wenn die Status der verschobenen Gruppe gesperrt sind, übernimmt sie den Status ihrer neuen übergeordneten Gruppe.
>
>Wenn die Status der verschobenen Gruppe entsperrt sind, übernimmt sie weder den Status der neuen übergeordneten Gruppe noch übernimmt die neue übergeordnete Gruppe den Status.
>
>Weitere Informationen zu Gruppenstatus finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) und [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png).

1. Wählen Sie die Zielgruppe aus, in die Sie die Gruppe verschieben möchten, und klicken Sie dann auf das Bearbeitungssymbol ![](assets/edit-icon.png).
1. Geben Sie im angezeigten Feld **Gruppe bearbeiten** unter **Gruppenmitglieder und Gruppenadministratoren** den Namen der Gruppe ein, die Sie verschieben möchten, und klicken Sie dann auf die Gruppe, wenn sie angezeigt wird.
1. Klicken Sie auf **Speichern**.

>[!TIP]
>
>Sie können eine Untergruppe auch zu einer Gruppe der obersten Ebene machen. Anweisungen finden Sie im Abschnitt &quot;[Entfernen einer Untergruppe aus ihrer übergeordneten Gruppe&quot;und machen Sie sie zu einer Gruppe der obersten Ebene](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make)&quot;im Artikel &quot;[Verwalten einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md)&quot;.
