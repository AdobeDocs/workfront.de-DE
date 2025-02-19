---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Externe URL mit benutzerdefiniertem Datenfeld'
description: Sie können einen Link zu einer internen benutzerdefinierten URL anzeigen, indem Sie ein berechnetes benutzerdefiniertes Feld namens „Benutzerdefinierte URL“ in einer Aufgabenansicht verwenden.
author: Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 6a1152bb86a856d60585db7d6ffd43a59a212a72
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# Ansicht: externe URL mit benutzerdefiniertem Datenfeld

<!--Audited: 11/2024-->

Sie können einen Link zu einer internen benutzerdefinierten URL mithilfe eines **berechneten benutzerdefinierten Felds** namens „Benutzerdefinierte URL“ in einer **Aufgabenansicht“**.

So können Sie direkt aus Ihren Berichten schnell Verknüpfungen von bestimmten Objekten in einer Ansicht zu bestimmten Bereichen der Anwendung erstellen.

Beim Erstellen eines berechneten benutzerdefinierten Felds müssen Sie zunächst das Feld und dann die Ansicht erstellen.

Die folgenden Abschnitte sind ein Beispiel für ein berechnetes benutzerdefiniertes Feld für Aufgaben. Das benutzerdefinierte Feld wird als benutzerdefinierte URL bezeichnet. In der benutzerdefinierten Ansicht werden der Wert des Felds sowie das Feld **URL** für Aufgaben angezeigt.

Mit denselben Schritten können Sie ähnliche berechnete benutzerdefinierte Felder und benutzerdefinierte Ansichten für alle Objekte im System erstellen, die über ein benutzerdefiniertes Formular verfügen.

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
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p> Aktuell: 
   <ul>
   <li>Änderung einer Ansicht anfordern</li> 
   <li>Planen der Änderung eines Berichts</li>
   </ul>
     </p>
     <p> Neu: 
   <ul>
   <li>Mitwirkende zum Ändern einer Ansicht</li> 
   <li>Standard zum Ändern eines Berichts</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen des berechneten benutzerdefinierten Feldes „Benutzerdefinierte URL“

Informationen zum Erstellen eines berechneten benutzerdefinierten Felds finden Sie unter [Hinzufügen berechneter Felder zu einem Formular](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

Wenn Sie Zugriff auf das Erstellen eines benutzerdefinierten Formulars haben, können Sie ein berechnetes benutzerdefiniertes Feld für Aufgaben namens „Benutzerdefinierte URL“ erstellen. Dieses Feld ist direkt mit der Unterregisterkarte **Übersicht** in der Registerkarte **Aufgabendetails** verknüpft.

1. Erstellen Sie ein berechnetes benutzerdefiniertes Feld.
1. Geben Sie im Feld Berechnung den folgenden Code ein:

   CONCAT(&#39;&#39;https://`<domain>`.my.workfront.com“,“/&quot;,„task/&quot;,ID,“/overview&#39;&#39;&#39;)

1. Ersetzen Sie &quot;`<domain>`&quot; durch den tatsächlichen Domain-Namen (ohne die Klammern). Der `/overview` Teil dieser URL leitet den Link zum Abschnitt **Übersicht** im linken Bedienfeld der Aufgabe weiter.

1. Fügen Sie nach dem Erstellen **berechneten benutzerdefinierten Felds** das **benutzerdefinierte Formular** mit diesem Feld an mehrere Aufgaben in Adobe Workfront an, die in der neuen Ansicht angezeigt werden sollen.

## Erstellen Sie die Ansicht, die die Felder „Benutzerdefinierte URL“ und „URL“ der Aufgabe anzeigt

Die Aufgabe **Ansicht** im folgenden Beispiel zeigt das **Berechnetes benutzerdefiniertes Feld** namens „Benutzerdefinierte URL“ als direkten Link zur Unterregisterkarte **Übersicht** innerhalb der Registerkarte **Details** sowie das **URL**-Feld der Aufgabe.

(assets/task-view-with-custom-url-field-quicksilver-350x70.png)

So passen Sie diese Ansicht an:

1. Zu einer Aufgabenliste gehen.
1. Erweitern Sie **Dropdown** Ansicht“ oben in der Aufgabenliste.
1. Klicken Sie **Ansicht anpassen**.
1. Entfernen Sie alle Spalten in der Ansicht mit Ausnahme der ersten Spalte.
1. Klicken Sie auf die Kopfzeile der ersten Spalte.
1. Klicken Sie **In Textmodus wechseln** > **Textmodus bearbeiten**.
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

   In diesem Beispiel ist die Spalte „Column.1“ In Zeilen wird der Wert im Feld „Benutzerdefinierte URL“ als Link zum Abschnitt „Übersicht **der Aufgabe angezeigt** „Spalte.2.“ zeigt den im Feld **URL** der Aufgabe gespeicherten Wert an.

1. Klicken Sie **Fertig** > **Ansicht speichern**.
