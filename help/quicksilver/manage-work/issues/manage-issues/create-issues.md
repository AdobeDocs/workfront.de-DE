---
product-area: projects
navigation-topic: manage-issues
title: Anfragen erstellen
description: Bei der Arbeit an einem Projekt kann es vorkommen, dass unerwartete Ereignisse auftreten. Sie können diese unerwarteten Ereignisse als Probleme für ein bestimmtes Projekt oder eine Aufgabe protokollieren. Benutzende mit entsprechender Zugriffsberechtigung können den Status von Problemen während des Projekts oder der Aufgabe anzeigen und überwachen und sich den Fortschritt ansehen. Dadurch entfallen lange E-Mail-Ketten oder Statusbesprechungen. Im Gegensatz zu Aufgaben, bei denen es sich um geplante Ereignisse handelt, stellen Probleme ungeplante Arbeitselemente in Adobe Workfront dar.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: 0542587bb3254dec5664de493c1c321528cf7f3e
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 0%

---

# Probleme erstellen

<!--Audited: 08/2025-->

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> 

<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span> 

-->

Bei der Arbeit an einem Projekt kann es vorkommen, dass unerwartete Ereignisse auftreten. Sie können diese unerwarteten Ereignisse als Probleme für ein bestimmtes Projekt oder eine Aufgabe protokollieren. Benutzende mit entsprechender Zugriffsberechtigung können den Status von Problemen während des Projekts oder der Aufgabe anzeigen und überwachen und sich den Fortschritt ansehen. Dadurch entfallen lange E-Mail-Ketten oder Statusbesprechungen. Im Gegensatz zu Aufgaben, bei denen es sich um geplante Ereignisse handelt, stellen Probleme ungeplante Arbeitselemente in Adobe Workfront dar.

Sie können auch Probleme zu Projekten als Anfragen hinzufügen. Weitere Informationen finden Sie unter [Erstellen und Senden von Adobe Workfront-Anfragen](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>Probleme und Anfragen werden in Workfront synonym verwendet. Sie können Probleme sowohl bei Projekten als auch bei Aufgaben aufzeichnen, um unvorhergesehene Arbeiten anzuzeigen, die bearbeitet werden müssen. Sie können auch Anfragen senden, die als Probleme in einem Projekt aufgezeichnet werden, das als Anfrage-Warteschlange bezeichnet wird.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <td>
   <ul><li>Mitwirkender oder höher</li>
   <li>Leicht oder höher, um Probleme im Abschnitt „Probleme“ einer Aufgabe oder eines Projekts zu bearbeiten</li></ul>
   Oder
   <ul><li>Anfrage oder höher</li> <li>Überprüfen Sie oder höher, um Probleme im Abschnitt „Probleme“ einer Aufgabe oder eines Projekts zu bearbeiten</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Anfragen bearbeiten</p> <p>Anzeigen oder Hochladen des Zugriffs auf Projekte und Aufgaben</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Tragen Sie zu oder höheren Berechtigungen mit der Möglichkeit bei, Probleme zu der Aufgabe oder dem Projekt hinzuzufügen, in dem Sie das Problem erstellen</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

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
   <td> <p>New license:</p>
   <ul><li>Contributor or higher</li>
   <li>Light or higher to edit issues in the Issues section of a task or project</li></ul>
   <p>Current license:</p>
  <ul><li>Request or higher</li> <li>Review or higher to edit issues in the Issues section of a task or a project</li></ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Issues</p> <p>View or higher access to Projects and Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute or higher permissions with ability to Add Issues to the task or project where you create the issue</p> </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

<!--
(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## Einschränkungen beim Erstellen von Problemen

Wenn Sie über die richtigen Zugriffsrechte und Berechtigungen verfügen, können Sie Probleme für ein Projekt oder eine Aufgabe erstellen. In den folgenden Fällen können Sie jedoch möglicherweise keine Probleme erstellen:

* Ihr Workfront-Administrator oder ein Gruppenadministrator muss das Hinzufügen von Problemen zu einem Projekt aktivieren, das sich in Ihren Projektvoreinstellungen im Status Abgeschlossen oder Inaktiv befindet. Informationen zum Festlegen von Projektvoreinstellungen finden Sie [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Sie können keine Probleme zu einem Projekt hinzufügen, das sich in der Phase „Ausstehende Genehmigungen“ befindet.

## Neues Anfrageformular vorbereiten

Ihr Unternehmen sollte über einen klar definierten Prozess verfügen, wann und wie ein Problem aufgezeichnet wird. Wenn Sie diesen Prozess konfigurieren, besteht der erste Schritt darin, das Formular zu erstellen, das zum Senden eines Problems erforderlich ist.

Benutzer können Probleme wie folgt zu einem Projekt hinzufügen:

* Direktes Hinzufügen zu Aufgaben und Projekten.
* An eine Anfrage-Warteschlange senden.

Das Formular Neues Problem kann wichtige Informationen enthalten, die bei der schnellen Lösung des Problems hilfreich sind.

Sie können das Formular „Neues Problem“ so konfigurieren, dass beim Hinzufügen von Problemen zum Projekt oder zu dessen Aufgaben durch Benutzer die folgenden Informationen einbezogen werden:

* Benutzerdefinierte Felder
* Genehmigungen
* Zuweisungen (Routingregeln)

Die Felder für neue Anfragen oder Anfragen werden im Abschnitt „Warteschlangendetails“ des Projekts definiert, in dem die Probleme protokolliert werden.

Informationen zum Konfigurieren des Abschnitts „Warteschlangendetails“ des Projekts finden Sie unter [Erstellen einer Anfragewarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Informationen zum Erstellen von Problemen durch Senden an eine Anfrage-Warteschlange finden Sie [ Abschnitt „Erstellen von Problemen durch Eingabe einer ](#create-issues-by-entering-a-new-request) Anfrage“ in diesem Artikel.

## Erstellen von Problemen in einer Aufgabe oder einem Projekt mithilfe der Schaltfläche „Neues Problem“

Nachdem Sie die Felder eines neuen Anfrageformulars in Ihrem Projekt definiert haben, können Sie mit der Erstellung von Anfragen beginnen.

So erstellen Sie ein Problem bei einer Aufgabe oder einem Projekt:

1. Wechseln Sie zu einem Projekt, in dem Sie das Problem erstellen möchten.
1. (Optional) Wenn Sie das Problem für eine Aufgabe protokollieren möchten, wechseln Sie zum Bereich **Aufgaben** und klicken Sie auf den Namen einer Aufgabe.
1. Klicken Sie auf **Abschnitt** Probleme“.

   Die Liste der Projektprobleme wird angezeigt

1. Klicken Sie **oben** der Problemliste auf „Neues Problem“.
Das Feld „Neues Problem“ wird angezeigt.

   ![Neues Problemfeld](assets/new-issue-box-matches-new-request-ui.png)

1. (Bedingt) Wenn der Projektersteller Warteschlangenthemen oder Themengruppen für das Projekt erstellt hat, werden sie zum neuen Anfrageformular hinzugefügt. Geben Sie **Themengruppe** oder das **Warteschlangenthema** Ihres neuen Problems an. Themengruppen und Warteschlangenthemen haben Namen, die an Ihre Umgebung angepasst wurden.\
   Weitere Informationen zum Erstellen von Themengruppen finden Sie unter [Themengruppen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Weitere Informationen zum Erstellen von Warteschlangenthemen finden Sie unter [Warteschlangenthemen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   * Wenn für das Projekt nur ein Warteschlangenthema festgelegt ist, wird es automatisch angezeigt.
   * Wenn die Themengruppe keine Warteschlangenthemen oder Themengruppen enthält, ist in der Dropdown-Liste Themengruppe nichts verfügbar.

1. Fügen Sie den Namen des Problems in das Feld **Betreff** ein und fügen Sie dann **Beschreibung** hinzu.

1. (Bedingt) Wenn der Projektersteller zugelassen hat, dass das Feld **Anfragetyp** im Formular „Neues Problem“ angezeigt wird, wählen Sie den Typ Ihres Problems aus den folgenden Optionen aus:

   * Fehlerbericht
   * Änderungsanforderung
   * Problem
   * Anfrage\
     Je nachdem, wie Ihr Workfront-Administrator Ihre Projektvoreinstellungen konfiguriert hat, können die Namen der Problemtypen für Sie unterschiedlich sein.

   >[!TIP]
   >
   >Die Anfragetypen müssen in den Warteschlangendetails und beim Erstellen des Warteschlangenthemas aktiviert werden, damit sie als Auswahl im Formular „Neues Problem“ angezeigt werden. Weitere Informationen finden Sie in den folgenden Artikeln:
   >* [Anfrage-Warteschlange erstellen](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [Warteschlangenthemen erstellen](../../requests/create-and-manage-request-queues/create-queue-topics.md)

1. Bitte die im Formular &quot;**Problem“ verfügbaren Felder**. Weitere Informationen zu den Feldern, die verfügbar sind, wenn Sie ein neues Problem eingeben, finden Sie unter [Probleme bearbeiten](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >Nicht alle problembezogenen Felder sind im Formular „Neues Problem“ verfügbar. Der Projektersteller aktiviert die Felder, die beim Erstellen eines Problems verfügbar sind, wenn er den Bereich Warteschlangendetails des Projekts definiert. Weitere Informationen finden Sie unter [Anforderungswarteschlange erstellen](../../requests/create-and-manage-request-queues/create-request-queue.md).


1. (Bedingt) Wenn die Warteschlangenthemen mit einem benutzerdefinierten Formular verknüpft sind, wird dieses benutzerdefinierte Formular im Formular &quot;**Problem“**.\
   Oder\
   Wenn das Projekt über den Bereich Warteschlangendetails mit einem benutzerdefinierten Problem-Formular verknüpft ist, wird das Formular im Formular **Neues Problem** nach den standardmäßigen Workfront-Feldern angezeigt.

   Weitere Informationen finden Sie unter [Erstellen einer Anfrage-Warteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Klicken Sie auf **Senden**.

   Probleme können mehreren Benutzern, Aufgabengebieten oder einem Team zugewiesen werden. Weitere Informationen zum Zuweisen und Verwalten von Anfragen finden Sie unter [Arbeiten und Teamanfragen verwalten](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).


## Probleme bei einer Aufgabe oder einem Projekt inline erstellen

>[!IMPORTANT]
>
>Der Projektbesitzer muss beim Definieren von Problemeinstellungen für das Projekt &quot;**Benutzern erlauben, Probleme** inline hinzuzufügen“ aktivieren, bevor Sie Probleme inline zum Projekt oder zu den Aufgaben hinzufügen können. Informationen zum Konfigurieren von Problemeinstellungen für ein Projekt finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).
>

Wenn Sie mehrere Probleme schnell hinzufügen möchten, können Sie Probleme für eine Aufgabe oder ein Projekt inline erstellen, indem Sie sie zu einer Liste von Problemen hinzufügen.

>[!NOTE]
>
>Wenn Sie Probleme inline hinzufügen, wendet Workfront das Formular „Neues Problem“ nicht auf die neuen Probleme an. Es wird nicht empfohlen, Probleme inline hinzuzufügen, wenn Sie möchten, dass Benutzende beim Eingeben von Problemen bestimmte Informationen angeben. Dies kann sich negativ auf das Problem-Reporting und später auf die Fähigkeit des/r Benutzenden, der/die dem Problem zugewiesen wurde, über alle Informationen zu verfügen, die zur Lösung des Problems erforderlich sind, auswirken.

So erstellen Sie Probleme inline:

1. Wechseln Sie zu einem Projekt, in dem Sie das Problem erstellen möchten.
1. (Optional) Wenn Sie das Problem für eine Aufgabe protokollieren möchten, gehen Sie zum Abschnitt **Aufgaben** und klicken Sie auf den Namen einer Aufgabe.
1. Klicken Sie im linken Bedienfeld **Abschnitt** Probleme“.
1. Klicken **unten** der Problemliste auf „Weitere Probleme hinzufügen“.

   Im Abschnitt „Probleme“ wird in der Problemliste eine neue Zeile erstellt.

   >[!TIP]
   >
   >Diese Option ist abgeblendet, wenn die Einstellung Benutzenden erlauben, Probleme inline hinzuzufügen im Feld Projekt bearbeiten deaktiviert ist. Weitere Informationen finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![Schaltfläche „Weitere Probleme hinzufügen“](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. Beginnen Sie, den Namen des Problems in das Namensfeld einzugeben, und fügen Sie dann weitere Informationen über das Problem inline hinzu.

   >[!TIP]
   >
   >Die Felder, die inline bearbeitet werden können, werden durch die Ansicht verfügbar gemacht, die Sie auf Ihre Problemliste anwenden. Möglicherweise können Sie den folgenden Feldtyp nicht inline bearbeiten:
   >   
   >* Felder, die zu einem anderen Objekt gehören
   >* Felder, auf die kein Bearbeitungszugriff besteht
   >* Felder, die Berechnungen sind und von Workfront automatisch aktualisiert werden

1. Klicken Sie auf die Eingabetaste, um die Inline-Bearbeitung abzuschließen, und fügen Sie das Problem dem Projekt oder der Aufgabe hinzu.

## Probleme durch Eingabe einer neuen Anfrage erstellen {#create-issues-by-entering-a-new-request}

Sie können Projekte als Empfänger für Probleme festlegen. Diese Projekttypen werden in Workfront als Anforderungswarteschlangen bezeichnet. Sie können auf Anfrage-Warteschlangen über den Bereich Anfragen im Hauptmenü zugreifen.

>[!TIP]
>
>Die Begriffe „Problem“ und „Anfrage“ sind in Workfront austauschbar.

Weitere Informationen zum Einrichten von Projekten als Anforderungswarteschlangen für den Empfang von Problemen finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). Informationen zum Senden von Anfragen finden Sie unter [Erstellen und Senden von Adobe Workfront-Anfragen](../../../manage-work/requests/create-requests/create-submit-requests.md).
