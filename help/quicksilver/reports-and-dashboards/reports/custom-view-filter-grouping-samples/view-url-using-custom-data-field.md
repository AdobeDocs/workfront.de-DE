---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Externe URL mit benutzerdefiniertem Datenfeld"
description: Sie können einen Link zu einer internen benutzerdefinierten URL anzeigen, indem Sie in einer Aufgabenansicht ein berechnetes benutzerdefiniertes Feld namens "Benutzerdefinierte URL"verwenden.
author: Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 4247f2b437a5627ac4cba5289573eb4f1c18c583
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Ansicht: externe URL mit benutzerdefiniertem Datenfeld

<!--Audited: 11/2024-->

Sie können einen Link zu einer internen benutzerdefinierten URL anzeigen, indem Sie ein **berechnetes benutzerdefiniertes Feld** mit dem Namen &quot;Benutzerdefinierte URL&quot;in einer **Aufgabenansicht** verwenden.

Auf diese Weise können Sie bestimmte Objekte in einer Ansicht schnell und direkt aus Ihren Berichten zu bestimmten Bereichen der Anwendung verknüpfen.

Beim Erstellen eines berechneten benutzerdefinierten Felds müssen Sie zunächst das Feld erstellen und dann die Ansicht erstellen.

Die folgenden Abschnitte sind ein Beispiel für ein berechnetes benutzerdefiniertes Feld für Aufgaben. Das benutzerdefinierte Feld heißt &quot;Benutzerdefinierte URL&quot;. Die benutzerdefinierte Ansicht zeigt den Wert des Felds sowie das Feld **URL** für Aufgaben an.

Mit denselben Schritten können Sie ähnliche berechnete benutzerdefinierte Felder und benutzerdefinierte Ansichten für alle Objekte im System erstellen, die über ein benutzerdefiniertes Formular verfügen.

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

## Erstellen Sie das berechnete benutzerdefinierte Feld &quot;Benutzerdefinierte URL&quot;

Informationen zum Erstellen eines berechneten benutzerdefinierten Felds finden Sie unter [Berechnete Felder zu einem Formular hinzufügen](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Wenn Sie Zugriff haben, um ein benutzerdefiniertes Formular zu erstellen, können Sie ein berechnetes benutzerdefiniertes Feld für Aufgaben namens &quot;Benutzerdefinierte URL&quot;erstellen. Dieses Feld verknüpft direkt mit der Unterregisterkarte **Übersicht** auf der Registerkarte **Aufgabendetails** .

1. Erstellen Sie ein berechnetes benutzerdefiniertes Feld.
1. Geben Sie im Feld Berechnung folgenden Code ein:

   CONCAT(&#39;&#39;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID,&quot;/overview&#39;&#39;)

1. Ersetzen Sie &quot;`<domain>`&quot; durch Ihren tatsächlichen Domänennamen ohne die Klammern. Der Abschnitt `/overview` dieser URL leitet den Link zum Abschnitt **Übersicht** im linken Bereich der Aufgabe weiter.

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
1. Klicken Sie auf **Wechseln zum Textmodus** > **Textmodus bearbeiten**.
1. Entfernen Sie den Text im Feld **Textmodus bearbeiten** und ersetzen Sie ihn durch den folgenden Code:


   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat= int
   column.0.link.lookup=link.view
   column.0.link.valuefield= objCode
   column.0.link.valueformat= val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.description=Custom URL
   column.1.link.isnewwindow=true
   column.1.link.url=customDataLabelsAsString(Custom URL)
   column.1.linkedname=direct
   column.1.listsort=customDataLabelsAsString(Custom URL)
   column.1.name=Custom URL
   column.1.querysort=URL
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=Custom URL
   column.1.valueformat=customDataLabelsAsString
   column.1.width=150
   column.2.descriptionkey=url
   column.2.linkedname=direct
   column.2.listsort=string(URL)
   column.2.namekey=url.abbr
   column.2.querysort=URL
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=URL
   column.2.valueformat=HTML
   column.2.width=150
   ```

   In diesem Beispiel ist &quot;column.1&quot;. -Zeilen zeigen den Wert im Feld &quot;Benutzerdefinierte URL&quot;als Link in den Abschnitt **Überblick** der Aufgabe; &quot;Spalte.2&quot;an. zeigt den Wert an, der im **URL-Feld** der Aufgabe gespeichert ist.

1. Klicken Sie auf **Fertig** > **Ansicht speichern**.
