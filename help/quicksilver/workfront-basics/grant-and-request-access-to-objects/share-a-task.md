---
title: Aufgabe freigeben
product-area: projects
navigation-topic: grant-and-request-access-to-objects
description: Ihr Adobe Workfront-Administrator kann Ihnen Zugriff auf die Ansicht oder Bearbeitung von Aufgaben gewähren, wenn Sie Zugriffsebenen zuweisen. Weitere Informationen zur Gewährung des Zugriffs auf Aufgaben finden Sie unter Zugriff auf Aufgaben gewähren .
author: Alina
feature: Get Started with Workfront
exl-id: 45da15cb-8880-41f7-a0de-939882c1f154
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 2%

---

# Aufgabe freigeben

Ihr Adobe Workfront-Administrator kann Ihnen Zugriff auf die Ansicht oder Bearbeitung von Aufgaben gewähren, wenn Sie Zugriffsebenen zuweisen. Weitere Informationen zur Gewährung des Zugriffs auf Aufgaben finden Sie unter [Gewähren des Zugriffs auf Aufgaben](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

Neben der Zugriffsstufe, die Benutzern zugewiesen wird, können Sie ihnen auch Berechtigungen für die Anzeige, Contribute oder Verwaltung bestimmter Aufgaben erteilen, auf die Sie Zugriff haben.

Berechtigungen beziehen sich auf ein Element in Workfront und legen fest, welche Aktionen für dieses Element durchgeführt werden können.

## Überlegungen beim Freigeben einer Aufgabe

Weitere Informationen finden Sie unter [Übersicht über die Freigabe von Berechtigungen für Objekte](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

* Der Ersteller einer Aufgabe verfügt standardmäßig über die Berechtigung &quot;Verwalten&quot;.
* Sie können Aufgaben einzeln oder mehrere gleichzeitig gemeinsam nutzen.\
  Das Freigeben von Aufgaben ist mit dem Freigeben anderer Objekte identisch. Weitere Informationen zum Freigeben von Elementen in Workfront finden Sie unter [Freigeben eines Objekts](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Sie können einer Aufgabe die folgenden Berechtigungen erteilen: 

   * Anzeigen
   * Verwalten
   * Mitwirken\
     ![](assets/screen-shot-2014-05-30-at-11.37.24-am-175x192.png) ![](assets/screen-shot-2014-01-23-at-1.12.40-pm-154x258.png) ![](assets/screen-shot-2014-01-22-at-10.53.00-am-182x252.png)

* Wenn Sie eine Aufgabe freigeben, erben Benutzer standardmäßig dieselben Berechtigungen für alle untergeordneten Objekte, die mit der Aufgabe verknüpft sind. Beispielsweise erben sie dieselben Berechtigungen für die untergeordneten Aufgaben, Probleme und Dokumente, die mit der Aufgabe verknüpft sind.\
  Weitere Informationen zur Hierarchie von Objekten in Workfront finden Sie unter  [Objekte in Adobe Workfront verstehen](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

  Der Workfront-Administrator kann angeben, ob Dokumente Berechtigungen von höheren Objekten in der Zugriffsebene des Benutzers erben sollen. Weitere Informationen zum Einschränken von geerbten Berechtigungen auf Dokumente finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

* Sie können geerbte Berechtigungen aus einer Aufgabe entfernen.\
  Weitere Informationen zum Entfernen vererbter Berechtigungen von Objekten finden Sie unter  [Entfernen von Berechtigungen aus Objekten](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Möglichkeiten zum Freigeben einer Aufgabe

Sie können eine Aufgabe wie folgt freigeben:

* Manuell, entweder einzeln oder in großen Mengen. Die manuelle Freigabe von Aufgaben ähnelt der Freigabe anderer Objekte in Workfront.

  Weitere Informationen zum Freigeben von Objekten in Workfront finden Sie unter  [Freigeben eines Objekts](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Gehen Sie wie folgt vor:

   * Legen Sie die Berechtigungen für die übergeordneten Objekte der Aufgabe fest: Projekt, Programm oder Portfolio. Aufgaben erben die Berechtigungen von ihren übergeordneten Objekten. Weitere Informationen zum Anzeigen von geerbten Berechtigungen für Objekte finden Sie unter [Vererbte Berechtigungen für Objekte anzeigen](../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).
   * Fügen Sie Entitäten zur Projektfreigabe in einer Vorlage hinzu, die zum Erstellen des Projekts verwendet wird, in dem sich die Aufgabe befindet. Informationen zum Freigeben von Projekten aus Vorlagen finden Sie unter [Freigeben einer Vorlage](../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   * Legen Sie die Berechtigungen für alle Aufgaben in einem Projekt fest, wenn Sie das Projekt bearbeiten. Informationen zum Verwalten des Zugriffs auf Aufgaben im Projekt basierend auf den Berechtigungen eines Benutzers für das Projekt finden Sie im Abschnitt [](../../manage-work/projects/manage-projects/edit-projects.md#access) im Artikel [Projekte bearbeiten](../../manage-work/projects/manage-projects/edit-projects.md) .

  >[!TIP]
  >
  >Wenn Sie nicht angeben, welche Aufgabenberechtigungen Benutzer erhalten sollen, wenn sie den Aufgaben im Projekt zugewiesen werden, erhalten sie standardmäßig dieselben Berechtigungen für das Projekt.

## Aufgabenberechtigungen

In der folgenden Tabelle finden Sie die Berechtigungen, die Sie Benutzern gewähren können, wenn sie eine Aufgabe anzeigen, Contribute oder verwalten können:

<table border="2" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Aktion</strong> </th> 
   <th><strong>Verwalten</strong> </th> 
   <th><strong>Contribute</strong> </th> 
   <th><strong>Anzeigen</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="row">Aufgabe(n) hinzufügen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Vorgänger hinzufügen</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Problem(e) hinzufügen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Aufgabe löschen</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row"> <p>Allgemeine Aufgabenbearbeitung<br></p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aufgabenstatus ändern</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aufgabenbegrenzung bearbeiten</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aufgabe anzeigen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Dokument(e) hinzufügen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Aufgabe kopieren*</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Aufgabe verschieben*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Stunden protokollieren</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Geplante Datumswerte ändern</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Accept-Zuweisung</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Zuweisen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Benutzerdefiniertes Formular anfügen</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Benutzerdefinierte Felder bearbeiten</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Erstellen eines Genehmigungsprozesses</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Aufgabe validieren</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Finanz bearbeiten*</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Hinzufügen/Bearbeiten von Ausgaben</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td scope="row">Finanzen anzeigen</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Aktualisierungen/Kommentare</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Freigeben</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td scope="row">Systemweit teilen</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

&#42;Wird durch die Zugriffsebene und die Berechtigungen für das Projekt gesteuert.
