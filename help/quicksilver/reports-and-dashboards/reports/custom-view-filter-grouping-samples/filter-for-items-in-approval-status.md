---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Nur Elemente mit einem Genehmigungsstatus anzeigen'
description: Sie können nur Elemente in einem bestimmten Status anzeigen, der sich derzeit in der ausstehenden Genehmigung befindet. Dies funktioniert bei allen anderen Objekten mit einem Genehmigungsstatus genauso.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 1%

---

# Filter: Nur Elemente mit einem Genehmigungsstatus anzeigen

<!--Audited: 10/2024-->

Sie können nur Elemente in einem bestimmten Status anzeigen, der sich derzeit in der ausstehenden Genehmigung befindet. Dies funktioniert bei allen anderen Objekten mit einem Genehmigungsstatus genauso.

Sie können die folgenden Objekte in einen Genehmigungsstatus versetzen:

* Aufgaben
* Probleme
* Projekte

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

## Nur Elemente im Genehmigungsstatus anzeigen

1. Zu einer Projektliste gehen.
1. Wählen Sie **Dropdown** Menü „Filter“ die Option **Neuer Filter**.
1. Wählen Sie „Filtern nach **Projekt: Status** und wählen Sie dann in der Liste den Status aus, nach dem Sie filtern möchten.

   Fügen Sie beispielsweise in einem Projektbericht den **Status Planung** ein, wenn Sie nur Projekte anzeigen möchten, die den Status &quot;**- Genehmigung steht aus“**.
1. Klicken Sie **Textmodus**.
1. Ändern Sie die `status`, indem Sie **:A** zum aus drei Buchstaben bestehenden Schlüssel des Status hinzufügen:
   <pre>status=PLN:A<br>status_mod=in</pre>

1. Klicken Sie **Übernehmen** > **Als neu speichern**.

   In der Liste werden nur Projekte angezeigt, die sich im Status Planung - Genehmigung steht aus befinden.
