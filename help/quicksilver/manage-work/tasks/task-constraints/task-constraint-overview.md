---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: Übersicht über Aufgabenbegrenzungen
description: Aufgabenbegrenzungen bestimmen, wann eine Aufgabe in einem Projekt gestartet und beendet werden soll.
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 6%

---

# Übersicht über Aufgabenbegrenzungen

Aufgabenbegrenzungen bestimmen, wann eine Aufgabe in einem Projekt gestartet und beendet werden soll.

## Übersicht über Aufgabenbeschränkungen

Beim Erstellen Ihres Projektplans treffen Sie Entscheidungen über die Reihenfolge und den Zeitrahmen Ihrer Aufgaben im Projekt. Aufgaben können unabhängig von jeder Aufgabensequenz funktionieren, können sich jedoch auf die Projekt-Timeline auswirken. Aufgabenbeschränkungen ermöglichen es einem Projektmanager, zu planen, wann bestimmte Aufgaben in einem Projekt gestartet oder abgeschlossen werden können.

Abhängig von der verwendeten Einschränkung müssen Sie möglicherweise ein geplantes Startdatum, ein geplantes Abschlussdatum oder beides für die Aufgabe angeben.

Begrenzungstypen, für die definierte Daten erforderlich sind, wirken sich auf Vorgängerbeziehungen aus.

>[!TIP]
>
>Erwägen Sie die Verwendung eines Beschränkungstyps, der bei Verwendung von Vorgängerbeziehungen zwischen Aufgaben keine bestimmten Daten erfordert.

In der folgenden Tabelle werden die einzelnen Einschränkungen und ihre Abkürzung angezeigt. Abkürzungen werden für Aufgabenlisten und beim Erstellen von Kick-Start-Importdateien verwendet. Klicken Sie auf den verknüpften Titel jeder Aufgabenbegrenzung, um weitere Informationen zu dieser Art von Beschränkung zu erhalten.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col>
 <thead> 
  <tr> 
   <th> <p><strong>Beschränkungsname</strong> </p> </th> 
   <th> <p><strong>Abkürzung</strong> </p> </th> 
   <th> <p><strong>Beschreibung</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">Übersicht über Aufgabenbeschränkungen: So bald wie möglich</a> </p> </td> 
   <td scope="col"> <p>SBWM</p> </td>
   <td scope="col"> <p>Platziert die Startzeit der Aufgabe so nah wie möglich am Anfang des Projekts.</p> 
   <p>Dies ist die Standardeinschränkung, wenn das Projekt einen Planungsmodus vom Startdatum verwendet und das standardmäßige Startdatum des Systems für eine neue Aufgabe auf Basierend auf dem geplanten Projektdatum festgelegt ist. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">Übersicht über Aufgabenbeschränkungen: So bald wie möglich </a> </p> </td> 
   <td scope="col"> <p>SSWM</p> </td> 
   <td scope="col"> <p>Platziert die Fertigstellungszeit der Aufgabe so nah wie möglich am Ende des Projekts.</p> 
   <p>Dies ist die Standardeinschränkung, wenn der Projektplanmodus vom Abschlussdatum ist und das System- oder Gruppenstandarddatum für das Startdatum einer Aufgabe auf Basis des geplanten Projektzeitraums liegt. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">Übersicht über Aufgabenbeschränkungen: Frühzeitige Verfügbarkeitszeit</a> </p> </td> 
   <td scope="col"> <p>FVZ</p> </td> 
 <td scope="col"> <p>Planung einer Aufgabe, die zum frühestmöglichen Zeitpunkt nach Berücksichtigung von Vorgängerbeziehungen beginnt.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">Übersicht über Aufgabenbeschränkungen: Neueste verfügbare Zeit</a> </p> </td> 
   <td scope="col"> <p>SMZ</p> </td> 
   <td scope="col"> <p>Planen Sie eine Aufgabe so, dass sie spätestens zum verfügbaren Zeitpunkt beginnt, nachdem Sie die Beziehungen zwischen Vorgänger und Nachfolger im Projekt in Betracht gezogen haben.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">Übersicht über Aufgabenbeschränkungen: Start nicht früher als</a> </p> </td> 
   <td scope="col"> <p>NFAA</p> </td> 
   <td scope="col"> <p>Zeitt den Beginn einer Aufgabe nach dem von Ihnen angegebenen Datum.</p> 
   <p>Dies ist die Standardeinschränkung, wenn der Projektplanmodus vom Startdatum ist und das standardmäßige Startdatum des Systems oder der Gruppe für eine neue Aufgabe auf Heute gesetzt ist.   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">Übersicht über Aufgabenbeschränkungen: Start nicht später als</a> </p> </td> 
   <td scope="col"> <p>NSAA</p> </td> 
   <td scope="col"> <p>Planung einer Aufgabe, die vor dem angegebenen Datum beginnt.</p> 
   <p>Dies ist die Standardeinschränkung, wenn der Projektplanmodus vom Abschlussdatum ist und das System- oder Gruppenstandarddatum für das Startdatum einer Aufgabe Heute ist. 
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">Übersicht über Aufgabenbeschränkungen: Beenden nicht früher als</a> </p> </td> 
   <td scope="col"> <p>NFBA</p> </td>
   <td scope="col"> <p>Zeitt den Abschluss einer Aufgabe nach dem von Ihnen angegebenen Datum.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">Übersicht über Aufgabenbeschränkungen: Finish No Later Than</a> </p> </td> 
   <td scope="col"> <p>NSBA</p> </td> 
   <td scope="col"> <p>Zeitt den Abschluss einer Aufgabe vor dem angegebenen Datum.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">Übersicht über Aufgabenbeschränkungen: Muss beginnen bei</a> </p> </td> 
   <td scope="col"> <p>MAA</p> </td> 
   <td scope="col"> <p>Zeitt eine Aufgabe so ein, dass sie genau an einem bestimmten Datum beginnt.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">Übersicht über Aufgabenbeschränkungen: Muss abgeschlossen sein am</a> </p> </td> 
   <td scope="col"> <p>MBWA</p> </td> 
   <td scope="col"> <p>Planung einer Aufgabe, die an einem bestimmten Datum endet.</p> </td>
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">Übersicht über Aufgabenbeschränkungen: Feste Datumswerte</a> </p> </td> 
   <td> <p>FIXT</p> </td> 
   <td> <p>Planung einer Aufgabe zum Beginn und Ende an einem bestimmten Datum.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Übersicht über die Standardbeschränkungen

Wenn Sie neue Aufgaben erstellen, wird Workfront automatisch eine Aufgabenbegrenzung auswählen.

Workfront verwendet zwei Variablen, um zu entscheiden, welche Aufgabenbegrenzung standardmäßig für eine neue Aufgabe ausgewählt ist:

* Die **Projektzeitplan ab** im Projekt.

  Weitere Informationen zum Feld &quot;Projektplan ab&quot;finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

* Die **Startdatum** von Ihrem Workfront- oder Gruppenadministrator im **Aufgaben und Probleme** Gebiet von **Einrichtung**.

  Weitere Informationen zu den Voreinstellungen für Aufgaben und Probleme finden Sie im Abschnitt &quot;Neue Standardeinstellungen für Aufgaben&quot;unter [Systemweite Aufgaben- und Problemeinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Die folgende Tabelle zeigt die standardmäßige Task-Beschränkung bei der Auswahl verschiedener Variablen für Ihr Projekt und Ihre neuen Aufgaben:

| Projektzeitplan ab | Task Start Date | Task Constraint Default |
|---|---|---|
| Startdatum | Auf Basis des geplanten Projektdatums | So bald wie möglich (SBWM) |
| Startdatum | Heute | Nicht früher anfangen als |
| Abschlussdatum | Auf Basis des geplanten Projektdatums | So bald wie möglich |
| Abschlussdatum | Heute | Nicht später anfangen als |
