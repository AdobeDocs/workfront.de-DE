---
product-area: templates
navigation-topic: templates-navigation-topic
title: Überblick über Projektvorlagen
description: Sie können Projektvorlagen verwenden, um die meisten wiederholbaren Prozesse, Informationen und Einstellungen zu erfassen, die mit den Projekten in Ihrer Organisation verbunden sind.
author: Alina
feature: Work Management
exl-id: cac7662f-f2ae-44f0-a0bb-1569c03d172e
TQID: https://experienceleague.adobe.com/9RlRNqkZYIcLjI5-he3f2BMtoXj3R--8MQbVUFmRHqI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87effid: d87de1f9-8e24-4c4d-aa4c-a403075091a1id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 702
ht-degree: 5%

---

# Überblick über Projektvorlagen

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
   * [Überblick über die Projektdauer](../../../manage-work/projects/planning-a-project/project-duration.md)

  Informationen zu den geplanten Stunden finden Sie unter [Überblick über geplante Stunden](../../../manage-work/tasks/task-information/planned-hours.md).

* Fügen Sie die Vorgängerbeziehungen zwischen den Aufgaben ganz am Ende hinzu, wenn Sie über ein klares Verständnis des zukünftigen Projektplans in seiner Gesamtheit verfügen. Das Hinzufügen von Vorgängern zu Vorlagenaufgaben ähnelt dem Hinzufügen von Vorgängern zu Aufgaben in einem Projekt.

  Informationen zum Hinzufügen von Vorgängern zu Aufgaben finden Sie unter [Übersicht über Aufgabenvorgänger](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

* Geben Sie an, für wen die Vorlage zur späteren Verwendung freigegeben werden soll und für wen die aus der Vorlage erstellten Projekte freigegeben werden sollen. Informationen zum Freigeben von Vorlagen finden Sie unter [Freigeben von Projektvorlagen](../../../manage-work/projects/create-and-manage-templates/share-project-template.md).
* Verwenden Sie globale Genehmigungsprozesse und fügen Sie sie nach Möglichkeit zu Ihren Vorlagen- und Vorlagenaufgaben hinzu. Dadurch wird Zeit gespart, wenn für Aufgaben oder das zukünftige Projekt dieselben Genehmigungen erforderlich sind.

  Informationen zum Erstellen von Genehmigungen finden Sie [Genehmigungsprozess für Arbeitselemente erstellen](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  Informationen zum Verknüpfen eines Genehmigungsprozesses mit einem Arbeitselement finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeit](../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

* Entscheiden Sie, welchen Dokumentspeicher Sie für Ihre zukünftigen Projekte verwenden möchten. Einige Organisationen haben Zugriff auf die folgenden Dokumentspeichertypen:

   * Legacy Workfront-Speicher
   * Cloud-Speicherplatz von Adobe

  Das Hinzufügen von Dokumenten unterscheidet sich je nach ausgewähltem Speichertyp. Der Speichertyp, den Sie für Ihre Vorlagen auswählen, wirkt sich auf den Speichertyp aus, den zukünftige Projekte erben.

  Das Hinzufügen von Vorlagen zu vorhandenen Projekten wirkt sich nicht auf den Speichertyp des Projekts aus.

  Weitere Informationen finden Sie auch unter:

   * [Erstellen einer Projektvorlage](/help/quicksilver/manage-work/projects/create-and-manage-templates/create-template.md)
   * [Übersicht über das Dokumentenmanagement für Projekte und zugehörige Objekte](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md)

## Möglichkeiten zum Erstellen von Vorlagen

Sie können eine neue Vorlage wie folgt erstellen:

* Von Grund auf.\
  Weitere Informationen zum Erstellen einer neuen Vorlage von Grund auf finden Sie unter [Erstellen einer Projektvorlage](../../../manage-work/projects/create-and-manage-templates/create-template.md).

* Aus vorhandenen Projekten durch Speichern eines Projekts als Vorlage.\
  Weitere Informationen zum Erstellen von Vorlagen aus vorhandenen Projekten finden Sie unter [Vorlage aus Projekt erstellen](../../../manage-work/projects/create-and-manage-templates/create-template-from-project.md).

* Durch Kopieren aus einer anderen Vorlage.\
  Weitere Informationen zum Kopieren einer vorhandenen Vorlage finden Sie unter [Kopieren einer ](../../../manage-work/projects/create-and-manage-templates/copy-template.md)).

* Mithilfe unserer Beispielvorlagen.\
  Weitere Informationen zum Erstellen Ihrer Vorlagen mithilfe unserer Beispielvorlagen finden Sie unter [Erstellen von Projektvorlagen aus Beispielen](../../../manage-work/projects/create-and-manage-templates/create-templates-from-examples.md).
