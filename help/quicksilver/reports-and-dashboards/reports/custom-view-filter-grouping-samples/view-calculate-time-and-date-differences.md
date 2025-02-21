---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ansicht: Uhrzeit- und Datumsunterschiede berechnen'
description: Erfahren Sie, wie Sie Zeit- und Datumsunterschiede berechnen.
author: Nolan
feature: Reports and Dashboards
exl-id: 548dd91f-02bc-43ed-8322-d0facf3488f0
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 0%

---

# Ansicht: Uhrzeit- und Datumsunterschiede berechnen

<!-- Audited: 11/2024 -->

>[!IMPORTANT]
>
>Sie können die Zeit- und Datumsdifferenz in Adobe Workfront zwischen zwei verschiedenen Objekten desselben Typs nicht berechnen. Sie können beispielsweise nicht die Uhrzeit- und Datumsdifferenz zwischen zwei Terminen für zwei verschiedene Projekte, Aufgaben oder Probleme berechnen.

Sie können die Differenz zwischen den folgenden Werten berechnen:

* Die Zeit- und Datumsdifferenz zwischen zwei Datumsfeldern auf demselben Objekt
* Die Zeit- und Datumsdifferenz zwischen einem Feld auf einem Objekt und einem anderen Feld auf dem übergeordneten Objekt

>[!TIP]
>
>Diese Berechnungen zeigen die Anzahl der Tage zwischen den beiden Datumsangaben an. Das Ergebnis wird in Tagen angezeigt. Der Zeitstempel im Datumsfeld wird ebenfalls berücksichtigt und auf die Anzahl der Tage können Dezimalstellen folgen, wenn die Zeitstempel nicht übereinstimmen. Wenn die Aufgabe zu spät abgeschlossen wurde, wird die Anzahl der Tage als negativer Wert angezeigt.

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
   <td> <p>Neu: </p><ul><li><p>Mitwirkende zum Ändern einer Ansicht </p></li><li>
   <p>Standard zum Ändern eines Berichts</p></li></ul><p>Oder</p><p>Aktuell:</p><ul><li><p>Änderung einer Ansicht anfordern </p></li><li>
   <p>Planen der Änderung eines Berichts</p> </li><ul></td> 
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

## Berechnung der Uhrzeit- und Datumsdifferenz zwischen zwei Datumsfeldern auf demselben Objekt

Sie können beispielsweise die Differenz zwischen dem geplanten Abschlussdatum und dem tatsächlichen Abschlussdatum einer Aufgabe berechnen.

![Datumsunterschied anzeigen](assets/view-planned-actual-completion-dates-datediff-column-new.png)

1. Zu einer Aufgabenliste gehen.
1. Klicken Sie **Dropdown** Menü „Ansicht“ auf **Neue Ansicht**.

1. Klicken Sie **Spalte hinzufügen** und geben Sie „Geplantes Abschlussdatum“ in das Feld **In dieser Spalte anzeigen** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

1. Klicken Sie auf **Spalte hinzufügen** und geben Sie „Tatsächliches Abschlussdatum“ in das Feld **In dieser Spalte anzeigen** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

1. Klicken Sie **Spalte hinzufügen** und dann auf **In Textmodus wechseln**.

1. Bewegen Sie den Mauszeiger über den Bereich für den Textmodus und klicken Sie auf **Klicken, um Text zu bearbeiten**.
1. Entfernen Sie den Text aus dem Feld **Textmodus** und ersetzen Sie ihn durch den folgenden Code:

   ```
    displayname=Planned-Actual Completion Date
    linkedname=direct
    querysort=plannedCompletionDate
    textmode=true
    valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)
    valueformat=HTML
   ```

1. Klicken Sie **Speichern** und dann **Ansicht speichern**.

## Berechnen Sie die Zeit- und Datumsdifferenz zwischen dem Feld eines Objekts und einem anderen Feld eines übergeordneten Objekts

Eine Liste der Objekte und der ihnen übergeordneten Objekte finden Sie im Abschnitt „Grundlagen der Interdependenz und Hierarchie von Objekten“ in [Grundlegendes zu Objekten in Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
Sie können beispielsweise die Differenz zwischen dem geplanten Abschlussdatum einer Aufgabe und dem geplanten Abschlussdatum der übergeordneten Aufgabe oder des Projekts, in dem die Aufgabe ausgeführt wird, berechnen.

![Geplanten Abschlussdatumsunterschied anzeigen](assets/view-project-planned-task-planned-completion-dates-datediff-column-new.png)

1. Zu einer Aufgabenliste gehen.
1. Klicken Sie **Dropdown** Menü „Ansicht“ auf **Neue Ansicht**.

1. Klicken Sie auf **Spalte hinzufügen** und geben Sie im Feld „In dieser Spalte anzeigen“ entweder „Geplantes Abschlussdatum des Projekts“ oder **Übergeordnetes Abschlussdatum** ein. Wählen Sie das Feld aus, wenn es in der Liste angezeigt wird.

1. Klicken Sie **Spalte hinzufügen** und geben Sie „Geplantes Abschlussdatum“ in das Feld **In dieser Spalte anzeigen** und wählen Sie es aus, wenn es in der Liste angezeigt wird.

1. Klicken Sie **Spalte hinzufügen** und dann auf **In Textmodus wechseln** > **Textmodus bearbeiten**.
1. Entfernen Sie den Text aus dem Feld **Textmodus bearbeiten** und ersetzen Sie ihn durch einen der folgenden Codes:

   * So zeigen Sie die Differenz zwischen dem geplanten Abschlussdatum des Projekts und dem der Aufgabe an:

     ```
      displayname=Project Planned Completion - Task Planned Completion (Days)
      textmode=true
      valueexpression=ROUND(DATEDIFF({project}.{plannedCompletionDate},{plannedCompletionDate}),2)
      valueformat=HTML
     ```

   * So zeigen Sie die Differenz zwischen dem geplanten Abschlussdatum der übergeordneten Aufgabe und dem der Aufgabe an:

     ```
      valueexpression=ROUND(DATEDIFF({parent}.{plannedCompletionDate},{plannedCompletionDate}),2)
      textmode=true<br>valueformat=HTML
      displayname=Parent Planned Completion - Planned Completion (Days)
     ```

1. Klicken Sie **Fertig** und dann **Ansicht speichern**.
