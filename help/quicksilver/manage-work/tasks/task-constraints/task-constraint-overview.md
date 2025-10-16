---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: Aufgabenbeschränkung - Übersicht
description: Aufgabenbeschränkungen bestimmen, wann eine Aufgabe in einem Projekt beginnen und enden soll.
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 6%

---

# Aufgabenbeschränkung - Übersicht

<!-- Audited: 12/2023 -->

Aufgabenbeschränkungen bestimmen, wann eine Aufgabe in einem Projekt beginnen und enden soll.

## Übersicht über Aufgabenbeschränkungen

Während Sie Ihren Projektplan erstellen, treffen Sie Entscheidungen über die Reihenfolge und den Zeitrahmen Ihrer Aufgaben im Projekt. Aufgaben können unabhängig von einer Aufgabensequenz funktionieren, sie können sich jedoch auf die Projektzeitleiste auswirken. Aufgabenbeschränkungen ermöglichen es einem Projektmanager zu planen, wann bestimmte Aufgaben in einem Projekt beginnen oder abgeschlossen werden können.

Abhängig von der von Ihnen verwendeten Einschränkung müssen Sie möglicherweise ein geplantes Startdatum, ein geplantes Abschlussdatum oder beides für die Aufgabe angeben.

Einschränkungstypen, für die ein definiertes Datum erforderlich ist, wirken sich auf Vorgängerbeziehungen aus.

>[!TIP]
>
>Erwägen Sie die Verwendung eines Einschränkungstyps, für den keine bestimmten Daten erforderlich sind, wenn Sie Vorgängerbeziehungen zwischen Aufgaben verwenden.

In der folgenden Tabelle werden jede Einschränkung und ihre Abkürzungen angezeigt. Die Abkürzungen werden in Aufgabenlisten und beim Erstellen von Kickstart-Importdateien verwendet. Klicken Sie auf den verknüpften Titel jeder Aufgabenbeschränkung, um weitere Informationen zu diesem Einschränkungstyp zu erhalten.

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col>
 <thead> 
  <tr> 
   <th> <p><strong>Einschränkungsname</strong> </p> </th> 
   <th> <p><strong>Abkürzung</strong> </p> </th> 
   <th> <p><strong>Beschreibung</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">Übersicht über die Aufgabenbeschränkung: So bald wie möglich</a> </p> </td> 
   <td scope="col"> <p>SBWM</p> </td>
   <td scope="col"> <p>Platziert die Startzeit der Aufgabe so nah wie möglich am Anfang des Projekts.</p> 
   <p>Dies ist die standardmäßige Einschränkung, wenn das Projekt den Planungsmodus ab dem Startdatum verwendet und wenn das standardmäßige Startdatum des Systems für eine neue Aufgabe auf Basierend auf dem geplanten Datum des Projekts festgelegt ist. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">Übersicht über die Aufgabenbeschränkung: So spät wie möglich </a> </p> </td> 
   <td scope="col"> <p>SSWM</p> </td> 
   <td scope="col"> <p>Platziert die Abschlusszeit der Aufgabe so nah wie möglich am Ende des Projekts.</p> 
   <p>Dies ist die Standardeinschränkung, wenn der Projektzeitplanmodus auf „Ab Abschlussdatum“ und der System- oder Gruppenstandard für das Startdatum einer Aufgabe auf „Basierend auf dem geplanten Projektdatum“ festgelegt ist. </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">Übersicht über die Aufgabenbeschränkung: Früheste verfügbare Zeit</a> </p> </td> 
   <td scope="col"> <p>FVZ</p> </td> 
 <td scope="col"> <p>Plant eine Aufgabe, um zum frühestmöglichen verfügbaren Zeitpunkt zu beginnen, nachdem alle Vorgängerbeziehungen berücksichtigt wurden.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">Übersicht über die Aufgabenbeschränkung: Letzte verfügbare Zeit</a> </p> </td> 
   <td scope="col"> <p>BREITENGRAD</p> </td> 
   <td scope="col"> <p>Legt fest, dass eine Aufgabe zum spätestens verfügbaren Zeitpunkt beginnt, nachdem Vorgänger-Nachfolger-Beziehungen im Projekt berücksichtigt wurden.</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">Übersicht über die Aufgabenbeschränkung: Nicht früher starten als</a> </p> </td> 
   <td scope="col"> <p>NFAA</p> </td> 
   <td scope="col"> <p>Plant eine Aufgabe, die nach dem von Ihnen angegebenen Datum beginnt.</p> 
   <p>Dies ist die Standardeinschränkung, wenn der Projektzeitplanmodus vom Startdatum ist und wenn das standardmäßige Startdatum des Systems oder der Gruppe für eine neue Aufgabe auf Heute festgelegt ist.   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">Übersicht über die Aufgabenbeschränkung: Spätestens starten nach</a> </p> </td> 
   <td scope="col"> <p>NSAA</p> </td> 
   <td scope="col"> <p>Plant eine Aufgabe, die vor dem angegebenen Datum beginnt.</p> 
   <p>Dies ist die Standardeinschränkung, wenn der Projektzeitplanmodus vom Abschlussdatum ist und wenn der System- oder Gruppenstandard für das Startdatum einer Aufgabe auf Heute gesetzt ist. 
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">Übersicht über die Aufgabenbeschränkung: Beenden nicht früher als</a> </p> </td> 
   <td scope="col"> <p>NFBA</p> </td>
   <td scope="col"> <p>Plant eine Aufgabe, die nach dem von Ihnen angegebenen Datum abgeschlossen werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">Übersicht über die Aufgabenbeschränkung: Spätestes Beenden</a> </p> </td> 
   <td scope="col"> <p>NSBA</p> </td> 
   <td scope="col"> <p>Plant eine Aufgabe, die vor dem angegebenen Datum abgeschlossen werden soll.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">Übersicht über die Aufgabenbeschränkung: Muss beginnen am</a> </p> </td> 
   <td scope="col"> <p>MAA</p> </td> 
   <td scope="col"> <p>Legt fest, dass eine Aufgabe genau an einem bestimmten Datum beginnt.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">Übersicht über die Aufgabenbeschränkung: Muss abgeschlossen sein am</a> </p> </td> 
   <td scope="col"> <p>MBWA</p> </td> 
   <td scope="col"> <p>Plant eine Aufgabe, die an einem bestimmten Datum endet.</p> </td>
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">Übersicht über die Aufgabenbeschränkung: Feste Datumswerte</a> </p> </td> 
   <td> <p>FIXT</p> </td> 
   <td> <p>Plant eine Aufgabe, die an einem bestimmten Datum beginnt und endet.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Übersicht über Standardeinschränkungen

Beim Erstellen neuer Aufgaben wird von Workfront automatisch eine Aufgabenbeschränkung ausgewählt.

Workfront verwendet zwei Variablen, um zu entscheiden, welche Aufgabenbeschränkung standardmäßig für eine neue Aufgabe ausgewählt wird:

* Das Feld **Projektzeitplan ab** im Projekt.

  Weitere Informationen über das Feld Projektzeitplan aus finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

* Die **Startdatum**, die von Ihrem Workfront- oder Gruppenadministrator im Bereich **Aufgaben und Probleme** von &quot;**&quot;** wurde.

  Informationen zu den Voreinstellungen für Aufgaben und Probleme finden Sie im Abschnitt [Neue Aufgaben](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#new-task-defaults) in [Konfigurieren von systemweiten Aufgaben- und Problem-Voreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Die folgende Tabelle zeigt die standardmäßige Aufgabenbeschränkung bei der Auswahl verschiedener Variablen für Ihr Projekt und Ihre neuen Aufgaben:

| Projektzeitplan von | Startdatum der Aufgabe | Standard für Aufgabenbeschränkung |
|---|---|---|
| Startdatum | Auf Basis des geplanten Projektdatums | So bald wie möglich (SBWM) |
| Startdatum | Heute | Nicht früher anfangen als |
| Fertigstellungsdatum | Auf Basis des geplanten Projektdatums | So spät wie möglich |
| Fertigstellungsdatum | Heute | Nicht später anfangen als |
