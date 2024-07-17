---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: In Berichten verwendete Berichterstellungselemente"
description: Diese Ansicht zeigt die Ansicht, den Filter und die Gruppierung an, die zum Erstellen der einzelnen Berichte in Adobe Workfront verwendet werden, wenn Sie sie in einer Berichtsliste verwenden.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 67f86523-e136-4768-af93-586a107b106f
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 1%

---

# Ansicht: In Berichten verwendete Berichterstellungselemente

Diese Ansicht zeigt die Ansicht, den Filter und die Gruppierung an, die zum Erstellen der einzelnen Berichte in Adobe Workfront verwendet werden, wenn Sie sie in einer Berichtsliste verwenden.

Sie können die

```
valuefields
```

oder

```
valueexpressions
```

in jedem Element des Berichts verwendet werden.

![report_with_elements_definitions.png](assets/report-with-elements-definitions-350x130.png)

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anforderung zum Ändern einer Ansicht </p>
   <p>Berichtänderung planen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## In Berichten verwendete Berichtselemente anzeigen

1. Gehen Sie zu einer Liste von Berichten.
1. Wählen Sie aus dem Dropdownmenü **Ansicht** die Option **Neue Ansicht** aus.

1. Im Bereich **Spaltenvorschau** werden alle Spalten mit Ausnahme einer entfernt.
1. Klicken Sie auf die Kopfzeile der verbleibenden Spalte und dann auf **In Textmodus wechseln**.
1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im Feld **Textmodus** finden, und ersetzen Sie ihn durch den folgenden Code:
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat=string<br>column.0.link.lookup=link.run<br>column.0.link.value=val(objCode){5)}column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=200<br>column.1.descriptionkey=objecttype{1 2}column.1.listsort=nested(view).string(uiObjCode)<br>column.1.namekey=objecttype.abbr<br>column.1.querysort=uiObjCode<br>column.1.valueField=uiObjCode<br>column.1.valueFormat=obj jCodeMessage<br>column.1.width=80<br>column.2.descriptionkey=enteredby<br>column.2.listsort=nested(redBy).string(lastName)<br>column.2.namekey=enteredby.abbr<br>column.2.querysort=enterBy:last Name<br>column.2.valueField=enterBy:name<br>column.2.valueFormat=HTML<br>column.2.width=130<br>column.3.displayName=Filterdefinition<br>column.3.textmode=true<br>column.3.valueField=filter:definition<br>.3.valueFormat=HTML<br>column.4.displayName=View definition<br>column.4.textmode=true<br>column.4.valueField=view:definition<br>column.4.valueFormat=HTML<br>column.5.displayName=Grouping definition<br>column.5.textmode=true<br>column.5.valueField=groupBy:definition<br>column.5.valueFormat=HTML<br><br><br></pre>

1. Klicken Sie auf **Ansicht speichern**.
