---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Auflösbare Objekte in einem Aufgaben- oder Projektbericht"
description: Sie können eine Liste aller auflösbaren Objekte in einer Projekt- oder Aufgabenansicht oder einem Bericht anzeigen.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Ansicht: Auflösbare Objekte in einem Aufgaben- oder Projektbericht

Sie können eine Liste aller auflösbaren Objekte in einer Projekt- oder Aufgabenansicht oder einem Bericht anzeigen.

Weitere Informationen zu auflösbaren Objekten finden Sie im Artikel [Übersicht über das Auflösen und Auflösen von Objekten](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

![list_of_resolvables_in_report.png](assets/list-of-resolvables-in-report-350x54.png)

Die Anwendung dieser Ansicht ist für Aufgaben und Projekte identisch.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Auflösbare Objekte in einem Aufgaben- oder Projektbericht anzeigen

1. Gehen Sie zu einer Liste der Aufgaben, die aus Problemen konvertiert wurden.
1. Aus dem **Ansicht** Dropdown-Menü auswählen **Neue Ansicht**.

1. Im **Spaltenvorschau** Bereich, klicken Sie **Spalte hinzufügen**.

1. Klicken Sie auf die Kopfzeile der neuen Spalte und dann auf **In den Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im **Textmodus** und ersetzen Sie sie durch den folgenden Code:

   <pre>displayName=Resolvables<br>listdelimiter=<br><br>listmethod=nested(resolvables).lists<br>textmode=true<br>type=iterate<br>valueField=name<br>valueFormat=HTML<br></pre>

1. Klicken **Ansicht speichern**.\
   In der neuen Spalte wird eine Liste aller auflösbaren Objekte angezeigt. Die Namen der Objekte in der Liste können nicht direkt mit den Objekten verknüpft werden.
