---
product-area: templates
navigation-topic: templates-navigation-topic
title: Entfernen von Vorlageninformationen aus einem Projekt
description: Sie können eine Vorlage nicht aus einem Projekt entfernen. Sie können Informationen, die zum Projekt hinzugefügt wurden, nur manuell entfernen, nachdem eine Vorlage an das Projekt angehängt wurde. Weitere Informationen zum Anhängen von Vorlagen finden Sie unter Anhängen einer Vorlage an ein Projekt.
author: Alina
feature: Work Management
exl-id: a8b6055a-7fac-4f9b-a880-10b2b85299b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '452'
ht-degree: 1%

---

# Entfernen von Vorlageninformationen aus einem Projekt

Sie können eine Vorlage nicht aus einem Projekt entfernen. Sie können Informationen, die zum Projekt hinzugefügt wurden, nur manuell entfernen, nachdem eine Vorlage an das Projekt angehängt wurde. Informationen zum Anhängen von Vorlagen finden Sie unter [Anhängen einer Vorlage an ein Projekt](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriff auf Aufgaben verwalten </p> <p>Contribute-Zugriff oder höher </p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Optionen zum Entfernen von Vorlageninformationen aus einem Projekt

Um Vorlageninformationen zu entfernen, die zum Projekt hinzugefügt wurden, führen Sie einen der folgenden Schritte aus:

* Entfernen Sie Informationen manuell aus dem Projekt, nachdem die Vorlage angehängt wurde.

  Weitere Informationen finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

* Löschen Sie die Aufgaben im Projekt, die mit der Vorlage hinzugefügt wurden.

  Weitere Informationen finden Sie im Abschnitt [Aufgaben löschen, die aus einer Vorlage erstellt wurden](#delete-tasks-created-from-a-template) in diesem Artikel.

* Löschen Sie die Vorlage aus Workfront. Durch das Löschen der Vorlage aus Workfront werden die aus der Vorlage hinzugefügten Aufgaben nicht aus den Projekten gelöscht.

  Weitere Informationen finden Sie unter [Löschen von Projektvorlagen](../../../manage-work/projects/create-and-manage-templates/delete-templates.md).

## Löschen von Aufgaben, die aus einer Vorlage erstellt wurden {#delete-tasks-created-from-a-template}

1. Wechseln Sie zum Abschnitt **Aufgaben** des Projekts.
1. Führen Sie einen der folgenden Schritte aus:

   * Erstellen Sie einen Filter für die Aufgabenliste, um nur Aufgaben anzuzeigen, die aus einer Vorlage mit der folgenden Anweisung erstellt wurden:

     ```
     Task >> Template Task ID >>Is Not Blank
     ```

     Informationen zum Erstellen eines Filters finden Sie unter [Erstellen oder Bearbeiten von Filtern in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md).

     Wenn Sie den Filter anwenden, werden nur Aufgaben in der Liste angezeigt, die mit einer Vorlagenaufgaben-ID verknüpft sind.

   * Erstellen Sie eine Ansicht für die Aufgabenliste, um die Felder **Vorlagenaufgaben-ID** oder **VorlagenAufgabenname** in einer Spalte anzuzeigen.

     Wenn Sie die Ansicht anwenden, wurden die Aufgaben, die Informationen in der Spalte &quot;Template Task ID&quot;oder &quot;Template Task Name&quot;enthalten, mithilfe einer Vorlage erstellt.

     Informationen zum Erstellen einer Ansicht finden Sie unter [Übersicht über Ansichten in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. Wählen Sie alle Aufgaben aus, die in Schritt 2 anhand einer Vorlage identifiziert wurden, und klicken Sie dann auf **das Löschsymbol***> Ja, löschen Sie es**. Weitere Informationen finden Sie unter [Aufgaben löschen](../../../manage-work/tasks/manage-tasks/delete-tasks.md).
