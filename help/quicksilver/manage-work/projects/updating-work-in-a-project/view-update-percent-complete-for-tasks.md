---
product-area: projects
navigation-topic: update-work-in-a-project
title: Prozentsatz für Abgeschlossene Aufgaben anzeigen und aktualisieren
description: Sie können den Prozentsatz der Abschlüsse einer Aufgabe aktualisieren, um den Fortschritt anzugeben, den Sie bei der Erfüllung der Aufgabe erzielt haben.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Prozentsatz für Abgeschlossene Aufgaben anzeigen und aktualisieren

<!--Audited:01/2024-->

Sie können den Prozentsatz der Abschlüsse einer Aufgabe aktualisieren, um den Fortschritt anzugeben, den Sie bei der Erfüllung der Aufgabe erzielt haben.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um Aufgaben manuell aktualisieren zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Neue Lizenz: Standard</p> 
   Oder
   <p>Aktuelle Lizenz: Arbeite oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für die Aufgabe verwalten</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Bereiche, in denen der prozentuale Abschluss einer Aufgabe aktualisiert werden kann

Sie können den Prozentsatz der Abschlüsse für eine Aufgabe in einem der folgenden Bereiche aktualisieren:

* **In einer Aufgabenliste**: Sie können den Prozentsatz des Abschlusses einer Aufgabe aktualisieren, wenn die Spalte &quot;Prozent abgeschlossen&quot;angezeigt wird.\
  Weitere Informationen zur Inline-Bearbeitung finden Sie unter [Inline-Bearbeitungselemente in einer Liste in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **In der Milestone-Ansicht**: Sie können den Prozentsatz der Abschlüsse einer Aufgabe aktualisieren, wenn Sie die Meilensteinansicht in einer Projektliste oder in einem Projektbericht verwenden. Weitere Informationen finden Sie unter [Verwenden der Milestone-Ansicht](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

<!--only in legacy commenting: 
* **As you update the task**:  You can update the percent complete option of a task when adding an update to the task.

  >[!IMPORTANT]
  >
  >This option displays only after you enable the Show Percent Complete option.  
  >To enable the percent complete update bar for tasks, do the following:   
  >
  >1. Go to the **Main** menu>your name>**More** icon next to your name >**Edit** > select **Show percent complete on update status**.   
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >-->

* **In der Aufgabenüberschrift**: Sie können den Prozentsatz der Abschlüsse einer Aufgabe in der Kopfzeile der Aufgabe aktualisieren. Weitere Informationen finden Sie unter [Aufgaben bearbeiten](../../tasks/manage-tasks/edit-tasks.md).

  ![](assets/nwe-updatetaskpercentinheader-350x54.png)


## Überlegungen zum Aktualisieren des prozentualen Abschlusses einer Aufgabe

* Wenn Sie eine Aufgabe als zu 100 % abgeschlossen markieren, wird der Aufgabenstatus auf &quot;Abgeschlossen&quot;aktualisiert.
* Für übergeordnete Aufgaben gibt es die folgenden Szenarien:
   * Sie können den prozentualen Abschluss einer übergeordneten Aufgabe nicht auf 100 % aktualisieren, wenn der Zusammenfassungsabschlussmodus des Projekts auf Automatisch eingestellt ist und die Unteraufgaben nicht abgeschlossen sind.
   * Sie können den Prozentsatz der Abschlüsse einer übergeordneten Aufgabe auf 100 % aktualisieren, wenn für den Zusammenfassungsabschlussmodus des Projekts &quot;Manuell&quot;festgelegt ist und die Unteraufgaben abgeschlossen oder unvollständig sind.

  Weitere Informationen finden Sie unter [Projekte bearbeiten](../manage-projects/edit-projects.md).

## Prozentsatz des Abschlusses einer Aufgabe aktualisieren

1. Navigieren Sie zu einem der folgenden Bereiche in Workfront:

   * Aufgabenliste
   * Eine Liste von Projekten und Anwendung der Milestone-Ansicht
   * Aufgabe durch Zugriff auf die Aufgabenseite
1. Suchen Sie die **Prozent abgeschlossen** -Feld für die Aufgabe, deren Prozentsatz Sie aktualisieren möchten.
1. Klicken Sie in das Feld &quot;Percent Complete&quot;und geben Sie eine Zahl zwischen 0 und 100 ein.

   Oder

   Klicken und ziehen Sie die **Prozent abgeschlossen** wird die erforderliche Zahl angezeigt, um anzugeben, wie viel der Aufgaben Sie abgeschlossen haben (sofern verfügbar).

   >[!NOTE]
   >
   >Wenn Sie angeben, dass 100 % der Aufgabe abgeschlossen ist, wird der Status der Aufgabe auch auf &quot;Abgeschlossen&quot;aktualisiert.


1. Drücken Sie die Eingabetaste in der Tastatur, um den Prozentsatz vollständig zu speichern.

Die Prozent abgeschlossen des Projekts wird ebenfalls automatisch aktualisiert.

