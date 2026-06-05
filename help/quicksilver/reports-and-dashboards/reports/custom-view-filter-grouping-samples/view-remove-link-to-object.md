---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Link zu einem Objekt in einer Spalte entfernen'
description: Einige Objekte, die Sie in einer Ansicht anzeigen, verknüpfen standardmäßig mit der Detailseite des Objekts . Beispielsweise ist die Spalte, die den Namen eines Projekts anzeigt, ein Link zum Projekt; die Spalte, die den Namen eines Benutzers anzeigt, ist ein Link zur Profilseite des Benutzers.
author: Courtney
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/J-FHP3ySrleMgoRDrh5xzapQfqjtwraEAwX8xwvKTuk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 372
ht-degree: 13%

---

# Ansicht: Link zu einem Objekt in einer Spalte entfernen

<!--Audited: 11/2024-->

Einige Objekte, die Sie in einer Ansicht anzeigen, verknüpfen standardmäßig mit der Detailseite des Objekts . Beispielsweise ist die Spalte, die den Namen eines Projekts anzeigt, ein Link zum Projekt; die Spalte, die den Namen eines Benutzers anzeigt, ist ein Link zur Profilseite des Benutzers.

Sie können diesen Link mithilfe des Textmodus in Spalten entfernen, die in allen Ansichten angezeigt werden.

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
   <p>Mitwirkender oder Anfrage zum Ändern einer Ansicht </p>
   <p>Standard oder Plan zum Ändern eines Berichts</p>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++


## Beispiel: Entfernen des Links zu einer Aufgabe aus der Spalte Aufgabenname in einer Aufgabenansicht:

1. Zu einer Aufgabenliste gehen.
1. Klicken Sie **Dropdown** Menü „Ansicht“ auf **Neue Ansicht**, um eine neue Ansicht zu erstellen.

   ODER

   Klicken Sie auf **Bearbeiten** Symbol ![Bearbeiten](assets/edit-icon.png), um eine vorhandene Ansicht zu bearbeiten, und wählen Sie dann die Ansicht aus.

1. Klicken Sie **Spalte hinzufügen**, um eine neue Spalte hinzuzufügen.

   ODER

   Klicken Sie auf eine vorhandene Spalte mit einem Link zu einem Objekt.

1. Klicken Sie **In Textmodus wechseln** > **Textmodus bearbeiten**.
1. Entfernen Sie den Text aus dem Feld **Textmodus bearbeiten** und ersetzen Sie ihn durch den folgenden Code:

   ```
   displayname=Task Name
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression={name}
   valueformat=Compound
   ```

   >[!TIP]
   >
   >Sie können ähnlichen Code für andere Objekte verwenden, indem Sie Folgendes anpassen:
   >
   >* Ersetzen Sie die `valuefield` Zeile des Codes durch `valueexpression` und behalten Sie denselben Namen, der in geschweiften Klammern nach dem Gleichheitszeichen enthalten ist, bei.
   >* Entfernen Sie alle Zeilen, die mit `link.` beginnen, aus dem ursprünglichen Text der Spalte. Entfernen Sie beispielsweise alle folgenden Zeilen:
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. Klicken Sie **Fertig** und dann **Ansicht speichern**.

