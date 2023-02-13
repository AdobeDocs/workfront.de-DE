---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Ansicht: Link zu einem Objekt in einer Spalte entfernen'
description: Einige Objekte, die Sie in einer Ansicht anzeigen, verlinken standardmäßig zur Seite Details des Objekts. Beispielsweise ist die Spalte, die den Namen eines Projekts anzeigt, ein Link zum Projekt. in der Spalte, in der der Name eines Benutzers angezeigt wird, ein Link zur Profilseite des Benutzers ist.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Ansicht: Link zu einem Objekt in einer Spalte entfernen

Einige Objekte, die Sie in einer Ansicht anzeigen, verlinken standardmäßig zur Seite Details des Objekts. Beispielsweise ist die Spalte, die den Namen eines Projekts anzeigt, ein Link zum Projekt. in der Spalte, in der der Name eines Benutzers angezeigt wird, ein Link zur Profilseite des Benutzers ist.

Sie können diesen Link mithilfe des Textmodus in Spalten entfernen, die in allen Ansichten angezeigt werden.

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

## Beispiel: Entfernen Sie den Link zu einer Aufgabe aus der Spalte &quot;Task Name&quot;in einer Aufgabenansicht:

1. Gehen Sie zu einer Liste von Aufgaben.
1. Aus dem **Ansicht** Dropdown-Menü, klicken Sie auf **Neue Ansicht** , um eine neue Ansicht zu erstellen.

   Oder

   Klicken Sie auf **Symbol Bearbeiten** ![](assets/edit-icon.png)

   , um eine vorhandene Ansicht zu bearbeiten, und wählen Sie dann die Ansicht aus.

1. Klicken **Spalte hinzufügen** um eine neue Spalte hinzuzufügen.

   Oder

   Klicken Sie auf eine vorhandene Spalte mit einer Verknüpfung zu einem Objekt.

1. Klicken **In den Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im **Textmodus** und ersetzen Sie sie durch den folgenden Code:

   <pre>displayName=Task Name<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br><strong>valueExpression={name}</strong><br>valueFormat=Compound</pre>

   >[!TIP]
   >
   >Sie können ähnlichen Code für andere Objekte verwenden, indem Sie Folgendes anpassen:
   >
   >   
   >   
   >   * Ersetzen Sie die **valueField** -Zeile des Codes mit **valueExpression** und behalten Sie den gleichen Namen, der auch in geschweiften Klammern steht, nach dem Gleichheitszeichen bei.
   >   
   >   
   >
   >   
   >   
   >   * Löschen Sie alle Zeilen, die mit > beginnen.

      >   
      >     ```>   
      >     link.
      >     ```   >   
      >   
      >     
      from the original text of the column. For example, eliminate all the following lines:
      >     <pre>link.linkproperty.0.name=ID</pre><pre>link.linkproperty.0.valuefield=ID</pre><pre>link.linkproperty.0.valueformat=string</pre><pre>link.lookup=link.view</pre><pre>link.value=val(objCode)</pre>
      >   
      >   
      >



1. Klicken **Speichern**, dann **Ansicht speichern**.
