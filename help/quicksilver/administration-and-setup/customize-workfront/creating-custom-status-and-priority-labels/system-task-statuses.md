---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Status von Systemaufgaben
description: Die drei integrierten Systemaufgabenstatus in Workfront sind erforderlich, d. h. Sie können sie entsperren, umbenennen und neu anordnen, sie jedoch nicht ausblenden oder löschen. Sie können auch neue Systemaufgabenstatus hinzufügen, um sie an die Anforderungen in Ihrem Unternehmen anzupassen. Das Ändern des Status einer Aufgabe ist in der Regel ein manueller Prozess, aber manchmal wird der Status einer Aufgabe automatisch geändert, abhängig von anderen Faktoren, die im System auftreten.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: b8c751c3-aed3-4836-a888-f3f8a5f08421
TQID: https://experienceleague.adobe.com/FACmZvT5v00-FS0lOBCMh347ZqM6c-Upfq4ITymVpV0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 409
ht-degree: 0%

---

# Status von Systemaufgaben

Die drei integrierten Systemaufgabenstatus in Workfront sind erforderlich, d. h. Sie können sie entsperren, umbenennen und neu anordnen, sie jedoch nicht ausblenden oder löschen.

Sie können auch neue Systemaufgabenstatus hinzufügen, um sie an die Anforderungen in Ihrem Unternehmen anzupassen.

Das Ändern des Status einer Aufgabe ist in der Regel ein manueller Prozess. Es gibt jedoch Zeiten, die in der folgenden Liste aufgeführt sind, wenn der Status einer Aufgabe automatisch geändert wird, abhängig von anderen Faktoren, die im System auftreten.

Die folgenden Aufgabenstatus werden mit Ihrer Workfront-Instanz bereitgestellt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Status der Systemaufgabe</th> 
   <th>Wenn dieser Status auftritt</th> 
   <th>Aktionen, die ausgeführt werden, wenn eine Aufgabe diesen Status aufweist</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Neu (erforderlicher Status)</td> 
   <td>Dies ist der Standardstatus für jede neu erstellte Aufgabe.</td> 
   <td>Wenn sich die Aufgabe in einem Projekt mit dem Status „Aktuell“ befindet, wird die Aufgabe auf der Registerkarte Arbeitsaufträge der Benutzer angezeigt, die den Aufgaben zugewiesen sind. Benutzer können jetzt mit der Arbeit an der Aufgabe beginnen.</td> 
  </tr> 
  <tr> 
   <td>In Bearbeitung (erforderlicher Status)</td> 
   <td>Sie können eine Aufgabe in diesen Status setzen, um anzugeben, dass die Arbeit an dieser Aufgabe begonnen hat.</td> 
   <td> <p>Wenn Sie eine Aufgabe als In Bearbeitung markieren, zeigt die Aufgabe einen Wert für das tatsächliche Startdatum an.</p> <p>Der Fortschritt der Aufgabe wird erst aufgezeichnet, wenn Sie den abgeschlossenen Prozentsatz der Aufgabe manuell aktualisieren.</p> </td> 
  </tr> 
  <tr> 
   <td>Abgeschlossen (erforderlicher Status)</td> 
   <td> <p>Sie können eine Aufgabe manuell als abgeschlossen markieren, wenn die Bearbeitung abgeschlossen ist.</p> <p>Wenn der Überwachungsmodus einer Aufgabe auf „Automatisch abschließen“ festgelegt ist, wird die Aufgabe automatisch als „Abgeschlossen“ markiert, wenn sie das geplante Abschlussdatum erreicht.</p> </td> 
   <td> <p>Wenn eine Aufgabe abgeschlossen ist, wird der abgeschlossene Prozentwert der Aufgabe als 100 % markiert. Die Aufgabe wird aus der Liste Meine Arbeit des Verantwortlichen im Bereich Startseite entfernt, wenn sie abgeschlossen ist.</p> <p>Wenn Sie eine Aufgabe als abgeschlossen markieren, wird in der Aufgabe ein Wert für das tatsächliche Abschlussdatum angezeigt.</p> <p><b>HINWEIS</b>: Wenn die Aufgabe unvollständige Probleme aufweist und Sie den Aufgabenstatus in „Abgeschlossen“ ändern, ändert sich der Status automatisch in „Abgeschlossen - Ausstehende Probleme“.</p> </td> 
  </tr> 
 </tbody> 
</table>
