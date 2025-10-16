---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Zeigt Objekte an, die nicht in der Standardschnittstelle enthalten sind'
description: Sie können in einer Ansicht Objekte anzeigen, die nicht in der Standardmodus-Oberfläche enthalten sind. Sie können dies nur tun, indem Sie über den Textmodus auf sie verweisen.
author: Nolan
feature: Reports and Dashboards
exl-id: c0138730-494b-4443-865a-44f8f00d5342
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Anzeigen : Zeigt Objekte an, die nicht in der Standardschnittstelle enthalten sind

Sie können in einer Ansicht Objekte anzeigen, die nicht in der Standardmodus-Oberfläche enthalten sind. Sie können dies nur tun, indem Sie über den Textmodus auf sie verweisen.\
Sie können auf eine der folgenden Arten festlegen, welche Felder in eine Ansicht aufgenommen werden können:

* Verwenden Sie den [API-Explorer](../../../wf-api/general/api-explorer.md), um andere Objekte zu finden, auf die über den Textmodus verwiesen werden kann.\
  Nicht alle im API Explorer dokumentierten Felder sind gültige Felder für den Textmodus. Einige Felder können nur über die API gemeldet werden.

* Suchen Sie das ID-Feld des -Objekts in einer Spalte. Die meisten Objekte mit einer Feld-ID verfügen auch über eine entsprechende Spalte oder einen Feldnamen, auf die bzw. den möglicherweise nicht über die Standardmodus-Oberfläche zugegriffen werden kann.

  Sie können den Textmodus verwenden, um die Spalte oder den Feldnamen anstelle der ID in eine Ansicht aufzunehmen, indem Sie die `fieldnameID` durch die `fieldname:name` ersetzen.

  In der Standardmodus-Benutzeroberfläche ist beispielsweise das Feld **Portfolio-Eigentümer-ID** für eine Projektansicht verfügbar, das Feld **Portfolio-** Name} jedoch nicht. Sie können den Textmodus verwenden, um den **Portfolio-Besitzernamen** in der Spalte einer Ansicht anzuzeigen.

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
   <p>Mitwirkender oder Anfrage zum Ändern eines Filters </p>
   <p>Standard oder Plan zum Ändern eines Berichts</p>
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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Beispiel: Hinzufügen der Spalte &quot;Portfolio-Eigentümername“ zu einer Projektansicht

1. Zu einer Projektliste gehen.
1. Klicken Sie **Dropdown** Menü „Ansicht“ auf **Neue Ansicht**.

1. Klicken Sie **Spalte hinzufügen** und geben Sie dann &quot;Portfolio-Eigentümer-ID“ in das Feld **In dieser Spalte anzeigen** ein. Wählen Sie es aus, wenn es in der Liste angezeigt wird.

1. Klicken Sie **Wechseln Sie in den Textmodus** und dann **Textmodus bearbeiten**.
1. Ersetzen Sie die `valuefield` (`valuefield=portfolio:ownerID`) durch die folgende Zeile:

   `valuefield=portfolio:owner:name`

   Oder

   Entfernen Sie den Text aus dem Feld **Textmodus bearbeiten** und ersetzen Sie ihn durch den folgenden Code:

   ```
   valuefield=portfolio:owner:name
   querysort=portfolio:ownerID
   valueformat=HTML
   displayname=Portfolio Owner Name
   linkedname=portfolio
   ```

   In diesem Beispiel sortiert der Bericht den Bericht nach der Portfolio-Eigentümer-ID, wie in der `querysort` angegeben.

   >[!TIP]
   >
   >Um ein beliebiges `ID` im Textmodus durch das `name` Feld zu ersetzen, ersetzen Sie `ID` in der `:name` Zeile immer durch `valuefield`.

1. Klicken Sie **Fertig** und dann **Ansicht speichern**.
