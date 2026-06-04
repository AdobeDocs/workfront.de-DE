---
product-area: templates
navigation-topic: templates-navigation-topic
title: Entfernen von Vorlageninformationen aus einem Projekt
description: Sie können keine Vorlage aus einem Projekt entfernen. Sie können nur manuell Informationen entfernen, die dem Projekt hinzugefügt wurden, nachdem eine Vorlage an das Projekt angehängt wurde. Informationen zum Anhängen von Vorlagen finden Sie unter Anhängen einer Vorlage an ein Projekt.
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/YGb9LSybhejKxNYvxqiw7pcGD5f8p-2BqXbHU1OHEFc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 395
ht-degree: 11%

---

# Entfernen von Vorlageninformationen aus einem Projekt

Sie können keine Vorlage aus einem Projekt entfernen. Sie können nur manuell Informationen entfernen, die dem Projekt hinzugefügt wurden, nachdem eine Vorlage an das Projekt angehängt wurde. Informationen zum Anhängen von Vorlagen finden Sie unter [Anhängen einer Vorlage an ein Projekt](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p>
   <p>Work oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben bearbeiten</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf Aufgaben verwalten </p> <p>Beitragen oder höherer Zugriff auf das Projekt</p>  </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to tasks </p> <p>Contribute or higher access to the project </p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## Optionen zum Entfernen von Vorlageninformationen aus einem Projekt

Um Vorlageninformationen zu entfernen, die dem Projekt hinzugefügt wurden, haben Sie folgende Möglichkeiten:

* Informationen manuell aus dem Projekt entfernen, nachdem die Vorlage angehängt wurde.

  Weitere Informationen finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

* Löscht die Aufgaben im Projekt, die mit der Vorlage hinzugefügt wurden.

  Weitere Informationen finden Sie [ Abschnitt „Löschen von Aufgaben, die aus einer Vorlage ](#delete-tasks-created-from-a-template) wurden“ in diesem Artikel.

* Löschen Sie die Vorlage aus Workfront. Beim Löschen der Vorlage aus Workfront werden die aus der Vorlage hinzugefügten Aufgaben nicht aus den Projekten gelöscht.

  Weitere Informationen finden Sie unter [Projektvorlagen löschen](../../../manage-work/projects/create-and-manage-templates/delete-templates.md).

## Aus einer Vorlage erstellte Aufgaben löschen {#delete-tasks-created-from-a-template}

1. Gehen Sie zum **Aufgaben** des Projekts.
1. Führen Sie einen der folgenden Schritte aus:

   * Erstellen Sie einen Filter für die Aufgabenliste, um nur Aufgaben anzuzeigen, die aus einer Vorlage mit der folgenden Anweisung erstellt wurden:

     ```
     Task >> Template Task ID >>Is Not Blank
     ```

     Informationen zum Erstellen eines Filters finden Sie unter [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

     Wenn Sie den Filter anwenden, werden in der Liste nur Aufgaben angezeigt, die mit einer Vorlagenaufgaben-ID verknüpft sind.

   * Erstellen Sie eine Ansicht für die Aufgabenliste, um die Felder **Vorlagenaufgabe-ID** oder **Vorlagenaufgabenname** in einer Spalte anzuzeigen.

     Wenn Sie die Ansicht anwenden, wurden die Aufgaben, die Informationen in der Spalte Vorlagenaufgaben-ID oder Vorlagenaufgabenname enthalten, mithilfe einer Vorlage erstellt.

     Weitere Informationen zum Erstellen einer Ansicht finden Sie unter [Ansichten - Übersicht in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Wählen Sie alle in Schritt 2 als aus einer Vorlage erstellt identifizierten Aufgaben aus und klicken Sie dann auf **Löschsymbol**> **, Löschen**. Weitere Informationen finden Sie unter [Aufgaben löschen](../../../manage-work/tasks/manage-tasks/delete-tasks.md).
