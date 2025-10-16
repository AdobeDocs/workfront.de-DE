---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Link zu einem Objekt in einer Spalte entfernen'
description: Einige Objekte, die Sie in einer Ansicht anzeigen, verknüpfen standardmäßig mit der Detailseite des Objekts . Beispielsweise ist die Spalte, die den Namen eines Projekts anzeigt, ein Link zum Projekt; die Spalte, die den Namen eines Benutzers anzeigt, ist ein Link zur Profilseite des Benutzers.
author: Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 0%

---

# Anzeigen : Entfernen eines Links zu einem Objekt in einer Spalte

<!--Audited: 11/2024-->

Einige Objekte, die Sie in einer Ansicht anzeigen, verknüpfen standardmäßig mit der Detailseite des Objekts . Beispielsweise ist die Spalte, die den Namen eines Projekts anzeigt, ein Link zum Projekt; die Spalte, die den Namen eines Benutzers anzeigt, ist ein Link zur Profilseite des Benutzers.

Sie können diesen Link mithilfe des Textmodus in Spalten entfernen, die in allen Ansichten angezeigt werden.

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

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++


## Beispiel: Entfernen des Links zu einer Aufgabe aus der Spalte Aufgabenname in einer Aufgabenansicht:

1. Zu einer Aufgabenliste gehen.
1. Klicken Sie **Dropdown** Menü „Ansicht“ auf **Neue Ansicht**, um eine neue Ansicht zu erstellen.

   Oder

   Klicken Sie auf **Bearbeiten** Symbol ![Bearbeiten](assets/edit-icon.png), um eine vorhandene Ansicht zu bearbeiten, und wählen Sie dann die Ansicht aus.

1. Klicken Sie **Spalte hinzufügen**, um eine neue Spalte hinzuzufügen.

   Oder

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

