---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Übersicht über das geplante Abschlussdatum für Projekte, Aufgaben und Probleme
description: Das geplante Abschlussdatum ist ein berechneter Echtzeitindikator dafür, wann das Projekt, die Aufgabe oder das Problem abgeschlossen sein wird. Wenn das Projekt, die Aufgabe oder das Problem als abgeschlossen markiert ist, ändert sich das vorgeschlagene Abschlussdatum in das Datum des tatsächlichen Abschlussdatums.
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# Übersicht über das geplante Abschlussdatum für Projekte, Aufgaben und Probleme

<!-- Audited: 1/2024 -->

Das geplante Abschlussdatum ist ein berechneter Echtzeitindikator dafür, wann das Projekt, die Aufgabe oder das Problem abgeschlossen sein wird. Wenn das Projekt, die Aufgabe oder das Problem als abgeschlossen markiert ist, ändert sich das vorgeschlagene Abschlussdatum in das Datum des tatsächlichen Abschlussdatums.

In den folgenden Abschnitten wird beschrieben, wie das geplante Abschlussdatum für Projekte, Aufgaben und Probleme bestimmt wird und wie Sie es finden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.


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
   <td> 
   <p>Neu: 
   <ul><li><p>Beitragende oder höher zur Anzeige des geplanten Abschlussdatums in einem Bericht</p></li> <li><p>Eine Standardlizenz zum Erstellen eines Berichts</p></li> </ul>

<p>Aktuell: 
   <ul><li><p>Überprüfen oder höher , um das voraussichtliche Abschlussdatum in einem Bericht anzuzeigen</p></li> 
   <li><p>Eine Planungslizenz zum Erstellen eines Berichts</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene</td> 
   <td> <p>Anzeigen oder höherer Zugriff auf Projekte</p> <p>Sie müssen Zugriff auf Berichte, Dashboards und Kalender bearbeiten haben, um einen Bericht erstellen zu können</p> <p>Sie müssen Zugriff auf Filter, Ansichten und Gruppierungen bearbeiten haben, um einen Bericht zu erstellen oder eine Listenansicht zu ändern</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für ein Projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## So bestimmt Adobe Workfront das geplante Abschlussdatum

Das vorgeschlagene Abschlussdatum ist ein berechnetes Feld, das nicht manuell geändert werden kann.

Die Kriterien zur Bestimmung des geplanten Abschlussdatums unterscheiden sich je nach angezeigtem Objekt:

* **Projekte:** Das geplante Abschlussdatum für Projekte entspricht dem geplanten Abschlussdatum der letzten Aufgabe des Projekts.

  Bei einem höheren Prozentsatz für &quot;complete&quot;wird beispielsweise das geplante Abschlussdatum der Aufgabe näher an den aktuellen Tag verschoben. Wenn der Status der Aufgabe Neu ist und das geplante Abschlussdatum der Aufgabe kurz oder vorüber ist, wird das geplante Abschlussdatum weiter in die Zukunft verschoben.

* **Aufgaben:** Das geplante Abschlussdatum für Aufgaben wird anhand der folgenden Kriterien bestimmt:

   * **Fortschrittsaktualisierungen, die der Aufgabenverantwortliche an der Aufgabe vorgenommen hat:** Fortschrittsaktualisierungen umfassen Änderungen am prozentualen Abschluss und Änderungen des Aufgabenstatus.
   * **Veröffentlichungsdatum:** Wenn der Aufgabenverantwortliche ein Zustimmungsdatum angibt, wird das geplante Abschlussdatum entsprechend dem Zustimmungsdatum geändert.

     Weitere Informationen zu &quot;Commit Dates&quot;finden Sie im Artikel [Übersicht über das Veröffentlichungsdatum](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **Vorgänger:** Wenn es keine Verzögerungen bei den Vorgängeraufgaben gibt, sollte das geplante Abschlussdatum mit dem geplanten Abschlussdatum übereinstimmen. Abhängige Aufgaben zeigen bei auftretenden Verzögerungen ein prognostiziertes Abschlussdatum an, das über dem geplanten Abschlussdatum liegt.

     Weitere Informationen zum geplanten Abschlussdatum von Aufgaben finden Sie unter [Übersicht über das geplante Abschlussdatum der Aufgabe](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

  >[!IMPORTANT]
  >
  >Wenn der Vorgänger einer Aufgabe über ein tatsächliches Abschlussdatum verfügt, erhalten die abhängigen Aufgaben ein prognostiziertes Abschlussdatum, wie im folgenden Szenario beschrieben:
  >
  >
  >Wenn das Projekt Aufgabe A, Aufgabe B und Aufgabe C umfasst und Aufgabe B der Nachfolger von Aufgabe A ist, ist Aufgabe C der Nachfolger von Aufgabe B und ein tatsächliches Abschlussdatum wird Aufgabe A hinzugefügt, wird das geplante Abschlussdatum automatisch für Aufgabe B neu berechnet (sofern der **Aktualisierungstyp** des Projekts auf &quot;Automatisch&quot;und &quot;Bei Änderung&quot;festgelegt ist), jedoch nicht für Aufgabe C neu berechnet. Derzeit berechnet Workfront aus Leistungsgründen das geplante Abschlussdatum für Aufgaben, die eine Ebene nach oben oder unten von der aktualisierten Aufgabe entfernt sind.

* **Probleme:** Das prognostizierte Abschlussdatum des Problems wird zunächst so eingestellt, dass es mit dem geplanten Abschlussdatum des Problems übereinstimmt.

  Wenn der Problemverantwortliche ein Commit-Datum angibt, ändern sich sowohl das geplante Abschlussdatum als auch das geplante Abschlussdatum entsprechend dem Commit-Datum.

  Weitere Informationen zu &quot;Commit Dates&quot;finden Sie im Artikel [Übersicht über das Veröffentlichungsdatum](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Anzeigen des geplanten Abschlussdatums

Sie können das geplante Abschlussdatum von Projekten, Aufgaben und Problemen in Berichten anzeigen. Sie können das geplante Abschlussdatum von Projekten und Aufgaben in anderen Bereichen von Workfront anzeigen.

### Anzeigen des geplanten Abschlussdatums eines Projekts {#view-the-projected-completion-date-of-a-project}

1. Wechseln Sie zu dem Projekt, in dem das geplante Abschlussdatum angezeigt werden soll.
1. Klicken Sie im linken Bereich auf **Projektdetails** .
1. Suchen Sie im Abschnitt **Überblick** > **Projektzeitraum** das Feld **Projiziertes Abschlussdatum** .

### Anzeigen des geplanten Abschlussdatums einer Aufgabe {#view-the-projected-completion-date-of-a-task}

1. Gehen Sie zu der Aufgabe, in der Sie das geplante Abschlussdatum anzeigen möchten.
1. Klicken Sie im linken Bereich auf **Aufgabendetails** .
1. Suchen Sie im Abschnitt **Überblick** > **Aufgabendaten und -begrenzung** nach dem Feld **Vorgeschlagenes Abschlussdatum** .

### Anzeigen des geplanten Abschlussdatums eines Problems {#view-the-projected-completion-date-of-an-issue}

Sie können das geplante Abschlussdatum nur für Probleme in einem Problembericht oder in der Listenansicht anzeigen. Das Erstellen einer Listenansicht ähnelt dem Erstellen einer Ansicht in einem Bericht.

So erstellen Sie einen Problembericht mit dem geplanten Abschlussdatum:

1. Erstellen Sie einen Problembericht, wie im Artikel [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) beschrieben.
1. Wählen Sie die Registerkarte **Spalten (Ansicht)** aus.
1. Klicken Sie auf **Spalte hinzufügen** und geben Sie im Feld **In dieser Spalte anzeigen:** das Feld **Voraussichtliches Abschlussdatum** ein.

1. Wählen Sie sie aus, wenn sie in der Liste unter dem Objekt **Problem** angezeigt wird.
1. Klicken Sie auf **Speichern + schließen**.

   Die Spalte **Voraussichtliches Abschlussdatum** im Bericht wird ausgefüllt.

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
