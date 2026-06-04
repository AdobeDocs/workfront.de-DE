---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Namen der übergeordneten Aufgaben in Großbuchstaben anzeigen'
description: Sie können diese Spalte zu einer Aufgabenansicht hinzufügen, um den Namen der übergeordneten Aufgaben in Großbuchstaben anzuzeigen.
author: Courtney
feature: Reports and Dashboards
exl-id: bb489920-6b17-4689-b432-b0c28bcb5d10
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/WYEh0h4BI8XzeV1TLSOix9-fgg33etfitS7U4rczXgo
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 244
ht-degree: 20%

---

# Ansicht: Namen der übergeordneten Aufgaben mit allen Obergrenzen anzeigen

<!--Audited: 10/2024-->

Sie können diese Spalte zu einer Aufgabenansicht hinzufügen, um den Namen der übergeordneten Aufgaben in Großbuchstaben anzuzeigen.

![Spalte mit übergeordneter Aufgabe in Großbuchstaben](assets/column-task-with-all-caps-parent-350x112.png)

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

## Namen der übergeordneten Aufgaben in Großbuchstaben anzeigen

Diese Spalte in einer Aufgabenansicht erstellen:

1. Zu einer Aufgabenliste gehen.
1. Wählen **aus dem Dropdown** Menü „Ansicht“ eine Ansicht aus und klicken Sie dann auf das **Bearbeiten**-Symbol ![Bearbeiten](assets/edit-icon.png).
oder\
   Wählen Sie **Dropdown** Menü „Ansicht“ die Option **Neue Ansicht**.

1. Klicken Sie im Bereich **Spaltenvorschau** auf die Kopfzeile der Spalte, die den Aufgabennamen in der Liste anzeigt.
1. Klicken Sie **Wechseln Sie in den Textmodus** und klicken Sie dann auf **Textmodus bearbeiten**.
1. Entfernen Sie den Text aus dem Feld **Textmodus** und ersetzen Sie ihn durch den folgenden Code:

   ```
   linkedname=direct
   namekey=name
   querysort=name
   styledef.case.0.comparison.icon=false
   styledef.case.0.comparison.leftmethod=numberOfChildren
   styledef.case.0.comparison.lefttext=numberOfChildren
   styledef.case.0.comparison.operator=gt
   styledef.case.0.comparison.operatortype=int
   styledef.case.0.comparison.righttext=0
   styledef.case.0.comparison.trueproperty.0.name=fontstyle
   styledef.case.0.comparison.trueproperty.0.value=bold
   valueexpression=IF({numberOfChildren}>"0",UPPER({name}),{name})
   valueformat=HTML
   ```

1. Klicken Sie **Fertig** und dann auf **Ansicht speichern**.
