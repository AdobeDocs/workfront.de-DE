---
product-area: projects
navigation-topic: update-work-in-a-project
title: Prozentsatz für Abgeschlossene Aufgaben anzeigen und aktualisieren
description: Sie können den Prozentsatz der Abschlüsse einer Aufgabe aktualisieren, um den Fortschritt anzugeben, den Sie bei der Erfüllung der Aufgabe erzielt haben.
author: Alina
feature: Work Management
exl-id: e53bca4d-1ed3-4e4d-8a35-217529a246dc
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# Prozentsatz für Abgeschlossene Aufgaben anzeigen und aktualisieren

Sie können den Prozentsatz der Abschlüsse einer Aufgabe aktualisieren, um den Fortschritt anzugeben, den Sie bei der Erfüllung der Aufgabe erzielt haben.

## Zugriffsanforderungen

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Sie müssen über folgenden Zugriff verfügen, um Aufgaben manuell aktualisieren zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für die Aufgabe verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.


## Bereiche, in denen der prozentuale Abschluss einer Aufgabe aktualisiert werden kann

Sie können den Prozentsatz der Abschlüsse für eine Aufgabe in einem der folgenden Bereiche aktualisieren:

* **In einer Aufgabenliste**: Sie können den Prozentsatz des Abschlusses einer Aufgabe aktualisieren, wenn die Spalte &quot;Prozent abgeschlossen&quot;angezeigt wird.\
  Weitere Informationen zur Inline-Bearbeitung finden Sie unter [Inline-Bearbeitungselemente in einer Liste in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

* **In der Milestone-Ansicht**: Sie können den Prozentsatz der Abschlüsse einer Aufgabe aktualisieren, wenn Sie die Meilensteinansicht in einer Projektliste oder in einem Projektbericht verwenden. Weitere Informationen finden Sie unter [Verwenden der Milestone-Ansicht](../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **Während der Aktualisierung der Aufgabe**: Sie können die Option zum prozentualen Abschluss einer Aufgabe aktualisieren, wenn Sie der Aufgabe ein Update hinzufügen.

  >[!IMPORTANT]
  >
  >Diese Option wird erst angezeigt, nachdem Sie die Option &quot;Prozentsatz abschließen anzeigen&quot;aktiviert haben.\
  >Gehen Sie wie folgt vor, um die Aktualisierungsleiste für die prozentuale Aktualisierung von Aufgaben zu aktivieren:
  >
  >1. Navigieren Sie zu **Main** Menü > Ihr Name >**Mehr** Symbol neben Ihrem Namen >**Bearbeiten** > Auswählen **Prozentualer Abschluss der Aktualisierung anzeigen**.\
  >![](assets/show-percent-complete-toggle-in-user-profile-350x243.png)  >

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

   Klicken und ziehen Sie die **Prozent abgeschlossen** wird die erforderliche Zahl angezeigt, um anzugeben, wie viel der Aufgaben Sie abgeschlossen haben.

   >[!NOTE]
   >
   >Wenn Sie angeben, dass 100 % der Aufgabe abgeschlossen ist, wird der Status der Aufgabe auch auf &quot;Abgeschlossen&quot;aktualisiert.


1. Drücken Sie die Eingabetaste in der Tastatur, um den Prozentsatz vollständig zu speichern.

