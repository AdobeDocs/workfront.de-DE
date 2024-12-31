---
title: Häufig gestellte Fragen zu Projekten
description: Häufig gestellte Fragen zu Projekten
author: Alina
draft: Probably
feature: Work Management
exl-id: be262d72-f4e4-4426-a6bc-23499667fc97
source-git-commit: 869a1f9e4fd7e3b65591050530b96d6dae9e230c
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 1%

---

# Häufig gestellte Fragen zu Projekten

Im Folgenden finden Sie häufig gestellte Fragen zu Projekten.

## Warum fehlt die Option Aufgabe oben/unten einfügen, wenn ich mit der rechten Maustaste auf eine Aufgabe in der Aufgabenliste klicke?

### Antwort

Um die Einfügeoptionen verwenden zu können, muss die Aufgabenliste nach Anzahl sortiert werden. Um die Spalte nach Zahl zu sortieren, klicken Sie auf **#** in der Spaltenüberschrift links neben **Aufgabenname**, um die Aufgabe nach Zahl zu sortieren.

## Was ist das tatsächliche Abschlussdatum?

### Antwort

Das tatsächliche Abschlussdatum gibt das Datum und die Uhrzeit des Abschlusses der Arbeit an. Weitere Informationen finden Sie unter [Übersicht über das tatsächliche Abschlussdatum des Projekts](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

## Warum fehlt die Einrückungs-/Ausrückungsschaltfläche?

### Antwort

Um die Schaltfläche zum Einrücken/Ausrücken zu verwenden, stellen Sie sicher, dass die Aufgaben nach der Aufgabennummer sortiert sind und keine Gruppierungen angewendet werden.

## Warum kann ich den Projektstatus nicht in „Abgeschlossen“ ändern?

Wenn ich versuche, mein Projekt als abgeschlossen zu markieren, erhalte ich die folgende Fehlermeldung:

![Project_FAQ_Complete_Error_message.png](assets/project-faq-complete-error-message-350x138.png)

### Antwort

Sie können den Status eines Projekts nicht in „Abgeschlossen“ ändern, wenn Sie eine der folgenden Funktionen in Ihrem Projekt haben:

* Unvollständige Aufgaben oder Probleme
* Aufgabe(n) oder Probleme im Status Ausstehende Genehmigung

## Warum kann ich den Projektstatus nicht von „Abgeschlossen“ in „Aktuell“ ändern?

### Antwort

Wenn der Fertigstellungsmodus des Projekts auf „Automatisch“ festgelegt ist und alle Aufgaben und Probleme abgeschlossen sind, wird der Status des Projekts automatisch auf „Abgeschlossen“ gesetzt, sodass Sie ihn nicht in einen anderen Status ändern können. Der Fertigstellungsmodus des Projekts muss auf Manuell festgelegt werden, damit ein vollständiges Projekt in „Aktuell“ umgewandelt werden kann. Weitere Informationen finden Sie unter [Der Projektstatus ändert sich nicht von Abgeschlossen in Aktuell](../../../manage-work/projects/tips-tricks-and-troubleshooting/project-status-does-not-change-from-complete-to-current.md).

## Warum kann ich ein Projekt nicht zu einem Portfolio hinzufügen, obwohl ich dazu über die richtigen Berechtigungen verfüge?

Obwohl ich über die richtigen Berechtigungen verfüge, fehlt die Schaltfläche Projekte hinzufügen auf der Registerkarte Projekte des Portfolios.

### Antwort

Dies liegt daran, dass der Portfolio-Status „Inaktiv“ ist. So ändern Sie den Status des Portfolios:

1. Klicken Sie auf **Portfolio-Details > Übersicht**.
1. Ändern Sie **Status** in **Aktiv.**

1. Klicken Sie auf **Speichern**.\
   Die **Projekte hinzufügen**-Schaltfläche sollte jetzt auf der Registerkarte **Projekte** angezeigt werden.

## Welchen Zugriff erhält ein Ressourcen-Manager, wenn er zu einem Projekt hinzugefügt wird?

### Antwort

Ressourcenmanager erhalten automatisch Verwaltungszugriff auf Projekte. Wenn Sie den Benutzer aus der Rolle „Ressourcen-Manager“ entfernen, wird nicht sein Zugriff auf die Verwaltungsfreigabe entfernt.

## Warum ändert sich der Projektstatus, wenn ich eine Gruppe hinzufüge?

### Antwort

Die Projektstatus ändern sich aufgrund der Standardstatus der Gruppe. Wenn Sie eine Gruppe zu einem Projekt hinzufügen, wird die Liste der Status auf die für die Gruppe festgelegten Standardstatus geändert.

Weitere Informationen finden Sie im Artikel [Erstellen oder Bearbeiten eines Status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## Was ist der Budgetstatus?

### Antwort

Der Budgetstatus gibt an, ob das Projekt derzeit zum Kapazitätsplaner hinzugefügt wurde und ob die Budgetberechnung abgeschlossen wurde.

Im Folgenden finden Sie Budgetstatus:

* Nicht enthalten : Das Projekt wird nicht zum Kapazitätsplaner hinzugefügt.
* Eingeschlossen, aber nicht berechnet - Das Projekt wird zum Kapazitätsplaner hinzugefügt, aber von der Budgetberechnung ausgeschlossen.
* Eingeschlossen und berechnet : Das Projekt wird zum Kapazitätsplaner hinzugefügt und in die Budgetberechnung einbezogen.

## Warum kann ich ein Projekt, dessen Eigentümer ich bin und für das ich Verwaltungsberechtigungen habe, nicht für ein Team freigeben? Ich kann das Team einfach nicht im Freigabedialogfeld des Projekts finden.

### Antwort

Der Adobe Workfront-Administrator hat Sie darauf beschränkt, nur Unternehmen, Gruppen und Teams anzuzeigen, denen Sie in Ihrer Zugriffsebene des s angehören. Das gesuchte Team gehört nicht zu den Teams, denen Sie angehören.

![](assets/view-only-team-groups-companies-they-belong-to-350x141.png)

Informationen dazu, wie Sie es einem Benutzer ermöglichen, alle Teams im System anzuzeigen, finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
