---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Status von Systemaufgaben
description: Die drei in Workfront integrierten Systemaufgabenstatus sind erforderlich. Das bedeutet, dass Sie sie entsperren, umbenennen und neu anordnen können, sie jedoch nicht ausblenden oder löschen können. Sie können auch neue Systemaufgabenstatus hinzufügen, die den Anforderungen in Ihrer Organisation entsprechen. Das Ändern des Status einer Aufgabe ist normalerweise ein manueller Prozess, aber manchmal wird der Status einer Aufgabe automatisch geändert, je nach anderen Faktoren, die im System auftreten.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Status von Systemaufgaben

Die drei in Workfront integrierten Systemaufgabenstatus sind erforderlich. Das bedeutet, dass Sie sie entsperren, umbenennen und neu anordnen können, sie jedoch nicht ausblenden oder löschen können.

Sie können auch neue Systemaufgabenstatus hinzufügen, die den Anforderungen in Ihrer Organisation entsprechen.

Das Ändern des Status einer Aufgabe ist normalerweise ein manueller Prozess. Es gibt jedoch in der folgenden Liste Zeiten, in denen der Status einer Aufgabe automatisch geändert wird, abhängig von anderen Faktoren, die im System auftreten.

Die folgenden Aufgabenstatus werden Ihrer Workfront-Instanz bereitgestellt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Status der Systemaufgaben</th> 
   <th>Wenn dieser Status auftritt</th> 
   <th>Aktionen, die auftreten, wenn eine Aufgabe diesen Status hat</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Neu (erforderlicher Status)</td> 
   <td>Dies ist der Standardstatus für jede neu erstellte Aufgabe.</td> 
   <td>Wenn sich die Aufgabe in einem Projekt mit dem Status "Aktuell"befindet, wird die Aufgabe auf der Registerkarte "Arbeitsanforderungen"der Benutzer angezeigt, die den Aufgaben zugewiesen sind. Benutzer können nun mit der Arbeit beginnen.</td> 
  </tr> 
  <tr> 
   <td>Wird ausgeführt (erforderlicher Status)</td> 
   <td>Sie können eine Aufgabe in diesen Status einfügen, um anzugeben, dass die Arbeit an dieser Aufgabe begonnen hat.</td> 
   <td> <p>Wenn Sie eine Aufgabe als In Bearbeitung markieren, zeigt die Aufgabe einen Wert für das tatsächliche Startdatum an.</p> <p>Der Fortschritt der Aufgabe wird erst aufgezeichnet, wenn Sie den Prozentsatz der abgeschlossenen Aufgaben manuell aktualisieren.</p> </td> 
  </tr> 
  <tr> 
   <td>Abgeschlossen (erforderlicher Status)</td> 
   <td> <p>Sie können eine Aufgabe manuell als abgeschlossen kennzeichnen, wenn die Arbeit daran abgeschlossen ist.</p> <p>Wenn der Tracking-Modus einer Aufgabe auf Automatisch abschließen festgelegt ist, wird die Aufgabe automatisch als abgeschlossen markiert, wenn sie das geplante Abschlussdatum erreicht.</p> </td> 
   <td> <p>Wenn eine Aufgabe abgeschlossen ist, wird der prozentuale Abschluss der Aufgabe als 100 % markiert. Die Aufgabe wird nach Abschluss aus der Arbeitsliste des Verantwortlichen im Startbereich entfernt.</p> <p>Wenn Sie eine Aufgabe als abgeschlossen markieren, zeigt die Aufgabe einen Wert für das tatsächliche Abschlussdatum an.</p> <p><b>HINWEIS</b>: Wenn die Aufgabe unvollständige Probleme aufweist und Sie den Aufgabenstatus in "Abgeschlossen"ändern, ändert sich der Status automatisch in "Abgeschlossen - Ausstehende Probleme".</p> </td> 
  </tr> 
 </tbody> 
</table>
