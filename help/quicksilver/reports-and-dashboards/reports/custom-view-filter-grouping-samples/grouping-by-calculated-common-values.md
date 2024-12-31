---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppierung: Organisieren Sie die Listenergebnisse nach einem berechneten Wert, der für alle Objekte in der Gruppierung gleich ist'
description: Sie können Ihre Aufgaben gruppiert nach Prozent abgeschlossen in den Bereichen 0-25, 26-50, 51-75, 75-99 und 100 anzeigen. Dazu können Sie im Textmodus eine Gruppierung erstellen.
author: Nolan
feature: Reports and Dashboards
exl-id: 93b743ce-7e54-4a96-933b-912e2107a84f
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Gruppierung: Organisieren Sie die Listenergebnisse nach einem berechneten Wert, der für alle Objekte in der Gruppierung gleich ist

<!--Audited: 10/2024-->

Sie können Ihre Aufgaben gruppiert nach Prozent abgeschlossen in den Bereichen 0-25, 26-50, 51-75, 75-99 und 100 anzeigen. Dazu können Sie im Textmodus eine Gruppierung erstellen.

![](assets/grouping-calculated-value-column-to-all-objects.png)

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
