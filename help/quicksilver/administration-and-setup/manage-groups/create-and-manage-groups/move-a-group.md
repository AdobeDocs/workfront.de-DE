---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-groups
title: Verschieben einer Gruppe
description: Sie können eine Gruppe in eine andere Gruppe verschieben, die Sie verwalten.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: f5227454-457d-40d3-865c-c2551471d83e
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# Verschieben einer Gruppe

Sie können eine Gruppe in eine andere Gruppe verschieben, die Sie verwalten.

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

## Eine Gruppe in eine andere Gruppe verschieben

>[!NOTE]
>
>Wenn die Status der verschobenen Gruppe gesperrt sind, übernimmt sie die Status der neuen übergeordneten Gruppe.
>
>Wenn die Status der verschobenen Gruppe entsperrt sind, übernimmt die neue übergeordnete Gruppe weder die Status der neuen übergeordneten Gruppe, noch übernimmt die neue übergeordnete Gruppe deren Status.
>
>Weitere Informationen zum Gruppenstatus finden Sie unter [Erstellen oder Bearbeiten eines ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) und [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![Gruppen](assets/groups-icon.png).

1. Wählen Sie die Zielgruppe aus, in die Sie die Gruppe verschieben möchten, und klicken Sie dann auf das Symbol Bearbeiten ![Symbol Bearbeiten](assets/edit-icon.png).
1. Geben Sie im angezeigten **Gruppe bearbeiten** unter **Gruppenmitglieder und Gruppenadministratoren** den Namen der Gruppe ein, die Sie verschieben möchten, und klicken Sie dann auf den Namen, wenn er angezeigt wird.
1. Klicken Sie auf **Speichern**.

>[!TIP]
>
>Sie können eine Untergruppe auch zu einer Gruppe der obersten Ebene machen. Anweisungen finden Sie im Abschnitt [Entfernen einer Untergruppe aus der übergeordneten Gruppe und Festlegen als Gruppe der obersten Ebene](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md#make) im Artikel [Verwalten einer Untergruppe](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/manage-subgroups.md).
