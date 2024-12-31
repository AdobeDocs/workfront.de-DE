---
content-type: overview
product-area: projects
navigation-topic: approvals
title: Übersicht über den Genehmigungsprozess
description: Sie können einen Genehmigungsprozess erstellen und ihn an ein Objekt anhängen, um sicherzustellen, dass bestimmte Benutzerinnen und Benutzer bestimmte Änderungen überprüfen, bevor das Objekt fortfährt.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: dd0822b6-80f1-4a2e-bf6a-0c425984f4d0
source-git-commit: e4de185f172b173dcc3ad966afa69ffb3bc479eb
workflow-type: tm+mt
source-wordcount: '1752'
ht-degree: 0%

---

# Übersicht über den Genehmigungsprozess

<!-- Audited: 12/2023 -->

Sie können einen Genehmigungsprozess erstellen und ihn an ein Objekt anhängen, um sicherzustellen, dass bestimmte Benutzerinnen und Benutzer bestimmte Änderungen überprüfen, bevor das Objekt fortfährt.

Dies ist für die folgenden Objekttypen in Adobe Workfront verfügbar:

* Arbeitselement (Projekt, Aufgabe oder Problem, Vorlage, Vorlagenaufgabe)
* Dokument
* Korrekturabzug

Dieser Artikel enthält allgemeine Informationen zu Genehmigungsprozessen, die mit Arbeitselementen verknüpft sind.
Anweisungen zum Erstellen eines Genehmigungsprozesses finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Typen von Genehmigungsprozessen für Arbeitselemente

Wenn Sie ein Adobe Workfront-Administrator oder ein Benutzer mit administrativem Zugriff auf Genehmigungsprozesse sind, können Sie die folgenden Genehmigungsprozesse für Projekte, Aufgaben und Probleme erstellen:

* **Globaler Genehmigungsprozess auf Systemebene**: Benutzer können diesen an einen der folgenden Punkte anhängen:

   * Ein Projekt, eine Aufgabe oder ein Problem im Abschnitt Genehmigungen .
   * Im Feld Projekt bearbeiten im Bereich „Standardgenehmigungsprozess für Aufgabe“
   * Im Abschnitt „Warteschlangendetails“ oder „Warteschlangenthema“ eines Projekts in den Bereichen des Standardgenehmigungsprozesses. Das Projekt muss als Anfrage-Warteschlange aktiviert werden.

* **Globaler Genehmigungsprozess auf Gruppenebene**: Benutzer können diese an Folgendes anhängen:

   * Ein Projekt, eine Aufgabe oder ein Problem, das zu der Gruppe gehört, die mit dem Genehmigungsprozess im Abschnitt Genehmigungen verknüpft ist
   * Im Feld Projekt bearbeiten im Bereich Standardgenehmigungsprozess der Aufgabe für ein Projekt, das zu der mit dem Genehmigungsprozess verknüpften Gruppe gehört
   * Im Abschnitt „Warteschlangendetails“ oder „Warteschlangenthema“ eines Projekts in den Bereichen des Standardgenehmigungsprozesses. Das Projekt muss als Anfrage-Warteschlange aktiviert sein und der mit dem Genehmigungsprozess verknüpften Gruppe angehören.

  Informationen zum Erstellen eines Genehmigungsprozesses auf System- oder Gruppenebene finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

* **Ein Genehmigungsprozess für den einmaligen Gebrauch**: Zur Verwendung mit einem einzelnen Projekt, einer einzelnen Aufgabe, einem einzelnen Problem, einer einzelnen Vorlage oder einer einzelnen Vorlagenaufgabe. Dieser Genehmigungsprozess betrifft nur das Objekt, das mit ihm verknüpft ist, und kann nicht mit anderen Objekten verknüpft werden.

  Weitere Informationen zum Erstellen eines einmaligen Genehmigungsprozesses finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>In diesem Artikel wird der Begriff „globaler Genehmigungsprozess“ verwendet, um von dem „einmaligen Genehmigungsprozess“ zu unterscheiden. Ein globaler Genehmigungsprozess kann wiederholt verwendet werden.
>
>Der Begriff „globaler Genehmigungsprozess auf Gruppenebene“ bezieht sich auf einen Genehmigungsprozess, der wiederholt für Elemente und mit Status verwendet werden kann, die nur mit einer bestimmten Gruppe verknüpft sind.

Informationen zum Erstellen eines Genehmigungsprozesses auf Systemebene oder eines Genehmigungsprozesses auf Gruppenebene finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Überlegungen zu Genehmigungsprozessen

* Sie müssen das Projekt, die Aufgabe, das Problem, die Vorlage oder die Vorlagenaufgabe erstellen, bevor der Genehmigungsprozess mit ihnen verknüpft werden kann.
* Ein Genehmigungsprozess ist immer mit zwei wesentlichen Dingen verbunden:

   * Jeder Genehmigungsprozess entspricht einem bestimmten Arbeitsaufgabenstatus im Workfront-System. Wenn Sie den Status eines Arbeitselements ändern, erfordert eine angehängte Genehmigung für diesen Status, dass die Statusänderung bestätigt wird, bevor der neue Status dem Element zugewiesen werden kann.

     >[!TIP]
     >
     >
     >   
     >   
     >   * Sie können eine Genehmigung auf Gruppenebene mit einem globalen Status oder einem Status auf Gruppenebene verknüpfen.
     >   * Sie können den Status eines Artikels, der einen Genehmigungsprozess verwendet, nicht in einen anderen als den mit dem Genehmigungsprozess verknüpften Status ändern.
     >   
     >   
     >     Wenn Sie beispielsweise eine Aufgabengenehmigung mit dem Status In Bearbeitung verknüpft haben, ändert die Aufgabe ihren Status automatisch in In Bearbeitung , wenn die Genehmigung erteilt wird. Der Status kann nicht automatisch in „Abgeschlossen“ oder in einen anderen Status geändert werden, der nicht mit der Genehmigung verknüpft ist.
     >   
     >   
     >

   * Die mit einem Genehmigungsprozess verknüpften Entitäten können Benutzer, Aufgabengebiete oder Teams sein. Die Benutzer sind letztendlich dafür verantwortlich, die Genehmigung zu akzeptieren oder abzulehnen. Sie können Benutzern, die eine bestimmte Rolle im Projekt erfüllen, Genehmigungen zuweisen. Sie können beispielsweise eine Genehmigung einem Projektbesitzer oder Sponsor zuweisen. Weitere Informationen finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

     Die folgenden Szenarien sind vorhanden:

      * Wenn Sie Aufgabengebiete eine Genehmigung zuweisen, kann jeder Benutzer im Projektteam, der mit dem Aufgabengebiet verknüpft ist, eine Entscheidung über die Genehmigung treffen. Die mit der Genehmigung verknüpfte Rolle kann entweder ihre Primäre Rolle oder eine beliebige andere Rolle sein.

        Informationen zum Projektteam finden Sie unter [Projektteam - Übersicht](../../manage-work/projects/planning-a-project/project-team-overview.md).

      * Wenn Sie einem Team eine Genehmigung zuweisen, kann jedes Mitglied dieses Teams eine Entscheidung über die Genehmigung treffen. Das mit der Genehmigung verknüpfte Team kann entweder sein Home-Team oder eines seiner anderen Teams sein.

        Informationen zu den Rollen und Teams von Benutzenden finden Sie unter [Bearbeiten des Benutzerprofils](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Wenn Sie ein Arbeitselement erstellen, ist daran nicht automatisch ein Genehmigungsprozess angehängt. Wenn Sie einen verwenden möchten, müssen Sie einen manuell anhängen. Weitere Informationen zum Anhängen eines Genehmigungsprozesses an einen Artikel finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeit](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
* Der Workfront-Administrator oder ein Benutzer mit administrativem Zugriff auf Genehmigungsprozesse kann globale Genehmigungsprozesse auf Systemebene erstellen, die im gesamten System verwendet werden können. Ein Gruppenadministrator mit administrativem Zugriff auf Genehmigungsprozesse kann einen globalen Genehmigungsprozess auf Gruppenebene erstellen, der nur von einer bestimmten Gruppe verwendet werden kann, die er verwaltet.
* Wenn Sie keinen vordefinierten globalen Genehmigungsprozess auf Systemebene oder Gruppenebene für ein Arbeitselement verwenden möchten, können Sie einen einmaligen Genehmigungsprozess erstellen und daran anhängen, wenn Sie Verwaltungsberechtigungen für das Objekt haben, für das Sie den Genehmigungsprozess anhängen möchten.

  >[!NOTE]
  >
  >Sie können einen einmaligen Genehmigungsprozess nur einmal für das spezifische Element verwenden, für das er erstellt wurde. Sie können globale Status sowie Gruppenstatus für einmalige Genehmigungsprozesse für Projekte, Aufgaben, Probleme, Vorlagen und Vorlagenaufgaben verknüpfen.

* Beim Anhängen eines Genehmigungsprozesses auf Gruppenebene an ein Element mit benutzerdefiniertem Status auf Gruppenebene kann das Ändern der Gruppe des Projekts zu einem Konflikt zwischen den Genehmigungsstatus der vorherigen Gruppe und den auf Systemebene vorhandenen Status führen. Erwägen Sie, die Genehmigungsprozesse auf Gruppenebene für das Projekt oder seine Aufgaben oder Probleme zu entfernen, bevor Sie die Gruppe aktualisieren. Informationen zum Erstellen von Genehmigungsprozessen auf Gruppenebene finden Sie unter [Genehmigungsprozesse auf Gruppenebene](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md). Informationen zum Erstellen benutzerdefinierter Gruppenstatus finden Sie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md). Informationen zum Aktualisieren der Gruppe eines Projekts finden Sie unter [Projekte bearbeiten](../../manage-work/projects/manage-projects/edit-projects.md).

## Der Genehmigungsprozess-Workflow

In diesem Abschnitt werden die folgenden Informationen zur Genehmigung von Arbeitselementen erläutert:

* [Wie Genehmigungsprozesse auf Status angewiesen sind](#how-approval-processes-rely-on-statuses)
* [Verwendung eines Genehmigungsprozesses durch einen typischen Workflow](#how-a-typical-workflow-uses-an-approval-process)

### Wie Genehmigungsprozesse auf Status angewiesen sind {#how-approval-processes-rely-on-statuses}

Durch das Anhängen eines Status an einen Genehmigungsprozess wird sichergestellt, dass der Artikel in der richtigen Reihenfolge durch Abteilungen bewegt wird.

**Beispiel** Sie können einen Genehmigungsprozess an den Status der Marketing-Abteilung anhängen, der eine Genehmigung der Finanzabteilung erfordert. Wenn dann jemand den Status für einen Arbeitselement in „Marketing-Abteilung“ ändert, kann der Artikel erst dann in diese Abteilung verschoben werden, wenn die Finanzabteilung ihn abzeichnet.

Weitere Informationen zum Status von Arbeitselementen finden Sie in den folgenden Artikeln:

* [Zugriff auf die Liste der Systemprojektstatus](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)
* [Zugriff auf die Liste der Systemaufgabenstatus](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)
* [Zugriff auf die Liste der Systemanfragestatus](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)

### Verwendung eines Genehmigungsprozesses durch einen typischen Workflow {#how-a-typical-workflow-uses-an-approval-process}

Das folgende Szenario zeigt, wie ein Genehmigungsprozess Benutzenden dabei hilft, Arbeiten zu genehmigen, während ein Workfront-Objekt einen Workflow mit mehreren Schritten in dieser Reihenfolge durchläuft:

1. Der Workfront-Administrator oder ein Benutzer mit administrativem Zugriff auf Genehmigungsprozesse erstellt einen Genehmigungsprozess für ein Projekt, eine Aufgabe oder ein Problem.

   >[!NOTE]
   >
   >Sie können Projektgenehmigungsprozesse an eine Vorlage und Aufgabengenehmigungsprozesse an eine Vorlagenaufgabe anhängen. Wenn anschließend jemand die Vorlage verwendet, um ein Projekt zu erstellen, wird der Genehmigungsprozess zu einem Projekt- bzw. Aufgabengenehmigungsprozess. Ein an eine Vorlage oder Vorlagenaufgabe angehängter Genehmigungsprozess zur einmaligen Verwendung bleibt ein Genehmigungsprozess zur einmaligen Verwendung für Projekte und Aufgaben.

1. Ein Benutzer mit der Berechtigung Verwalten für das Projekt, die Aufgabe oder das Problem hängt den Genehmigungsprozess an das Element an oder erstellt eine Einmalgenehmigung für das Element.
1. Ein dem Arbeitselement zugewiesener Benutzer ändert seinen Status in den Status, der den Genehmigungsprozess initiiert, und der Genehmigungsprozess beginnt. (Die Person, die den Genehmigungsprozess erstellt hat, hat die Beziehung zwischen dem Status und dem Genehmigungsprozess definiert.)
1. Die benannten genehmigenden Personen erhalten eine Benachrichtigung über den ausstehenden Genehmigungsprozess und überprüfen das Arbeitselement.
1. Der Genehmigungsprozess endet, nachdem die designierten genehmigenden Personen alle Schritte des Prozesses genehmigt haben. Wenn er/sie einen Schritt ablehnt, wird der Status entweder auf einen vordefinierten Status zurückgesetzt oder es wird ein Problem erstellt. (Die Person, die den Genehmigungsprozess erstellt hat, hat definiert, welche dieser automatisierten Schritte nach einer Ablehnung durchgeführt werden.)

**Beispiel** Ein Werbe-Team hat den Status Bereit zum Drucken und einen Genehmigungsprozess namens Designer/ Copywriter Signoff erstellt, die mit diesem Status verknüpft sind. Dieser Genehmigungsprozess wird konfiguriert, um:

* Genehmigung durch den Designer und Werbetexter des Teams verlangen
* Wenn jemand den Status eines Arbeitselements in „Bereit zum Drucken“ ändert, starten

Ein Broschüren-Projektbesitzer hängt den Genehmigungsprozess von Designer/Copywriter Signoff an das Broschüren-Projekt an.

Wenn im Projekt der Status Bereit zum Drucken geändert wird, erhalten Copywriter und Designer Benachrichtigungen, in denen sie aufgefordert werden, das Projekt zu genehmigen oder abzulehnen. Während des Genehmigungsprozesses wird der Status der Projekte, wenn beraten wird, ob sie genehmigt werden sollen oder nicht, als Bereit zum Drucken - Genehmigung ausstehend angezeigt.

Nachdem beide die Broschüre in Workfront genehmigt haben, ändert sich der Projektstatus in Bereit für den Druck.

## Dokumentengenehmigungsprozesse

Dokumentgenehmigungen werden für eine allgemeinere Genehmigung verwendet. Feedback wird im Chat-Format auf der Registerkarte Aktualisierungen erfasst. Sie können die Genehmigungsschaltflächen verwenden, um Änderungen zu genehmigen, abzulehnen oder zu genehmigen.

Informationen zum Hinzufügen von Genehmigern zu einem Dokument nach dem Hochladen in Workfront finden Sie unter [Dokumentgenehmigungen anfordern](../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Genehmigungsprozesse für Korrekturabzüge

Genehmigungen von Korrekturabzügen werden für eine eingehendere Überprüfung verwendet und umfassen im Allgemeinen kompliziertere Workflows. Feedback wird mit Markup-Tools im Proofing Viewer erfasst. Sie können die Genehmigungsschaltflächen verwenden, um Änderungen zu genehmigen, abzulehnen oder zu genehmigen.

Informationen zum Hinzufügen eines automatisierten Workflows zu einem Korrekturabzug und zur Bestimmung bestimmter Benutzer im Workflow als Genehmiger des Korrekturabzugs finden Sie unter [Erstellen eines erweiterten Korrekturabzugs mit einem automatisierten Workflow](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Konfigurieren von Einstellungen für Arbeitselementgenehmigungsprozesse

Als Workfront-Administrator können Sie globale Einstellungen für Arbeitselementgenehmigungsprozesse in Ihrem System konfigurieren. Diese Einstellungen bestimmen verschiedene Regeln für Genehmigungsprozesse, z. B. wie lange eine Genehmigungsentscheidung offen bleiben darf oder wie Sie die Genehmigungsdelegierung in Ihrem System verwalten. Weitere Informationen zu den Einstellungen für den Genehmigungsprozess finden Sie unter [Konfigurieren globaler Genehmigungseinstellungen](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).
