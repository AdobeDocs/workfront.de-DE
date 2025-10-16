---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Anzeigen: Projekt mit allen Benutzenden und Rollen des Projektteams'
description: Diese Projektansicht zeigt eine Liste der dem Projekt-Team zugewiesenen Benutzer und Aufgabengebiete.
author: Nolan
feature: Reports and Dashboards
exl-id: 84a1e065-992e-4aa5-81ba-e699ac704837
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Anzeigen: Projekt mit allen Benutzenden und Rollen des Projektteams

<!--Audited: 11/2024-->

Diese Projektansicht zeigt eine Liste der dem Projekt-Team zugewiesenen Benutzer und Aufgabengebiete.

>[!NOTE]
>
>Wenn das Aufgabengebiet in derselben Zeile wie ein Benutzer aufgeführt ist, bedeutet dies nicht, dass der Benutzer diese Rolle im Projekt ausfüllt oder dass dem Benutzer diese Rolle in seinem Profil zugewiesen ist.

![PROJECT_CUSTOM_VIEW_WITH_ALL_USERS_AND_ROLES_ON_THE_PROJECT_PNG](assets/project-custom-view-350x52.png)

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

## Ein Projekt mit allen Benutzern und Rollen des Projektteams anzeigen

1. Zu einer Projektliste gehen.
1. Wählen Sie **Dropdown** Menü „Ansicht“ die Option **Neue Ansicht**.

1. Entfernen Sie im Bereich **Spaltenvorschau** alle Spalten mit Ausnahme einer Spalte.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte und dann auf **In Textmodus wechseln** > **Textmodus bearbeiten**.
1. Entfernen Sie den Text aus dem Feld **Textmodus bearbeiten** und ersetzen Sie ihn durch den folgenden Code:




   <pre>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=int<br>column.0.link.lookup=link.view<br>column.0.link.valueField=objCode<br>column.0.link.valueFormat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.nameKey=name.abbr<br>column.0.querysort name<br>column.0.shortView=false<br>column.0.stretch=60<br>column.0.valueField=name<br>column.0.valueFormat=HTMLHTML HTML <br>column.0.width=150<br>column.1.description=Team Users<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valueField=userID<br>column.1.link.linkproperty.0.valueFormat=int<br>column.1.link.page=/userView.cmd<br>column.1.listentraliiter=column.1.listmethod=nested(Users).listsColumn.1.namekey=user.pluralwidthColumn.1.userStretch=30<br>Column=iterateDateColumnValue.1.5 Roles<br>column.2.link.link.property.0.name=ID<br>column.2.link.linkproperty.0.valueField=ID<br>column.2.link.linkproperty.0.valueFormat=intColumn.2.link.page=/roleView.cmdstretchColumn.2.listdelimiIter=Column2.listmethod=nested(roles).listsColumn.2.namekey=jobrole.pluralwidth.2.stretch=10<br><br> <br> <br> <br> <br> <br> <br> <br> <br> <br> <br> <br> <br> <br> <br> Column.2.type=iterateColumn2.Value5</pre>

1. Klicken Sie **Fertig** > **Ansicht speichern**.
