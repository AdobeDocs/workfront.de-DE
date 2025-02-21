---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Anzeigen : Anzeigen von Programm- und Portfolio-Informationen in einer Aufgabenansicht'
description: Diese Aufgabenansicht zeigt das Programm und Portfolio an, die mit dem Projekt der Aufgabe verknüpft sind. Diese Informationen sind beim Erstellen einer Aufgabenansicht in Report Builder nicht verfügbar. Diese Informationen sind nur im Textmodus verfügbar.
author: Nolan
feature: Reports and Dashboards
exl-id: cdd5a1e9-3cbf-4951-b803-fca544b2519a
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Anzeigen : Anzeigen von Programm- und Portfolio-Informationen in einer Aufgabenansicht

Diese Aufgabenansicht zeigt das Programm und Portfolio an, die mit dem Projekt der Aufgabe verknüpft sind. Diese Informationen sind beim Erstellen einer Aufgabenansicht in Report Builder nicht verfügbar. Diese Informationen sind nur im Textmodus verfügbar.

Die Ansicht enthält auch Links zu Projekten, Programmen und Portfolio aus einer Aufgabenliste.

![Programm und Portfolio anzeigen](assets/view--program-and-portfolio-350x116.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

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
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkender zum Ändern eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filter ändern </p></li>
   <li><p>Planen der Änderung eines Berichts</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anzeigen von Programm- und Portfolio-Informationen in einer Aufgabenansicht

1. Zu einer Aufgabenliste gehen.
1. Wählen Sie **Dropdown** Menü „Ansicht“ die Option **Neue Ansicht**.

1. Entfernen Sie **Bereich „Spaltenvorschau** alle Spalten mit Ausnahme einer Spalte.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte, klicken Sie auf **Wechseln in den Textmodus** und dann **Textmodus bearbeiten**.
1. Entfernen Sie den Text aus dem Feld **Textmodus bearbeiten** und ersetzen Sie ihn durch den folgenden Code:

   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=project
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=project:ID
   column.1.link.linkproperty.0.valueformat=int
   column.1.link.lookup=link.view
   column.1.link.valuefield=project:objCode
   column.1.link.valueformat=val
   column.1.linkedname=project
   column.1.listsort=nested(project).string(name)
   column.1.namekey=project
   column.1.querysort=project:name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=project:name
   column.1.valueformat=HTML
   column.1.width=150
   column.2.descriptionkey=program
   column.2.displayname=Program
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=project:program:ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.valuefield=project:program:objCode
   column.2.link.valueformat=val
   column.2.linkedname=project
   column.2.listsort=nested(project:program).string(name)
   column.2.namekey=project
   column.2.querysort=project:program:name
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=project:program:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.descriptionkey=portfolio
   column.3.displayname=Portfolio
   column.3.link.linkproperty.0.name=ID
   column.3.link.linkproperty.0.valuefield=project:portfolio:ID
   column.3.link.linkproperty.0.valueformat=int
   column.3.link.lookup=link.view
   column.3.link.valuefield=project:portfolio:objCode
   column.3.link.valueformat=val
   column.3.linkedname=project
   column.3.listsort=nested(project:portfolio).string(name)
   column.3.namekey=project
   column.3.querysort=project:portfolio:name
   column.3.shortview=false
   column.3.stretch=0
   column.3.valuefield=project:portfolio:name
   column.3.valueformat=HTML
   column.3.width=150 
   ```

1. Klicken Sie **Fertig** > **Ansicht speichern**.
