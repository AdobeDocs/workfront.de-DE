---
product-area: projects
navigation-topic: update-work-in-a-project
title: Prozentsätze für abgeschlossene Aufgaben anzeigen und aktualisieren
description: Sie können den abgeschlossenen Prozentsatz einer Aufgabe aktualisieren, um den Fortschritt anzugeben, den Sie bei der Aufgabe bis zur Fertigstellung gemacht haben. Die Aktualisierung des Prozentsatzes für abgeschlossene Probleme ähnelt der Aktualisierung für eine Aufgabe. In diesem Artikel wird beschrieben, wie Sie den abgeschlossenen Prozentwert einer Aufgabe aktualisieren.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '692'
ht-degree: 3%

---

# Prozentwert der abgeschlossenen Aufgaben anzeigen und aktualisieren

<!--Audited: 05/2025-->

Sie können den abgeschlossenen Prozentsatz einer Aufgabe aktualisieren, um den Fortschritt anzugeben, den Sie bei der Aufgabe bis zur Fertigstellung gemacht haben.

Die Aktualisierung des Prozentsatzes für abgeschlossene Probleme ähnelt der Aktualisierung für eine Aufgabe. In diesem Artikel wird beschrieben, wie Sie den abgeschlossenen Prozentwert einer Aufgabe aktualisieren.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p> 
   <p>Work oder höher</p>
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

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New license: Standard</p> 
   Or
   <p>Current license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Bereiche, in denen Sie den abgeschlossenen Prozentwert einer Aufgabe aktualisieren können

Sie können den abgeschlossenen Prozentsatz für eine Aufgabe in einem der folgenden Bereiche aktualisieren:

* **In einer Aufgabenliste**: Sie können den Prozentwert der Fertigstellung einer Aufgabe aktualisieren, wenn die Spalte Prozent abgeschlossen angezeigt wird.

  Weitere Informationen zur Inline-Bearbeitung finden Sie unter [Inline-Bearbeitung von Elementen in einer Liste in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **In der Meilenstein-Ansicht**: Sie können den abgeschlossenen Prozentwert einer Aufgabe aktualisieren, wenn Sie die Meilenstein-Ansicht für eine Projektliste oder einen Projektbericht verwenden.

  >[!TIP]
  >
  >  Sie können den Prozentsatz der abgeschlossenen Probleme nicht in der Ansicht Meilenstein aktualisieren.


  Weitere Informationen finden Sie unter [Verwenden der Meilenstein -Ansicht](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **In der Aufgabenkopfzeile**: Sie können den abgeschlossenen Prozentsatz einer Aufgabe in der Aufgabenkopfzeile aktualisieren.

  ![Prozentwert in der Kopfzeile aktualisieren](assets/nwe-updatetaskpercentinheader-350x54.png)

* **Im Zusammenfassungsbereich einer Aufgabe**: Sie können den Prozentwert der Fertigstellung einer Aufgabe oben im Zusammenfassungsbereich aktualisieren, wenn Sie die Aufgabe in den folgenden Bereichen anzeigen:

   * Aufgabenliste oder Bericht
   * Arbeitszeittabelle
   * Workload Balancer

  ![Prozentuale Aktualisierung in der Aufgabenzusammenfassung hervorgehoben](assets/update-percent-complete-in-task-summary-highlighted.png)

  Weitere Informationen finden Sie unter [Übersicht](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)

* **Startseite**: Sie können den Prozentwert der abgeschlossenen Aufgaben oder Probleme über das Bedienfeld Zusammenfassung im Bereich Startseite oder über das Widget Meine Arbeit aktualisieren.

  Weitere Informationen finden Sie [Erste Schritte mit der Startseite](/help/quicksilver/workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

## Überlegungen zur Aktualisierung des Prozentsatzes der Fertigstellung einer Aufgabe

* Wenn Sie eine Aufgabe als zu 100 % abgeschlossen markieren, wird der Aufgabenstatus auf „Abgeschlossen“ aktualisiert. Der Status eines Problems wird auf „Geschlossen“ aktualisiert.
* Durch das Abschließen einer Aufgabe wird auch der abgeschlossene Prozentsatz des übergeordneten Elements und des Projekts aktualisiert.
* Die folgenden Szenarien sind für übergeordnete Aufgaben und Projekte vorhanden:
   * Sie können den abgeschlossenen Prozentsatz einer übergeordneten Aufgabe nicht auf 100 % aktualisieren, wenn der Fertigstellungsmodus Zusammenfassung des Projekts auf „Automatisch“ eingestellt ist und die Teilaufgaben nicht abgeschlossen sind.
   * Sie können den Prozentwert der Fertigstellung einer übergeordneten Aufgabe oder eines Projekts auf 100 % aktualisieren, wenn der Zusammenfassungsabschlussmodus des Projekts auf „Manuell“ eingestellt ist und die Teilaufgaben abgeschlossen oder abgeschlossen sind.

  Weitere Informationen finden Sie unter [Projekte bearbeiten](../manage-projects/edit-projects.md).

## Prozentuale Fertigstellung einer Aufgabe aktualisieren

1. Wechseln Sie zu einem der Bereiche, in denen Sie den abgeschlossenen Prozentsatz einer Aufgabe aktualisieren möchten.

   Weitere Informationen finden Sie im Abschnitt [Bereiche, in denen Sie den abgeschlossenen Prozentsatz einer Aufgabe aktualisieren können](#areas-where-you-can-update-the-percent-complete-of-a-task) in diesem Artikel.

1. Suchen Sie das Feld **Prozent abgeschlossen** für die Aufgabe, deren Prozentsatz aktualisiert werden soll.

   >[!TIP]
   >
   >Das Feld „Prozent abgeschlossen“ wird immer oben im Zusammenfassungsfenster angezeigt.

1. Klicken Sie in das Feld **Prozent abgeschlossen** und geben Sie eine Zahl zwischen 0 und 100 ein.

   ODER

   Klicken Sie auf die blaue Blase **Prozent abgeschlossen** und ziehen Sie sie auf die erforderliche Zahl, um anzugeben, wie viel von der Aufgabe Sie abgeschlossen haben, falls verfügbar.

   >[!NOTE]
   >
   >    * Wenn Sie in die Blase „Prozent abgeschlossen“ klicken, können Sie keine Dezimalzahl eingeben.
   >    * Wenn Sie den blauen Kreis per Drag-and-Drop in das Bedienfeld Zusammenfassung ziehen, wird der Bereich Prozent abgeschlossen in Schritten von einem Punkt aktualisiert.
   >
   >    * Wenn Sie die blaue Blase in die Aufgabenkopfzeile ziehen und dort ablegen, wird der Prozentsatz der Fertigstellung in Schritten von 5 Punkten aktualisiert.

1. Drücken Sie die Eingabetaste auf der Tastatur, um den Prozentwert zu speichern.

   Der abgeschlossene Prozentsatz des Projekts oder übergeordneter Aufgaben wird möglicherweise ebenfalls automatisch aktualisiert.

   Der Status der Aufgabe oder des Problems wird ebenfalls aktualisiert.

