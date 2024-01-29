---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ansicht: Unterschiede bei Uhrzeit und Datum berechnen"
description: Erfahren Sie, wie Sie Zeit- und Datumsunterschiede berechnen können.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 548dd91f-02bc-43ed-8322-d0facf3488f0
source-git-commit: 4c12a692971f437a3b248e4a601d4145ce626553
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# Ansicht: Zeit- und Datumsunterschiede berechnen

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>Sie können die Zeit- und Datumsdifferenz in Adobe Workfront nicht zwischen zwei verschiedenen Objekten desselben Typs berechnen. Sie können beispielsweise nicht die Zeit- und Datumsdifferenz zwischen zwei Daten aus zwei verschiedenen Projekten, Aufgaben oder Problemen berechnen.

Sie können den Unterschied zwischen den folgenden Werten berechnen:

* Zeit- und Datumsdifferenz zwischen zwei Datumsfeldern im selben Objekt
* Die Zeit- und Datumsdifferenz zwischen einem Feld eines Objekts und einem anderen Feld des übergeordneten Objekts

>[!TIP]
>
>Diese Berechnungen zeigen die Anzahl der Tage zwischen den beiden Daten an. Das Ergebnis wird in Tagen angezeigt. Der Zeitstempel im Datumsfeld wird ebenfalls berücksichtigt, und die Anzahl der Tage kann von Dezimalstellen gefolgt werden, wenn die Zeitstempel nicht übereinstimmen. Wenn die Aufgabe zu spät abgeschlossen wurde, wird die Anzahl der Tage als negativer Wert angezeigt.

## Zugriffsanforderungen

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
   <td> <p>Neu: </p><ul><li><p>Mitwirkender beim Ändern einer Ansicht </p></li><li>
   <p>Standard zum Ändern eines Berichts</p></li></ul><p>Oder</p><p>Aktuell:</p><ul><li><p>Anforderung zum Ändern einer Ansicht </p></li><li>
   <p>Berichtänderung planen</p> </li><ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten, um eine Ansicht zu ändern</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für einen Bericht verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## die Zeit- und Datumsdifferenz zwischen zwei Datumsfeldern desselben Objekts berechnen

Sie können beispielsweise die Differenz zwischen dem geplanten Abschlussdatum und dem tatsächlichen Abschlussdatum einer Aufgabe berechnen.

![](assets/view-planned-actual-completion-dates-datediff-column-new.png)

1. Gehen Sie zu einer Liste von Aufgaben.
1. Aus dem **Ansicht** Dropdown-Menü, klicken Sie auf **Neue Ansicht**.

1. Klicks **Spalte hinzufügen** und beginnen Sie mit der Eingabe von &quot;Geplantes Abschlussdatum&quot;im **In dieser Spalte anzeigen** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

1. Klicks **Spalte hinzufügen** und beginnen Sie mit der Eingabe von &quot;Tatsächliches Abschlussdatum&quot;im **In dieser Spalte anzeigen** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

1. Klicks **Spalte hinzufügen** Klicken Sie auf **In den Textmodus wechseln**.

1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im **Textmodus** und ersetzen Sie sie durch den folgenden Code:

   ```
    displayname=Planned-Actual Completion Date
    linkedname=direct
    querysort=plannedCompletionDate
    textmode=true
    valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)
    valueformat=HTML
   ```

1. Klicks **Speichern**, dann **Ansicht speichern**.

## Berechnung der Zeit- und Datumsdifferenz zwischen dem Feld eines Objekts und einem anderen Feld eines übergeordneten Objekts

Eine Liste der Objekte und ihrer übergeordneten Elemente finden Sie im Abschnitt &quot;Die Interdependenz und Hierarchie von Objekten verstehen&quot;unter [Objekte in Adobe Workfront verstehen](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
Sie können beispielsweise die Differenz zwischen dem geplanten Abschlussdatum einer Aufgabe und dem geplanten Abschlussdatum der übergeordneten Aufgabe oder des Projekts berechnen, in dem sich die Aufgabe befindet.

![](assets/view-project-planned-task-planned-completion-dates-datediff-column-new.png)

1. Gehen Sie zu einer Liste von Aufgaben.
1. Aus dem **Ansicht** Dropdown-Menü, klicken Sie auf **Neue Ansicht**.

1. Klicks **Spalte hinzufügen** und beginnen Sie mit der Eingabe von &quot;Projekt geplant Abschlussdatum&quot;oder &quot;Übergeordnetes Abschlussdatum&quot;in die **In dieser Spalte anzeigen** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

1. Klicks **Spalte hinzufügen** und beginnen Sie mit der Eingabe von &quot;Geplantes Abschlussdatum&quot;im **In dieser Spalte anzeigen** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

1. Klicks **Spalte hinzufügen** Klicken Sie auf **In den Textmodus wechseln**.

1. Bewegen Sie den Mauszeiger über den Textmodusbereich und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text, den Sie im **Textmodus** und ersetzen Sie sie durch einen der folgenden Codes:

   * So zeigen Sie den Unterschied zwischen dem geplanten Abschlussdatum des Projekts und dem der Aufgabe an:

     ```
      displayname=Project Planned Completion - Task Planned Completion (Days)
      textmode=true
      valueexpression=ROUND(DATEDIFF({project}.{plannedCompletionDate},{plannedCompletionDate}),2)
      valueformat=HTML
     ```

   * So zeigen Sie den Unterschied zwischen dem geplanten Abschlussdatum der übergeordneten Aufgabe und dem der Aufgabe an:

     ```
      valueexpression=ROUND(DATEDIFF({parent}.{plannedCompletionDate},{plannedCompletionDate}),2)
      textmode=true<br>valueformat=HTML
      displayname=Parent Planned Completion - Planned Completion (Days)
     ```

1. Klicks **Speichern**, dann **Ansicht speichern**.
