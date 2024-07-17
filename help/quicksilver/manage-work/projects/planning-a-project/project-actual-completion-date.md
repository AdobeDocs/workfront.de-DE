---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Übersicht über das tatsächliche Abschlussdatum des Projekts
description: Projekte, Aufgaben und Probleme haben in Adobe Workfront das tatsächliche Abschlussdatum. Dies ist das Datum, an dem das Projekt, die Aufgabe oder das Problem als abgeschlossen markiert wurde.
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
source-git-commit: c593eab154a0942995b1f913e7189450913faac0
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# Übersicht über das tatsächliche Abschlussdatum des Projekts

Projekte, Aufgaben und Probleme haben in Adobe Workfront das tatsächliche Abschlussdatum. Dies ist das Datum, an dem das Projekt, die Aufgabe oder das Problem als abgeschlossen markiert wurde.

## Tatsächliche Abschlussdaten

Das Datum des tatsächlichen Abschlusses stellt das tatsächliche Datum und die Uhrzeit des tatsächlichen Abschlusses der Arbeiten dar. Wenn eine Aufgabe oder ein Problem als Fertig oder Fertig markiert ist, legt Workfront das Datum der Statusänderung des Elements automatisch als Datum des tatsächlichen Abschlusses der Aufgabe oder des Problems fest. Wenn dieses Datum nicht genau dem Zeitpunkt entspricht, zu dem die Aufgabe oder das Problem tatsächlich abgeschlossen wurde, können Sie das tatsächliche Abschlussdatum manuell bearbeiten.

Sie können beispielsweise eine Aufgabe oder ein Problem &quot;Fertig&quot;am Montag markieren, Sie wissen jedoch, dass die Arbeit am vorigen Freitag abgeschlossen wurde. Nachdem Sie die Aufgabe oder das Problem mit Fertig markiert haben, können Sie das tatsächliche Abschlussdatum der Aufgabe oder des Problems manuell auf das Datum des vorherigen Freitags aktualisieren, um den tatsächlichen Abschluss widerzuspiegeln.

Das tatsächliche Abschlussdatum eines Projekts kann nicht manuell bearbeitet werden. Sie können jedoch den Projektstatus manuell ändern, wodurch eine Änderung an seinem tatsächlichen Abschlussdatum Trigger werden kann.

Das tatsächliche Abschlussdatum eines Projekts wird wie folgt festgelegt:

* Durch manuelles Aktualisieren des Projektstatus: Wenn der Abschlussmodus des Projekts auf &quot;Manuell&quot;festgelegt ist und Sie den Projektstatus manuell auf &quot;Abgeschlossen&quot;ändern, wird das tatsächliche Abschlussdatum des Projekts in Trigger mit dem Datum und der Uhrzeit der letzten abgeschlossenen Aufgabe aktualisiert.
* Wenn die letzte Aufgabe des Projekts automatisch abgeschlossen ist: Wenn der Abschlussmodus des Projekts auf Automatisch eingestellt ist und Sie die letzte Aufgabe als Abgeschlossen markieren oder das tatsächliche Abschlussdatum der letzten Aufgabe aktualisieren, wird das tatsächliche Abschlussdatum des Projekts ebenfalls mit diesem Datum aktualisiert.

  Informationen zum Festlegen des Abschlussmodus eines Projekts finden Sie im Artikel [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

  >[!NOTE]
  >
  >Workfront verwendet das tatsächliche Abschlussdatum aus der Aufgabe des Projekts, das zuletzt abgeschlossen wurde, als tatsächlichen Abschlussdatum für das gesamte Projekt.

Ein Workfront- oder Gruppenadministrator bestimmt, ob Workfront das aktuelle Datum oder das geplante Abschlussdatum einer Aufgabe oder ein Problem verwendet, wenn diese auf Fertig stellen oder geschlossen eingestellt sind. Informationen zum Festlegen von Aufgaben- und Problemeinstellungen finden Sie unter [Konfigurieren von systemweiten Aufgaben- und Problemeinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## Tatsächliche Abschlussdaten suchen

Das tatsächliche Abschlussdatum befindet sich in den folgenden Bereichen von Workfront:

* Bereiche mit Projekt-, Aufgaben- und Problemdetails
* Bearbeiten der Felder &quot;Projekt&quot;, &quot;Aufgabe&quot;und &quot;Problem&quot;
* Bereich für Projekt-, Aufgaben- und Problemaktualisierungen als Systemaktualisierung.
* Projekt-, Aufgaben- oder Problemlisten oder Berichte.

Weitere Informationen zum Erstellen von Berichten finden Sie im Artikel [Benutzerspezifischen Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
