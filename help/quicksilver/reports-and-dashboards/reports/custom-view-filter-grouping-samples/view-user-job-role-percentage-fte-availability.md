---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Prozentsatz der FTE-Verfügbarkeit der Benutzerauftragsrolle"
description: Sie können der Ansicht einer Benutzerliste eine Spalte hinzufügen, um eine Liste der mit dem Benutzer verknüpften Vorgangsrollen sowie den Prozentsatz der FTE-Verfügbarkeit für jede Vorgangsrolle anzuzeigen, wie im Benutzerprofil definiert.
author: Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 66de6c952272f52876f8e912c96d1526575b6f0b
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Ansicht: Prozentsatz der FTE-Verfügbarkeit der Benutzerauftragsrolle

<!--Audited: 11/2024-->

Sie können der Ansicht einer Benutzerliste eine Spalte hinzufügen, um eine Liste der mit dem Benutzer verknüpften Vorgangsrollen sowie den Prozentsatz der FTE-Verfügbarkeit für jede Vorgangsrolle anzuzeigen, wie im Benutzerprofil definiert.

Informationen zum Definieren des Prozentsatzes der FTE-Verfügbarkeit für Benutzer finden Sie unter [Profil eines Benutzers bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

![user_with_percent_available_per_role.png](assets/user-with-percent-avialbility-per-role-350x138.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p> Aktuell: 
   <ul>
   <li>Anforderung zum Ändern einer Ansicht</li> 
   <li>Berichtänderung planen</li>
   </ul>
     </p>
     <p> Neu: 
   <ul>
   <li>Mitwirkender beim Ändern einer Ansicht</li> 
   <li>Standard zum Ändern eines Berichts</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prozentsatz der FTE-Verfügbarkeit für Benutzerauftragsrolle anzeigen

1. Navigieren Sie zu einer Liste von Benutzern.
1. Wählen Sie aus dem Dropdownmenü **Ansicht** die Option **Neue Ansicht** aus.

1. Klicken Sie im Bereich **Spaltenvorschau** auf **Spalte hinzufügen**.

1. Klicken Sie auf die Kopfzeile der neuen Spalte und dann auf **In Textmodus wechseln** > **Textmodus bearbeiten**.
1. Entfernen Sie den Text, den Sie im Feld **Textmodus bearbeiten** finden, und ersetzen Sie ihn durch den folgenden Code:

   ```
   displayname=Roles Time Percentage
   listdelimiter=
   listmethod=nested(userRoles).lists
   textmode=true
   type=iterate
   valueexpression=CONCAT({role},'-',{timePercentage},'%')
   valueformat=HTML
   ```

1. Klicken Sie auf **Fertig** und dann auf **Ansicht speichern**.

1. (Optional) Aktualisieren Sie den Ansichtsnamen und klicken Sie dann auf **Ansicht speichern**.
