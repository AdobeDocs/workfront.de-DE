---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Inhalt einer Spalte ausblenden'
description: Möglicherweise möchten Sie die Informationen in der Spalte einer Ansicht ausblenden. Sie können dazu den Textmodus der Spalte ändern.
author: Courtney
feature: Reports and Dashboards
exl-id: f4c3e1ca-d750-4f8b-835c-254c20ad72b3
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 13%

---

# Ansicht: Inhalt einer Spalte ausblenden

<!--Audited: 11/2024-->

Möglicherweise möchten Sie die Informationen in der Spalte einer Ansicht ausblenden. Sie können dazu den Textmodus der Spalte ändern.

>[!NOTE]
>
>* Sie können ausgeblendete Spalten verwenden, um nach einem bestimmten Objekt zu sortieren, das nicht in der Ansicht angezeigt werden soll.\
>  Beispielsweise können Sie in einer Vorgangsansicht nach Vorgangsnummer sortieren und die Informationen zur Vorgangsnummer in der Ansicht ausblenden. In diesem Fall hilft das in der Spalte referenzierte Objekt beim Sortieren der Ansicht, aber die Informationen dieses Objekts werden nicht in der Ansicht angezeigt.
>* Wenn Sie eine Spalte ausblenden, beachten Sie, dass die Informationen in der Spalte ausgeblendet sind, die Spalte jedoch weiterhin in der Ansicht vorhanden ist.

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

## Beispiel: Sortieren und Ausblenden der Spalte &quot;Vorgangsnummer&quot; in einer Vorgangsansicht:

1. Wechseln Sie zu einer Liste von Aufgaben.
1. Klicken Sie im Dropdown-Menü **Ansicht** auf **Neue Ansicht**.

1. Klicken Sie auf **Spalte hinzufügen**, und geben Sie im Feld **In dieser Spalte anzeigen** &quot;Vorgangsnummer&quot; ein. Wählen Sie diese Spalte aus, wenn sie in der Liste angezeigt wird.

1. Klicken Sie auf **In Textmodus wechseln**, dann auf **Textmodus bearbeiten**.
1. Entfernen Sie den Text, den Sie im Feld **Textmodus bearbeiten** finden, und ersetzen Sie ihn durch folgenden Code:

   ```
   displayname=
   linkedname=direct
   querysort=taskNumber
   sortOrder=1
   sortType=asc
   textmode=true
   value=
   valueformat=int
   width=0
   ```

   Die wichtigsten Änderungen in diesem Code, die die Spalte ausblenden, sind:

   * `displayname=`: Diese Zeile muss leer sein.
   * `valuefield=`: Diese Zeile muss durch `value=` ersetzt werden, das leer sein muss.
   * `width=`: Je nach Feld muss dieser Wert **0** oder **1** sein.

1. Klicken Sie auf **Fertig** und anschließend auf **Ansicht speichern**.
