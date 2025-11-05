---
product-area: projects
navigation-topic: approvals
title: Einen neuen oder vorhandenen Genehmigungsprozess mit Arbeit verknüpfen
description: Dieser Artikel beschreibt, wie Sie Genehmigungsprozesse mit Arbeitselementen verknüpfen können. Informationen zum Verknüpfen von Genehmigungen mit Korrekturabzügen oder Dokumenten finden Sie in den folgenden Artikeln.
author: Courtney and Alina
feature: Work Management, Digital Content and Documents
sexl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
exl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
source-git-commit: ac24b2486b9fc5a0b8c2944a6ec240140238b908
workflow-type: tm+mt
source-wordcount: '1821'
ht-degree: 0%

---

# Einen neuen oder vorhandenen Genehmigungsprozess mit Arbeit verknüpfen

Dieser Artikel beschreibt, wie Sie Genehmigungsprozesse mit Arbeitselementen verknüpfen können. Informationen zum Verknüpfen von Genehmigungen mit Korrekturabzügen oder Dokumenten finden Sie in den folgenden Artikeln:

* [Erstellen eines erweiterten Korrekturabzugs mit einem automatisierten Workflow](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Dokumentgenehmigungen anfordern](../../review-and-approve-work/manage-approvals/request-document-approvals.md)

Sie können einen globalen oder einmaligen Genehmigungsprozess mit einem Arbeitselement in Adobe Workfront verknüpfen. Die folgenden Szenarien sind vorhanden:

* Verknüpfen Sie einen vorhandenen globalen Genehmigungsprozess mit einem Projekt, einer Aufgabe, einem Problem, einer Vorlage oder einer Vorlagenaufgabe. Einige globale Genehmigungsprozesse stehen allen Gruppen im System zur Verfügung. Globale Genehmigungsprozesse auf Gruppenebene stehen nur bestimmten Gruppen zur Verfügung.
* Erstellen Sie einen Genehmigungsprozess für den einmaligen Gebrauch und verknüpfen Sie ihn mit einem vorhandenen Projekt, einer vorhandenen Aufgabe, einem vorhandenen Problem, einer vorhandenen Vorlage oder einer vorhandenen Vorlagenaufgabe.

>[!NOTE]
>
>In diesem Artikel wird der Begriff „globaler Genehmigungsprozess“ verwendet, um von dem „einmaligen Genehmigungsprozess“ zu unterscheiden. Ein globaler Genehmigungsprozess kann wiederholt verwendet werden.
>
>Der Begriff „globaler Genehmigungsprozess auf Gruppenebene“ bezieht sich auf einen Genehmigungsprozess, der wiederholt für Elemente und mit Status verwendet werden kann, die nur mit einer bestimmten Gruppe verknüpft sind.

Weitere allgemeine Informationen zu Genehmigungsprozessen finden Sie unter [Übersicht über Genehmigungsprozesse](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

Informationen zum Erstellen eines globalen Genehmigungsprozesses finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Standard</p>
   <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte, Aufgaben, Probleme oder Vorlagen bearbeiten oder höher</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Projekt, die Aufgabe, das Problem oder die Vorlage</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Verknüpfen von Genehmigungsprozessen mit Arbeitselementen

Zusätzlich zu den unten beschriebenen Überlegungen empfehlen wir, die allgemeinen Überlegungen zu Genehmigungsprozessen in Workfront zu überprüfen. Weitere Informationen finden Sie unter [Übersicht über den Genehmigungsprozess](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Approvals can only be associated with the status of a project, task, or issue in Workfront.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Each approval process corresponds with a status option in the Workfront system. When you change the status of a work item, an attached approval for that status requires the status change to be confirmed before the new status can be assigned to the item.</p> <p>(NOTE: the two drafted bullets have been moved to the approval-process-in-workfront article)</p> </li>
  -->

* Sie müssen das Projekt, die Aufgabe, das Problem, die Vorlage oder die Vorlagenaufgabe erstellen, bevor der Genehmigungsprozess mit ihnen verknüpft werden kann.
* Wenn Sie einen Genehmigungsprozess an ein Element für einen Status anhängen, der erfolgreich war und in dem sich das Element derzeit befindet, wird der Genehmigungsprozess nicht ausgelöst und es werden keine Benachrichtigungen an die genehmigenden Personen gesendet.

  **Beispiel** Wenn sich eine Aufgabe im Status „Abgeschlossen“ befindet und Sie einen Genehmigungsprozess anhängen, der mit dem Status „Abgeschlossen“ verknüpft ist, führt die Genehmigung nicht zum Trigger.

* Wenn Sie einen Genehmigungsprozess an den ersten Status eines Elements anhängen (indem Sie eine Vorlage für Aufgaben und Projekte verwenden, die Warteschlangen-Setup-Einstellungen für Probleme verwenden oder die Aufgabeneinstellungen eines Projekts für neue Aufgaben definieren), werden die Genehmigungsprozesse umgangen, wenn die gesendete Genehmigung zurückgerufen wird. In diesem Fall erhalten die genehmigenden Personen keine Benachrichtigungen.

  Weitere Informationen zum Aufrufen von Genehmigungen finden Sie unter [Genehmigungen anzeigen](../../review-and-approve-work/manage-approvals/view-approvals.md).

  >[!TIP]
  >
  >Der erste Status für eine Aufgabe oder ein Problem ist Neu. Der erste Status für ein Projekt ist der Status, den Ihr Workfront-Administrator in den Projektvoreinstellungen in Ihrem System ausgewählt hat. Weitere Informationen finden [ unter „Systemweite Projektvoreinstellungen konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Die Zuordnung von Genehmigungsprozessen zu einem Objekt wird im Bereich Aktualisierungen für das Objekt nicht aufgezeichnet.
* Ein Genehmigungsprozess kann nicht mit einer übergeordneten Aufgabe verknüpft werden.
* Durch das Hinzufügen eines Benutzers, Teams oder einer Rolle als genehmigende Person werden diesem Benutzer bzw. dieser Person nicht automatisch Berechtigungen für das Objekt erteilt, das mit dieser Genehmigung verknüpft ist. Sie erhalten Berechtigungen für das Objekt, wenn der Genehmigungsschritt ausgelöst wird. Andernfalls müssen die Objekte für sie freigegeben werden, bevor sie eine Genehmigungsentscheidung treffen können.

In den folgenden Abschnitten werden die verschiedenen Methoden zum Verknüpfen eines Genehmigungsprozesses mit einem Projekt, einer Aufgabe oder einem Problem beschrieben.

## Verknüpfen eines globalen Genehmigungsprozesses mit einem Arbeitselement {#associate-a-global-approval-process-with-a-work-item}

Sie können einen globalen Genehmigungsprozess mit einem Arbeitselement (Projekt, Aufgabe, Problem, Vorlage, Vorlagenaufgabe) verknüpfen.

Sie können auf jeden globalen Genehmigungsprozess zugreifen, solange er für eine Gruppe, der Sie angehören, oder für alle Gruppen im System freigegeben ist.

<!--The global approval process must be available to the group associated with the work item or to all groups in the system.-->

>[!NOTE]
>
>Sie können Projektgenehmigungsprozesse an eine Vorlage und Aufgabengenehmigungsprozesse an eine Vorlagenaufgabe anhängen. Wenn anschließend jemand die Vorlage verwendet, um ein Projekt zu erstellen, wird der Genehmigungsprozess zu einem Projekt- bzw. Aufgabengenehmigungsprozess. Ein an eine Vorlage oder Vorlagenaufgabe angehängter Genehmigungsprozess zur einmaligen Verwendung bleibt ein Genehmigungsprozess zur einmaligen Verwendung für Projekte und Aufgaben.

Informationen dazu, wie Workfront-Administratoren einen globalen Genehmigungsprozess für alle Gruppen im System konfigurieren können und wie Gruppenadministratoren Genehmigungen für eine Gruppe erstellen können, finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
>
>Sie können auch einen globalen Genehmigungsprozess an Ihre spezifischen Anforderungen anpassen. Weitere Informationen finden Sie im Abschnitt [Ändern eines globalen Genehmigungsprozesses für die Verwendung für ein bestimmtes Objekt](#modify-a-global-approval-process-for-use-on-a-specific-object) in diesem Artikel.

So verknüpfen Sie einen vorhandenen globalen Genehmigungsprozess mit einem Projekt, einer Aufgabe, einem Problem, einer Vorlage oder einer Vorlagenaufgabe:

1. Wechseln Sie zu dem Arbeitselement, mit dem Sie einen Genehmigungsprozess verknüpfen möchten.
1. Klicken Sie **linken** auf „Genehmigungen“.

   ![Abschnitt „Genehmigungen“ in der Aufgabe](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. ![Vorhandene verwenden oder Einzelnutzungsgenehmigungen erstellen](assets/use-existing-or-create-single-use-approvals-menus-on-pti-classic-350x50.png)

   Der ausgewählte Genehmigungsprozess wird angezeigt.

1. Erweitern Sie das **Vorhandenes verwenden** Dropdown-Menü und wählen Sie einen vorhandenen Genehmigungsprozess aus.

   ![Menü „Genehmigungen“](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

   Der ausgewählte Genehmigungsprozess wird angezeigt.

   ![Vorhandene Genehmigung an Aufgabe angehängt](assets/existing-approval-attached-to-task-redesigned-nwe-350x355.png)

1. Klicken Sie auf **Speichern**.
1. (Optional) Klicken Sie auf Genehmigungsprozess bearbeiten , wenn Sie die vorhandene Genehmigung, die Sie dem Element zugeordnet haben, ändern möchten. Dadurch wird der globale Genehmigungsprozess in einen einmaligen Genehmigungsprozess geändert. Weitere Informationen finden Sie im Abschnitt [Ändern eines globalen Genehmigungsprozesses für die Verwendung für ein bestimmtes Objekt](#modify-a-global-approval-process-for-use-on-a-specific-object) in diesem Artikel.

## Ändern eines globalen Genehmigungsprozesses für die Verwendung für ein bestimmtes Objekt {#modify-a-global-approval-process-for-use-on-a-specific-object}

Ihr Workfront-Administrator oder Gruppenadministrator erstellt globale Genehmigungsprozesse, die Sie verwenden können, wie beschrieben unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Das Ändern eines an ein Element angehängten globalen Genehmigungsprozesses ist mit dem Ändern eines einmaligen Genehmigungsprozesses identisch.

Sie können einen globalen Genehmigungsprozess an die spezifischen Anforderungen des Projekts, der Aufgabe oder des Problems anpassen, das bzw. die Sie mit ihm verknüpfen.

>[!IMPORTANT]
>
>Wenn Sie einen globalen Genehmigungsprozess ändern, wird dieser zu einem einmaligen Genehmigungsprozess, der nur für das Objekt verwendet werden kann, an dem Sie ihn geändert haben. Der globale Genehmigungsprozess bleibt unverändert.
>
>Beachten Sie beim Ändern eines globalen Genehmigungsprozesses die folgenden Einschränkungen:
>
>* Der Genehmigungsprozess wird nur für das Projekt, die Aufgabe oder das Problem geändert, mit dem bzw. der Sie den Genehmigungsprozess verknüpfen.
>* Zukünftige Änderungen, die von einem Administrator am ursprünglichen globalen Genehmigungsprozess vorgenommen werden, spiegeln den von Ihnen geänderten globalen Genehmigungsprozess nicht wider.
>

So ändern Sie einen Genehmigungsprozess, der bereits an ein Element angehängt ist:

1. Fügen Sie dem Projekt, der Aufgabe oder dem Problem einen globalen Genehmigungsprozess hinzu.

   Anweisungen finden Sie im Abschnitt [Verknüpfen eines globalen Genehmigungsprozesses mit einem Arbeitselement](#associate-a-global-approval-process-with-a-work-item) in diesem Artikel.

   >[!IMPORTANT]
   >
   >Stellen Sie sicher, dass Sie beim Hinzufügen **Genehmigung auf** Speichern“ klicken.

1. Nachdem der globale Genehmigungsprozess hinzugefügt wurde, klicken Sie auf **Bearbeiten** Symbol ![Bearbeiten](assets/edit-icon.png) in der rechten oberen Ecke der Seite „Genehmigung“. Diese Aktion wandelt den globalen Genehmigungsprozess oder den Genehmigungsprozess auf Gruppenebene in einen einmaligen Genehmigungsprozess um.
1. Nehmen Sie Änderungen am vorhandenen Genehmigungsprozess vor. Weitere Informationen finden Sie im Abschnitt [Verknüpfen eines einmaligen Genehmigungsprozesses mit einem Projekt, einer Aufgabe, einem Problem, einer Vorlage oder einer ](#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task)) in diesem Artikel.
1. Klicken Sie **Speichern** und anschließend erneut auf **Speichern**, um zu bestätigen, dass Sie den globalen Genehmigungsprozess in einen einmaligen Genehmigungsprozess konvertieren möchten, der nur für dieses Objekt verfügbar ist.

## Verknüpfen eines einmaligen Genehmigungsprozesses mit einem Projekt, einer Aufgabe, einem Problem, einer Vorlage oder einer Vorlagenaufgabe {#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task}

Sie können einen einmaligen Genehmigungsprozess erstellen, der nur für ein bestimmtes Projekt, eine bestimmte Aufgabe oder ein bestimmtes Problem verwendet werden kann.

Sie können einen Genehmigungsprozess für den einmaligen Gebrauch auch mit einer Vorlage oder Vorlagenaufgabe verknüpfen, damit er für Projekte und Aufgaben verfügbar ist, die aus der Vorlage erstellt wurden.

>[!NOTE]
>
>Sie können einen Genehmigungsprozess für den einmaligen Gebrauch mit einem beliebigen Status auf Systemebene oder Gruppenebene für ein Projekt, eine Aufgabe, ein Problem, eine Vorlage oder eine Vorlagenaufgabe verknüpfen. Weitere Informationen zum Workfront-Status finden Sie [Erstellen oder Bearbeiten eines Status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Wenn Sie einen Genehmigungsprozess auf diese Weise erstellen, können Sie einen benutzerdefinierten Genehmigungsprozess erstellen, der Ihren Anforderungen entspricht. Der Genehmigungsprozess kann jedoch nicht mit anderen Arbeitselementen in der Zukunft verknüpft werden.

Alternativ können Sie einen globalen Genehmigungsprozess für ein bestimmtes Element ändern, der auch zu einem einmaligen Genehmigungsprozess wird. Weitere Informationen finden Sie im Abschnitt [Ändern eines globalen Genehmigungsprozesses für die Verwendung für ein bestimmtes Objekt](#modify-a-global-approval-process-for-use-on-a-specific-object) in diesem Artikel.

So erstellen Sie einen Genehmigungsprozess für den einmaligen Gebrauch:

1. Wechseln Sie zu dem Projekt, der Aufgabe, dem Problem, der Vorlage oder der Vorlagenaufgabe, dem bzw. der Sie einen Genehmigungsprozess zuordnen möchten.
1. Klicken Sie **linken** auf „Genehmigungen“.

   ![Abschnitt „Genehmigungen“ in der Aufgabe](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Klicken Sie **Einmalige Verwendung erstellen**.

   ![Menü „Genehmigungen“](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

1. Führen Sie die Schritte ab Schritt 6 im Abschnitt „Erstellen eines globalen Genehmigungsprozesses auf Systemebene oder Gruppenebene für Arbeitselemente“ im Artikel „Erstellen [ Genehmigungsprozesses für Arbeitselemente“ ](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: overtime, ensure step 6 is still accurate here)&nbsp;</p>
   -->

   >[!TIP]
   >
   >Nachdem Sie den einmaligen Genehmigungsprozess angehängt haben, wird er im Feld Genehmigungsprozess innerhalb des Felds Bearbeiten von Vorlagen und Vorlagenaufgaben als &quot;`<Custom>`&quot; angezeigt. Informationen zum Bearbeiten von Vorlagen oder Vorlagenaufgaben finden Sie in den folgenden Artikeln:
   >
   >* [Projektvorlagen bearbeiten](../../manage-work/projects/create-and-manage-templates/edit-templates.md)
   >* [Vorlagenaufgaben bearbeiten](../../manage-work/projects/create-and-manage-templates/edit-template-task.md)

   <!--
   ><p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be removed when they bring the new Edit Template/ Template Task boxes to NWE) </p>   >
   -->

## Entfernen oder Löschen eines Genehmigungsprozesses aus einem Arbeitselement

Sie können einen globalen Genehmigungsprozess oder einen Genehmigungsprozess auf Gruppenebene entfernen oder einen einmaligen Genehmigungsprozess aus einem Projekt, einer Aufgabe oder einem Problem löschen, das zuvor damit verknüpft war.

Die folgenden Szenarien sind vorhanden: 

* Beim Entfernen des globalen Genehmigungsprozesses oder des Genehmigungsprozesses auf Gruppenebene wird die Genehmigung nicht gelöscht. Die Genehmigung bleibt für die zukünftige Verwendung verfügbar.
* Wenn ein Genehmigungsprozess für einen einzelnen Benutzer gelöscht wird, wird er aus Workfront gelöscht und kann nicht wiederhergestellt werden.

So entfernen oder löschen Sie einen Genehmigungsprozess aus einem Arbeitselement:

1. Wechseln Sie zum Projekt, zur Aufgabe, zum Problem, zur Vorlage oder zur Vorlagenaufgabe, in dem bzw. der Sie einen zuvor hinzugefügten Genehmigungsprozess entfernen möchten.
1. Klicken Sie **linken** auf „Genehmigungen“.

   ![Abschnitt „Genehmigungen“ in der Aufgabe](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Klicken Sie auf eines der folgenden Symbole in der rechten oberen Ecke des Abschnitts Genehmigungen , je nachdem, welcher Genehmigungstyp mit dem Element verknüpft ist:

   * **Entfernen** Symbol ![Entfernen-Symbol](assets/remove-icon---x-in-circle.png) für globale Genehmigungen oder Gruppengenehmigungen.
   * **Das Symbol** Löschen![Symbol Löschen](assets/delete.png) für Genehmigungen zur einmaligen Verwendung.

1. Klicken Sie **Entfernen** oder **Löschen** zur Bestätigung.

   Der Genehmigungsprozess wird aus dem Arbeitselement entfernt.

## Automatisches Verknüpfen eines Genehmigungsprozesses mit Arbeitselementen

Sie können einen Genehmigungsprozess mithilfe der folgenden Workflows automatisch mit Arbeitselementen verknüpfen:

* Für Projekte und Aufgaben können Sie einen Genehmigungsprozess mithilfe einer Vorlage verknüpfen. Sie können einen vorhandenen Genehmigungsprozess an die Registerkarte Vorlagengenehmigungen oder die Registerkarte Vorlagenaufgabe - Genehmigungen anhängen. Informationen zum Verknüpfen einer vorhandenen Genehmigung mit einem Arbeitselement finden Sie unter [Verknüpfen eines globalen Genehmigungsprozesses mit einem Arbeitselement](#associate-a-global-approval-process-with-a-work-item) in diesem Artikel.
* Für neue Aufgaben an einem vorhandenen Projekt können Sie einen globalen Genehmigungsprozess oder einen globalen Genehmigungsprozess auf Gruppenebene im Bereich Aufgabeneinstellungen des Felds Projekt bearbeiten verknüpfen. Weitere Informationen finden Sie im Abschnitt „Aufgabeneinstellungen“ im Artikel [Projekte bearbeiten](../../manage-work/projects/manage-projects/edit-projects.md).
* Bei Problemen können Sie jedem neuen Problem, das einem Projekt hinzugefügt wird, eine Genehmigung zuordnen, indem Sie einen vorhandenen Genehmigungsprozess mit einer Anfrage-Warteschlange verknüpfen. Informationen zum Konfigurieren von Anfragewarteschlangen finden Sie unter [Erstellen einer Anfragewarteschlange](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
