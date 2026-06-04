---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppierung: Organisieren Sie die Listenergebnisse nach einem berechneten Wert, der für alle Objekte in der Gruppierung gleich ist'
description: Sie können Ihre Aufgaben gruppiert nach Prozent abgeschlossen in den Bereichen 0-25, 26-50, 51-75, 75-99 und 100 anzeigen. Dazu können Sie im Textmodus eine Gruppierung erstellen.
author: Courtney
feature: Reports and Dashboards
exl-id: 93b743ce-7e54-4a96-933b-912e2107a84f
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/VnaXts6I1BhZJXLUABom3d3Lky11dpgwHvzkZ9kiC-c
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 247
ht-degree: 22%

---

# Gruppierung: Listenergebnisse nach einem berechneten Wert organisieren, der für alle Objekte in der Gruppierung gleich ist

<!--Audited: 10/2024-->

Sie können Ihre Aufgaben gruppiert nach Prozent abgeschlossen in den Bereichen 0-25, 26-50, 51-75, 75-99 und 100 anzeigen. Dazu können Sie im Textmodus eine Gruppierung erstellen.

![Gruppierung nach berechnetem Wert](assets/grouping-calculated-value-column-to-all-objects.png)

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

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Organisieren der Listenergebnisse nach einem berechneten Wert, der für alle Objekte in der Gruppierung gleich ist

So wenden Sie diese Gruppierung auf eine Aufgabenliste an:

1. Zu einer Aufgabenliste gehen.
1. Wählen Sie aus dem **Gruppierung** Dropdown-Menü **Neue Gruppierung** aus.

1. Klicken Sie **In Textmodus wechseln**.
1. Fügen Sie im verfügbaren Bereich den folgenden Code hinzu:

   ```
   textmode=true
   group.0.valueexpression=IF({percentComplete}>=0&&{percentComplete}<=25,'0-25%',IF({percentComplete}>25&&{percentComplete}<=50,'26-50%',IF({percentComplete}>50&&{percentComplete}<=75,'51-75%',IF({percentComplete}>75&&{percentComplete}<=100,'76-100%',''))))
   group.0.linkedname=direct
   group.0.valueformat=doubleAsString
   group.0.namekey=percentComplete
   ```

1. Klicken Sie **Fertig** und dann **Gruppierung speichern**.
1. (Optional) Aktualisieren Sie den Gruppierungsnamen und klicken Sie dann auf **Gruppierung speichern**.
