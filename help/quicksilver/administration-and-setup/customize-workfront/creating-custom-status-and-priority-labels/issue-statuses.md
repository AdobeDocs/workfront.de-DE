---
title: Zugriff auf die Liste der Systemfehlerstatus
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Sie können den Status eines Problems verwenden, um Benutzern im System anzuzeigen, in welchem Entwicklungsstadium ein Problem zu einem bestimmten Zeitpunkt vorliegt.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9bdaec2f-acdf-4cbf-a308-ebcc861dbb89
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '1444'
ht-degree: 0%

---

# Zugriff auf die Liste der Systemfehlerstatus

Sie können den Status eines Problems verwenden, um Benutzern im System anzuzeigen, in welchem Entwicklungsstadium ein Problem zu einem bestimmten Zeitpunkt vorliegt.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Standard</p>
       <p>Oder</p>
       <p>Aktuell: Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Status von Zugriffsproblemen

Sie können auf den Status von Problemen auf Systemebene zugreifen und diesen ändern. Sie können einige Informationen zu den Standardsystemstatus bearbeiten oder neue benutzerdefinierte Status erstellen. Weitere Informationen zum Erstellen benutzerdefinierter Status oder Bearbeiten des Systemstatus finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

So greifen Sie auf den Status von Problemen auf Systemebene zu:

{{step-1-to-setup}}

1. Klicken Sie auf **Projekteinstellungen** > **Status**.

1. Klicken Sie auf die Registerkarte **Probleme** , um den in Workfront verfügbaren Problemstatus anzuzeigen.

   ![](assets/issue-status.png)

## Status von Systemproblemen

Workfront verfügt über 10 ursprüngliche Problemstatus. Die ersten 4 in der Tabelle unten sind erforderlich. Das bedeutet, dass Sie sie entsperren, umbenennen und neu anordnen können, sie jedoch nicht ausblenden oder löschen können.

Sie können benutzerdefinierte Problemstatus hinzufügen, um den Anforderungen in Ihrer Organisation zu entsprechen. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Für Benutzer ist das Ändern des Status eines Problems normalerweise ein manueller Prozess. Es gibt jedoch Situationen, die in der folgenden Liste beschrieben werden, wenn sich der Status eines Problems automatisch ändert, je nach anderen Faktoren, die im System auftreten.

Die folgenden Problemstatus werden mit Ihrer Workfront-Instanz bereitgestellt:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Status des Systemfehlers</th> 
   <th>Verwendung des Status</th> 
   <th>Was geschieht im Status?</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Neu (erforderlicher Status)</td> 
   <td>Dies ist der Standardstatus für jedes neu erstellte Problem.</td> 
   <td>Wenn sich das Problem in einem Projekt mit dem Status "Aktuell"befindet, wird das Problem auf der Registerkarte "Arbeitsanforderungen"der Benutzer angezeigt, die dem Problem zugewiesen sind. Benutzer können jetzt mit der Bearbeitung des Problems beginnen.</td> 
  </tr> 
  <tr> 
   <td>Wird ausgeführt (erforderlicher Status)</td> 
   <td> <p>Sie können ein Problem in diesen Status einfügen, um anzugeben, dass die Arbeit an diesem Problem begonnen hat.</p> <p>Wenn die Lösung des Problems mit einem anderen Objekt (einer Aufgabe, einem Projekt oder einem anderen Problem) verbunden ist, wird der Problemstatus automatisch in Wird ausgeführt geändert, wenn Sie den Status des aufgelösten Objekts in Wird ausgeführt ändern. </p> <p>Weitere Informationen zum Auflösen von Objekten finden Sie unter <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Übersicht über das Auflösen und Auflösen von Objekten </a>.</p> </td> 
   <td> <p>Wenn sich das Problem in einem Projekt mit dem Status "Aktuell"befindet, wird das Problem auf der Registerkarte "Arbeiten am"der Benutzer angezeigt, die dem Problem zugewiesen sind.</p> <p>Wenn ein Problem in Bearbeitung ist, zeigt das Problem einen Wert für das tatsächliche Startdatum an.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>Geschlossen (erforderlicher Status)</td> 
   <td> <p>Sie können ein Problem manuell als geschlossen markieren, wenn die Arbeit daran abgeschlossen ist. </p> <p>Wenn die Lösung des Problems mit einem anderen Objekt (einer Aufgabe, einem Projekt oder einem anderen Problem) verbunden ist, wird der Problemstatus automatisch in Geschlossen geändert, wenn Sie den Status des auflösenden Objekts in Geschlossen ändern.</p> <p>Weitere Informationen zum Auflösen von Objekten finden Sie unter <a href="../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md" class="MCXref xref">Übersicht über das Auflösen und Auflösen von Objekten </a>.</p> </td> 
   <td> <p>Wenn ein Problem geschlossen wird, wird das Problem aus der Liste "Arbeiten an"des Verantwortlichen entfernt. In diesem Fall zeigt das Problem einen Wert für das tatsächliche Abschlussdatum an. </p> <p>Wenn alle Aufgaben abgeschlossen sind und Probleme in einem Projekt geschlossen sind, kann das Projekt abgeschlossen werden.</p> </td> 
  </tr> 
  <tr> 
   <td>Auf Halten (erforderlicher Status)</td> 
   <td> <p>Sie können ein Problem manuell als "Auf Abbrechen"markieren, um anzugeben, dass es eine Verzögerung beim Abschließen des Problems gegeben hat. </p> </td> 
   <td> <p>Wenn sich das Problem in einem Projekt mit dem Status "Aktuell"befindet, wird das Problem auf der Registerkarte "Arbeiten am"der Benutzer angezeigt, die dem Problem zugewiesen sind. </p> <p>Wenn alle Aufgaben für ein Projekt abgeschlossen sind, das Projekt jedoch mindestens ein On Hold-Problem aufweist, kann das Projekt nicht abgeschlossen werden. </p> </td> 
  </tr> 
  <tr> 
   <td>Neu geöffnet (entspricht In Bearbeitung)</td> 
   <td> <p>Sie können ein Problem in diesem Status platzieren, um anzuzeigen, dass die Arbeit an diesem Problem nicht ganz abgeschlossen war, als das Problem zuvor geschlossen wurde, und dass es erneut geöffnet werden musste, um die Arbeit abzuschließen.</p> </td> 
   <td> <p>Wenn sich das Problem in einem Projekt mit dem Status "Aktuell"befindet, wird das Problem auf der Registerkarte "Arbeitsanforderungen"der Benutzer angezeigt, die dem Problem zugewiesen sind. Benutzer können jetzt mit der Bearbeitung des Problems beginnen.</p> <p>Dieser Status ist für die Berichterstellung wichtig, um zwischen Problemen zu unterscheiden, die zum ersten Mal geöffnet sind (normalerweise im neuen Status), und Problemen, die geöffnet werden, nachdem sie zuvor geschlossen wurden (normalerweise im Status Neu ). </p> </td> 
  </tr> 
  <tr> 
   <td>Abwarten von Feedback (entspricht On Hold)</td> 
   <td>Sie können ein Problem in diesen Status einfügen, um anzugeben, dass Sie auf Feedback warten (normalerweise vom Primären Kontakt), bevor Sie mit der Bearbeitung des Problems fortfahren können. </td> 
   <td> <p>Wenn sich das Problem in einem Projekt mit dem Status "Aktuell"befindet, wird das Problem auf der Registerkarte "Arbeiten am"der Benutzer angezeigt, die dem Problem zugewiesen sind.</p> <p>Wenn ein Problem auf Feedback wartet, kann ein Projekt nicht abgeschlossen werden.</p> <p>Dieser Status ist für die Berichterstellung wichtig, um zwischen aktuell offenen, aber in Bearbeitung befindlichen Problemen (normalerweise im Status In Bearbeitung ) und Problemen zu unterscheiden, die aktuell geöffnet sind, aber nicht bearbeitet werden, da mehr Feedback erforderlich ist, um sie abzuschließen (normalerweise im Status Erwartetes Feedback ).</p> </td> 
  </tr> 
  <tr> 
   <td>Kann nicht dupliziert werden (entspricht geschlossen)</td> 
   <td>Sie können ein Problem in diesen Status einfügen, um anzugeben, dass Sie das Problem schließen, aber das Problem, das das Öffnen des Problems ausgelöst hat, konnte nicht angezeigt werden. Das Problem könnte noch existieren, kann aber nicht zu einem bestimmten Zeitpunkt repliziert werden. </td> 
   <td> <p>Dieser Status ist für die Berichterstellung wichtig, um zwischen abgeschlossenen Problemen und Problemen zu unterscheiden, deren Problem behoben wurde (in der Regel im Status Geschlossen ), und Problemen, deren Problem zu einem bestimmten Zeitpunkt nicht sichtbar ist (in der Regel im Status Kann duplizieren ).</p> <p>Wenn ein Problem als "Kann nicht duplizieren"markiert ist, wird das Problem aus der Liste "Arbeiten an"des Verantwortlichen entfernt. In diesem Fall zeigt das Problem einen Wert für das tatsächliche Abschlussdatum an.</p> <p>Wenn alle Aufgaben in einem Projekt abgeschlossen sind und sich einige Probleme im Status Kann nicht duplizieren befinden, kann das Projekt abgeschlossen werden.</p> </td> 
  </tr> 
  <tr> 
   <td>Gelöst (entspricht geschlossen)</td> 
   <td>Sie können ein Problem in diesen Status einfügen, um anzugeben, dass Sie das Problem schließen und das Problem, das das Problem verursacht hat, tatsächlich behoben wurde.</td> 
   <td> <p>Dieser Status ist für die Berichterstellung wichtig, um zwischen Problemen zu unterscheiden, die mit oder ohne Lösung geschlossen werden (normalerweise im Status "Geschlossen"), und Problemen, die mit einer tatsächlichen Auflösung geschlossen werden (normalerweise im Status "Gelöst").</p> <p>Wenn ein Problem als gelöst markiert ist, wird das Problem aus der Liste "Arbeiten an"des Verantwortlichen entfernt. In diesem Fall zeigt das Problem einen Wert für das tatsächliche Abschlussdatum an.</p> <p>Wenn alle Aufgaben in einem Projekt abgeschlossen sind und sich mindestens ein Problem im Status Gelöst befindet, kann das Projekt abgeschlossen werden. </p> </td> 
  </tr> 
  <tr> 
   <td>Verified Complete (entspricht geschlossen)</td> 
   <td>Sie können ein Problem in diesen Status einfügen, um anzugeben, dass Sie das Problem schließen und sichergestellt haben, dass das Problem, das das Problem verursacht hat, behoben wurde.</td> 
   <td> <p>Wenn ein Problem als "Verified Complete"markiert ist, wird das Problem aus der Liste "Working On"des Verantwortlichen entfernt. In diesem Fall zeigt das Problem einen Wert für das tatsächliche Abschlussdatum an.</p> <p>Wenn alle Aufgaben in einem Projekt abgeschlossen sind und sich einige Probleme im Status "Verified Complete"befinden, kann das Projekt abgeschlossen werden.</p> </td> 
  </tr> 
  <tr> 
   <td>Nicht auflösen (entspricht geschlossen)</td> 
   <td>Sie können ein Problem in diesen Status einfügen, um anzugeben, dass Sie das Problem schließen, das Problem, das es verursacht hat, kann jedoch nicht gelöst werden.</td> 
   <td> <p>Dieser Status ist für die Berichterstellung wichtig, um zwischen Problemen zu unterscheiden, die mit oder ohne Lösung geschlossen werden (normalerweise im Status "Geschlossen"), und Problemen, die ohne tatsächliche Lösung geschlossen werden (normalerweise im Status "Nicht aufgelöst").</p> <p>Wenn ein Problem als "Nicht beheben"markiert ist, wird das Problem aus der Liste "Arbeiten an"des Verantwortlichen entfernt. In diesem Fall zeigt das Problem einen Wert für das tatsächliche Abschlussdatum an.</p> <p>Wenn alle Aufgaben in einem Projekt abgeschlossen sind und mindestens ein Problem den Status "Wird nicht aufgelöst"aufweist, kann das Projekt abgeschlossen werden.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anpassen des Problemstatus

Ein Workfront-Administrator kann Workfront den Status von Problemen auf Systemebene und Gruppenebene hinzufügen und die Reihenfolge ändern, in der Benutzer sie sehen. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Ein Gruppenadministrator kann einen benutzerspezifischen Status für eine Gruppe hinzufügen. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
