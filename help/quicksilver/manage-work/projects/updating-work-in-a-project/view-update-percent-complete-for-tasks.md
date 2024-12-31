---
product-area: projects
navigation-topic: update-work-in-a-project
title: Prozentsätze für abgeschlossene Aufgaben anzeigen und aktualisieren
description: Sie können den abgeschlossenen Prozentsatz einer Aufgabe aktualisieren, um den Fortschritt anzugeben, den Sie bei der Aufgabe bis zur Fertigstellung gemacht haben.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: 1e69d715f343bfef1e5aee658a1dff12abfc61a0
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 0%

---

# Prozentwert der abgeschlossenen Aufgaben anzeigen und aktualisieren

<!--Audited:01/2024-->

Sie können den abgeschlossenen Prozentsatz einer Aufgabe aktualisieren, um den Fortschritt anzugeben, den Sie bei der Aufgabe bis zur Fertigstellung gemacht haben.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um Aufgaben manuell aktualisieren zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neue Lizenz: Standard</p> 
   Oder
   <p>Aktuelle Lizenz: Arbeit oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten der Berechtigungen für die Aufgabe</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Bereiche, in denen Sie den abgeschlossenen Prozentwert einer Aufgabe aktualisieren können

Sie können den abgeschlossenen Prozentsatz für eine Aufgabe in einem der folgenden Bereiche aktualisieren:

* **In einer Aufgabenliste**: Sie können den Prozentwert der Fertigstellung einer Aufgabe aktualisieren, wenn die Spalte „Prozent abgeschlossen“ angezeigt wird.\
  Weitere Informationen zur Inline-Bearbeitung finden Sie unter [Inline-Bearbeitung von Elementen in einer Liste in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **In der Meilenstein-Ansicht**: Sie können den abgeschlossenen Prozentwert einer Aufgabe aktualisieren, wenn Sie die Meilenstein-Ansicht für eine Projektliste oder einen Projektbericht verwenden. Weitere Informationen finden Sie unter [Verwenden der Meilenstein -Ansicht](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

<!--only in legacy commenting: 
* **As you update the task**:  You can update the percent complete option of a task when adding an update to the task.

  >[!IMPORTANT]
  >
  >This option displays only after you enable the Show Percent Complete option.  
  >To enable the percent complete update bar for tasks, do the following:   
  >
  >1. Go to the **Main** menu>your name>**More** icon next to your name >**Edit** > select **Show percent complete on update status**.   
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >-->

* **In der Aufgabenkopfzeile**: Sie können den abgeschlossenen Prozentsatz einer Aufgabe in der Aufgabenkopfzeile aktualisieren. Weitere Informationen finden Sie unter [Aufgaben bearbeiten](../../tasks/manage-tasks/edit-tasks.md).

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)

* **Im Zusammenfassungsbereich einer Aufgabe**: Sie können den Prozentwert der Fertigstellung einer Aufgabe oben im Zusammenfassungsbereich aktualisieren, wenn Sie die Aufgabe in den folgenden Bereichen anzeigen:

   * Aufgabenliste oder Bericht
   * Arbeitszeittabelle
   * Workload Balancer

  ![](assets/update-percent-complete-in-task-summary-highlighted.png)

  Weitere Informationen finden Sie unter [Übersicht](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)

* **Startseite**: Sie können den Prozentwert der abgeschlossenen Aufgaben oder Probleme über das Bedienfeld Zusammenfassung im Bereich Startseite oder über das Widget Meine Arbeit aktualisieren.

  Weitere Informationen finden Sie [Erste Schritte mit der Startseite](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

## Überlegungen zur Aktualisierung des Prozentsatzes der Fertigstellung einer Aufgabe

* Wenn Sie eine Aufgabe als zu 100 % abgeschlossen markieren, wird der Aufgabenstatus auf „Abgeschlossen“ aktualisiert.
* Die folgenden Szenarien existieren für übergeordnete Aufgaben:
   * Sie können den abgeschlossenen Prozentsatz einer übergeordneten Aufgabe nicht auf 100 % aktualisieren, wenn der Fertigstellungsmodus Zusammenfassung des Projekts auf „Automatisch“ eingestellt ist und die Teilaufgaben nicht abgeschlossen sind.
   * Sie können den abgeschlossenen Prozentsatz einer übergeordneten Aufgabe auf 100 % aktualisieren, wenn der Fertigstellungsmodus Zusammenfassung des Projekts auf „Manuell“ eingestellt ist und die Teilaufgaben abgeschlossen oder unvollständig sind.

  Weitere Informationen finden Sie unter [Projekte bearbeiten](../manage-projects/edit-projects.md).

## Prozentuale Fertigstellung einer Aufgabe aktualisieren

1. Wechseln Sie zu einem der folgenden Bereiche in Workfront:

   * Aufgabenliste
   * Liste der Projekte und Anwendung der Meilenstein -Ansicht
   * Eine Aufgabe durch Zugriff auf die Aufgabenseite
1. Suchen Sie das Feld **Prozent abgeschlossen** für die Aufgabe, deren Prozentsatz aktualisiert werden soll.

   >[!TIP]
   >
   >  Das Feld „Prozent abgeschlossen“ wird immer oben im Zusammenfassungsfenster angezeigt.


1. Klicken Sie in das Feld **Prozent abgeschlossen** und geben Sie eine Zahl zwischen 0 und 100 ein.

   Oder

   Klicken Sie auf die **Prozent abgeschlossen** und ziehen Sie sie auf die erforderliche Zahl, um anzugeben, wie viel von der Aufgabe Sie abgeschlossen haben, falls verfügbar.

   >[!NOTE]
   >
   >Wenn Sie angeben, dass 100 % der Aufgabe abgeschlossen ist, wird der Status der Aufgabe ebenfalls auf Abgeschlossen aktualisiert.


1. Drücken Sie die Eingabetaste auf der Tastatur, um den Prozentwert zu speichern.

Der Prozentwert der Fertigstellung des Projekts wird ebenfalls automatisch aktualisiert.

