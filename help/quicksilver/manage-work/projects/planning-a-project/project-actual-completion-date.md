---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Übersicht über das tatsächliche Abschlussdatum des Projekts
description: Projekte, Aufgaben und Probleme haben in Adobe Workfront ein tatsächliches Abschlussdatum. Dies ist das Datum, an dem das Projekt, die Aufgabe oder das Problem als abgeschlossen markiert wurden.
author: Alina
feature: Work Management
exl-id: 0baba359-a61d-43d7-8336-1f45c7f34374
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 0%

---

# Übersicht über das tatsächliche Abschlussdatum des Projekts

Projekte, Aufgaben und Probleme haben in Adobe Workfront ein tatsächliches Abschlussdatum. Dies ist das Datum, an dem das Projekt, die Aufgabe oder das Problem als abgeschlossen markiert wurden.

## Tatsächliche Abschlussdaten

Das tatsächliche Abschlussdatum gibt das tatsächliche Datum und die Uhrzeit des Abschlusses der Arbeit an. Wenn eine Aufgabe oder ein Problem als „Fertig“ oder „Abgeschlossen“ markiert wird, setzt Workfront das Datum der Statusänderung des Elements automatisch auf das tatsächliche Abschlussdatum der Aufgabe oder des Problems. Wenn dieses Datum keine genaue Angabe des Zeitpunkts ist, zu dem die Aufgabe oder das Problem tatsächlich abgeschlossen wurde, können Sie das tatsächliche Abschlussdatum manuell bearbeiten.

Sie können beispielsweise eine Aufgabe oder ein Problem als „Fertig“ am Montag markieren, aber Sie wissen, dass die Arbeit am vorherigen Freitag abgeschlossen wurde. Nachdem Sie die Aufgabe oder das Problem als „Erledigt“ gekennzeichnet haben, können Sie das tatsächliche Abschlussdatum der Aufgabe oder des Problems manuell auf das Datum des vorherigen Freitags aktualisieren, um den tatsächlichen Abschluss widerzuspiegeln.

Sie können das tatsächliche Abschlussdatum eines Projekts nicht manuell bearbeiten, aber Sie können den Status eines Projekts manuell ändern, wodurch eine Änderung am tatsächlichen Abschlussdatum Trigger werden kann.

Das tatsächliche Abschlussdatum eines Projekts wird wie folgt festgelegt:

* Durch manuelles Aktualisieren des Projektstatus: Wenn der Fertigstellungsmodus des Projekts auf „Manuell“ festgelegt ist und Sie den Status des Projekts manuell in „Abgeschlossen“ ändern, wird dadurch das tatsächliche Fertigstellungsdatum des Projekts auf das Datum und die Uhrzeit der zuletzt abgeschlossenen Aufgabe Trigger.
* Automatisch, wenn die letzte Aufgabe des Projekts abgeschlossen ist: Wenn der Fertigstellungsmodus des Projekts auf „Automatisch“ eingestellt ist und Sie die letzte Aufgabe als „Abgeschlossen“ markieren oder das tatsächliche Fertigstellungsdatum der letzten Aufgabe aktualisieren, wird das tatsächliche Fertigstellungsdatum des Projekts ebenfalls mit diesem Datum aktualisiert.

  Informationen zum Festlegen des Fertigstellungsmodus eines Projekts finden Sie im Artikel [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

  >[!NOTE]
  >
  >Workfront verwendet das tatsächliche Abschlussdatum aus der Aufgabe des Projekts, die zuletzt abgeschlossen wurde, als tatsächliches Abschlussdatum für das gesamte Projekt.

Ein Workfront- oder Gruppen-Administrator bestimmt, ob Workfront das heutige Datum oder das geplante Abschlussdatum einer Aufgabe oder eines Problems verwendet, wenn diese auf „Abgeschlossen“ oder „Geschlossen“ gesetzt sind. Informationen zum Festlegen von Voreinstellungen für Aufgaben und Probleme finden Sie [Konfigurieren von systemweiten Voreinstellungen für Aufgaben und Probleme](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--this statement is confusing, not sure what it is referring to, so I am drafting this for now: The value for the Actual Completion Date is always what is considered the current date and time.-->



## Tatsächliche Abschlussdaten suchen

Das tatsächliche Abschlussdatum liegt in den folgenden Bereichen von Workfront:

* Projekt-, Aufgaben- und Problemdetailbereiche
* Projekt-, Aufgaben- und Problemfelder bearbeiten
* Projekt-, Aufgaben- und Problem-Updates als System-Update.
* Projekt-, Aufgaben- oder Problemlisten oder Berichte.

Weitere Informationen zum Erstellen von Berichten finden Sie im Artikel [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
