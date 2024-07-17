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

## Warum fehlt &quot;Aufgabe oben/unten einfügen&quot;, wenn ich mit der rechten Maustaste auf eine Aufgabe in der Aufgabenliste klicke?

### Antwort

Um die Einfügeoptionen verwenden zu können, muss die Aufgabenliste nach Anzahl sortiert sein. Um die Spalte nach Zahl zu sortieren, klicken Sie in der Spaltenüberschrift links von **Aufgabenname** auf **#** , um die Aufgabe nach Zahl neu zu ordnen.

## Welches ist das tatsächliche Abschlussdatum?

### Antwort

Das Datum des tatsächlichen Abschlusses stellt das Datum und die Uhrzeit des Abschlusses der Arbeit dar. Weitere Informationen finden Sie unter [Übersicht über das tatsächliche Abschlussdatum des Projekts](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

## Warum fehlt die Einzug-/Ausschlussschaltfläche?

### Antwort

Um die Schaltfläche &quot;Einzug/Ausrücken&quot;verwenden zu können, müssen Sie sicherstellen, dass die Aufgaben nach der Aufgabennummer sortiert sind und keine Gruppierungen angewendet werden.

## Warum kann ich den Projektstatus nicht in Abgeschlossen ändern?

Ich erhalte die folgende Fehlermeldung, wenn ich versuche, mein Projekt als abgeschlossen zu kennzeichnen:

![Project_FAQ_Complete_Error_message.png](assets/project-faq-complete-error-message-350x138.png)

### Antwort

Sie können den Status eines zu beendenden Projekts nicht ändern, wenn Sie Folgendes in Ihrem Projekt haben:

* Unvollständige Aufgaben oder Probleme
* Aufgabe oder Probleme im Status der ausstehenden Genehmigung

## Warum kann ich den Projektstatus nicht von Fertig stellen in Aktuell ändern?

### Antwort

Wenn der Abschlussmodus des Projekts auf Automatisch eingestellt ist, wechselt der Status des Projekts nach Abschluss aller Aufgaben und Probleme automatisch zu Abgeschlossen und Sie können ihn nicht in einen anderen Status ändern. Der Abschlussmodus des Projekts muss auf Manuell eingestellt sein, damit ein komplettes Projekt in &quot;Aktuell&quot;umgewandelt werden kann. Weitere Informationen finden Sie unter [Der Projektstatus ändert sich nicht von &quot;Complete&quot;in &quot;Current](../../../manage-work/projects/tips-tricks-and-troubleshooting/project-status-does-not-change-from-complete-to-current.md)&quot;.

## Warum kann ich einem Portfolio kein Projekt hinzufügen, obwohl ich über die entsprechenden Berechtigungen verfügt?

Ich habe zwar die richtigen Berechtigungen, aber die Schaltfläche Projekte hinzufügen fehlt auf der Registerkarte Projekte des Portfolios.

### Antwort

Die Ursache liegt darin, dass der Portfolio-Status inaktiv ist. So ändern Sie den Status des Portfolios:

1. Klicken Sie auf **Portfolio Details > Übersicht**.
1. Ändern Sie den **Status** in **Aktiv.**

1. Klicken Sie auf **Speichern**.\
   Die Schaltfläche **Projekte hinzufügen** sollte jetzt auf der Registerkarte **Projekte** angezeigt werden.

## Welchen Zugriff erhält ein Ressourcen-Manager beim Hinzufügen zu einem Projekt?

### Antwort

Ressourcen-Manager erhalten automatisch Zugriff auf Projekte verwalten. Wenn Sie den Benutzer aus der Rolle &quot;Ressourcen-Manager&quot;entfernen, wird der Zugriff auf &quot;Freigabe verwalten&quot;nicht entfernt.

## Warum ändert sich der Projektstatus beim Hinzufügen einer Gruppe?

### Antwort

Der Projektstatus ändert sich aufgrund des Standardstatus der Gruppe. Wenn Sie eine Gruppe zu einem Projekt hinzufügen, wird die Liste der Status zu den für die Gruppe festgelegten Standardstatus geändert.

Weitere Informationen finden Sie im Artikel [Status erstellen oder bearbeiten](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md) .

## Was ist der Budgetstatus?

### Antwort

Der Budgetstatus zeigt an, ob das Projekt derzeit dem Kapazitätsplaner hinzugefügt wird und ob die Budgetberechnung abgeschlossen ist.

Im Folgenden finden Sie Budgetstatus:

* Nicht eingeschlossen - Das Projekt wird nicht zum Kapazitätsplaner hinzugefügt.
* Einbezogen, aber nicht berechnet - Das Projekt wird dem Kapazitätsplaner hinzugefügt, ist jedoch von der Budgetberechnung ausgeschlossen.
* Einbezogen und berechnet - Das Projekt wird zum Kapazitätsplaner hinzugefügt und in die Budgetberechnung einbezogen.

## Warum kann ich ein Projekt, für das ich Eigentümer bin und für das ich Verwaltungsberechtigungen für ein Team habe, nicht freigeben? Ich kann das Team einfach nicht im Freigabedialogfeld des Projekts finden.

### Antwort

Der Adobe Workfront-Administrator beschränkte sich auf die Anzeige von Unternehmen, Gruppen und Teams, denen Sie in Ihrer Zugriffsebene der angehören. Das Team, das Sie suchen, gehört nicht zu den Teams, denen Sie angehören.

![](assets/view-only-team-groups-companies-they-belong-to-350x141.png)

Informationen dazu, wie Sie einem Benutzer die Anzeige aller Teams im System ermöglichen, finden Sie unter [Erstellen oder Ändern benutzerdefinierter Zugriffsebenen](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
