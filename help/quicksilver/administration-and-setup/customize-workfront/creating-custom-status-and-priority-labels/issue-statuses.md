---
title: Zugriff auf die Liste der Systemanfragestatus
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Mit dem Status eines Problems können Sie Benutzenden im System anzeigen, in welchem Entwicklungsstadium sich ein Problem zu einem bestimmten Zeitpunkt befindet.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9bdaec2f-acdf-4cbf-a308-ebcc861dbb89
source-git-commit: 366043a786c94f1bc40ad3b20af175bb84c94742
workflow-type: tm+mt
source-wordcount: '1422'
ht-degree: 0%

---

# Zugriff auf die Liste der Systemanfragestatus

Mit dem Status eines Problems können Sie Benutzenden im System anzeigen, in welchem Entwicklungsstadium sich ein Problem zu einem bestimmten Zeitpunkt befindet.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Systemadministrator</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Zugriff auf Problemstatus

Sie können auf Systemebene auf Problemstatus zugreifen und diese ändern. Sie können einige Informationen zum Standardsystemstatus bearbeiten oder neue benutzerdefinierte Status erstellen. Weitere Informationen zum Erstellen benutzerdefinierter Status oder Bearbeiten des Systemstatus finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

So greifen Sie auf den Problemstatus auf Systemebene zu:

{{step-1-to-setup}}

1. Klicken Sie **Projektvoreinstellungen** > **Status**.

1. Klicken Sie auf **Probleme**, um die in Workfront verfügbaren Problemstatus anzuzeigen.

   ![Problemstatus](assets/issue-status.png)

## Systemanfragestatus

Workfront verfügt über 10 ursprüngliche Problemstatus. Die ersten 4 in der folgenden Tabelle sind erforderlich, was bedeutet, dass Sie sie entsperren, umbenennen und neu anordnen können, sie jedoch nicht ausblenden oder löschen können.

Sie können je nach Bedarf in Ihrer Organisation benutzerdefinierte Problemstatus hinzufügen. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Für Benutzende ist das Ändern des Status eines Problems in der Regel ein manueller Prozess. Es gibt jedoch Situationen, die in der folgenden Liste beschrieben werden, wenn sich der Status eines Problems automatisch ändert, abhängig von anderen Faktoren, die im System auftreten.

Die folgenden Problemstatus werden mit Ihrer Workfront-Instanz bereitgestellt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Systemanfragestatus</th> 
   <th>So können Sie den Status verwenden</th> 
   <th>Was passiert im Status?</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Neu (erforderlicher Status)</td> 
   <td>Dies ist der Standardstatus für jedes neu erstellte Problem.</td> 
   <td>Wenn sich das Problem in einem Projekt mit dem Status „Aktuell“ befindet, wird das Problem auf der Registerkarte „Arbeitsanfragen“ der Benutzenden angezeigt, die dem Problem zugewiesen sind. Benutzer können jetzt mit der Bearbeitung des Problems beginnen.</td> 
  </tr> 
  <tr> 
   <td>In Bearbeitung (erforderlicher Status)</td> 
   <td> <p>Sie können ein Problem in diesem Status platzieren, um anzugeben, dass die Arbeit an diesem Problem begonnen hat.</p> <p>Wenn die Lösung des Problems mit einem anderen Objekt (einer Aufgabe, einem Projekt oder einem anderen Problem) verbunden ist, wird der Problemstatus automatisch in In Bearbeitung geändert, wenn Sie den Status des Lösungsobjekts in In Bearbeitung ändern. </p> <p>Weitere Informationen zum Auflösen von Objekten finden Sie unter <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Übersicht über das Auflösen und das Auflösen von Objekten </a>.</p> </td> 
   <td> <p>Wenn sich das Problem in einem Projekt mit dem Status „Aktuell“ befindet, wird das Problem auf der Registerkarte „Arbeiten an“ der Benutzenden angezeigt, die dem Problem zugewiesen sind.</p> <p>Wenn ein Problem in Bearbeitung ist, wird ein Wert für das tatsächliche Startdatum angezeigt.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Geschlossen (erforderlicher Status)</td> 
   <td> <p>Sie können ein Problem manuell als „Geschlossen“ markieren, wenn die Bearbeitung abgeschlossen ist. </p> <p>Wenn die Problemlösung mit einem anderen Objekt verbunden ist (einer Aufgabe, einem Projekt oder einem anderen Problem), wird der Problemstatus automatisch in Geschlossen geändert, wenn Sie den Status des Lösungsobjekts in Geschlossen ändern.</p> <p>Weitere Informationen zum Auflösen von Objekten finden Sie unter <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Übersicht über das Auflösen und das Auflösen von Objekten </a>.</p> </td> 
   <td> <p>Wenn ein Problem geschlossen wird, wird das Problem aus der Liste der bearbeiteten Elemente des Empfängers entfernt. In diesem Fall zeigt das Problem einen Wert für das tatsächliche Abschlussdatum an. </p> <p>Wenn alle Aufgaben abgeschlossen und Probleme für ein Projekt geschlossen sind, kann das Projekt abgeschlossen werden.</p> </td> 
  </tr> 
  <tr> 
   <td>Halten (erforderlicher Status)</td> 
   <td> <p>Sie können ein Problem manuell als „Zurückgestellt“ markieren, um anzugeben, dass es bei der Behebung des Problems zu einer Verzögerung gekommen ist. </p> </td> 
   <td> <p>Wenn sich das Problem in einem Projekt mit dem Status „Aktuell“ befindet, wird das Problem auf der Registerkarte „Arbeiten an“ der Benutzenden angezeigt, die dem Problem zugewiesen sind. </p> <p>Wenn alle Aufgaben in einem Projekt abgeschlossen sind, aber mindestens ein Halten-Problem im Projekt vorhanden ist, kann das Projekt nicht abgeschlossen werden. </p> </td> 
  </tr> 
  <tr> 
   <td>Erneut geöffnet (entspricht in Bearbeitung)</td> 
   <td> <p>Sie können ein Problem in diesem Status platzieren, um anzugeben, dass die Arbeit an diesem Problem nicht ganz abgeschlossen war, als das Problem zuvor geschlossen wurde, und dass es erneut geöffnet werden musste, um die Arbeit abzuschließen.</p> </td> 
   <td> <p>Wenn sich das Problem in einem Projekt mit dem Status „Aktuell“ befindet, wird das Problem auf der Registerkarte „Arbeitsanfragen“ der Benutzenden angezeigt, die dem Problem zugewiesen sind. Benutzer können jetzt mit der Bearbeitung des Problems beginnen.</p> <p>Dieser Status ist beim Reporting wichtig, um zwischen Problemen zu unterscheiden, die zum ersten Mal offen sind (normalerweise im Status Neu ), und Problemen, die geöffnet sind, nachdem sie zuvor geschlossen wurden (normalerweise im Status Erneut geöffnet ). </p> </td> 
  </tr> 
  <tr> 
   <td>Warten auf Feedback (entspricht Halten)</td> 
   <td>Sie können in diesem Status ein Problem platzieren, um anzugeben, dass Sie auf Feedback warten (normalerweise vom Primären Kontakt), bevor Sie mit der Bearbeitung des Problems fortfahren können. </td> 
   <td> <p>Wenn sich das Problem in einem Projekt mit dem Status „Aktuell“ befindet, wird das Problem auf der Registerkarte „Arbeiten an“ der Benutzenden angezeigt, die dem Problem zugewiesen sind.</p> <p>Wenn ein Problem auf Feedback wartet, kann ein Projekt nicht abgeschlossen werden.</p> <p>Dieser Status ist beim Reporting wichtig, um zwischen Problemen zu unterscheiden, die derzeit offen sind, aber bearbeitet werden (normalerweise im Status In Bearbeitung), und Problemen, die derzeit offen sind, aber nicht bearbeitet werden, da mehr Feedback erforderlich ist, um sie abzuschließen (normalerweise im Status Feedback ausstehend).</p> </td> 
  </tr> 
  <tr> 
   <td>Kann nicht duplizieren (entspricht „geschlossen„)</td> 
   <td>Sie können ein Problem in diesem Status platzieren, um anzugeben, dass Sie das Problem schließen, aber Sie konnten das Problem, das zum Öffnen des Problems führte, nicht sehen. Das Problem kann möglicherweise weiterhin bestehen, kann jedoch zu einem bestimmten Zeitpunkt nicht repliziert werden. </td> 
   <td> <p>Dieser Status ist beim Reporting wichtig, um zwischen Problemen zu unterscheiden, die abgeschlossen wurden und deren Problem behoben wurde (normalerweise im Status Geschlossen ), und Problemen, deren Problem zu einem bestimmten Zeitpunkt nicht sichtbar ist (normalerweise im Status Nicht duplizieren ).</p> <p>Wenn ein Problem als „Kann nicht duplizieren“ markiert ist, wird das Problem aus der Liste der bearbeiteten Elemente des Empfängers entfernt. In diesem Fall zeigt das Problem einen Wert für das tatsächliche Abschlussdatum an.</p> <p>Wenn alle Aufgaben in einem Projekt abgeschlossen sind und einige Probleme den Status „Kann nicht duplizieren“ aufweisen, kann das Projekt abgeschlossen werden.</p> </td> 
  </tr> 
  <tr> 
   <td>Gelöst (entspricht Geschlossen)</td> 
   <td>Sie können ein Problem in diesem Status platzieren, um anzugeben, dass Sie das Problem schließen und das Problem, durch das es verursacht wurde, tatsächlich behoben wurde.</td> 
   <td> <p>Dieser Status ist beim Reporting wichtig, um zwischen Problemen zu unterscheiden, die mit oder ohne Lösung geschlossen wurden (normalerweise im Status Geschlossen ), und Problemen, die mit einer tatsächlichen Lösung geschlossen wurden (normalerweise im Status Gelöst ).</p> <p>Wenn ein Problem als „Gelöst“ markiert wird, wird das Problem aus der Liste der zu bearbeitenden Personen entfernt. In diesem Fall zeigt das Problem einen Wert für das tatsächliche Abschlussdatum an.</p> <p>Wenn alle Aufgaben in einem Projekt abgeschlossen sind und sich mindestens ein Problem im Status „Gelöst“ befindet, kann das Projekt abgeschlossen werden. </p> </td> 
  </tr> 
  <tr> 
   <td>Verifiziert abgeschlossen (entspricht geschlossen)</td> 
   <td>Sie können ein Problem in diesem Status platzieren, um anzugeben, dass Sie das Problem schließen und überprüft haben, ob das Problem, das das Problem verursacht hat, behoben wurde.</td> 
   <td> <p>Wenn ein Problem als „Geprüft abgeschlossen“ markiert wird, wird das Problem aus der Liste der bearbeiteten Elemente des Empfängers entfernt. In diesem Fall zeigt das Problem einen Wert für das tatsächliche Abschlussdatum an.</p> <p>Wenn alle Aufgaben in einem Projekt abgeschlossen sind und einige Probleme den Status Geprüft abgeschlossen aufweisen, kann das Projekt abgeschlossen werden.</p> </td> 
  </tr> 
  <tr> 
   <td>Kann nicht aufgelöst werden (entspricht „geschlossen„)</td> 
   <td>Sie können ein Problem in diesem Status platzieren, um anzugeben, dass Sie das Problem schließen, das Problem, das es verursacht hat, jedoch nicht gelöst werden kann.</td> 
   <td> <p>Dieser Status ist beim Reporting wichtig, um zwischen Problemen zu unterscheiden, die mit oder ohne Lösung geschlossen wurden (normalerweise im Status Geschlossen ), und Problemen, die ohne tatsächliche Lösung geschlossen wurden (normalerweise im Status Nicht aufgelöst ).</p> <p>Wenn ein Problem als „Wird nicht behoben“ gekennzeichnet ist, wird das Problem aus der Liste der bearbeiteten Elemente des Verantwortlichen entfernt. In diesem Fall zeigt das Problem einen Wert für das tatsächliche Abschlussdatum an.</p> <p>Wenn alle Aufgaben in einem Projekt abgeschlossen sind und sich mindestens ein Problem im Status Wird nicht behoben befindet, kann das Projekt abgeschlossen werden.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anfragestatus anpassen

Ein Workfront-Administrator kann Workfront Problemstatus auf Systemebene und Gruppenebene hinzufügen und die Reihenfolge ändern, in der Benutzer sie sehen. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Ein Gruppenadministrator bzw. eine Gruppenadministratorin kann einen benutzerdefinierten Status hinzufügen, der für eine Gruppe spezifisch ist. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
