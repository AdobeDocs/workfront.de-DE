---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Link zu einem Objekt in einer Spalte entfernen"
description: Einige Objekte, die Sie in einer Ansicht anzeigen, verlinken standardmäßig zur Seite Details des Objekts. Beispielsweise ist die Spalte, die den Namen eines Projekts anzeigt, ein Link zum Projekt. Die Spalte, die den Namen eines Benutzers anzeigt, ist ein Link zur Profilseite des Benutzers.
author: Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 17a277a5a63a521ec7285e3f5051bfd42fc204bf
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Ansicht: Link zu einem Objekt in einer Spalte entfernen

<!--Audited: 11/2024-->

Einige Objekte, die Sie in einer Ansicht anzeigen, verlinken standardmäßig zur Seite Details des Objekts. Beispielsweise ist die Spalte, die den Namen eines Projekts anzeigt, ein Link zum Projekt. Die Spalte, die den Namen eines Benutzers anzeigt, ist ein Link zur Profilseite des Benutzers.

Sie können diesen Link mithilfe des Textmodus in Spalten entfernen, die in allen Ansichten angezeigt werden.

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
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p> Aktuell: 
   <ul>
   <li>Anforderung zum Ändern einer Ansicht</li> 
   <li>Berichtänderung planen</li>
   </ul>
     </p>
     <p> Neu: 
   <ul>
   <li>Mitwirkender beim Ändern einer Ansicht</li> 
   <li>Standard zum Ändern eines Berichts</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Beispiel: Entfernen Sie den Link zu einer Aufgabe aus der Spalte &quot;Task Name&quot;in einer Aufgabenansicht:

1. Gehen Sie zu einer Liste von Aufgaben.
1. Klicken Sie im Dropdownmenü **Ansicht** auf **Neue Ansicht** , um eine neue Ansicht zu erstellen.

   Oder

   Klicken Sie auf das Symbol **Bearbeiten** ![](assets/edit-icon.png)

   um eine vorhandene Ansicht zu bearbeiten, wählen Sie die Ansicht aus.

1. Klicken Sie auf **Spalte hinzufügen** , um eine neue Spalte hinzuzufügen.

   Oder

   Klicken Sie auf eine vorhandene Spalte mit einer Verknüpfung zu einem Objekt.

1. Klicken Sie auf **Wechseln zum Textmodus** > **Textmodus bearbeiten**.
1. Entfernen Sie den Text, den Sie im Feld **Textmodus bearbeiten** finden, und ersetzen Sie ihn durch den folgenden Code:

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
   >* Ersetzen Sie die Zeile `valuefield` des Codes durch `valueexpression` und behalten Sie den gleichen Namen, der nach dem Gleichheitszeichen in geschweiften Klammern steht, bei.
   >* Entfernen Sie alle Zeilen, die mit `link.` beginnen, aus dem Originaltext der Spalte. Löschen Sie beispielsweise alle folgenden Zeilen:
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. Klicken Sie auf **Fertig** und dann auf **Ansicht speichern**.

