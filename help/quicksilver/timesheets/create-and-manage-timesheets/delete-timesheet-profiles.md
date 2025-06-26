---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Arbeitszeittabellen-Profile löschen
description: Sie können ein Arbeitszeittabellen-Profil löschen, das möglicherweise nicht mehr relevant ist.
author: Alina
feature: Timesheets
exl-id: 1fb39f74-205b-485e-9e8b-a2ab3f9f1ac4
source-git-commit: 04818bc054c3bab6e6208b6678365549664d1594
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 0%

---

# Arbeitszeittabellen-Profile löschen

<!--Audited:6/2025-->

Durch das Erstellen und Zuweisen von Arbeitszeittabellen-Profilen zu Benutzenden wird die Konsistenz bei der Erstellung von Arbeitszeittabellen durch Adobe Workfront sichergestellt.

Sie können ein Arbeitszeittabellen-Profil löschen, das möglicherweise nicht mehr relevant ist.

Informationen zu Arbeitszeittabellen-Profilen finden Sie [Erstellen, Bearbeiten und Zuweisen von Arbeitszeittabellen-Profilen](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neu: Standard</p>
   Oder
   <p>Aktuell: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen administrativen Zugriff auf Arbeitszeittabellen haben. </p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Arbeitszeittabellen-Profile löschen

1. Klicken Sie auf **Hauptmenü** Symbol ![](assets/main-menu-icon.png) oben rechts in Adobe Workfront und dann auf **Setup** ![](assets/gear-icon-settings.png).

1. Wenn Sie ein Arbeitszeittabellen-Profil löschen, das im gesamten System verwendet wird, klicken Sie auf **Arbeitszeittabelle und Stunden**.

   Oder

   Wenn Sie ein Arbeitszeittabellen-Profil für eine Gruppe löschen, klicken Sie auf **Gruppen** und dann auf den Namen der Gruppe.

1. Klicken Sie **Arbeitszeittabellen-Profile**.
1. Wählen Sie mindestens ein Arbeitszeittabellen-Profil aus, das Sie löschen möchten, und klicken Sie dann auf **Mehr** > **Löschen**.
1. (Bedingt) Wenn das Arbeitszeittabellen-Profil bereits Benutzenden zugewiesen ist, wird das Feld **Ersatz-Arbeitszeittabellen** angezeigt. Gehen Sie folgendermaßen vor:
   1. Wählen Sie in der Dropdown-Liste ein anderes Arbeitszeittabellen-Profil aus. Das Arbeitszeittabellen-Profil, das Sie löschen möchten, wird durch das Arbeitszeittabellen-Profil ersetzt, durch das Sie es für alle zugewiesenen Benutzer ersetzen. Arbeitszeittabellen werden entsprechend dem neu zugewiesenen Profil im folgenden Arbeitszeittabellen-Generierungszyklus generiert.
   1. Klicken Sie auf **Löschen**, um den Löschvorgang zu bestätigen.
1. (Bedingt) Wenn das Arbeitszeittabellen-Profil keinen Benutzenden zugewiesen ist, wird das Feld **Arbeitszeittabelle löschen** angezeigt.

   Klicken Sie **Löschen**, um den Löschvorgang zu bestätigen.
