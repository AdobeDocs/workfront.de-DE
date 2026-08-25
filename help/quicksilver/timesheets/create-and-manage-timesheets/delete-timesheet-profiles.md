---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Löschen von Arbeitszeittabellenprofilen
description: Sie können ein Arbeitszeittabellen-Profil löschen, das möglicherweise nicht mehr relevant ist.
author: Lisa
feature: Timesheets
exl-id: 1fb39f74-205b-485e-9e8b-a2ab3f9f1ac4
source-git-commit: dbb2e1aee18e6435a79ee2071f0bd5ba84ce2af3
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 17%

---

# Löschen von Arbeitszeittabellenprofilen

<!--Audited:6/2025-->

Durch das Erstellen und Zuweisen von Arbeitszeittabellen-Profilen zu Benutzenden wird die Konsistenz bei der Erstellung von Arbeitszeittabellen durch Adobe Workfront sichergestellt.

Sie können ein Arbeitszeittabellen-Profil löschen, das möglicherweise nicht mehr relevant ist.

Informationen zu Arbeitszeittabellen-Profilen finden Sie [Erstellen, Bearbeiten und Zuweisen von Arbeitszeittabellen-Profilen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
   <td>
   <p>Standard</p>
   <p>Abo</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td><p>Administrativer Zugriff auf Arbeitszeittabellen</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Löschen von Arbeitszeittabellenprofilen

{{step-1-to-setup}}

1. Wenn Sie ein Arbeitszeittabellen-Profil auf Systemebene löschen, klicken Sie auf **Arbeitszeittabelle und Stunden**.

   ODER

   Wenn Sie ein Arbeitszeittabellen-Profil für eine Gruppe löschen, klicken Sie auf **Gruppen** > auf den Namen der Gruppe und dann auf **Arbeitszeittabellen-Profile**.
1. Wählen Sie mindestens ein Arbeitszeittabellen-Profil aus, das Sie löschen möchten, und klicken Sie dann für das systemweite Arbeitszeittabellen-Profil auf das **Mehr**-Symbol ![Mehr](assets/more-icon.png) > **Löschen**.

1. Klicken Sie **Arbeitszeittabellen-Profile**.
1. Wählen Sie mindestens ein Arbeitszeittabellen-Profil aus, das Sie löschen möchten, und klicken Sie dann auf das Symbol Mehr ![Mehr](assets/more-icon.png) > **Löschen**.
ODER
Klicken Sie für **Arbeitszeittabellen-Profil auf** > **Löschen**.
1. (Bedingt) Wenn das Arbeitszeittabellen-Profil bereits Benutzenden zugewiesen ist, wird das Feld **Ersatz-Arbeitszeittabellen** angezeigt. Gehen Sie folgendermaßen vor:
   1. Wählen Sie in der Dropdown-Liste ein anderes Arbeitszeittabellen-Profil aus. Das Arbeitszeittabellen-Profil, das Sie löschen möchten, wird durch das Arbeitszeittabellen-Profil ersetzt, durch das Sie es für alle zugewiesenen Benutzer ersetzen. Arbeitszeittabellen werden entsprechend dem neu zugewiesenen Profil im folgenden Arbeitszeittabellen-Generierungszyklus generiert.
   1. Klicken Sie auf **Löschen**, um den Löschvorgang zu bestätigen.
1. (Bedingt) Wenn das Arbeitszeittabellen-Profil keinen Benutzenden zugewiesen ist, wird das Feld **Arbeitszeittabelle löschen** angezeigt.

   Klicken Sie **Löschen**, um den Löschvorgang zu bestätigen.
