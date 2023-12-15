---
product-area: templates
navigation-topic: templates-navigation-topic
title: Übersicht über Projektvorlagen
description: Sie können Projektvorlagen verwenden, um die meisten wiederholbaren Prozesse, Informationen und Einstellungen zu erfassen, die mit den Projekten in Ihrer Organisation verbunden sind.
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
source-git-commit: ca4da5302198d8fffc8b706baa3b3aeaa1f738e3
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 1%

---

# Übersicht über Projektvorlagen

<!-- Audited: 12/2023 -->

Sie können Projektvorlagen verwenden, um die meisten wiederholbaren Prozesse, Informationen und Einstellungen zu erfassen, die mit den Projekten in Ihrer Organisation verbunden sind.

Sie können Aufgaben, Warteschlangenthemen, benutzerdefinierte Formulare und Dokumente in Ihrer Vorlage definieren.

Nach dem Erstellen von Vorlagen können Sie diese an bestehende Projekte anhängen oder sie zum Erstellen neuer Projekte verwenden. Alle Informationen auf der Vorlage werden an die Projekte übermittelt, die mit der Vorlage erstellt werden.

## Vorteile der Verwendung von Vorlagen in Adobe Workfront

Im Folgenden finden Sie einige Vorteile der Verwendung von Vorlagen zum Erstellen Ihrer Projekte:

* Dadurch sparen Sie Zeit und Mühe bei der Erstellung von sich wiederholenden neuen Projekten.
* Sie verfügen über konsistente Informationen für alle Projekte, die im Umfang ähnlich sind.
* Dies ist hilfreich bei der Berichterstellung zu Projekten. Sie können beispielsweise Berichte zu Projekten erstellen, die dieselbe Vorlage verwenden, um ihren Fortschritt zu vergleichen und Verbesserungen hinsichtlich des Abschlusses zu finden.
* Zusätzlich zur Definition der zukünftigen Projekteinstellungen können Sie die folgenden Informationen für das zukünftige Projekt zu einer Vorlage hinzufügen:

   * Aufgaben
   * Dokumente
   * Genehmigungen
   * Warteschlangendetails
   * Warteschlangenthemen
   * Themengruppen
   * Routing-Regeln
   * Benutzerdefinierte Forms
   * Firmen- und Gruppeninformationen

## Best Practices zum Erstellen von Vorlagen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is not an extensive list, but we are updating it as we go.)</p>
-->

Beachten Sie beim Erstellen von Vorlagen Folgendes:

* Weisen Sie keine Benutzer Vorlagenaufgaben zu. Obwohl Sie die Aufgaben nicht zuweisen können, wird empfohlen, Aufgaben Auftragsrollen zuzuweisen. Auf diese Weise erhalten Sie eine Vorstellung davon, welche Benutzer den Aufgaben zugewiesen werden können, wenn Sie das Projekt mithilfe der Vorlage erstellen.
* Geben Sie Ihren Vorlagenaufgaben immer den Wert Dauer und Geplante Stunden . Jede Aufgabe im Projekt sollte mit einer Dauer verknüpft sein, in der die Aufgabe geöffnet bleiben kann, sowie mit einem Wert für die geplante Stunde, innerhalb derer die Aufgabe tatsächlich abgeschlossen werden muss. Aufgaben ohne diese Informationen können bei der Verwendung von Tools zur Ressourcenverwaltung in Workfront nicht ordnungsgemäß für Ressourcen budgetiert werden.

  Weitere Informationen zur Dauer finden Sie in den folgenden Artikeln:

   * [Übersicht über Aufgabendauer und -dauer](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Übersicht über die Projektdauer](../../../manage-work/projects/planning-a-project/project-duration.md)

  Weitere Informationen zu geplanten Stunden finden Sie unter [Übersicht über geplante Stunden](../../../manage-work/tasks/task-information/planned-hours.md).

* Fügen Sie die Vorgängerbeziehungen zwischen den Aufgaben am Ende hinzu, wenn Sie ein klares Verständnis des zukünftigen Projektplans in seiner Gesamtheit haben. Das Hinzufügen von Vorgängern zu Vorlagenaufgaben ähnelt dem Hinzufügen von Vorgängern zu Aufgaben in einem Projekt.

  Informationen zum Hinzufügen von Vorgängern zu Aufgaben finden Sie unter [Übersicht über die Vorgänger von Aufgaben](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Geben Sie an, für wen die Vorlage freigegeben werden soll und für wen die Projekte, die aus der Vorlage erstellt werden, freigegeben werden sollen. Informationen zum Freigeben von Vorlagen finden Sie unter [Projektvorlagen freigeben](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* Verwenden Sie globale Validierungsprozesse und fügen Sie sie nach Möglichkeit zu Ihren Vorlagen- und Vorlagenaufgaben hinzu. Dies spart Zeit, wenn Aufgaben oder das zukünftige Projekt dieselben Genehmigungen durchlaufen müssen.

  Informationen zum Erstellen von Genehmigungen finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  Informationen zum Verknüpfen eines Genehmigungsprozesses mit einem Arbeitselement finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Methoden zum Erstellen von Vorlagen

Sie können eine neue Vorlage wie folgt erstellen:

* Von Grund auf neu.\
  Weitere Informationen zum Erstellen einer neuen Vorlage finden Sie unter [Erstellen einer Projektvorlage](../../../manage-work/projects/create-and-manage-templates/create-template.md).

* Aus vorhandenen Projekten durch Speichern eines Projekts als Vorlage.\
  Weitere Informationen zum Erstellen von Vorlagen aus vorhandenen Projekten finden Sie unter [Vorlage aus Projekt erstellen](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md).

* durch Kopieren aus einer anderen Vorlage.\
  Weitere Informationen zum Kopieren einer vorhandenen Vorlage finden Sie unter [Kopieren einer Projektvorlage](../../../manage-work/projects/create-and-manage-templates/copy-template.md).

* Mithilfe unserer Beispielvorlagen.\
  Weitere Informationen zum Erstellen Ihrer Vorlagen mithilfe unserer Beispielvorlagen finden Sie unter [Erstellen von Projektvorlagen aus Beispielen](../../../manage-work/projects/create-and-manage-templates/create-templates-from-examples.md).
