---
product-area: templates
navigation-topic: templates-navigation-topic
title: Projektvorlage - Übersicht
description: Sie können Projektvorlagen verwenden, um die meisten wiederholbaren Prozesse, Informationen und Einstellungen zu erfassen, die mit den Projekten in Ihrer Organisation verbunden sind.
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '613'
ht-degree: 2%

---

# Projektvorlage - Übersicht

<!-- Audited: 12/2023 -->

Sie können Projektvorlagen verwenden, um die meisten wiederholbaren Prozesse, Informationen und Einstellungen zu erfassen, die mit den Projekten in Ihrer Organisation verbunden sind.

Sie können Aufgaben, Warteschlangenthemen und benutzerdefinierte Formulare definieren und Dokumente in Ihrer Vorlage anhängen.

Nach dem Erstellen von Vorlagen können Sie sie an vorhandene Projekte anhängen oder zum Erstellen neuer Projekte verwenden. Alle Informationen über die Vorlage werden in die Projekte übertragen, die damit erstellt werden.

## Vorteile der Verwendung von Vorlagen in Adobe Workfront

Im Folgenden finden Sie einige Vorteile der Verwendung von Vorlagen zum Erstellen Ihrer Projekte:

* Dadurch sparen Sie Zeit und Mühe bei der Erstellung neuer Projekte, die sich wiederholen.
* Sie verfügen über konsistente Informationen in Projekten mit ähnlichem Umfang.
* Dies ist hilfreich bei der Berichterstellung über Projekte. Sie können beispielsweise Berichte zu Projekten erstellen, die dieselbe Vorlage verwenden, um ihren Fortschritt zu vergleichen und Verbesserungen bei der Durchführung zu finden.
* Zusätzlich zur Definition der zukünftigen Projekteinstellungen können Sie einer Vorlage die folgenden Informationen für das zukünftige Projekt hinzufügen:

   * Aufgaben
   * Dokumente
   * Genehmigungen
   * Warteschlangendetails
   * Warteschlangenthemen
   * Themengruppen
   * Routing-Regeln
   * Benutzerdefinierte Formulare
   * Unternehmens- und Gruppeninformationen

## Best Practices für die Erstellung von Vorlagen

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:this is not an extensive list, but we are updating it as we go.)</p>
-->

Beachten Sie beim Erstellen von Vorlagen Folgendes:

* Keine Benutzer Vorlagenaufgaben zuweisen. Obwohl Sie die Zuweisung von Aufgaben aufheben können, empfehlen wir Ihnen, Aufgabengebiete zuzuweisen. Auf diese Weise können Sie sich ein Bild davon machen, welche Benutzer den Aufgaben zugewiesen werden können, wenn Sie das Projekt mithilfe der Vorlage erstellen.
* Geben Sie für Vorlagenaufgaben immer die Werte Dauer und Geplante Stunden an. Jede Aufgabe im Projekt sollte einer Dauer zugeordnet werden, wie lange die Aufgabe offen bleiben kann, sowie einem Wert für „Geplante Stunde“, wie lange die Aufgabe tatsächlich dauert. Aufgaben ohne diese Informationen können bei der Verwendung von Ressourcenverwaltungstools in Workfront nicht ordnungsgemäß für Ressourcen budgetiert werden.

  Informationen zur Dauer finden Sie in den folgenden Artikeln:

   * [Übersicht über die Aufgabendauer und den Dauertyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Übersicht über die Projektdauer](../../../manage-work/projects/planning-a-project/project-duration.md)

  Informationen zu den geplanten Stunden finden Sie unter [Übersicht über die geplanten Stunden](../../../manage-work/tasks/task-information/planned-hours.md).

* Fügen Sie die Vorgängerbeziehungen zwischen den Aufgaben ganz am Ende hinzu, wenn Sie über ein klares Verständnis des zukünftigen Projektplans in seiner Gesamtheit verfügen. Das Hinzufügen von Vorgängern zu Vorlagenaufgaben ähnelt dem Hinzufügen von Vorgängern zu Aufgaben in einem Projekt.

  Informationen zum Hinzufügen von Vorgängern zu Aufgaben finden Sie unter [Übersicht über Aufgabenvorgänger](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Geben Sie an, für wen die Vorlage zur späteren Verwendung freigegeben werden soll und für wen die aus der Vorlage erstellten Projekte freigegeben werden sollen. Informationen zum Freigeben von Vorlagen finden Sie unter [Freigeben von Projektvorlagen](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* Verwenden Sie globale Genehmigungsprozesse und fügen Sie sie nach Möglichkeit zu Ihren Vorlagen- und Vorlagenaufgaben hinzu. Dadurch wird Zeit gespart, wenn für Aufgaben oder das zukünftige Projekt dieselben Genehmigungen erforderlich sind.

  Informationen zum Erstellen von Genehmigungen finden Sie [Genehmigungsprozess für Arbeitselemente erstellen](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  Informationen zum Verknüpfen eines Genehmigungsprozesses mit einem Arbeitselement finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Möglichkeiten zum Erstellen von Vorlagen

Sie können eine neue Vorlage wie folgt erstellen:

* Von Grund auf.\
  Weitere Informationen zum Erstellen einer neuen Vorlage von Grund auf finden Sie unter [Erstellen einer Projektvorlage](../../../manage-work/projects/create-and-manage-templates/create-template.md).

* Aus vorhandenen Projekten durch Speichern eines Projekts als Vorlage.\
  Weitere Informationen zum Erstellen von Vorlagen aus vorhandenen Projekten finden Sie unter [Vorlage aus Projekt erstellen](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md).

* Durch Kopieren aus einer anderen Vorlage.\
  Weitere Informationen zum Kopieren einer vorhandenen Vorlage finden Sie unter [Kopieren einer &#x200B;](../../../manage-work/projects/create-and-manage-templates/copy-template.md)).

* Mithilfe unserer Beispielvorlagen.\
  Weitere Informationen zum Erstellen Ihrer Vorlagen mithilfe unserer Beispielvorlagen finden Sie unter [Erstellen von Projektvorlagen aus Beispielen](../../../manage-work/projects/create-and-manage-templates/create-templates-from-examples.md).
