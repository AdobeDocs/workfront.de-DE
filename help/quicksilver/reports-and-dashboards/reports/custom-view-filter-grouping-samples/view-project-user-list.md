---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Anzeigen: Liste der Projektbenutzer mit Aufgabengebieten'
description: Sie können diese Ansicht in einer Projektliste oder einem Bericht anwenden, um eine Liste der mit dem Projekt verknüpften Benutzer sowie eine Liste der Aufgabengebiete anzuzeigen, die sie im Projekt ausführen.
author: Nolan
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 0%

---

# Anzeigen: Liste der Projektbenutzer mit Aufgabengebieten

<!--Audited: 11/2024-->

Sie können diese Ansicht in einer Projektliste oder einem Bericht anwenden, um eine Liste der mit dem Projekt verknüpften Benutzer sowie eine Liste der Aufgabengebiete anzuzeigen, die sie im Projekt ausführen.

Die Informationen in diesem Bericht finden Sie auch im Bereich Personen des Projekts.

>[!TIP]
>
>Wenn für die Benutzer keine Aufgabengebiete aufgelistet sind, Sie aber wissen, dass sie in ihren Benutzerprofilen Aufgabengebieten zugeordnet sind, bedeutet dies möglicherweise, dass sie Aufgaben und Problemen zugewiesen sind, aber möglicherweise nicht mit einem Aufgabengebiet für die Aufgabe oder das Problem verknüpft sind, oder dass die im Bericht aufgelisteten Benutzer nicht die Beauftragten für Aufgaben und Probleme sind, sondern andere Rollen für das Projekt erfüllen (z. B. Inhaber oder Sponsor).

![project_with_user_and_role_information_report.png](assets/project-with-user-and-role-information-report-350x100.png)

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


## Anzeigen einer Liste von Projektbenutzenden mit Aufgabengebieten

1. Zu einer Projektliste gehen.
1. Wählen Sie **Dropdown** Menü „Ansicht“ die Option **Neue Ansicht**.
1. Entfernen Sie im Bereich **Spaltenvorschau** alle Spalten mit Ausnahme einer Spalte.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte und dann auf **In Textmodus wechseln** > **Textmodus bearbeiten**.
1. Entfernen Sie den Text aus dem Feld **Textmodus bearbeiten** und ersetzen Sie ihn durch den folgenden Code:

   ```
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.section=0
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=200
   column.1.displayname=Project Users
   column.1.listdelimiter=<br>
   column.1.listmethod=nested(projectUsers).lists
   column.1.textmode=true
   column.1.type=iterate
   column.1.valueexpression={user}.{name}
   column.1.valueformat=HTML
   column.2.displayname=Project Roles
   column.2.listdelimiter=<br>
   column.2.listmethod=nested(projectUserRoles).lists
   column.2.textmode=true
   column.2.type=iterate
   column.2.valueexpression={role}.{name}
   column.2.valueformat=HTML
   ```

1. Klicken Sie **Fertig** > **Ansicht speichern**.
