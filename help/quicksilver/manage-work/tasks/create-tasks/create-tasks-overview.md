---
product-area: projects
navigation-topic: create-tasks
title: Aufgaben erstellen - Übersicht
description: Sie können Aufgaben in einem Projekt erst erstellen, nachdem Sie das Projekt erstellt haben.
author: Alina
feature: Work Management
exl-id: 7bd6578e-9288-4793-ba07-a0c126c479b9
TQID: https://experienceleague.adobe.com/-xOLBxAGitQAXXRxHSr6R9mv-2hfuLOq0VZKB2TzuqI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 9053a824ecec4feb35a612b26aebb91904ef2546
workflow-type: tm+mt
source-wordcount: 926
ht-degree: 0%

---

# Erstellen von Aufgaben – Überblick

Sie können Aufgaben in einem Projekt erst erstellen, nachdem Sie das Projekt erstellt haben.

Nachdem Sie beispielsweise ein Projekt erstellt haben, können Sie Aufgaben hinzufügen und sie ändern, um den Projektplan zu organisieren. Weitere Informationen zum Erstellen eines Projekts finden Sie unter [Erstellen eines Projekts](../../../manage-work/projects/create-projects/create-project.md). Informationen zum Erstellen von Aufgaben finden Sie unter [Erstellen von Aufgaben in einem Projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md).

In diesem Artikel werden Überlegungen, Einschränkungen und Standardeinstellungen beschrieben, die beim Erstellen von Aufgaben gelten.

## Möglichkeiten zum Erstellen von Aufgaben in einem Projekt

Sie können Aufgaben auf folgende Weise für ein Projekt erstellen:

* von Grund auf neu erstellen, wie [Erstellen von Aufgaben in einem Projekt](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md) beschrieben.
* Kopieren Sie Aufgaben in dasselbe Projekt oder in ein neues Projekt oder duplizieren Sie Aufgaben für dasselbe Projekt, wie unter [&#x200B; und doppelte Aufgaben beschrieben](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* Verschieben von Aufgaben von einem Projekt in ein anderes, wie unter [Verschieben von Aufgaben](../../../manage-work/tasks/manage-tasks/move-tasks.md) beschrieben.

## Einschränkungen beim Erstellen von Aufgaben

Wenn Sie den richtigen Zugriff und die richtigen Berechtigungen haben, können Sie Aufgaben für ein Projekt erstellen. In den folgenden Fällen können Sie jedoch möglicherweise keine Aufgaben erstellen:

* Ihr Adobe Workfront-Administrator oder ein Gruppenadministrator muss das Hinzufügen von Aufgaben zu einem Projekt aktivieren, das sich in Ihren Projektvoreinstellungen im Status Abgeschlossen oder Inaktiv befindet. Informationen zum Festlegen von Projektvoreinstellungen finden Sie [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Sie können keine Aufgaben zu einem Projekt hinzufügen, das sich in der Phase „Ausstehende Genehmigung“ befindet.

## Die maximal zulässige Anzahl von Aufgaben für ein Projekt

Ein Projekt kann bis zu 5.000 Aufgaben enthalten. Im Projekt wird eine Warnmeldung angezeigt, wenn Sie sich dem Limit nähern, wenn Sie das Limit erreicht haben und versuchen, es zu überschreiten.

Je nach der Anzahl der Aufgaben in Ihren Projekten, für die diese Begrenzung festgelegt wurde, kann Ihre Workfront-Instanz mehr als 5.000 Aufgaben in einem einzigen Projekt zulassen.

Wenn Sie mehr als 5.000 Aufgaben in ein Projekt einbeziehen können, beachten Sie Folgendes:

* Das Aufgabenlimit für Ihre Workfront-Umgebung ist auf die aktuelle Anzahl von Aufgaben in Ihrem größten Projekt plus zusätzliche 10 % festgelegt.

  Wenn beispielsweise ein Projekt in Ihrer Workfront-Instanz 10.000 Aufgaben enthält, beträgt das Limit für jedes Projekt in Ihrer Workfront-Instanz 11.000 Aufgaben.

* Kleinere Projekte verbessern die Leistung und minimieren Verwaltungsherausforderungen, die große Projekte begleiten.

## Standardwerte für Aufgaben beim Hinzufügen von Aufgaben zu einem Projekt

Es gibt zwei Arten von Standardinformationen, die von Workfront bei der Erstellung automatisch für Aufgaben aktualisiert werden:

* Standardinformationen auf Systemebene

  Ihr Workfront-Administrator oder ein Gruppenadministrator legt die Standardeinstellungen für Aufgaben auf Systemebene im Bereich Aufgaben und Probleme der Projektvoreinstellungen fest. Informationen zu Aufgaben- und Problemeinstellungen finden Sie [Konfigurieren von systemweiten Aufgaben- und Problemeinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md) oder [Konfigurieren von Aufgaben- und Problemeinstellungen für eine Gruppe](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

* Standardinformationen auf Projektebene

  Im Rest dieses Abschnitts werden die Standardeinstellungen auf Projektebene beschrieben, die Sie als Projekt-Manager für alle neuen Aufgaben definieren können, die einem Projekt hinzugefügt werden

Wenn Sie einem Projekt eine Aufgabe hinzufügen, hängt Workfront je nach Einrichtung des Projekts möglicherweise automatisch einen Genehmigungsprozess oder benutzerdefinierte Formulare an die Aufgabe an.

Informationen dazu, wie Sie ein Projekt so konfigurieren, dass diese standardmäßig hinzugefügt werden, finden Sie im Abschnitt „Aufgaben“ im Artikel [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

Beachten Sie beim Definieren von Standardinformationen, die mit Aufgaben verknüpft werden sollen, die einem Projekt auf Projektebene hinzugefügt werden:

* Sie müssen über Verwaltungsberechtigungen für das Projekt verfügen, um die Standardeinstellungen für den Aufgabengenehmigungsprozess und benutzerdefinierte Formulare zu definieren.
* Alle neuen Aufgaben werden mit dem Genehmigungsprozess erstellt und die benutzerdefinierten Formulare werden bei der Bearbeitung des Projekts definiert.
* Sie können diese Standardeinstellungen ändern, wenn Sie Aufgaben im Feld Aufgabe bearbeiten hinzufügen, aber nicht, wenn Sie Aufgaben in der Inline-Bearbeitung hinzufügen.
* Sie können den Validierungsprozess und die benutzerdefinierten Formulare für Aufgaben in einer Vorlage definieren.

   * Wenn ein Projekt über diese Vorlage erstellt wird, werden der Genehmigungsprozess und benutzerdefinierte Formulare automatisch auf das Projekt angewendet.
   * Wenn eine Vorlage an ein vorhandenes Projekt angehängt wird, behält das Projekt den ursprünglichen Aufgabengenehmigungsprozess und die benutzerdefinierten Formulareinstellungen bei, sofern sie definiert sind. Wenn sie nicht definiert sind, werden die Einstellungen aus der Vorlage zu den Einstellungen für das Projekt.
   * Wenn eine Vorlage an ein vorhandenes Projekt angehängt wird, behalten die Aufgaben, die dem Projekt über die Vorlage hinzugefügt werden, den Genehmigungsprozess und die benutzerdefinierten Formulareinstellungen bei, die sie für die Vorlage hatten, unabhängig von den Aufgabeneinstellungen für das Projekt.

  Informationen zum Anhängen einer Vorlage an ein Projekt finden Sie unter [Anhängen einer Vorlage an ein Projekt](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Wenn Sie das Projekt kopieren, werden die Standardeinstellungen der Aufgabe auf das neue Projekt übertragen.

  Informationen zum Kopieren eines Projekts finden Sie unter [Kopieren eines Projekts](../../../manage-work/projects/manage-projects/copy-project.md).

* Wenn Sie Aufgaben von einem Projekt in ein anderes kopieren und das Zielprojekt unterschiedliche Standardeinstellungen für Aufgaben hat, behalten die kopierten Aufgaben die Standardeinstellungen des ursprünglichen Projekts bei, es sei denn, sie werden beim Kopieren gelöscht.
* Wenn Sie eine Aufgabe im selben Projekt duplizieren, werden die benutzerdefinierten Formulare und der Genehmigungsprozess an die doppelte Aufgabe übertragen.

  Informationen zum Kopieren und Duplizieren von Aufgaben finden Sie unter [Aufgaben kopieren und duplizieren](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).

* Wenn Sie die Aufgabe in ein anderes Projekt verschieben, werden die Standardaufgabeneinstellungen für die Aufgaben aus dem ursprünglichen Projekt gespeichert, unabhängig von den standardmäßigen Aufgabeneinstellungen für das neue Projekt.

  Informationen zum Verschieben von Aufgaben finden Sie unter [Aufgaben verschieben](../../../manage-work/tasks/manage-tasks/move-tasks.md).

* Wenn Ihr Unternehmen sowohl den alten Workfront- als auch den Adobe-Cloud-Speicher verwendet, können Sie keine Aufgaben zwischen Projekten verschieben oder kopieren, die unterschiedliche Speichertypen verwenden.

  Weitere Informationen finden Sie unter [Übersicht über das Dokumentenmanagement für Projekte und zugehörige Objekte](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md).
