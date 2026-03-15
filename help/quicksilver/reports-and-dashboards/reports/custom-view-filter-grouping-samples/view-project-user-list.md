---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Liste von Projektbenutzern mit Auftragsrollen'
description: Sie können diese Ansicht in einer Projektliste oder einem Bericht anwenden, um eine Liste der Benutzer anzuzeigen, die dem Projekt zugeordnet sind, sowie eine Liste der Auftragsrollen, die sie für das Projekt ausführen.
author: Courtney
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 14%

---

# Ansicht: Liste der Projektbenutzenden mit Aufgabengebieten

<!--Audited: 11/2024-->

Sie können diese Ansicht in einer Projektliste oder einem Bericht anwenden, um eine Liste der Benutzer anzuzeigen, die dem Projekt zugeordnet sind, sowie eine Liste der Auftragsrollen, die sie für das Projekt ausführen.

Die Informationen in diesem Bericht finden Sie auch im Bereich Personen des Projekts.

>[!TIP]
>
>Wenn keine Jobrollen für die Benutzer aufgelistet sind, aber Sie wissen, dass sie mit Jobrollen in ihren Benutzerprofilen verknüpft sind, kann dies bedeuten, dass sie Vorgängen und Problemen zugewiesen sind, aber möglicherweise nicht mit einer Jobrolle für den Vorgang oder das Problem verknüpft sind, oder dass die im Bericht aufgeführten Benutzer nicht die Bevollmächtigten für Vorgänge und Probleme sind, sondern andere Rollen im Projekt erfüllen (z. B. Eigentümer oder Sponsor).

![project_with_user_and_role_information_report.png](assets/project-with-user-and-role-information-report-350x100.png)

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
   <p>Mitwirkender oder Anforderung zum Ändern einer Ansicht </p>
   <p>Standard oder Abo zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Bearbeitungszugriff auf Filter, Ansichten, Gruppierungen zum Ändern einer Ansicht</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++


## Anzeigen einer Liste von Projektbenutzern mit Arbeitsrollen

1. Gehen Sie zu einer Liste von Projekten.
1. Wählen Sie im Dropdown-Menü **Ansicht** die Option **Neue Ansicht**.
1. Entfernen Sie im Bereich **Spaltenvorschau** alle Spalten mit Ausnahme einer Spalte.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte, und klicken Sie dann auf **In Textmodus wechseln** > **Textmodus bearbeiten**.
1. Entfernen Sie den Text, den Sie im Feld **Textmodus bearbeiten** finden, und ersetzen Sie ihn durch folgenden Code:

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

1. Klicken Sie auf **Fertig** > **Ansicht speichern**.
