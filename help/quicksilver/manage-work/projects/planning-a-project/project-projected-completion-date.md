---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Übersicht über das voraussichtliche Abschlussdatum für Projekte, Aufgaben und Probleme
description: Das voraussichtliche Abschlussdatum ist ein Echtzeitindikator für den Zeitpunkt, zu dem das Projekt, die Aufgabe oder das Problem abgeschlossen wird. Wenn das Projekt, die Aufgabe oder das Problem als „Abgeschlossen“ gekennzeichnet ist, ändert sich das voraussichtliche Abschlussdatum in das tatsächliche Abschlussdatum.
author: Alina
feature: Work Management
exl-id: dde400e6-189f-4431-8f2f-7142ce424826
source-git-commit: 811d8076a0b344e863b25aa253a0fb1c102f0435
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# Übersicht über das voraussichtliche Abschlussdatum für Projekte, Aufgaben und Probleme

<!-- Audited: 1/2024 -->

Das voraussichtliche Abschlussdatum ist ein Echtzeitindikator für den Zeitpunkt, zu dem das Projekt, die Aufgabe oder das Problem abgeschlossen wird. Wenn das Projekt, die Aufgabe oder das Problem als „Abgeschlossen“ gekennzeichnet ist, ändert sich das voraussichtliche Abschlussdatum in das tatsächliche Abschlussdatum.

In den folgenden Abschnitten wird beschrieben, wie das voraussichtliche Abschlussdatum für Projekte, Aufgaben und Probleme ermittelt wird und wie Sie es finden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
   <p>Neu: 
   <ul><li><p>Mitarbeiter oder höher, um das voraussichtliche Abschlussdatum in einem Bericht anzuzeigen</p></li> <li><p>Eine Standardlizenz zum Erstellen eines Berichts</p></li> </ul>

<p>Aktuell: 
   <ul><li><p>Überprüfen Sie oder höher, um das voraussichtliche Abschlussdatum in einem Bericht anzuzeigen</p></li> 
   <li><p>Planlizenz zum Erstellen eines Berichts</p> </li></ul>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte anzeigen oder höher</p> <p>Sie müssen Bearbeitungszugriff auf Berichte, Dashboards und Kalender haben, um einen Bericht zu erstellen</p> <p>Sie müssen Bearbeitungszugriff auf Filter, Ansichten oder Gruppierungen haben, um einen Bericht erstellen oder eine Listenansicht ändern zu können</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Erweitern von Berechtigungen für ein Projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Wie Adobe Workfront das voraussichtliche Abschlussdatum bestimmt

Das voraussichtliche Abschlussdatum ist ein berechnetes Feld, das nicht manuell geändert werden kann.

Die Kriterien, die zur Bestimmung des voraussichtlichen Abschlussdatums verwendet werden, unterscheiden sich je nach dem Objekt, das Sie anzeigen:

* **Projekte:** Das voraussichtliche Abschlussdatum für Projekte entspricht dem voraussichtlichen Abschlussdatum der letzten Aufgabe im Projekt.

  Beispiel: Ein höherer Prozentsatz der Fertigstellung verschiebt das voraussichtliche Abschlussdatum der Aufgabe näher an den aktuellen Tag. Wenn der Status der Aufgabe „Neu“ lautet und das geplante Abschlussdatum der Aufgabe geschlossen ist oder bereits überschritten wurde, geht das voraussichtliche Abschlussdatum weiter in die Zukunft.

* **Aufgaben:** Das voraussichtliche Abschlussdatum für Aufgaben wird anhand der folgenden Kriterien bestimmt:

   * **Fortschrittsaktualisierungen, die vom Aufgabenbevollmächtigten an der Aufgabe vorgenommen wurden** Zu den Fortschrittsaktualisierungen gehören Änderungen an „Prozent abgeschlossen“ und Änderungen am Aufgabenstatus.
   * **Commit-Datum** Wenn der Aufgabenzugewiesene ein Commit-Datum angibt, ändert sich das voraussichtliche Abschlussdatum, sodass es dem Commit-Datum entspricht.

     Weitere Informationen zu Commit-Terminen finden Sie im Artikel [Übersicht über Commit-Datum](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

   * **Vorgänger:** Wenn es bei den Vorgängeraufgaben keine Verzögerungen gibt, sollte das voraussichtliche Abschlussdatum mit dem geplanten Abschlussdatum übereinstimmen. Wenn Verzögerungen auftreten, zeigen abhängige Aufgaben ein voraussichtliches Abschlussdatum an, das nach dem geplanten Abschlussdatum liegt.

     Weitere Informationen zum geplanten Abschlussdatum von Aufgaben finden Sie unter [Übersicht über das geplante Abschlussdatum der Aufgabe](../../../manage-work/tasks/task-information/task-planned-completion-date.md).

  >[!IMPORTANT]
  >
  >Wenn der Vorgänger einer Aufgabe ein tatsächliches Abschlussdatum hat, erhalten die abhängigen Aufgaben ein voraussichtliches Abschlussdatum, wie im folgenden Szenario beschrieben:
  >
  >
  >Wenn das Projekt über Aufgabe A, Aufgabe B und Aufgabe C verfügt und Aufgabe B die Nachfolge von Aufgabe A ist, Aufgabe C die Nachfolge von Aufgabe B ist und ein tatsächliches Abschlussdatum zu Aufgabe A hinzugefügt wird, wird das voraussichtliche Abschlussdatum für Aufgabe B automatisch neu berechnet (vorausgesetzt, der **Aktualisierungstyp** des Projekts ist auf „Automatisch“ und „Bei Änderung“ eingestellt), es wird jedoch für Aufgabe C nicht neu berechnet. Derzeit berechnet Workfront aus Leistungsgründen das voraussichtliche Abschlussdatum für Aufgaben, die eine Ebene nach oben oder unten von der aktualisierten Aufgabe entfernt sind.

* **Probleme:** Das voraussichtliche Abschlussdatum der Anfrage ist zunächst so festgelegt, dass es dem geplanten Abschlussdatum der Anfrage entspricht.

  Wenn der Problembevollmächtigte ein Commit-Datum angibt, ändern sich sowohl das projizierte Abschlussdatum als auch das geplante Abschlussdatum, sodass es dem Commit-Datum entspricht.

  Weitere Informationen zu Commit-Terminen finden Sie im Artikel [Übersicht über Commit-Datum](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Voraussichtliches Abschlussdatum anzeigen

Sie können das voraussichtliche Abschlussdatum von Projekten, Aufgaben und Problemen in Berichten anzeigen. Sie können das voraussichtliche Abschlussdatum von Projekten und Aufgaben in anderen Bereichen von Workfront anzeigen.

### Anzeigen des voraussichtlichen Abschlussdatums eines Projekts {#view-the-projected-completion-date-of-a-project}

1. Wechseln Sie zu dem Projekt, in dem Sie das voraussichtliche Abschlussdatum anzeigen möchten.
1. Klicken Sie **linken** auf „Projektdetails“.
1. Suchen Sie das Feld **Voraussichtliches Abschlussdatum** im Abschnitt **Übersicht** > **Projektdaten**.

### Anzeigen des voraussichtlichen Abschlussdatums einer Aufgabe {#view-the-projected-completion-date-of-a-task}

1. Wechseln Sie zu der Aufgabe, bei der Sie das voraussichtliche Abschlussdatum anzeigen möchten.
1. Klicken Sie **linken** auf „Aufgabendetails“.
1. Suchen Sie das Feld **Voraussichtliches Abschlussdatum** im Abschnitt **Übersicht** > **Aufgabendaten und**).

### Anzeigen des voraussichtlichen Abschlussdatums eines Problems {#view-the-projected-completion-date-of-an-issue}

Das voraussichtliche Abschlussdatum für Anfragen kann nur in einem Problembericht oder in einer Listenansicht angezeigt werden. Das Erstellen einer Listenansicht ähnelt dem Erstellen der Ansicht in einem Bericht.

So erstellen Sie einen Anfragebericht mit dem voraussichtlichen Abschlussdatum:

1. Erstellen Sie einen Problembericht, wie im Artikel [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) beschrieben.
1. Wählen Sie die **Spalten (Ansicht)** aus.
1. Klicken Sie **Spalte hinzufügen** und geben Sie **Voraussichtliches Abschlussdatum** in das Feld **In dieser Spalte anzeigen:** ein.

1. Wählen Sie es aus, wenn es in der Liste unter dem Objekt **Problem** angezeigt wird.
1. Klicken Sie auf **Speichern + schließen**.

   Die **„Voraussichtliches Abschlussdatum** im Bericht wird ausgefüllt.

   ![](assets/issue-projected-completion-date-in-view-nwe-350x148.png)
