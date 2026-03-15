---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Zeigt Objekte an, die nicht in der Standardbenutzeroberfläche enthalten sind'
description: Sie können Objekte, die nicht in der Standardmodusschnittstelle enthalten sind, in einer Ansicht anzeigen. Sie können dies nur tun, indem Sie sie über den Textmodus referenzieren.
author: Courtney
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 9%

---

# Ansicht: Zeigt Objekte an, die nicht in der Standardschnittstelle enthalten sind.

Sie können in einer Ansicht Objekte anzeigen, die nicht in der Standardmodus-Oberfläche enthalten sind. Sie können dies nur tun, indem Sie über den Textmodus auf sie verweisen.\
Sie können auf eine der folgenden Arten bestimmen, welche Felder in einer Ansicht enthalten sein können:

* Verwenden Sie den [API-Explorer](../../../wf-api/general/api-explorer.md), um andere Objekte zu ermitteln, auf die im Textmodus verwiesen werden kann.\
  Nicht alle im API-Explorer dokumentierten Felder sind für den Textmodus gültig. Einige Felder können nur über die API gemeldet werden.

* Suchen Sie das ID-Feld des Objekts in einer Spalte. Die meisten Objekte mit einer Feld-ID haben auch einen entsprechenden Spalten- oder Feldnamen, auf den möglicherweise nicht über die Oberfläche im Standardmodus zugegriffen werden kann.

  Sie können den Textmodus verwenden, um anstelle der ID den Spalten- oder Feldnamen in eine Ansicht aufzunehmen, indem Sie `fieldnameID` durch `fieldname:name` ersetzen.

  Beispielsweise ist in der Standardmodusschnittstelle das Feld **Portfolio-Eigentümer-ID** für eine Projektansicht verfügbar, das Feld **Portfolio-Eigentümername** jedoch nicht. Sie können den Textmodus verwenden, um den Namen des Eigentümers des **Portfolios** in der Spalte einer Ansicht anzuzeigen.

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
   <p>Anbieter oder Anforderung zum Ändern eines Filters </p>
   <p>Standard oder Abo zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards, Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Bearbeitungszugriff auf Filter, Ansichten, Gruppierungen zum Ändern eines Filters</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Beispiel: Hinzufügen der Spalte &quot;Portfolio-Eigentümername“ zu einer Projektansicht

1. Gehen Sie zu einer Liste von Projekten.
1. Klicken Sie im Dropdown-Menü **Ansicht** auf **Neue Ansicht**.

1. Klicken Sie auf **Spalte hinzufügen**, geben Sie im Feld **In dieser Spalte anzeigen** die Portfolio-Eigentümer-ID ein, und wählen Sie sie aus, wenn sie in der Liste angezeigt wird.

1. Klicken Sie auf **In Textmodus wechseln**, dann auf **Textmodus bearbeiten**.
1. Ersetzen Sie die Zeile `valuefield` (`valuefield=portfolio:ownerID`) durch die folgende Zeile:

   `valuefield=portfolio:owner:name`

   ODER

   Entfernen Sie den Text, den Sie im Feld **Textmodus bearbeiten** finden, und ersetzen Sie ihn durch folgenden Code:

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   In diesem Beispiel sortiert der Bericht den Bericht nach der Portfolio-Eigentümer-ID, wie in der Zeile `querysort` angegeben.

   >[!TIP]
   >
   >Um ein beliebiges `ID` im Textmodus durch das `name` Feld zu ersetzen, ersetzen Sie `ID` in der `:name` Zeile immer durch `valuefield`.

1. Klicken Sie **Fertig** und dann **Ansicht speichern**.
