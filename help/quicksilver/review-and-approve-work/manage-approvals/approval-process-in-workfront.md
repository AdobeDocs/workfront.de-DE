---
content-type: overview
product-area: projects
navigation-topic: approvals
title: Übersicht über den Genehmigungsprozess
description: Sie können einen Genehmigungsprozess erstellen und an ein Objekt anhängen, um sicherzustellen, dass bestimmte Benutzer bestimmte Änderungen überprüfen, bevor das Objekt fortgesetzt wird.
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

Sie können einen Genehmigungsprozess erstellen und an ein Objekt anhängen, um sicherzustellen, dass bestimmte Benutzer bestimmte Änderungen überprüfen, bevor das Objekt fortgesetzt wird.

Dies ist für die folgenden Objekttypen in Adobe Workfront verfügbar:

* Arbeitselement (Projekt, Aufgabe oder Problem, Vorlage, Vorlagenaufgabe)
* Dokument
* Korrekturabzug

Dieser Artikel enthält allgemeine Informationen zu Genehmigungsprozessen, die mit Arbeitselementen verknüpft sind.
Anweisungen zum Erstellen eines Genehmigungsprozesses finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Arten von Genehmigungsverfahren für Arbeitselemente

Wenn Sie Adobe Workfront-Administrator oder Benutzer mit Administratorzugriff auf Genehmigungsprozesse sind, können Sie die folgenden Genehmigungsprozesse für Projekte, Aufgaben und Probleme erstellen:

* **Globaler Genehmigungsprozess auf Systemebene**: Benutzer können diese an Folgendes anhängen:

   * Ein Projekt, eine Aufgabe oder ein Problem im Abschnitt Genehmigungen
   * Im Feld &quot;Projekt bearbeiten&quot;im Bereich &quot;Task Default Approval Process&quot;
   * Im Bereich Warteschlangendetails oder Warteschlangenthema eines Projekts in den Bereichen Standardgenehmigungsprozess . Das Projekt muss als Anforderungswarteschlange aktiviert sein.

* **Globale Validierung auf Gruppenebene**: Benutzer können diese an Folgendes anhängen:

   * Ein Projekt, eine Aufgabe oder ein Problem, das/das zu der Gruppe gehört, die dem Genehmigungsprozess im Abschnitt &quot;Genehmigungen&quot;zugeordnet ist
   * Im Feld &quot;Projekt bearbeiten&quot;im Bereich &quot;Task Default Approval Process&quot;für ein Projekt, das zu der Gruppe gehört, die dem Genehmigungsprozess zugeordnet ist
   * Im Bereich Warteschlangendetails oder Warteschlangenthema eines Projekts in den Bereichen Standardgenehmigungsprozess . Das Projekt muss als Anforderungswarteschlange aktiviert werden und zu der Gruppe gehören, die dem Genehmigungsprozess zugeordnet ist.

  Informationen zum Erstellen eines Genehmigungsprozesses auf System- oder Gruppenebene finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

* **Ein Validierungsprozess für die einmalige Verwendung**: Zur Verwendung mit einem einzelnen Projekt, einer Aufgabe, einem Problem, einer Vorlage oder einer Vorlagenaufgabe. Dieser Validierungsprozess betrifft nur das zugehörige Objekt und kann nicht mit anderen Objekten verknüpft werden.

  Informationen zum Erstellen eines Validierungsprozesses für die einmalige Verwendung finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

>[!NOTE]
>
>In diesem Artikel wird der Begriff &quot;globaler Genehmigungsprozess&quot;verwendet, um von &quot;Genehmigungsprozess für einmalige Verwendung&quot;zu unterscheiden. Ein globaler Genehmigungsprozess kann wiederholt verwendet werden.
>
>Der Begriff &quot;Globaler Validierungsprozess auf Gruppenebene&quot;bezieht sich auf einen Validierungsprozess, der wiederholt für Elemente und mit Status verwendet werden kann, die nur einer bestimmten Gruppe zugeordnet sind.

Informationen zum Erstellen eines Validierungsprozesses auf Systemebene oder eines Validierungsprozesses auf Gruppenebene finden Sie unter [Erstellen eines Validierungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Überlegungen zu Validierungsprozessen

* Sie müssen das Projekt, die Aufgabe, das Problem, die Vorlage oder die Vorlagenaufgabe erstellen, bevor ihnen der Genehmigungsprozess zugeordnet werden kann.
* Ein Genehmigungsprozess ist immer mit zwei wesentlichen Elementen verknüpft:

   * Jeder Validierungsprozess entspricht einem bestimmten Arbeitselement-Status im Workfront-System. Wenn Sie den Status eines Arbeitselements ändern, muss bei einer angehängten Genehmigung für diesen Status die Statusänderung bestätigt werden, bevor dem Element der neue Status zugewiesen werden kann.

     >[!TIP]
     >
     >
     >   
     >   
     >   * Sie können eine Gruppengenehmigung mit einem Status auf globaler oder Gruppenebene verknüpfen.
     >   * Sie können den Status eines Elements, das einen Validierungsprozess verwendet, nicht in einen anderen Status ändern als den, der dem Validierungsprozess zugeordnet ist.
     >   
     >   
     >     Wenn Sie beispielsweise eine Aufgabengenehmigung mit dem Status In Bearbeitung haben, ändert die Aufgabe ihren Status automatisch in Wird ausgeführt , wenn die Genehmigung erteilt wird. Der Status kann nicht automatisch in Abgeschlossen oder in einen anderen Status geändert werden, der nicht mit der Genehmigung verknüpft ist.
     >   
     >   
     >

   * Bei den mit einem Genehmigungsprozess verknüpften Entitäten kann es sich um Benutzer, Vorgangsrollen oder Teams handeln. Die Benutzer sind letztendlich dafür verantwortlich, die Genehmigung anzunehmen oder abzulehnen. Sie können Benutzern, die eine bestimmte Rolle im Projekt erfüllen, Genehmigungen zuweisen. Sie können beispielsweise einem Projekteigentümer oder Sponsor eine Genehmigung zuweisen. Weitere Informationen finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

     Die folgenden Szenarien existieren:

      * Wenn Sie Auftrags-Rollen eine Genehmigung zuweisen, kann jeder Benutzer im Projektteam, der mit der Auftragsrolle verknüpft ist, eine Entscheidung über die Genehmigung treffen. Die mit der Genehmigung verknüpfte Rolle kann entweder ihre Primäre Rolle oder eine beliebige andere Rolle sein.

        Weitere Informationen zum Projektteam finden Sie unter [Übersicht über das Projektteam](../../manage-work/projects/planning-a-project/project-team-overview.md).

      * Wenn Sie einem Team eine Genehmigung zuweisen, kann jedes Mitglied dieses Teams eine Entscheidung über die Genehmigung treffen. Das mit der Validierung verbundene Team kann entweder sein Startseiten-Team oder eines seiner anderen Teams sein.

        Informationen zu den Rollen und Teams eines Benutzers finden Sie unter [Profil eines Benutzers bearbeiten](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Wenn Sie ein Arbeitselement erstellen, wird ihm nicht automatisch ein Genehmigungsprozess angehängt. Sie müssen eines manuell anhängen, wenn Sie eines verwenden möchten. Informationen zum Anhängen eines Genehmigungsprozesses an ein Element finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).
* Der Workfront-Administrator oder ein Benutzer mit Administratorzugriff auf Genehmigungsprozesse kann globale Genehmigungsprozesse auf Systemebene erstellen, die im gesamten System verwendet werden können. Ein Gruppenadministrator mit Administratorrechten für Genehmigungsprozesse kann einen globalen Validierungsprozess auf Gruppenebene erstellen, der nur von einer bestimmten Gruppe verwendet werden kann, die er verwaltet.
* Wenn Sie keinen vordefinierten globalen Genehmigungsprozess auf Systemebene oder Gruppenebene für ein Arbeitselement verwenden möchten, können Sie einen Validierungsprozess für die einmalige Verwendung erstellen und an ihn anhängen, wenn Sie über Verwaltungsberechtigungen verfügen, um das Objekt zu verwalten, für das Sie den Genehmigungsprozess anhängen möchten.

  >[!NOTE]
  >
  >Sie können einen einmaligen Genehmigungsprozess nur einmal für das spezifische Element verwenden, für das er erstellt wurde. Sie können globale Status sowie Gruppenstatus für Genehmigungsprozesse mit einmaliger Verwendung für Projekte, Aufgaben, Probleme, Vorlagen und Vorlagenaufgaben zuordnen.

* Wenn Sie einen Validierungsprozess auf Gruppenebene mithilfe benutzerdefinierter Status auf Gruppenebene an ein Element anhängen, kann das Ändern der Gruppe des Projekts zu einem Konflikt zwischen dem Genehmigungsstatus der vorherigen Gruppe und den auf Systemebene vorhandenen Status führen. Erwägen Sie, die Genehmigungsprozesse auf Gruppenebene für das Projekt oder dessen Aufgaben oder Probleme zu entfernen, bevor Sie die Gruppe aktualisieren. Informationen zum Erstellen von Genehmigungsprozessen auf Gruppenebene finden Sie unter [Genehmigungsprozesse auf Gruppenebene](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md). Informationen zum Erstellen benutzerdefinierter Gruppenstatus finden Sie unter [Erstellen oder Bearbeiten eines Gruppenstatus](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md). Informationen zum Aktualisieren der Gruppe eines Projekts finden Sie unter [Projekte bearbeiten](../../manage-work/projects/manage-projects/edit-projects.md).

## Genehmigungsprozess-Workflow

In diesem Abschnitt wird Folgendes zur Genehmigung von Arbeitselementen erläutert:

* [Wie Genehmigungsprozesse auf Status basieren](#how-approval-processes-rely-on-statuses)
* [Verwendung eines Validierungsprozesses in einem typischen Workflow](#how-a-typical-workflow-uses-an-approval-process)

### Wie Validierungsprozesse auf Status basieren {#how-approval-processes-rely-on-statuses}

Wenn Sie einem Genehmigungsprozess einen Status anhängen, wird sichergestellt, dass der Artikel in der richtigen Reihenfolge durch die Abteilungen geleitet wird.

**Beispiel:** Sie können einen Genehmigungsprozess an den Status der Marketingabteilung anhängen, der eine Genehmigung durch die Finanzabteilung erfordert. Wenn dann jemand den Status für ein Arbeitselement in &quot;Marketing-Abteilung&quot;ändert, kann das Element erst dann in diese Abteilung verschoben werden, wenn die Finanzabteilung es abmeldet.

Weitere Informationen zum Status von Arbeitselementen finden Sie in den folgenden Artikeln:

* [Zugriff auf die Liste der Systemprojektstatus](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)
* [Zugriff auf die Liste der Systemaufgabenstatus](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)
* [Zugriff auf die Liste der Systemfehlerstatus](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)

### Verwendung eines Validierungsprozesses in einem typischen Workflow {#how-a-typical-workflow-uses-an-approval-process}

Das folgende Szenario zeigt, wie ein Genehmigungsprozess Benutzern dabei hilft, die Arbeit eines Workfront-Objekts zu validieren, während ein Workflow mit mehreren Schritten in dieser Reihenfolge durchläuft:

1. Der Workfront-Administrator oder ein Benutzer mit Administratorzugriff auf Genehmigungsprozesse erstellt einen Genehmigungsprozess für ein Projekt, eine Aufgabe oder ein Problem.

   >[!NOTE]
   >
   >Sie können Projektgenehmigungsprozesse an eine Vorlage anhängen und Aufgabengenehmigungsprozesse an eine Vorlagenaufgabe. Wenn Sie dies tun und jemand die Vorlage zum Erstellen eines Projekts verwendet, wird der Genehmigungsprozess zu einem Projekt- bzw. Aufgabenvalidierungsprozess. Ein an eine Vorlage oder Vorlagenaufgabe angehängter Genehmigungsprozess für eine einmalige Verwendung bleibt ein einmaliger Genehmigungsprozess für Projekte und Aufgaben.

1. Ein Benutzer mit der Berechtigung &quot;Verwalten&quot;für das Projekt, die Aufgabe oder das Problem hängt den Genehmigungsprozess an das Element an oder erstellt eine Einzelverwendungsgenehmigung für das Element.
1. Ein dem Arbeitselement zugewiesener Benutzer ändert seinen Status in den Status, der den Genehmigungsprozess startet und der Genehmigungsprozess beginnt. (Die Person, die den Genehmigungsprozess erstellt hat, hat die Beziehung zwischen dem Status und dem Genehmigungsprozess definiert.)
1. Die benannten Genehmiger erhalten eine Benachrichtigung über den Prozess der ausstehenden Genehmigung und überprüfen das Arbeitselement.
1. Der Genehmigungsprozess endet, nachdem die vorgesehenen Genehmiger alle Schritte des Prozesses genehmigt haben. Wenn sie einen Schritt ablehnen, wird der Status entweder auf einen vordefinierten Status zurückgesetzt oder es wird ein Problem erstellt. (Die Person, die den Validierungsprozess erstellt hat, hat definiert, welche dieser automatisierten Schritte nach einer Zurückweisung durchgeführt werden.)

**Beispiel:** Ein Werbeteam hat den Status Bereit zum Drucken und einen Genehmigungsprozess mit dem Namen Designer/Copywriter Signoff erstellt, dass sie diesem Status zugeordnet sind. Dieser Validierungsprozess ist konfiguriert für:

* Genehmigung durch Designer und Kopierer des Teams erforderlich
* Initiieren, wenn jemand den Status eines Arbeitselements in &quot;Bereit zum Drucken&quot;ändert

Ein Broschürenprojektbesitzer hängt den Genehmigungsprozess von Designer/Copywriter Signoff an das Prospektprojekt an.

Wenn jemand im Projekt den Status in Druckbereit ändert, erhält der Werbetexter und der Designer Benachrichtigungen, die ihn auffordern, ihn zu genehmigen oder abzulehnen. Während des Genehmigungsprozesses wird der Status der Projekte bei der Entscheidung, ob sie genehmigt werden sollen oder nicht, als Druckbereit - Genehmigung ausstehend angezeigt.

Nachdem beide die Broschüre in Workfront genehmigt haben, ändert sich der Projektstatus in Druckbereit .

## Dokumentgenehmigungsverfahren

Dokumentgenehmigungen werden für eine allgemeinere Genehmigung verwendet. Das Feedback wird im Chat-Format auf der Registerkarte Updates erfasst. Mithilfe der Validierungsschaltflächen können Sie Änderungen genehmigen, ablehnen oder genehmigen.

Informationen zum Hinzufügen von Genehmigern zu einem Dokument nach dem Hochladen in Workfront finden Sie unter [Dokumentgenehmigungen anfordern](../../review-and-approve-work/manage-approvals/request-document-approvals.md).

## Validierungsprozesse

Testversandgenehmigungen werden für eine tiefere Überprüfung verwendet und umfassen im Allgemeinen kompliziertere Workflows. Feedback wird mit Markup-Tools im Testversand-Viewer erfasst. Mithilfe der Validierungsschaltflächen können Sie Änderungen genehmigen, ablehnen oder genehmigen.

Informationen zum Hinzufügen eines automatisierten Workflows zu einem Dokumententest und zum Ausweisen bestimmter Benutzer im Workflow als Genehmiger für den Testversand finden Sie unter [Erstellen eines erweiterten Testversands mit einem automatisierten Workflow](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Konfigurieren von Einstellungen für Vorgänge zur Genehmigung von Arbeitselementen

Als Workfront-Administrator können Sie globale Einstellungen für Vorgänge zur Genehmigung von Arbeitselementen in Ihrem System konfigurieren. Diese Einstellungen bestimmen verschiedene Regeln für Genehmigungsprozesse, z. B. wie lange eine Genehmigungsentscheidung offen bleiben soll oder wie Sie die Validierungsdelegierung in Ihrem System verwalten. Weitere Informationen zu den Einstellungen für den Genehmigungsprozess finden Sie unter [Globale Genehmigungseinstellungen konfigurieren](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md).
