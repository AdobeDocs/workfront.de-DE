---
product-area: projects
navigation-topic: create-tasks
title: Erstellen von Aufgaben in einem Projekt
description: Sie können Aufgaben in einem Projekt erst erstellen, nachdem Sie das Projekt erstellt haben.
author: Alina
feature: Work Management, Tasks
role: User
exl-id: 96f80e7b-6ad5-40ae-861d-8d97c570f2ac
source-git-commit: 4a4efe7d8a354bc9ec22a607fe6e75040e7cca24
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 1%

---

# Erstellen von Aufgaben in einem Projekt

Sie können Aufgaben in einem Projekt erst erstellen, nachdem Sie das Projekt erstellt haben.

Beispielsweise können Sie nach der Erstellung eines Projekts Aufgaben hinzufügen und ändern, um den Projektplan zu organisieren. Weitere Informationen zum Erstellen eines Projekts finden Sie unter [Projekt erstellen](../../../manage-work/projects/create-projects/create-project.md).

Informationen zum Erstellen persönlicher Aufgaben, die sich nicht in einem Projekt befinden, finden Sie im Abschnitt &quot;Erstellen einer persönlichen Aufgabe&quot;im Artikel [Erstellen von Arbeitselementen aus dem Startbereich](../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

In diesem Artikel wird beschrieben, wie Sie Aufgaben von Grund auf neu erstellen. Sie können Aufgaben auch wie folgt erstellen:

* Durch Kopieren oder Duplizieren vorhandener Aufgaben. Weitere Informationen finden Sie unter [Aufgaben kopieren und duplizieren](../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md).
* durch Verschieben von Aufgaben von einem Projekt in ein anderes. Weitere Informationen finden Sie unter [Aufgaben verschieben](../../../manage-work/tasks/manage-tasks/move-tasks.md).

## Zugriffsanforderungen

<!--drafted for P&P - replace the table:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront license*</p> </td> 
   <td><p>Current license: Standard</p> 
   Or
   <p>Legacy license: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to tasks, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Grant access to tasks</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project with ability to Add Tasks or higher</p> <p>When you create a task you automatically receive Manage permissions to the task</p> <p> For information about task permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Share a task </a>. </p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Adobe Workfront-Lizenz*</p> </td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen zum Zugriff auf Aufgaben finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md" class="MCXref xref">Zugriff auf Aufgaben gewähren</a>. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Beitragen Sie Berechtigungen zum Projekt mit der Möglichkeit, Aufgaben oder höher hinzuzufügen.</p> <p>Wenn Sie eine Aufgabe erstellen, erhalten Sie automatisch Verwaltungsberechtigungen für die Aufgabe</p> <p> Weitere Informationen zu Aufgabenberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-task.md" class="MCXref xref">Aufgabe freigeben </a>. </p> <p>Informationen zum Anfordern zusätzlicher Berechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Erstellen von Aufgaben in einem Projekt

1. Wechseln Sie zu dem Projekt, in dem Sie eine Aufgabe erstellen möchten.
1. Klicken **Aufgaben** im linken Bereich.
1. (Bedingt) Wenn Sie die Aufgabenliste derzeit in einer agilen Ansicht anzeigen, klicken Sie auf die Schaltfläche **Listenansicht** icon ![](assets/list-view-in-agile-view-for-tasks.png) in der oberen rechten Ecke, um die Aufgabenliste anzuzeigen.
1. (Optional) Klicken Sie auf die **Planmodus** icon ![](assets/nwe-plan-mode-icon-task-list.png) und wählen Sie **Manuelles Speichern** Wählen Sie entweder **Standard** oder **Timeline-Planung**. Dadurch wird die **Automatische Speicherung** -Option, die standardmäßig aktiviert ist.

   ![Manuelles Speichern auswählen](assets/manual-save-option.png)

   >[!TIP]
   >
   >Sie können Ihre Änderungen rückgängig machen, wenn Sie Manuelles Speichern auswählen.

1. Erstellen Sie eine neue Aufgabe, indem Sie einen der folgenden Schritte ausführen:

   * Klicken **Neue Aufgabe** oben in der Aufgabenliste
   * Klicken **Weitere Aufgaben hinzufügen** am Ende der Aufgabenliste

   ![](assets/qs-new-task-or-add-task-buttons-in-list-highlighted-350x242.png)

1. (Bedingt) Wenn Sie auf **Neue Aufgabe** Führen Sie folgende Schritte aus:

   1. Geben Sie eines der Felder in der Liste der begrenzten Felder in der **Neue Aufgabe** und klicken Sie auf **Aufgabe erstellen** , wenn Sie eine Aufgabe schnell erstellen möchten.

      Oder

      Um alle Felder für die Aufgabe zu aktualisieren, klicken Sie auf **Weitere Optionen** , um **Aufgabe erstellen** ankreuzen.

      ![](assets/nwe-create-task-small-screen-350x272.png)

      Die **Aufgabe erstellen** wird geöffnet.

      ![](assets/create-task-larger-box-nwe-350x244.png)

       

      >[!NOTE]
      >
      >Je nachdem, wie Ihr Workfront-Administrator unsere Layoutvorlage eingerichtet hat, werden in den Feldern im Feld &quot;Aufgabe erstellen&quot;möglicherweise verschiedene Felder in Ihrer Umgebung angezeigt. Weitere Informationen finden Sie unter [Detailansicht mithilfe einer Layoutvorlage anpassen](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   1. Geben Sie Informationen für die folgenden Bereiche im linken Bereich des Felds Aufgabe erstellen an:

      * Aufgabenname
      * Übersicht
      * Arbeitsaufträge
      * Benutzerdefinierte Formulare
      * Finanzielle Details
      * Einstellungen

        Informationen zum Definieren aller Aufgabenfelder für eine Aufgabe finden Sie unter [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

   1. (Bedingt und optional) Wenn die Aufgabe wiederkehrend sein soll, aktualisieren Sie die **Häufigkeit der Wiederholungen** -Feld. Weitere Informationen zum Erstellen wiederkehrender Aufgaben finden Sie unter [Wiederkehrende Aufgaben erstellen](../../../manage-work/tasks/create-tasks/create-recurring-tasks.md).
   1. (Optional) Klicken Sie auf **Dokumente** im linken Bereich, um ein Dokument an die neue Aufgabe anzuhängen, und klicken Sie dann auf **Hinzufügen oder Verknüpfen von Dateien** , um der Aufgabe ein Dokument von Ihrem Computer oder einem anderen Dienst hinzuzufügen oder Dokumente und Ordner von Ihrem Computer oder einem anderen Dienst zu verknüpfen.

1. (Bedingt) Wenn Sie auf **Weitere Aufgaben hinzufügen** in Schritt 5 die Eingabe der Aufgabeninformationen über die Inline-Bearbeitung starten und die Eingabetaste drücken.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this stays accurate)</p>
   -->

   Es wird empfohlen, diese Option insbesondere beim Hinzufügen mehrerer Aufgaben zur Liste zu verwenden.

   ![](assets/ctp4-350x26.png)

1. (Bedingt) Führen Sie einen der folgenden Schritte aus:

   * Wenn Sie auf **Neue Aufgabe** Klicken Sie in Schritt 5 auf **Aufgabe erstellen** , um Ihre Änderungen zu speichern und die neue Aufgabe zu Ihrem Projekt hinzuzufügen.

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?)</p>   
     -->

   * Wenn Sie auf **Weitere Aufgaben hinzufügen** Gehen Sie in Schritt 5 wie folgt vor:

     <!--   
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is this step still right?) </p>   
     -->

      1. Klicken Sie auf eine beliebige Stelle im Browser, um Ihre Änderungen zu senden, oder drücken Sie die Eingabetaste.
      1. (Optional) Wählen Sie in der Aufgabenliste die neu erstellte Aufgabe aus und klicken Sie auf **Einzug**.

         Dadurch wird die neue Aufgabe zu einer untergeordneten Aufgabe oder Unteraufgabe der vorherigen Aufgabe.

         Weitere Informationen zu untergeordneten Aufgaben finden Sie unter [Aufgabenübersicht](../../../manage-work/tasks/task-information/tasks-overview.md).

      1. (Bedingt) Wenn Sie die **Automatische Speicherung** Option nach dem Drücken **Weitere Aufgaben hinzufügen**, können Sie Folgendes tun:

         * Klicken **Rückgängig** jederzeit die letzte Änderung rückgängig machen oder **Abbrechen** um alle Änderungen rückgängig zu machen, die Sie an der Aufgabenliste vorgenommen haben.
         * Wenn Sie zuvor auf **Rückgängig** klicken **Wiederholen** , um die letzte Änderung, die Sie abgebrochen haben, erneut anzuwenden.
         * Klicken **Speichern** , um Ihre Änderungen in der Aufgabenliste zu speichern.
