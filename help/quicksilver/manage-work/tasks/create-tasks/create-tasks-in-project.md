---
product-area: projects
navigation-topic: create-tasks
title: Erstellen von Aufgaben in einem Projekt
description: Sie können Aufgaben in einem Projekt erst erstellen, nachdem Sie das Projekt erstellt haben.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 96f80e7b-6ad5-40ae-861d-8d97c570f2ac
source-git-commit: 1e69d715f343bfef1e5aee658a1dff12abfc61a0
workflow-type: tm+mt
source-wordcount: '959'
ht-degree: 1%

---

# Erstellen von Aufgaben in einem Projekt

<!-- Audited: 10/2024 -->

Sie können Aufgaben in Adobe Workfront wie folgt erstellen:

* Erstellen Sie eine Aufgabe in einem Projekt von Grund auf neu, nachdem das Projekt erstellt wurde.

  Nach der Erstellung eines Projekts können Sie Aufgaben hinzufügen und ändern, um den Projektplan zu organisieren. Weitere Informationen zum Erstellen eines Projekts finden Sie unter [Erstellen eines Projekts](../../../manage-work/projects/create-projects/create-project.md).

* Erstellen Sie Aufgaben durch Hinzufügen einer Vorlage zu einem Projekt.

  Weitere Informationen finden Sie unter [Anhängen einer Vorlage an ein Projekt](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

* Erstellen Sie persönliche Aufgaben und verschieben Sie sie in ein Projekt.

  Sie können persönliche Aufgaben erstellen, indem Sie einen der folgenden Schritte ausführen:

   * Erstellen einer Ad-hoc-Arbeitserforderung und Senden an einen Benutzer
   * Erstellen eines zu erledigenden Elements im Bereich &quot;Home&quot;

  Informationen zum Erstellen persönlicher Aufgaben, die sich nicht auf ein Projekt beziehen, finden Sie unter [Persönliche Aufgaben erstellen](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md).

  Sie können persönliche Aufgaben in ein Projekt verschieben und sie werden zu Arbeitsaufgaben.

In diesem Artikel wird beschrieben, wie Sie Aufgaben von Grund auf neu erstellen und persönliche Aufgaben in ein Projekt verschieben können.

Sie können Aufgaben auch wie folgt erstellen:

* Durch Kopieren oder Duplizieren vorhandener Aufgaben. Weitere Informationen finden Sie unter [Kopieren und Duplizieren von Aufgaben](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* durch Verschieben von Aufgaben von einem Projekt in ein anderes. Weitere Informationen finden Sie unter [Verschieben von Aufgaben](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront-Lizenz</p> </td> 
   <td><p>Aktuell: Arbeit oder höher</p> 
   Oder
   <p>Neu: Standard</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Contribute-Berechtigungen für das Projekt mit der Möglichkeit, Aufgaben hinzuzufügen oder höher</p> <p>Wenn Sie eine Aufgabe erstellen, erhalten Sie automatisch Verwaltungsberechtigungen für die Aufgabe</p> <p> Weitere Informationen zu Aufgabenberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Aufgabe freigeben </a>. </p> <p>Informationen zum Anfordern zusätzlicher Berechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen von Aufgaben in einem Projekt

1. Wechseln Sie zu dem Projekt, in dem Sie eine Aufgabe erstellen möchten.
1. Klicken Sie im linken Bereich auf **Aufgaben** .
1. (Bedingt) Wenn Sie die Aufgabenliste derzeit in einer agilen Ansicht anzeigen, klicken Sie oben rechts auf das Symbol **Listenansicht** ![](assets/list-view-in-agile-view-for-tasks.png) , um die Aufgabenliste anzuzeigen.
1. (Optional) Klicken Sie auf das Symbol &quot;**Planmodus**&quot;![](assets/nwe-plan-mode-icon-task-list.png) und wählen Sie &quot;**Manuelles Speichern**&quot;. Wählen Sie dann entweder &quot;**Standard**&quot;oder &quot;**Timeline-Planung**&quot;. Dadurch wird die standardmäßig aktivierte Option **Autosave** deaktiviert.

   ![Manuelles Speichern auswählen](assets/manual-save-option.png)

   >[!TIP]
   >
   >Sie können Ihre Änderungen rückgängig machen, wenn Sie Manuelles Speichern auswählen.

1. Erstellen Sie eine neue Aufgabe, indem Sie einen der folgenden Schritte ausführen:

   * Klicken Sie oben in der Aufgabenliste auf **Neue Aufgabe** .
   * Klicken Sie unten in der Aufgabenliste auf **Weitere Aufgaben hinzufügen** .

   ![](assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png)

1. (Bedingt) Wenn Sie auf **Neue Aufgabe** geklickt haben, gehen Sie wie folgt vor:

   1. Geben Sie eines der Felder in der beschränkten Liste von Feldern im Feld **Neue Aufgabe** an und klicken Sie dann auf **Aufgabe erstellen** , wenn Sie eine Aufgabe schnell erstellen möchten.

      Oder

      Um alle Felder für die Aufgabe zu aktualisieren, klicken Sie auf **Mehr Optionen** , um das Feld **Aufgabe erstellen** zu öffnen.

      ![](assets/nwe-create-task-small-screen-350x272.png)

      Das Feld **Aufgabe erstellen** wird geöffnet.

      ![](assets/create-task-larger-box-nwe-350x244.png)

       

      >[!NOTE]
      >
      >Je nachdem, wie Ihr Workfront-Administrator unsere Layoutvorlage eingerichtet hat, werden in den Feldern im Feld &quot;Aufgabe erstellen&quot;möglicherweise verschiedene Felder in Ihrer Umgebung angezeigt. Weitere Informationen finden Sie unter [Anpassen der Detailansicht mithilfe einer Layoutvorlage](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   1. Geben Sie Informationen für die folgenden Bereiche im linken Bereich des Felds Aufgabe erstellen an:

      * Aufgabenname
      * Übersicht
      * Arbeitsaufträge
      * Benutzerdefinierte Formulare
      * Finanzielle Details
      * Einstellungen

        Informationen zum Definieren aller Aufgabenfelder für eine Aufgabe finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   1. (Bedingt und optional) Wenn die Aufgabe wiederkehrend sein soll, aktualisieren Sie das Feld **Häufigkeit der Wiederholung** . Weitere Informationen zum Erstellen wiederkehrender Aufgaben finden Sie unter [Erstellen wiederkehrender Aufgaben](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).
   1. (Optional) Klicken Sie im linken Bereich auf **Dokumente** , um ein Dokument an die neue Aufgabe anzuhängen, und klicken Sie dann auf **Dateien hinzufügen oder verknüpfen** , um ein Dokument von Ihrem Computer oder einem anderen Dienst zur Aufgabe hinzuzufügen oder Dokumente und Ordner von Ihrem Computer oder einem anderen Dienst zu verknüpfen.

1. (Bedingt) Wenn Sie in Schritt 5 auf &quot;**Weitere Aufgaben hinzufügen**&quot;geklickt haben, geben Sie die Aufgabeninformationen über die Inline-Bearbeitung ein und drücken Sie die Eingabetaste.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this stays accurate)</p>
   -->

   Es wird empfohlen, diese Option insbesondere beim Hinzufügen mehrerer Aufgaben zur Liste zu verwenden.

   ![](assets/add-more-tasks-inline.png)

1. (Bedingt) Führen Sie einen der folgenden Schritte aus:

   * Wenn Sie in Schritt 5 auf **Neue Aufgabe** geklickt haben, klicken Sie auf **Aufgabe erstellen** , um Ihre Änderungen zu speichern und die neue Aufgabe zu Ihrem Projekt hinzuzufügen.

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?)</p>   
     -->

   * Wenn Sie in Schritt 5 auf **Weitere Aufgaben hinzufügen** geklickt haben, gehen Sie wie folgt vor:

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?) </p>   
     -->

      1. Klicken Sie auf eine beliebige Stelle im Browser, um Ihre Änderungen zu senden, oder drücken Sie die Eingabetaste.
      1. (Optional) Wählen Sie in der Aufgabenliste die neu erstellte Aufgabe aus und klicken Sie dann auf **Einzug**.

         Dadurch wird die neue Aufgabe zu einer untergeordneten Aufgabe oder Unteraufgabe der vorherigen Aufgabe.

         Weitere Informationen zu untergeordneten Aufgaben finden Sie unter [Unteraufgaben erstellen](/help/quicksilver/manage-work/tasks/create-tasks/create-subtasks.md).

      1. (Bedingt) Wenn Sie die Option **Autosave** nach dem Drücken von **Add More Tasks** deaktiviert haben, können Sie Folgendes tun:

         * Klicken Sie jederzeit auf **Rückgängig** , um Ihre letzte Änderung rückgängig zu machen, oder auf **Abbrechen** , um alle Änderungen rückgängig zu machen, die Sie an der Aufgabenliste vorgenommen haben.
         * Wenn Sie zuvor auf **Rückgängig** geklickt haben, klicken Sie auf **Wiederholen** , um die letzte Änderung, die Sie abgebrochen haben, erneut anzuwenden.
         * Klicken Sie auf **Speichern** , um Ihre Änderungen in der Aufgabenliste zu speichern.

## Erstellen von Aufgaben durch Verschieben einer persönlichen Aufgabe in ein Projekt

1. (Bedingt) Stellen Sie sicher, dass Sie oder andere Benutzer persönliche Aufgaben erstellt haben.

   Weitere Informationen finden Sie unter [Persönliche Aufgaben erstellen](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md).
1. Erstellen Sie einen Filter für persönliche Aufgaben und wenden Sie ihn auf einen Aufgabenbericht oder eine Aufgabenliste an.

   Weitere Informationen finden Sie unter [Filter: persönliche Aufgaben](/help/quicksilver/reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-personal-tasks.md).

   ![](assets/personal-tasks-report.png)
1. Klicken Sie auf einen Aufgabennamen im Bericht &quot;Persönliche Aufgabe&quot;, um ihn zu öffnen.

   Workfront speichert persönliche Aufgaben in einem nicht aufgelisteten persönlichen Projekt, das immer nach folgendem Muster benannt ist: &quot;&lt; vollständiger Name des Benutzers > Aufgaben des Benutzers. Beispielsweise könnte ein persönliches Projekt &quot;Rick&#39;s Tasks&quot;heißen.

1. Klicken Sie auf der Aufgabenseite auf das Menü **Mehr** ![](assets/more-icon.png) und dann auf **Verschieben**. Weitere Informationen zum Verschieben von Aufgaben finden Sie unter [Verschieben von Aufgaben](/help/quicksilver/manage-work/tasks/manage-tasks/move-tasks.md).

   Nachdem Sie die Aufgabe abgeschlossen haben, wird die Aufgabe im ausgewählten Projekt angezeigt. Die Timeline des Projekts kann von der Timeline der neuen Aufgabe betroffen sein.
