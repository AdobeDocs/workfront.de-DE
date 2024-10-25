---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Nur Elemente im Genehmigungsstatus anzeigen'
description: Sie können nur Elemente mit einem bestimmten Status anzeigen, der sich derzeit in "Ausstehende Genehmigung"befindet. Dies gilt für alle anderen Objekte mit Genehmigungsstatus.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 1%

---

# Filter: Nur Elemente im Genehmigungsstatus anzeigen

<!--Audited: 10/2024-->

Sie können nur Elemente mit einem bestimmten Status anzeigen, der sich derzeit in &quot;Ausstehende Genehmigung&quot;befindet. Dies gilt für alle anderen Objekte mit Genehmigungsstatus.

Sie können die folgenden Objekte in einen Genehmigungsstatus platzieren:

* Aufgaben
* Probleme
* Projekte

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
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkende bei der Änderung eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filteranforderung </p></li>
   <li><p>Berichtänderung planen</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Nur Elemente im Genehmigungsstatus anzeigen

1. Gehen Sie zu einer Projektliste.
1. Wählen Sie aus dem Dropdownmenü **Filter** die Option **Neuer Filter** aus.
1. Wählen Sie die Filterung nach **Projekt: Status** aus und wählen Sie dann den Status aus, nach dem Sie filtern möchten.

   Fügen Sie beispielsweise in einem Projektbericht **Status gleich Planung** hinzu, wenn Sie nur Projekte anzeigen möchten, die den Status **Planung - Ausstehende Genehmigung** aufweisen.
1. Klicken Sie auf **Textmodus**.
1. Ändern Sie die Zeile `status`, indem Sie dem 3-Buchstaben-Schlüssel des Status **:A** hinzufügen:
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Klicken Sie auf **Anwenden** > **Als neu speichern**.

   In der Liste werden nur Projekte angezeigt, die den Status Planung - Ausstehende Genehmigung aufweisen.
