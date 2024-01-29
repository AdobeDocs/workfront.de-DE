---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Übersicht über das geplante Abschlussdatum für Projekte, Aufgaben und Probleme
description: Das geplante Abschlussdatum ist ein berechneter Echtzeitindikator dafür, wann das Projekt, die Aufgabe oder das Problem abgeschlossen sein wird. Wenn das Projekt, die Aufgabe oder das Problem als abgeschlossen markiert ist, ändert sich das vorgeschlagene Abschlussdatum in das Datum des tatsächlichen Abschlussdatums.
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: d71ee30378c39975366f4f257e3f7b17aba0c0ae
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---

# Übersicht über das geplante Abschlussdatum für Projekte, Aufgaben und Probleme

<!-- Audited: 1/2024 -->

Das geplante Abschlussdatum ist ein berechneter Echtzeitindikator dafür, wann das Projekt, die Aufgabe oder das Problem abgeschlossen sein wird. Wenn das Projekt, die Aufgabe oder das Problem als abgeschlossen markiert ist, ändert sich das vorgeschlagene Abschlussdatum in das Datum des tatsächlichen Abschlussdatums.

In den folgenden Abschnitten wird beschrieben, wie das geplante Abschlussdatum für Projekte, Aufgaben und Probleme bestimmt wird und wie Sie es finden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Neu: 
   <ul><li><p>Beitragende oder höher zur Anzeige des geplanten Abschlussdatums in einem Bericht</p></li> <li><p>Eine Standardlizenz zum Erstellen eines Berichts</p></li> </ul>

<p>Aktuell: 
   <ul><li><p>Überprüfen oder höher , um das voraussichtliche Abschlussdatum in einem Bericht anzuzeigen</p></li> 
   <li><p>Eine Planungslizenz zum Erstellen eines Berichts</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Anzeigen oder höherer Zugriff auf Projekte</p> <p>Sie müssen Zugriff auf Berichte, Dashboards und Kalender bearbeiten haben, um einen Bericht erstellen zu können</p> <p>Sie müssen Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten haben, um einen Bericht zu erstellen oder eine Listenansicht zu ändern</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für ein Projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## So bestimmt Adobe Workfront das geplante Abschlussdatum

Das vorgeschlagene Abschlussdatum ist ein berechnetes Feld, das nicht manuell geändert werden kann.

Die Kriterien zur Bestimmung des geplanten Abschlussdatums unterscheiden sich je nach angezeigtem Objekt:

* **Projekte:** Das vorgeschlagene Abschlussdatum für Projekte entspricht dem geplanten Abschlussdatum der letzten Aufgabe des Projekts.

  Bei einem höheren Prozentsatz für &quot;complete&quot;wird beispielsweise das geplante Abschlussdatum der Aufgabe näher an den aktuellen Tag verschoben. Wenn der Status der Aufgabe Neu ist und das geplante Abschlussdatum der Aufgabe kurz oder vorüber ist, wird das geplante Abschlussdatum weiter in die Zukunft verschoben.

* **Aufgaben:** Das geplante Abschlussdatum für Aufgaben wird anhand der folgenden Kriterien bestimmt:

   * **Fortschrittsaktualisierungen der Aufgabe durch den Aufgabenverantwortlichen:** Zu Fortschrittsaktualisierungen gehören Änderungen am prozentualen Abschluss und Änderungen des Aufgabenstatus.
   * **Commit Date:** Wenn der Aufgabenverantwortliche ein Bestätigungsdatum angibt, wird das vorgeschlagene Abschlussdatum so geändert, dass es mit dem Zustimmungsdatum übereinstimmt.

     Weitere Informationen zu &quot;Commit Dates&quot;finden Sie im Artikel [Datum bestätigen - Übersicht](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **Vorgänger:** Wenn es keine Verzögerungen bei den Vorgängeraufgaben gibt, sollte das geplante Abschlussdatum mit dem geplanten Abschlussdatum übereinstimmen. Abhängige Aufgaben zeigen bei auftretenden Verzögerungen ein prognostiziertes Abschlussdatum an, das über dem geplanten Abschlussdatum liegt.

     Weitere Informationen zum geplanten Abschlussdatum von Aufgaben finden Sie unter [Übersicht über die geplante Aufgabe - Abschlussdatum](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

  >[!IMPORTANT]
  >
  >Wenn der Vorgänger einer Aufgabe über ein tatsächliches Abschlussdatum verfügt, erhalten die abhängigen Aufgaben ein prognostiziertes Abschlussdatum, wie im folgenden Szenario beschrieben:
  >
  >
  >Wenn das Projekt Aufgabe A, Aufgabe B und Aufgabe C umfasst und Aufgabe B der Nachfolger von Aufgabe A ist, ist Aufgabe C der Nachfolger von Aufgabe B und ein tatsächliches Abschlussdatum wird Aufgabe A hinzugefügt, wird das geplante Abschlussdatum automatisch für Aufgabe B neu berechnet (sofern die **Aktualisierungstyp** des Projekts ist auf Automatisch und Bei Änderung eingestellt), wird es jedoch nicht für Aufgabe C neu berechnet. Derzeit berechnet Workfront aus Leistungsgründen das geplante Abschlussdatum für Aufgaben, die eine Ebene nach oben oder unten von der aktualisierten Aufgabe entfernt sind. 

* **Probleme:** Das Problem Projected Completion Date (Geschätztes Abschlussdatum) wurde ursprünglich so eingestellt, dass es dem Problem Plantes Abschlussdatum entspricht.

  Wenn der Problemverantwortliche ein Commit-Datum angibt, ändern sich sowohl das geplante Abschlussdatum als auch das geplante Abschlussdatum entsprechend dem Commit-Datum.

  Weitere Informationen zu &quot;Commit Dates&quot;finden Sie im Artikel [Datum bestätigen - Übersicht](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Anzeigen des geplanten Abschlussdatums

Sie können das geplante Abschlussdatum von Projekten, Aufgaben und Problemen in Berichten anzeigen. Sie können das geplante Abschlussdatum von Projekten und Aufgaben in anderen Bereichen von Workfront anzeigen.

### Anzeigen des geplanten Abschlussdatums eines Projekts {#view-the-projected-completion-date-of-a-project}

1. Wechseln Sie zu dem Projekt, in dem das geplante Abschlussdatum angezeigt werden soll.
1. Klicks **Projektdetails** im linken Bereich.
1. Suchen Sie die **Voraussichtlicher Abschluss** im Feld **Übersicht** > **Projektdaten** Abschnitt.

### Anzeigen des geplanten Abschlussdatums einer Aufgabe {#view-the-projected-completion-date-of-a-task}

1. Gehen Sie zu der Aufgabe, in der Sie das geplante Abschlussdatum anzeigen möchten.
1. Klicks **Aufgabendetails** im linken Bereich.
1. Suchen Sie die **Voraussichtlicher Abschluss** im Feld **Übersicht** > **Aufgabendaten und -begrenzung** Abschnitt.

### Anzeigen des geplanten Abschlussdatums eines Problems {#view-the-projected-completion-date-of-an-issue}

Sie können das geplante Abschlussdatum nur für Probleme in einem Problembericht oder in der Listenansicht anzeigen. Das Erstellen einer Listenansicht ähnelt dem Erstellen einer Ansicht in einem Bericht.

So erstellen Sie einen Problembericht mit dem geplanten Abschlussdatum:

1. Erstellen Sie einen Problembericht, wie im Artikel beschrieben. [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Wählen Sie die **Spalten (Ansicht)** Registerkarte.
1. Klicks **Spalte hinzufügen**, und beginnen Sie mit der Eingabe **Voraussichtlicher Abschluss** im **In dieser Spalte anzeigen:** -Feld.

1. Wählen Sie es aus, wenn es in der Liste unter der **Problem** -Objekt. 
1. Klicks **Speichern und schließen**.

   Die **Voraussichtlicher Abschluss** -Spalte im Bericht gefüllt. 

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
