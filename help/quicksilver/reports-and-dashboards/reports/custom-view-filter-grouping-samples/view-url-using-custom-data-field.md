---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: externe URL mit benutzerdefiniertem Datenfeld"
description: Sie können einen Link zu einer internen benutzerdefinierten URL anzeigen, indem Sie in einer Aufgabenansicht ein berechnetes benutzerdefiniertes Feld namens "Benutzerdefinierte URL"verwenden.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 1ae65d18419bf4235a7c97614b539811643110cc
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# Ansicht: externe URL mit benutzerdefiniertem Datenfeld

Sie können einen Link zu einer internen benutzerdefinierten URL anzeigen, indem Sie ein **berechnetes benutzerdefiniertes Feld** mit dem Namen &quot;Benutzerdefinierte URL&quot;in einer **Aufgabenansicht** verwenden.

Auf diese Weise können Sie bestimmte Objekte in einer Ansicht schnell und direkt aus Ihren Berichten zu bestimmten Bereichen der Anwendung verknüpfen.

Beim Erstellen eines berechneten benutzerdefinierten Felds müssen Sie zunächst das Feld erstellen und dann die Ansicht erstellen.

Die folgenden Abschnitte sind ein Beispiel für ein berechnetes benutzerdefiniertes Feld für Aufgaben. Das benutzerdefinierte Feld heißt &quot;Benutzerdefinierte URL&quot;. Die benutzerdefinierte Ansicht zeigt den Wert des Felds sowie das Feld **URL** für Aufgaben an.

Mit denselben Schritten können Sie ähnliche berechnete benutzerdefinierte Felder und benutzerdefinierte Ansichten für alle Objekte im System erstellen, die über ein benutzerdefiniertes Formular verfügen.

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

## Erstellen Sie das berechnete benutzerdefinierte Feld &quot;Benutzerdefinierte URL&quot;

Informationen zum Erstellen eines berechneten benutzerdefinierten Felds finden Sie unter [Berechnete Felder zu einem Formular hinzufügen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Wenn Sie Zugriff haben, um ein benutzerdefiniertes Formular zu erstellen, können Sie ein berechnetes benutzerdefiniertes Feld für Aufgaben namens &quot;Benutzerdefinierte URL&quot;erstellen. Dieses Feld verknüpft direkt mit der Unterregisterkarte **Übersicht** auf der Registerkarte **Aufgabendetails** .

1. Erstellen Sie ein berechnetes benutzerdefiniertes Feld.
1. Geben Sie im Feld Berechnung folgenden Code ein:

   CONCAT(&#39;&#39;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID,&quot;/overview&#39;&#39;)

1. Ersetzen Sie &quot;`<domain>`&quot; durch Ihren tatsächlichen Domänennamen ohne die Klammern.

   Der/Die/Das

   ```
   /overview
   ```

   -Teil dieser URL leitet den Link zum Abschnitt **Übersicht** im linken Bereich der Aufgabe weiter.

1. Fügen Sie nach der Erstellung Ihres **berechneten benutzerdefinierten Felds** das Feld **Benutzerdefiniertes Formular** mit diesem Feld an mehrere Aufgaben in Adobe Workfront an, die in Ihrer neuen Ansicht angezeigt werden sollen.

## Erstellen Sie die Ansicht, die die Felder &quot;Benutzerdefinierte URL&quot;und &quot;URL&quot;der Aufgabe anzeigt

Die Aufgabe **Anzeigen** im folgenden Beispiel zeigt das **berechnete benutzerdefinierte Feld** mit dem Namen &quot;Benutzerdefinierte URL&quot;als direkten Link zur Unterregisterkarte **Überblick** auf der Registerkarte **Details** der Aufgabe sowie das Feld **URL** der Aufgabe an.

![](assets/task-view-with-custom-url-field-quicksilver-350x70.png)

So passen Sie diese Ansicht an:

1. Gehen Sie zu einer Liste von Aufgaben.
1. Erweitern Sie das Dropdown-Menü **Ansicht** oben in der Aufgabenliste.
1. Klicken Sie auf **Ansicht anpassen**.
1. Entfernen Sie alle Spalten in der Ansicht, mit Ausnahme der ersten Spalte.
1. Klicken Sie auf die Kopfzeile der ersten Spalte.
1. Klicken Sie oben rechts auf der Benutzeroberfläche auf **In den Textmodus wechseln** .
1. Klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Fügen Sie den Textmodus unten in Ihre Spalte ein.\
   In diesem Beispiel ist &quot;column.1&quot;. zeigt den Wert im Feld &quot;Benutzerdefinierte URL&quot;als Link in die **Übersicht** der Aufgabe an. &quot;Column.2.&quot; zeigt den Wert an, der im **URL-Feld** der Aufgabe gespeichert ist.
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valueField=ID<br>column.0.link.linkproperty.0.valueFormat= int<br>column.0.link.lookup=link.view<br>column.0.link.valueField= objCode<br> column.0.link.valueFormat= val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.extending=10<br>column.0.valueField=name<br>column.0.valueFormat=HTML<br>column.0.width=150<br>column.1.description=Custom URL<br>column.1.link.isnewwindow=true<br>column.1.link.url=customDataLabelsAsString(Custom URL){1 8}column.1.linkedname=direct<br>column.1.listsort=customDataLabelsAsString(Custom URL)<br>column.1.name=Custom URL<br>column.1.querysort=URL<br>column.1.shortview=false<br>column.1.gestreckch=0<br>column.1 efield=Custom URL<br>column.1.valueFormat=customDataLabelsAsString<br>column.1.width=150<br>column.2.descriptionkey=url<br>column.2.linkedname=direct<br>column.2.listsort=string(URL)<br>column.2 ekey=url.abbr<br>column.2.querysort=URL<br>column.2.shortview=false<br>column.2.gestreckch=0<br>column.2.valueField=URL<br>column.2.valueFormat=HTML<br>column.2.width=150<br></pre>

1. Klicken Sie auf **Ansicht speichern**.
