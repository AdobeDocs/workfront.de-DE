---
product-area: projects
navigation-topic: approvals
title: Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit
description: In diesem Artikel wird beschrieben, wie Sie Genehmigungsprozesse mit Arbeitselementen verknüpfen können. Informationen zum Verknüpfen von Genehmigungen mit Testsendungen oder Dokumenten finden Sie in den folgenden Artikeln.
author: Courtney and Alina
feature: Work Management, Digital Content and Documents
sexl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
exl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
source-git-commit: c6e3e3d8d4fd6b6916c8fd49983bc3572949acaa
workflow-type: tm+mt
source-wordcount: '1880'
ht-degree: 0%

---

# Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit

In diesem Artikel wird beschrieben, wie Sie Genehmigungsprozesse mit Arbeitselementen verknüpfen können. Informationen zum Verknüpfen von Genehmigungen mit Testsendungen oder Dokumenten finden Sie in den folgenden Artikeln:

* [Erstellen eines erweiterten Testversands mit einem automatisierten Workflow](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [Dokumentgenehmigungen anfordern](../../review-and-approve-work/manage-approvals/request-document-approvals.md)

Sie können einen globalen Genehmigungsprozess oder einen Genehmigungsprozess für eine einmalige Verwendung mit einem Arbeitselement in Adobe Workfront verknüpfen. Die folgenden Szenarien existieren:

* Verknüpfen eines vorhandenen globalen Genehmigungsprozesses mit einem Projekt, einer Aufgabe, einem Problem, einer Vorlage oder einer Vorlagenaufgabe. Einige globale Genehmigungsprozesse stehen allen Gruppen im System zur Verfügung. Globale Validierungsprozesse auf Gruppenebene sind nur für bestimmte Gruppen verfügbar.
* Erstellen Sie einen Validierungsprozess für die einmalige Verwendung und verknüpfen Sie ihn mit einem vorhandenen Projekt, einer Aufgabe, einem Problem, einer Vorlage oder einer Vorlagenaufgabe.

>[!NOTE]
>
>In diesem Artikel wird der Begriff &quot;globaler Genehmigungsprozess&quot;verwendet, um von &quot;Genehmigungsprozess für einmalige Verwendung&quot;zu unterscheiden. Ein globaler Genehmigungsprozess kann wiederholt verwendet werden.
>
>Der Begriff &quot;Globaler Validierungsprozess auf Gruppenebene&quot;bezieht sich auf einen Validierungsprozess, der wiederholt für Elemente und mit Status verwendet werden kann, die nur einer bestimmten Gruppe zugeordnet sind.

Allgemeine Informationen zu Genehmigungsprozessen finden Sie unter [Validierungsprozess - Übersicht](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

Informationen zum Erstellen eines globalen Genehmigungsprozesses finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsstufe*</td> 
   <td> <p>Zugriff auf Projekte, Aufgaben, Probleme oder Vorlagen bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Projekt, die Aufgabe, das Problem oder die Vorlage</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

+++

## Überlegungen zum Zuordnen von Genehmigungsprozessen zu Arbeitselementen

Zusätzlich zu den unten beschriebenen Überlegungen empfehlen wir, die allgemeinen Überlegungen zu Genehmigungsprozessen in Workfront erneut aufzurufen. Weitere Informationen finden Sie unter [Übersicht über den Genehmigungsprozess](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Approvals can only be associated with the status of a project, task, or issue in Workfront.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Each approval process corresponds with a status option in the Workfront system. When you change the status of a work item, an attached approval for that status requires the status change to be confirmed before the new status can be assigned to the item.</p> <p>(NOTE: the two drafted bullets have been moved to the approval-process-in-workfront article)</p> </li>
  -->

* Sie müssen das Projekt, die Aufgabe, das Problem, die Vorlage oder die Vorlagenaufgabe erstellen, bevor ihnen der Genehmigungsprozess zugeordnet werden kann.
* Wenn Sie einen Validierungsprozess an ein Element für einen Status anhängen, der übergeben wurde und in dem sich das Element derzeit befindet, wird der Validierungsprozess nicht ausgelöst und es werden keine Benachrichtigungen an die Genehmiger gesendet.

  **Beispiel:** Wenn eine Aufgabe den Status Abgeschlossen aufweist und Sie einen Genehmigungsprozess anhängen, der mit dem Status Abgeschlossen verknüpft ist, wird die Genehmigung nicht Trigger.

* Wenn Sie einen Genehmigungsprozess an den ersten Status eines Elements anhängen (mithilfe einer Vorlage für Aufgaben und Projekte, mithilfe der Einstellungen für die Warteschlangeneinrichtung für Probleme oder durch Definition der Aufgabeneinstellungen eines Projekts für neue Aufgaben), werden die Genehmigungsprozesse umgangen, wenn die gesendete Genehmigung zurückgerufen wird. In diesem Fall erhalten die Genehmiger keine Benachrichtigungen.

  Weitere Informationen zum Aufrufen von Genehmigungen finden Sie unter [Genehmigungen anzeigen](../../review-and-approve-work/manage-approvals/view-approvals.md).

  >[!TIP]
  >
  >Der erste Status für eine Aufgabe oder ein Problem ist &quot;Neu&quot;. Der erste Status für ein Projekt ist der Status, den Ihr Workfront-Administrator in den Projektoptionen in Ihrem System ausgewählt hat. Weitere Informationen finden Sie unter [Systemweite Projekteigenschaften konfigurieren](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* Die Zuordnung von Genehmigungsprozessen zu einem Objekt wird im Bereich Updates für das Objekt nicht aufgezeichnet.
* Sie können einen Genehmigungsprozess nicht mit einer übergeordneten Aufgabe verknüpfen.
* Wenn Benutzer, Teams oder Rollen als Genehmiger hinzugefügt werden, erhalten sie nicht automatisch Berechtigungen für das mit dieser Genehmigung verknüpfte Objekt. Sie erhalten Berechtigungen für das Objekt, wenn der Genehmigungsschritt ausgelöst wird. Andernfalls müssen die Objekte für sie freigegeben werden, bevor sie eine Genehmigungsentscheidung treffen können.

In den folgenden Abschnitten werden die verschiedenen Methoden zum Verknüpfen eines Genehmigungsprozesses mit einem Projekt, einer Aufgabe oder einem Problem beschrieben.

## Verknüpfen eines globalen Genehmigungsprozesses mit einem Arbeitselement {#associate-a-global-approval-process-with-a-work-item}

Sie können einen globalen Genehmigungsprozess mit einem Arbeitselement (Projekt, Aufgabe, Problem, Vorlage, Vorlagenaufgabe) verknüpfen.

Der globale Genehmigungsprozess muss für die mit dem Arbeitselement verknüpfte Gruppe oder für alle Gruppen im System verfügbar sein.

>[!NOTE]
>
>Sie können Projektgenehmigungsprozesse an eine Vorlage anhängen und Aufgabengenehmigungsprozesse an eine Vorlagenaufgabe. Wenn Sie dies tun und jemand die Vorlage zum Erstellen eines Projekts verwendet, wird der Genehmigungsprozess zu einem Projekt- bzw. Aufgabenvalidierungsprozess. Ein an eine Vorlage oder Vorlagenaufgabe angehängter Genehmigungsprozess für eine einmalige Verwendung bleibt ein einmaliger Genehmigungsprozess für Projekte und Aufgaben.

Informationen dazu, wie Workfront-Administratoren einen globalen Genehmigungsprozess für alle Gruppen im System konfigurieren können und wie Gruppenadministratoren Genehmigungen für eine Gruppe erstellen können, finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
>
>Sie können auch einen globalen Genehmigungsprozess an Ihre spezifischen Anforderungen anpassen. Weitere Informationen finden Sie im Abschnitt [Globalen Genehmigungsprozess für ein bestimmtes Objekt ändern](#modify-a-global-approval-process-for-use-on-a-specific-object) in diesem Artikel.

So verknüpfen Sie einen vorhandenen globalen Genehmigungsprozess mit einer Projekt-, Aufgaben-, Ausgabe-, Vorlagen- oder Vorlagenaufgabe:

1. Wechseln Sie zu dem Arbeitselement, mit dem Sie einen Genehmigungsprozess verknüpfen möchten.
1. Klicken Sie im linken Bereich auf **Genehmigungen** .

   Möglicherweise müssen Sie auf **Mehr anzeigen** und dann auf **Genehmigungen** klicken.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. ![](assets/use-existing-or-create-single-use-approvals-menus-on-pti-classic-350x50.png)

   Der gewählte Validierungsprozess wird angezeigt.

1. Erweitern Sie das Dropdownmenü **Vorhandenen** verwenden und wählen Sie einen vorhandenen Genehmigungsprozess aus.

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

   Der gewählte Validierungsprozess wird angezeigt.

   ![](assets/existing-approval-attached-to-task-redesigned-nwe-350x355.png)

1. Klicken Sie auf **Speichern**.
1. (Optional) Klicken Sie auf Genehmigungsprozess bearbeiten , wenn Sie die vorhandene Genehmigung ändern möchten, die Sie dem Element angehängt haben. Dadurch wird der globale Validierungsprozess in einen Validierungsprozess für die einmalige Verwendung geändert. Weitere Informationen finden Sie im Abschnitt [Globalen Genehmigungsprozess für ein bestimmtes Objekt ändern](#modify-a-global-approval-process-for-use-on-a-specific-object) in diesem Artikel.

## Globalen Genehmigungsprozess zur Verwendung für ein bestimmtes Objekt ändern {#modify-a-global-approval-process-for-use-on-a-specific-object}

Ihr Workfront-Administrator oder Gruppenadministrator erstellt globale Genehmigungsprozesse, die Sie verwenden können, wie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) beschrieben.

Das Ändern eines globalen Genehmigungsprozesses, der an ein Element angehängt wird, entspricht dem Ändern eines Validierungsprozesses für die einmalige Verwendung.

Sie können einen globalen Genehmigungsprozess an die jeweiligen Anforderungen des Projekts, der Aufgabe oder des Problems anpassen, das Sie damit verbinden.

>[!IMPORTANT]
>
>Wenn Sie einen globalen Genehmigungsprozess ändern, wird dieser zu einem Genehmigungsprozess für einzelne Anwendungen, der nur für das Objekt verwendet werden kann, an dem Sie ihn geändert haben. Der globale Genehmigungsprozess bleibt unverändert.
>
>Beachten Sie beim Ändern eines globalen Genehmigungsprozesses die folgenden Einschränkungen:
>
>* Der Genehmigungsprozess wird nur für das Projekt, die Aufgabe oder das Problem geändert, mit dem/dem Sie den Genehmigungsprozess verbinden.
>* Künftige Änderungen, die von einem Administrator am ursprünglichen globalen Genehmigungsprozess vorgenommen werden, spiegeln nicht den von Ihnen geänderten globalen Genehmigungsprozess wider.
>

So ändern Sie einen bereits an ein Element angehängten Genehmigungsprozess:

1. Fügen Sie dem Projekt, der Aufgabe oder dem Problem einen globalen Genehmigungsprozess hinzu.

   Anweisungen finden Sie im Abschnitt [Verknüpfen eines globalen Genehmigungsprozesses mit einem Arbeitselement](#associate-a-global-approval-process-with-a-work-item) in diesem Artikel.

   >[!IMPORTANT]
   >
   >Stellen Sie sicher, dass Sie beim Hinzufügen der Genehmigung auf **Speichern** klicken.

1. Nachdem der globale Genehmigungsprozess hinzugefügt wurde, klicken Sie auf das Symbol **Bearbeiten** ![](assets/edit-icon.png) oben rechts auf der Genehmigungsseite. Dadurch wird der Genehmigungsprozess auf globaler oder Gruppenebene zu einem Genehmigungsprozess für die einmalige Verwendung.
1. Nehmen Sie Änderungen am vorhandenen Genehmigungsprozess vor. Weitere Informationen finden Sie im Abschnitt [Verknüpfen eines Validierungsprozesses für die einmalige Verwendung mit einem Projekt, einer Aufgabe, einem Problem, einer Vorlage oder einer Vorlagenaufgabe](#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task) in diesem Artikel.
1. Klicken Sie auf &quot;**Speichern**&quot;und dann erneut auf &quot;**Speichern**&quot;, um zu bestätigen, dass Sie den globalen Genehmigungsprozess in einen Einzelverwendungs-Genehmigungsprozess konvertieren möchten, der nur für dieses Objekt verfügbar ist.

## Verknüpfen eines einmaligen Genehmigungsprozesses mit einer Projekt-, Aufgaben-, Problem-, Vorlagen- oder Vorlagenaufgabe {#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task}

Sie können einen Genehmigungsprozess für eine einmalige Verwendung erstellen, der nur für ein bestimmtes Projekt, eine bestimmte Aufgabe oder ein bestimmtes Problem verwendet werden kann.

Sie können auch einen Validierungsprozess für die einmalige Verwendung mit einer Vorlage oder Vorlagenaufgabe verknüpfen, damit er für Projekte und Aufgaben verfügbar ist, die aus der Vorlage erstellt werden.

>[!NOTE]
>
>Sie können einen Validierungsprozess für die einmalige Verwendung mit einem beliebigen Status auf System- oder Gruppenebene für ein Projekt, eine Aufgabe, ein Problem, eine Vorlage oder eine Vorlagenaufgabe verknüpfen. Weitere Informationen zum Workfront-Status finden Sie unter [Erstellen oder Bearbeiten eines Status](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

Durch die Erstellung eines Validierungsprozesses auf diese Weise können Sie einen benutzerdefinierten Validierungsprozess erstellen, der Ihren Anforderungen entspricht. Der Genehmigungsprozess kann jedoch nicht mit anderen Arbeitselementen in der Zukunft verknüpft werden.

Alternativ können Sie einen globalen Genehmigungsprozess für ein bestimmtes Element ändern, der auch zu einem Genehmigungsprozess für einzelne Anwendungen wird. Weitere Informationen finden Sie im Abschnitt [Globalen Genehmigungsprozess für ein bestimmtes Objekt ändern](#modify-a-global-approval-process-for-use-on-a-specific-object) in diesem Artikel.

So erstellen Sie einen Validierungsprozess für die einmalige Verwendung:

1. Wechseln Sie zur Projekt-, Aufgaben-, Ausgabe-, Vorlagen- oder Vorlagenaufgabe, der Sie einen Genehmigungsprozess zuordnen möchten.
1. Klicken Sie im linken Bereich auf **Genehmigungen** .

   Möglicherweise müssen Sie auf **Mehr anzeigen** > **Genehmigungen** klicken.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Klicken Sie auf **Einmalige Verwendung erstellen**.

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

1. Führen Sie die Schritte aus, die mit Schritt 6 im Abschnitt &quot;Erstellen eines globalen Genehmigungsprozesses auf Systemebene oder Gruppenebene für Arbeitselemente&quot;im Artikel [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md) beginnen.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: overtime, ensure step 6 is still accurate here)&nbsp;</p>
   -->

   >[!TIP]
   >
   >Nachdem Sie den Validierungsprozess für die einmalige Verwendung angehängt haben, wird er im Feld Validierungsprozess im Feld Bearbeiten der Vorlagen und Vorlagenaufgaben als &quot;`<Custom>`&quot; angezeigt. Informationen zum Bearbeiten von Vorlagen oder Vorlagenaufgaben finden Sie in den folgenden Artikeln:
   >
   >* [Bearbeiten von Projektvorlagen](../../manage-work/projects/create-and-manage-templates/edit-templates.md)
   >* [Bearbeiten einer Vorlagenaufgabe](../../manage-work/projects/create-and-manage-templates/edit-template-task.md)

   <!--
   ><p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be removed when they bring the new Edit Template/ Template Task boxes to NWE) </p>   >
   -->

## Entfernen oder Löschen eines Genehmigungsprozesses aus einem Arbeitselement

Sie können einen globalen Validierungsprozess oder einen Validierungsprozess auf Gruppenebene entfernen oder einen einmaligen Validierungsprozess aus einem Projekt, einer Aufgabe oder einem Problem löschen, das bzw. das zuvor damit verknüpft wurde.

Die folgenden Szenarien existieren: 

* Wenn Sie den Validierungsprozess auf globaler oder Gruppenebene entfernen, wird die Validierung nicht gelöscht. Die Genehmigung bleibt für die zukünftige Verwendung verfügbar.
* Durch das Löschen eines Validierungsprozesses für einzelne Benutzer wird dieser aus Workfront gelöscht und kann nicht wiederhergestellt werden.

So entfernen oder löschen Sie einen Genehmigungsprozess aus einem Arbeitselement:

1. Wechseln Sie zu dem Projekt, der Aufgabe, dem Problem, der Vorlage oder der Vorlagenaufgabe, in dem Sie einen zuvor hinzugefügten Genehmigungsprozess entfernen möchten.
1. Klicken Sie im linken Bereich auf **Genehmigungen** .

   Möglicherweise müssen Sie auf **Mehr anzeigen** > **Genehmigungen** klicken.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. Klicken Sie auf eines der folgenden Symbole in der oberen rechten Ecke des Bereichs Genehmigungen , je nachdem, welcher Typ der Genehmigung dem Element zugeordnet ist:

   * **Das Symbol** Entfernen ![](assets/remove-icon---x-in-circle.png) für Genehmigungen auf globaler oder Gruppenebene.
   * **Das Symbol** Löschen ![](assets/delete.png) für Einzelgenehmigungen.

1. Klicken Sie zur Bestätigung auf **Entfernen** oder **Löschen** .

   Der Genehmigungsprozess wird aus dem Arbeitselement entfernt.

## Automatisches Verknüpfen eines Genehmigungsprozesses mit Arbeitselementen

Mithilfe der folgenden Workflows können Sie einen Genehmigungsprozess automatisch mit Arbeitselementen verknüpfen:

* Bei Projekten und Aufgaben können Sie mithilfe einer Vorlage einen Genehmigungsprozess verknüpfen. Sie können einen vorhandenen Genehmigungsprozess an die Registerkarte Vorlagengenehmigungen oder die Registerkarte VorlagenAufgabengenehmigungen anhängen. Informationen zum Verknüpfen einer vorhandenen Genehmigung mit einem Arbeitselement finden Sie unter [Verknüpfen eines globalen Genehmigungsprozesses mit einem Arbeitselement ](#associate-a-global-approval-process-with-a-work-item) in diesem Artikel.
* Bei neuen Aufgaben für ein vorhandenes Projekt können Sie im Bereich Aufgabeneinstellungen im Feld Projekt bearbeiten einen globalen Genehmigungsprozess oder einen globalen Genehmigungsprozess auf Gruppenebene verknüpfen. Weitere Informationen finden Sie im Abschnitt &quot;Aufgabeneinstellungen&quot;im Artikel [Projekte bearbeiten](../../manage-work/projects/manage-projects/edit-projects.md).
* Bei Problemen können Sie jede neue Ausgabe, die einem Projekt hinzugefügt wird, mit einer Genehmigung verknüpfen, indem Sie einen vorhandenen Genehmigungsprozess mit einer Anforderungswarteschlange verknüpfen. Informationen zum Konfigurieren von Anforderungswarteschlangen finden Sie unter [Erstellen einer Anforderungswarteschlange](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
