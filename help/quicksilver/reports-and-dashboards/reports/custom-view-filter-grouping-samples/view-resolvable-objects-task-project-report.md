---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Auflösbare Objekte in einem Aufgaben- oder Projektbericht'
description: Sie können eine Liste aller lösbaren Objekte in einer Projekt- oder Aufgabenansicht oder einem Bericht anzeigen.
author: Nolan
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
source-git-commit: 17a277a5a63a521ec7285e3f5051bfd42fc204bf
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Ansicht: Auflösbare Objekte in einem Aufgaben- oder Projektbericht

<!--Audited: 11/2024-->

Sie können eine Liste aller lösbaren Objekte in einer Projekt- oder Aufgabenansicht oder einem Bericht anzeigen.

Weitere Informationen zu auflösbaren Objekten finden Sie im Artikel [Übersicht über auflösbare und auflösbare Objekte](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

![list_of_resolvables_in_report.png](assets/list-of-resolvables-in-report-350x54.png)

Die Anwendung dieser Ansicht ist für Aufgaben und Projekte identisch.

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
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p> Aktuell: 
   <ul>
   <li>Änderung einer Ansicht anfordern</li> 
   <li>Planen der Änderung eines Berichts</li>
   </ul>
     </p>
     <p> Neu: 
   <ul>
   <li>Mitwirkende zum Ändern einer Ansicht</li> 
   <li>Standard zum Ändern eines Berichts</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Auflösbare Objekte in einem Aufgaben- oder Projektbericht anzeigen

1. Navigieren Sie zu einer Liste der Aufgaben oder Projekte, die aus Problemen konvertiert wurden.
1. Klicken Sie **Dropdown** Menü „Ansicht“ auf **Neue Ansicht**.

1. Klicken Sie im Bereich **Spaltenvorschau** auf **Spalte hinzufügen**.

1. Klicken Sie auf die Kopfzeile der neuen Spalte und dann auf **Wechseln in den Textmodus** > **Textmodus bearbeiten**.
1. Entfernen Sie den Text aus dem Feld **Textmodus bearbeiten** und ersetzen Sie ihn durch den folgenden Code:

   ```
   displayname=Resolvables
   listdelimiter=<br>
   listmethod=nested(resolvables).lists
   textmode=true
   type=iterate
   valuefield=name
   valueformat=HTML
   ```

1. Klicken Sie **Fertig** > **Ansicht speichern**.\
   In der neuen Spalte wird eine Liste aller auflösbaren Objekte angezeigt. Die Namen der Objekte in der Liste können nicht direkt mit den Objekten verknüpft werden.
