---
product-area: projects
navigation-topic: manage-issues
title: Erstellen von Problemen
description: Bei der Arbeit an einem Projekt können Sie feststellen, dass unerwartete Ereignisse auftreten. Sie können diese unerwarteten Ereignisse als Probleme für ein bestimmtes Projekt oder eine Aufgabe protokollieren. Benutzer mit dem entsprechenden Zugriff können den Status von Problemen im Zuge des Fertigstellungsprozesses des Projekts oder der Aufgabe anzeigen und überwachen, sodass längere E-Mail-Ketten oder Statussitzungen nicht mehr erforderlich sind. Im Gegensatz zu Aufgaben, bei denen es sich um geplante Ereignisse handelt, stellen Probleme ungeplante Arbeitselemente in Adobe Workfront dar.
author: Alina
feature: Work Management
topic: Collaboration
role: User
exl-id: 2a4488fb-fe2f-422a-887c-996f6367afc5
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '1522'
ht-degree: 0%

---

# Erstellen von Problemen

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](../../../administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> 

<span class="preview">For information about the current release, see [Fourth Quarter 2023 release overview](../../../product-announcements/product-releases/23-q4-release-activity/23-q4-release-overview.md). </span> 

-->

Bei der Arbeit an einem Projekt können Sie feststellen, dass unerwartete Ereignisse auftreten. Sie können diese unerwarteten Ereignisse als Probleme für ein bestimmtes Projekt oder eine Aufgabe protokollieren. Benutzer mit dem entsprechenden Zugriff können den Status von Problemen im Zuge des Fertigstellungsprozesses des Projekts oder der Aufgabe anzeigen und überwachen, sodass längere E-Mail-Ketten oder Statussitzungen nicht mehr erforderlich sind. Im Gegensatz zu Aufgaben, bei denen es sich um geplante Ereignisse handelt, stellen Probleme ungeplante Arbeitselemente in Adobe Workfront dar.

Sie können Projekte auch als Anfragen hinzufügen. Weitere Informationen finden Sie unter [Erstellen und Senden von Adobe Workfront-Anforderungen](../../../manage-work/requests/create-requests/create-submit-requests.md).

>[!TIP]
>
>Probleme und Anforderungen werden in Workfront synonym verwendet. Sie können Probleme sowohl bei Projekten als auch bei Aufgaben aufzeichnen, um auf unvorhergesehene Arbeit hinzuweisen, die behoben werden muss. Sie können auch Anfragen senden, die als Probleme in einem Projekt aufgezeichnet werden, das als Anforderungswarteschlange bezeichnet wird.

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
   <td> <p>Überprüfen oder höher zum Hinzufügen von Problemen zu einem Projekt oder einer Aufgabe</p> <p>Anfrage oder höher zum Hinzufügen von Problemen als Anforderungen mithilfe einer Anforderungswarteschlange.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Probleme bearbeiten</p> <p>Anzeigen oder höherer Zugriff auf Projekte und Aufgaben</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen zum Zugriff auf Probleme in Ihrer Zugriffsebene finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Zugriff auf Probleme gewähren</a>. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Beitragen Sie oder höhere Berechtigungen mit der Möglichkeit, Probleme zur Aufgabe oder zum Projekt hinzuzufügen, in der Sie das Problem erstellen</p> <p> Informationen zum Gewähren von Berechtigungen für Probleme finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Problem freigeben </a></p> <p>Informationen zum Anfordern zusätzlicher Berechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

<!--
(NOTE: in NWE Requestors CAN see the Issues tab on a project but in classic they cannot! However, even when they DO see it, they cannot enter the issues - logged this issue for it but they might decide not to fix it: https://hub.workfront.com/issue/60181e28000058980cce29597185b2d6/updates?email-source=comm)</p>
-->

## Einschränkungen beim Erstellen von Problemen

Wenn Sie über den richtigen Zugriff und die richtigen Berechtigungen verfügen, können Sie Probleme für ein Projekt oder eine Aufgabe erstellen. In den folgenden Fällen können Sie jedoch möglicherweise keine Probleme erstellen:

* Der Workfront-Administrator oder ein Gruppenadministrator muss das Hinzufügen von Problemen zu einem Projekt aktivieren, das sich im Bereich &quot;Projekteinstellungen&quot;im Status &quot;Abgeschlossen&quot;oder &quot;Dead&quot;befindet. Weitere Informationen zum Festlegen von Projektvoreinstellungen finden Sie unter [Systemweite Projektvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
* Sie können einem Projekt, das sich in &quot;Ausstehende Genehmigung&quot;befindet, keine Probleme hinzufügen.

## Formular &quot;Neues Problem vorbereiten&quot;

Ihr Unternehmen sollte über einen klar definierten Prozess verfügen, in dem festgelegt wird, wann und wie ein Problem aufgezeichnet wird. Wenn Sie diesen Prozess konfigurieren, besteht der erste Schritt darin, das Formular zu erstellen, das zum Senden eines Problems erforderlich ist. Unabhängig davon, ob Sie zulassen, dass Aufgaben und Projekte direkt hinzugefügt werden, oder ob Sie Anforderungswarteschlangen haben, in denen Probleme gesendet werden, können Sie definieren, welche Workfront-Felder sowie welche benutzerdefinierten Felder für Benutzer verfügbar sind, wenn sie neue Probleme senden und ausgefüllt werden müssen. Das Formular Neues Problem kann wichtige Informationen enthalten, die bei der schnellen Lösung des Problems hilfreich sind.

Die Felder für die neuen Probleme in einem Projekt werden im Abschnitt Warteschlangendetails des Projekts definiert, in dem die Probleme protokolliert werden. Weitere Informationen zum Konfigurieren des Abschnitts &quot;Warteschlangendetails&quot;des Projekts finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Informationen zum Erstellen von Problemen durch Senden an eine Anforderungswarteschlange finden Sie in der [Erstellen von Problemen durch Eingabe einer neuen Anforderung](#create-issues-by-entering-a-new-request) in diesem Artikel beschrieben.

## Erstellen von Problemen in einer Aufgabe oder einem Projekt mithilfe der Schaltfläche &quot;Neues Problem&quot;

Nachdem Sie die Felder eines neuen Ausgabedarstellungsformulars in Ihrem Projekt definiert haben, können Sie mit der Erstellung von Problemen beginnen.

<!-- OLD UI: redesigned on Oct 26, 2023:

Creating issues differs depending on which environment you choose to create the issue. 

### Create issues on a task or project using the New Issue button in the Production environment

To create an issue on a task or a project:

1. Go to a project where you want to create the issue. 
1. (Optional) If you want to log the issue for a task, go to the **Tasks** area, then click the name of a task. 
1. Click the **Issues** section.

   
1. Click **New Issue**.

  

1. (Conditional) If the project creator created Queue Topics or Topic Groups on the project they are added to the new issue form. Specify the **Topic Group** or the **Queue Topic** of your new issue. Topic Groups and Queue Topics have names customized to your environment.  
   For more information about creating Topic Groups, see [Create Topic Groups](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). For more information about creating Queue Topics, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   ![](assets/new-issue-screen-when-creating-issue-from-list-project-level-nwe-350x422.png)

   * If there is only one Queue Topic set on the project, it is displayed automatically.
   * If the Topic Group does not have any Queue Topics or Topic Groups under it, nothing is available in the Topic Group drop-down.

1. (Conditional) If the project creator allowed for the **Request Type** field to display on the New Issue form, select the type of your issue from the following options:

   * Bug Report
   * Change Order
   * Issue
   * Request  
     Depending on how your Workfront administrator has configured your Project Preferences, the names of the issue types might be different for you. 

   >[!TIP]
   >
   >The Request Types must be enabled in the Queue Details and as well as when creating the Queue Topic to display as a selection in the New Issue form. For information, see the following articles: 
   >* [Create a Request Queue](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [Create Queue Topics](../../requests/create-and-manage-request-queues/create-queue-topics.md)


1. Add a name for the new issue in the **Issue Name** field. 
1. Continue specifying the fields available in the **New Issue** form. For more information about the fields available as you enter a new issue, see [Edit issues](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >Not all the issue-related fields are available in the New Issue form. The project creator enables the fields available when creating an issue when they define the Queue Details area of the project. For more information, see [Create a Requests Queue](../../requests/create-and-manage-request-queues/create-request-queue.md). 


1. (Conditional) If the Queue Topics are associated with a custom form, that custom form will display in the **New Issue** form.  
   Or  
   If the project is associated with an issue custom form through the Queue Details area, the form displays in the **New Issue** form, after the default Workfront fields.

   For information, see [Create a Request Queue](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Click **Save New Issue.**

Issues can be assigned to multiple users, job roles or to a team. For more information about assigning and managing requests, see [Manage work and team requests](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).

<!--When this is coming to Production, remove the "Production" section above and replace it with the following content:
-->

So erstellen Sie ein Problem für eine Aufgabe oder ein Projekt:

1. Gehen Sie zu einem Projekt, in dem Sie das Problem erstellen möchten.
1. (Optional) Wenn Sie das Problem für eine Aufgabe protokollieren möchten, navigieren Sie zum **Aufgaben** und klicken Sie auf den Namen einer Aufgabe.
1. Klicken Sie auf **Probleme** Abschnitt.

   Die Liste der Projektprobleme wird angezeigt

1. Klicks **Neues Problem** oben in der Problemliste.
Das Feld Neues Problem wird angezeigt.

   ![](assets/new-issue-box-matches-new-request-ui.png)

1. (Bedingt) Wenn der Projektersteller Warteschlangenthemen oder Themengruppen für das Projekt erstellt hat, werden sie zum neuen Ausstellungsformular hinzugefügt. Geben Sie die **Themengruppe** oder **Warteschlangenthema** Ihres neuen Problems. Für Themengruppen und Warteschlangenthemen wurden Namen an Ihre Umgebung angepasst.\
   Weitere Informationen zum Erstellen von Themengruppen finden Sie unter [Themengruppen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md). Weitere Informationen zum Erstellen von Warteschlangenthemen finden Sie unter [Erstellen von Warteschlangenthemen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   * Wenn im Projekt nur ein Queue-Thema festgelegt ist, wird es automatisch angezeigt.
   * Wenn die Themengruppe keine Warteschlangenthemen oder Themengruppen darunter enthält, ist nichts in der Dropdown-Liste Themengruppe verfügbar.

1. Fügen Sie den Namen des Problems im **Betreff** ein Feld und fügen Sie dann eine **Beschreibung**.

1. (Bedingt) Wenn der Projektersteller für die **Anfragetyp** -Feld, das im Formular Neues Problem angezeigt werden soll, wählen Sie aus den folgenden Optionen den Typ Ihres Problems aus:

   * Bug-Bericht
   * Änderungsanforderung
   * Problem
   * Anfrage\
     Je nachdem, wie Ihr Workfront-Administrator Ihre Projekteinstellungen konfiguriert hat, können die Namen der Problemtypen für Sie unterschiedlich sein.

   >[!TIP]
   >
   >Die Anfragetypen müssen in den Warteschlangendetails sowie beim Erstellen des Warteschlangenthemas aktiviert sein, damit es im Formular &quot;Neues Problem&quot;als Auswahl angezeigt wird. Weitere Informationen finden Sie in den folgenden Artikeln:
   >* [Erstellen einer Anforderungswarteschlange](../../requests/create-and-manage-request-queues/create-request-queue.md)
   >  * [Erstellen von Warteschlangenthemen](../../requests/create-and-manage-request-queues/create-queue-topics.md)

1. Geben Sie weiterhin die Felder an, die im **Neues Problem** Formular. Weitere Informationen zu den Feldern, die bei Eingabe eines neuen Problems verfügbar sind, finden Sie unter [Probleme bearbeiten](../../../manage-work/issues/manage-issues/edit-issues.md).

   >[!IMPORTANT]
   >
   >Nicht alle Problemfelder sind im Formular Neue Ausgabe verfügbar. Der Projektersteller aktiviert die Felder, die beim Erstellen eines Problems verfügbar sind, wenn er den Bereich &quot;Queue Details&quot;des Projekts definiert. Weitere Informationen finden Sie unter [Erstellen einer Anforderungswarteschlange](../../requests/create-and-manage-request-queues/create-request-queue.md).


1. (Bedingt) Wenn die Warteschlangenthemen mit einem benutzerdefinierten Formular verknüpft sind, wird dieses benutzerdefinierte Formular im **Neues Problem** Formular.\
   Oder\
   Wenn das Projekt mit einem benutzerdefinierten Formular für ein Problem über den Bereich &quot;Queue Details&quot;verknüpft ist, wird das Formular im **Neues Problem** Formular nach den standardmäßigen Workfront-Feldern.

   Weitere Informationen finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Klicks **Einsenden**.

   Probleme können mehreren Benutzern, Auftragsrollen oder einem Team zugewiesen werden. Weitere Informationen zum Zuweisen und Verwalten von Anforderungen finden Sie unter [Verwalten von Arbeits- und Teamanfragen](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md).


## Erstellen von Problemen in einer Aufgabe oder einem Projekt inline

>[!IMPORTANT]
>
>Der Projektinhaber muss **Benutzern erlauben, Probleme inline hinzuzufügen** beim Definieren von Problemeinstellungen für das Projekt, bevor Sie Probleme inline zum Projekt oder zu den Aufgaben hinzufügen können. Informationen zum Konfigurieren von Problemeinstellungen für ein Projekt finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).
>

Wenn Sie mehrere Probleme schnell hinzufügen möchten, können Sie Probleme für eine Aufgabe oder ein Projekt inline erstellen, indem Sie sie zu einer Liste von Problemen hinzufügen.

>[!NOTE]
>
>Wenn Sie Probleme inline hinzufügen, wendet Workfront das Formular &quot;Neues Problem&quot;nicht auf die neuen Probleme an. Es wird nicht empfohlen, Probleme inline hinzuzufügen, wenn Sie möchten, dass Benutzer bei der Eingabe von Problemen bestimmte Informationen angeben. Dies kann sich negativ auf die Problemberichterstellung und später auf die Fähigkeit des dem Problem zugewiesenen Benutzers auswirken, über alle zur Lösung des Problems erforderlichen Informationen zu verfügen.

So erstellen Sie Probleme inline:

1. Gehen Sie zu einem Projekt, in dem Sie das Problem erstellen möchten.
1. (Optional) Wenn Sie das Problem für eine Aufgabe protokollieren möchten, navigieren Sie zum **Aufgaben** und klicken Sie auf den Namen einer Aufgabe.
1. Klicken Sie auf **Probleme** im linken Bereich.
1. Klicks **Weitere Probleme hinzufügen** unten in der Problemliste.

   Eine neue Zeile wird in der Liste der Probleme im Abschnitt Probleme erstellt.

   >[!TIP]
   >
   >Diese Option ist abgeblendet, wenn die Einstellung Benutzern das Hinzufügen von Problemen inline erlauben im Feld Projekt bearbeiten deaktiviert ist. Weitere Informationen finden Sie unter [Projekte bearbeiten](../../../manage-work/projects/manage-projects/edit-projects.md).

   ![](assets/add-more-issues-button-highlighted-issue-list-nwe-350x272.png)

1. Beginnen Sie mit der Eingabe des Namens des Problems in das Feld Name und fügen Sie dann weitere Informationen zum Problem inline hinzu.

   >[!TIP]
   >
   >Die Felder, die zur Inline-Bearbeitung verfügbar sind, werden von der Ansicht bereitgestellt, die Sie auf Ihre Problemliste anwenden. Möglicherweise können Sie folgende Feldtypen nicht inline bearbeiten:
   >   
   >* Felder, die zu einem anderen Objekt gehören
   >* Felder, auf die Sie keinen Zugriff haben
   >* Felder, die Berechnungen entsprechen und von Workfront automatisch aktualisiert werden

1. Klicken Sie auf Enter , um die Inline-Bearbeitung abzuschließen und das Problem dem Projekt oder der Aufgabe hinzuzufügen.

## Erstellen von Problemen durch Eingabe einer neuen Anforderung {#create-issues-by-entering-a-new-request}

Sie können Projekte als Container für Probleme festlegen. Diese Projektarten werden in Workfront als Anforderungswarteschlangen bezeichnet. Sie können über Ihren Anforderungsbereich im Hauptmenü auf Anforderungswarteschlangen zugreifen.

>[!TIP]
>
>Die Begriffe &quot;Problem&quot;und &quot;Anfrage&quot;sind in Workfront austauschbar.

Weitere Informationen zum Einrichten von Projekten als Anforderungswarteschlangen für den Empfang von Problemen finden Sie unter [Erstellen einer Anforderungswarteschlange](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md). Informationen zum Senden von Anfragen finden Sie unter [Erstellen und Senden von Adobe Workfront-Anforderungen](../../../manage-work/requests/create-requests/create-submit-requests.md).
