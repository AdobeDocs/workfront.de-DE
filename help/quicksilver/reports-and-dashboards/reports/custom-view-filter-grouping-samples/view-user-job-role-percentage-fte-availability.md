---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Prozentsatz der FTE-Verfügbarkeit für Benutzeraufgabengebiet'
description: Sie können der Ansicht einer Benutzerliste eine Spalte hinzufügen, um eine Liste der Aufgabengebiete anzuzeigen, mit denen der Benutzer verknüpft ist, sowie den Prozentsatz der FTE-Verfügbarkeit für jedes Aufgabengebiet, wie im Benutzerprofil definiert.
author: Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 0%

---

# Anzeigen: Prozentsatz der FTE-Verfügbarkeit für das Aufgabengebiet des Benutzers

<!--Audited: 11/2024-->

Sie können der Ansicht einer Benutzerliste eine Spalte hinzufügen, um eine Liste der Aufgabengebiete anzuzeigen, mit denen der Benutzer verknüpft ist, sowie den Prozentsatz der FTE-Verfügbarkeit für jedes Aufgabengebiet, wie im Benutzerprofil definiert.

Informationen zum Definieren des Prozentsatzes der FTE-Verfügbarkeit für -Benutzer finden Sie [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

![user_with_percent_available_per_role.png](assets/user-with-percent-avialbility-per-role-350x138.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Mitwirkender oder Anfrage zum Ändern einer Ansicht </p>
   <p>Standard oder Plan zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Prozentualen Anteil der FTE-Verfügbarkeit für Benutzeraufgabengebiet anzeigen

1. Zu einer Benutzerliste wechseln.
1. Wählen Sie **Dropdown** Menü „Ansicht“ die Option **Neue Ansicht**.

1. Klicken Sie im Bereich **Spaltenvorschau** auf **Spalte hinzufügen**.

1. Klicken Sie auf die Kopfzeile der neuen Spalte und dann auf **Wechseln in den Textmodus** > **Textmodus bearbeiten**.
1. Entfernen Sie den Text aus dem Feld **Textmodus bearbeiten** und ersetzen Sie ihn durch den folgenden Code:

   ```
   displayname=Roles Time Percentage
   listdelimiter=
   listmethod=nested(userRoles).lists
   textmode=true
   type=iterate
   valueexpression=CONCAT({role},'-',{timePercentage},'%')
   valueformat=HTML
   ```

1. Klicken Sie **Fertig** und dann **Ansicht speichern**.

1. (Optional) Aktualisieren Sie den Ansichtsnamen und klicken Sie dann auf **Ansicht speichern**.
