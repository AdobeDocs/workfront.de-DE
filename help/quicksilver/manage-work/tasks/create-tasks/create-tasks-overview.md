---
product-area: projects
navigation-topic: create-tasks
title: Übersicht über Aufgaben erstellen
description: Sie können Aufgaben in einem Projekt erst erstellen, nachdem Sie das Projekt erstellt haben.
author: Alina
feature: Work Management
exl-id: 7bd6578e-9288-4793-ba07-a0c126c479b9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 0%

---

# Übersicht über Aufgaben erstellen

Sie können Aufgaben in einem Projekt erst erstellen, nachdem Sie das Projekt erstellt haben.

Beispielsweise können Sie nach der Erstellung eines Projekts Aufgaben hinzufügen und ändern, um den Projektplan zu organisieren. Weitere Informationen zum Erstellen eines Projekts finden Sie unter [Erstellen eines Projekts](../../../manage-work/projects/create-projects/create-project.md). Weitere Informationen zum Erstellen von Aufgaben finden Sie unter [Erstellen von Aufgaben in einem Projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

In diesem Artikel werden Überlegungen, Einschränkungen und Standardeinstellungen beschrieben, die beim Erstellen von Aufgaben gelten.

## Methoden zum Erstellen von Aufgaben in einem Projekt

Sie können Aufgaben für ein Projekt wie folgt erstellen:

* Von Grund auf, wie unter [Erstellen von Aufgaben in einem Projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) beschrieben.
* Kopieren Sie Aufgaben in dasselbe Projekt oder in ein neues Projekt oder duplizieren Sie Aufgaben im selben Projekt, wie unter [Kopieren und Duplizieren von Aufgaben](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md) beschrieben.
* Verschieben Sie Aufgaben von einem Projekt in ein anderes, wie in [Verschieben von Aufgaben](../../../manage-work/tasks/manage-tasks/move-tasks.md) beschrieben.

## Einschränkungen beim Erstellen von Aufgaben

Wenn Sie über den richtigen Zugriff und die richtigen Berechtigungen verfügen, können Sie Aufgaben für ein Projekt erstellen. In den folgenden Fällen ist es jedoch nicht möglich, Aufgaben zu erstellen:

* Der Adobe Workfront-Administrator oder ein Gruppenadministrator muss das Hinzufügen von Aufgaben zu einem Projekt aktivieren, das sich im Bereich &quot;Projekteinstellungen&quot;im Status &quot;Abgeschlossen&quot;oder &quot;Dead&quot;befindet. Weitere Informationen zum Festlegen von Projektvoreinstellungen finden Sie unter [Konfigurieren von systemweiten Projekteigenschaften](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Sie können einem Projekt, das sich in &quot;Ausstehende Genehmigung&quot;befindet, keine Aufgaben hinzufügen.

## Die maximal zulässige Anzahl von Aufgaben für ein Projekt

Ein Projekt kann bis zu 5.000 Aufgaben enthalten. Eine Warnmeldung wird im Projekt angezeigt, wenn Sie sich dem Grenzwert nähern, wenn Sie den Grenzwert erreicht haben und versuchen, den Grenzwert zu überschreiten.

Je nachdem, wie viele Aufgaben in Ihren Projekten enthalten waren, als diese Einschränkung auferlegt wurde, kann Ihre Workfront-Instanz mehr als 5.000 Aufgaben in einem Projekt ermöglichen.

Wenn Sie mehr als 5.000 Aufgaben in ein einzelnes Projekt einbeziehen können, beachten Sie Folgendes:

* Die Aufgabenbegrenzung für Ihre Workfront-Umgebung ist auf die aktuelle Anzahl an Aufgaben in Ihrem größten Projekt sowie weitere 10 % festgelegt.

  Wenn beispielsweise ein Projekt in Ihrer Workfront-Instanz 10.000 Aufgaben enthält, beträgt die Grenze für jedes Projekt in Ihrer Workfront-Instanz 11.000 Aufgaben.

* Kleinere Projekte verbessern die Leistung und minimieren Managementaufgaben, die große Projekte begleiten.

## Aufgabenstandardwerte beim Hinzufügen von Aufgaben zu einem Projekt

Es gibt zwei Arten von Standardinformationen, die Workfront automatisch für Aufgaben aktualisiert, wenn Sie diese erstellen:

* Standardinformationen auf Systemebene

  Ihr Workfront-Administrator oder ein Gruppenadministrator legt die Standardeinstellungen auf Systemebene für Aufgaben im Bereich &quot;Aufgaben und Probleme&quot;unter &quot;Projektanvoreinstellungen&quot;fest. Informationen zu den Voreinstellungen für Aufgaben und Probleme finden Sie unter [Konfigurieren von systemweiten Aufgaben- und Problemeinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) oder [Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

* Standardinformationen auf Projektebene

  Im Rest dieses Abschnitts werden die Standardeinstellungen auf Projektebene beschrieben, die Sie als Projektmanager für alle neuen Aufgaben definieren können, die einem Projekt hinzugefügt werden

Wenn Sie eine Aufgabe zu einem Projekt hinzufügen, hängt es davon ab, wie das Projekt eingerichtet ist, Workfront kann der Aufgabe automatisch einen Genehmigungsprozess oder benutzerdefinierte Formulare anhängen.

Weitere Informationen zum Konfigurieren eines Projekts, um diese standardmäßig hinzuzufügen, finden Sie im Abschnitt &quot;Aufgaben&quot;im Artikel [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md) .

Beachten Sie beim Definieren von Standardinformationen, die mit Aufgaben verknüpft werden sollen, die einem Projekt auf Projektebene hinzugefügt werden, Folgendes:

* Sie müssen über Verwaltungsberechtigungen für das Projekt verfügen, um die Standardeinstellungen für den Aufgabengenehmigungsprozess und benutzerdefinierte Formulare zu definieren.
* Alle neuen Aufgaben werden mit dem Validierungsprozess und den benutzerdefinierten Formularen erstellt, die beim Bearbeiten des Projekts definiert werden.
* Sie können diese Standardeinstellungen ändern, wenn Sie Aufgaben über das Feld &quot;Aufgabe bearbeiten&quot;hinzufügen, aber nicht, wenn Sie Aufgaben in der Inline-Bearbeitung hinzufügen.
* Sie können den Genehmigungsprozess und die benutzerdefinierten Formulare für Aufgaben in einer Vorlage definieren.

   * Wenn ein Projekt aus dieser Vorlage erstellt wird, werden der Genehmigungsprozess und benutzerdefinierte Formulare automatisch auf das Projekt angewendet.
   * Wenn eine Vorlage an ein vorhandenes Projekt angehängt wird, behält das Projekt den ursprünglichen Aufgabengenehmigungsprozess und die benutzerdefinierten Formulareinstellungen bei, sofern sie definiert sind. Wenn sie nicht definiert sind, werden die Einstellungen aus der Vorlage zu den Einstellungen für das Projekt.
   * Wenn eine Vorlage an ein vorhandenes Projekt angehängt wird, behalten die aus der Vorlage hinzugefügten Aufgaben den Genehmigungsprozess und die benutzerdefinierten Formulareinstellungen, die sie in der Vorlage hatten, unabhängig von den Aufgabeneinstellungen für das Projekt bei.

  Weitere Informationen zum Anhängen einer Vorlage an ein Projekt finden Sie unter [Anhängen einer Vorlage an ein Projekt](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Wenn Sie das Projekt kopieren, werden die Standardeinstellungen der Aufgabe an das neue Projekt übertragen.

  Weitere Informationen zum Kopieren eines Projekts finden Sie unter [Kopieren eines Projekts](../../../manage-work/projects/manage-projects/copy-project.md).

* Wenn Sie Aufgaben von einem Projekt in ein anderes kopieren und das Zielprojekt unterschiedliche Standardeinstellungen für Aufgaben hat, bleiben die Standardeinstellungen des Originalprojekts bei den kopierten Aufgaben erhalten, es sei denn, sie werden beim Kopieren gelöscht.
* Wenn Sie eine Aufgabe in dasselbe Projekt duplizieren, werden die benutzerdefinierten Formulare und der Genehmigungsprozess in die duplizierte Aufgabe übertragen.

  Informationen zum Kopieren und Duplizieren von Aufgaben finden Sie unter [ [Aufgaben kopieren und duplizieren](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

* Wenn Sie die Aufgabe in ein anderes Projekt verschieben, werden die Standardeinstellungen für die Aufgaben des ursprünglichen Projekts gespeichert, unabhängig von den Standardeinstellungen der Aufgabe für das neue Projekt.

  Informationen zum Verschieben von Aufgaben finden Sie unter [Verschieben von Aufgaben](../../../manage-work/tasks/manage-tasks/move-tasks.md).
