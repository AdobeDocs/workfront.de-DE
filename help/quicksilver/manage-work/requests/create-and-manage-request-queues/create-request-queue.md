---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Anfrage-Warteschlange erstellen
description: Sie können eine Anfrage-Warteschlange einrichten, in der Benutzer gelegentliche Anfragen eingeben können, die nicht für die Arbeit an einem Projekt geplant sind. Beispielsweise kann eine Helpdesk-Anfragewarteschlange eingerichtet werden, um alle Benutzeranfragen zu erfassen, die an eine IT-Abteilung gesendet werden.
author: Lisa
feature: Work Management, Requests
topic: Collaboration
role: User, Admin
exl-id: 385420aa-0962-4b67-9d0d-b153dcf302cf
source-git-commit: dbf96fd133bc9d37e4a3950f3551a566764a889b
workflow-type: tm+mt
source-wordcount: '2855'
ht-degree: 2%

---


# Anfrage-Warteschlange erstellen

<!--Audited: 12/2023-->

<!--
<THIS IS CONNECTED TO THE PRODUCT IN BLUEPRINTS. DO NOT MOVE/ CHANGE URL>
-->

<!--hide/ comment out the entire "create requests in Production" section and just edit and leave  only the preview section when it releases to Production; also remove the template blurb when the queue details is unshimmed for templates-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


Sie können eine Anfrage-Warteschlange einrichten, in der Benutzer gelegentliche Anfragen eingeben können, die nicht für die Arbeit an einem Projekt geplant sind. Beispielsweise kann eine Helpdesk-Anfragewarteschlange eingerichtet werden, um alle Benutzeranfragen zu erfassen, die an eine IT-Abteilung gesendet werden.

Anfragen werden zu Problemen in Adobe Workfront und werden zu Projekten hinzugefügt.

Das Einrichten einer Anfrage-Warteschlange hilft beim Formalisieren von Informationen zu Problemen, die einem Projekt hinzugefügt werden. Alle an das Projekt gesendeten Probleme werden auf die gleiche Weise gesendet und folgen demselben Pfad zum Abschluss.

Sie können die folgenden Objekte als Anfrage-Warteschlangen in Workfront einrichten:

* Projekte
* Vorlagen. Projekte, die aus Vorlagen erstellt werden, die als Anforderungswarteschlangen eingerichtet wurden, werden zu Anforderungswarteschlangen.

Um ein Projekt oder eine Vorlage als Anfrage-Warteschlange einzurichten, müssen Sie den Bereich Warteschlangendetails des Projekts oder der Vorlage bearbeiten.

In diesem Artikel wird beschrieben, wie Sie ein Projekt als Anfrage-Warteschlange konfigurieren können, in der Benutzer Anfragen senden können. Das Einrichten von Warteschlangendetails für eine Vorlage ähnelt dem Einrichten dieser Details für das Projekt.

Weitere Informationen zum Senden einer neuen Anfrage an eine Anfrage-Warteschlange finden Sie unter [Anforderungen kopieren und senden](../create-requests/copy-and-submit-requests.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Neue Lizenz: Standard </p>
   Oder
   <p>Aktuelle Lizenz: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p> Verwalten von Berechtigungen für das Projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Übersicht über Anfrage-Warteschlangen

Sie richten eine Anfrage-Warteschlange als Projekt ein. Wenn Sie das Projekt als Anfrage-Warteschlange festlegen, kann über den Bereich Anfragen in Adobe Workfront auf die Warteschlange zugegriffen werden. Wenn Sie die Anfrage-Warteschlange anpassen, passen Sie auch die Formularbenutzer an, die beim Senden der Anfragen ausgefüllt werden.

In diesem Artikel wird beschrieben, wie Sie eine Anfrage-Warteschlange aus einem vorhandenen Projekt erstellen. Um jedoch Konsistenz für den Anfrageeingangsprozess zu gewährleisten oder um mehrere Ebenen für Reporting-Zwecke und eine bessere Verwaltung hinzuzufügen, können Sie auch zusätzliche Bausteine einer Anfragewarteschlange konfigurieren, die in der folgenden Tabelle beschrieben werden.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Warteschlangendetails</td> 
   <td> <p>Sie müssen ein Projekt als Anfrage-Warteschlange im Bereich Warteschlangendetails einrichten. Dieser Schritt ist obligatorisch. </p> <p>Weitere Informationen finden Sie im <a href="#create-a-request-queue" class="MCXref xref">Erstellen einer Anfrage</a>Warteschlange) in diesem Artikel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Themengruppen</td> 
   <td> <p>Hierbei handelt es sich um zusätzliche Menüs, in denen Anfragen anhand gängiger Funktionen klassifiziert werden. Beispielsweise empfiehlt es sich für eine IT-Anfrage-Warteschlange, Themengruppen „Vor Ort“ und „Remote“ zu verwenden. </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md" class="MCXref xref">Themengruppen erstellen</a>. </p> <p>Dies ist optional.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Warteschlangenthemen</td> 
   <td> <p>Hierbei handelt es sich um zusätzliche Menüs, in denen Anfragen, die derselben Themengruppe angehören, basierend auf gemeinsamen Funktionen klassifiziert werden. Eine Themengruppe kann mehrere Warteschlangenthemen enthalten. </p> <p>Beispielsweise kann die Themengruppe „Vor-Ort“ für die IT-Anforderungswarteschlange die Warteschlangenthemen „Hardware“, „Software“ und „Netzwerk“ enthalten. </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md" class="MCXref xref">Warteschlangenthemen erstellen</a>. </p> <p>Dies ist optional.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Routing-Regeln</td> 
   <td> <p>Sie ermöglichen es Ihnen, jede Anfrage an einen Benutzer, ein Aufgabengebiet, ein Team oder ein Projekt weiterzuleiten. </p> <p>Weitere Informationen finden Sie unter <a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">Routing-Regeln erstellen</a>. </p> <p>Dies ist optional.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anfrage-Warteschlange erstellen

<!--at production release on April 10, do the following: take the first sentence here out; hide/ comment out the first section (Create a Request Queue in the Production environment); remove the title of the "Create a Request Queue in the Preview environment and leave that section as the only way to create request queues; search for any visible references of production/ preview and remove them from the entire article-->

Das Erstellen einer Anfrage-Warteschlange unterscheidet sich je nach verwendeter Umgebung.

<!--

### Create a Request Queue in the Production environment

This section describes how you can define Queue Details for the following objects:

* A project in the Production environment
* A template in the Production or Preview environment

When you set up a project as a Request Queue, the project status must be Current in order to display in the Requests area of Workfront.

>[!TIP]
>
>Your Workfront or group administrator might assign you to a custom Layout Template that might not include some of the sections described in the following steps.


To create a Request Queue:

1. Go to the project that you want to set up as a Request Queue.
1. (Optional) Click **Project Details** in the left panel and add a **Description** to the project in the **Overview** area. This information displays on all new requests.
1. Click **Queue Details** in the left panel. You might need to click **Show More**, then **Queue Details**.

   This opens the Queue Details section.

   ![Queue Details top of the section](assets/classic-queue-setup-top-of-the-setup-form-350x248.png)   

1. Specify the following information:

   * **Publish as Help Request Queue:** Select this option to identify this project as a request queue. All incoming issues are considered Requests.  
     When this option is not selected, the project behaves like a standard project in Workfront and all incoming issues are issues.
   
   * **Who can add requests to this queue:** Select which users have access to add requests to this queue. You can allow the following groups of people to see the Request Queue in their Requests area of the Global Navigation Bar when they add a new request:

     |Who can enter requests | Description|
     |---|---|
     | Anyone  |Any Workfront user with an active account can view this request queue and add requests to it |
     | People with view access to this project |Users with View permissions to the project can view and add requests to this queue |
     | People in this project's company |Users who belong to the company associated with this project can view and add requests to this queue. If there is a company associated with the project, the name of the company is listed in parentheses after this setting.  |
     | People in this project's group |Users who belong to the group associated with this project can view and add requests to this queue. If there is a group associated with the project, the name of the group is listed in parentheses after this setting, in gray font.  |

   * **Share with these links:** The following options enable you to provide direct access to the Request Queue and the forms associated with it to users outside of Workfront or to Workfront users using an external page. For information about embedding a request queue in a dashboard as an external page, see [Embed a request queue in a dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

     Users must already have access rights to the Request Queue in order to gain direct access. Using either option described here does not automatically grant access to users.

     >[!TIP]
     >
     >Users must first log in to Workfront before gaining access to the request queue when they access the Request Queue page from another application.

      * **Direct Access URL:** When a user accesses this URL from a browser, the user is taken directly to the New Request  section in the Requests area and this request is selected by default for them.

        ![Share request queue with direct URL embedded in dashboard](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

        >[!NOTE]
        >
        >You can display a Request Queue in a dashboard as an external page. In this case, the request queue is preselected, but you can select any other request queue from the Request Type field. users can change the Request Type. Navigation components of the Requests also display.

      * **Embed Code:** Use this HTML code to embed the request queue form as an iframe within any HTML page.  
        If users are not already authenticated to Workfront when they view the page where the code is embedded, the Workfront login dialog box is displayed. After users log in, the Request Queue form is displayed.

        >[!NOTE]
        >
        >When displaying a Request Queue in an iframe, only the request form displays, the request name is preselected and dimmed. User cannot change the Request type. Navigation components of the Requests area do not display.

        In order for the request queue form to be displayed when using this embed code, you must enable the "Allow embedding of Workfront in an iframe" setting in your system setup. For more information about enabling embedding of Workfront in an iframe, see [Configure system security preferences](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). If this setting is not enabled, the iframe is displayed as blank.

        You can adjust various aspects of how the embedded form is displayed, as follows:

        <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>Functionality</strong> </p> </th> 
           <th> <p><strong>Solution</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>Adjust the size of the frame</p> </td> 
           <td> <p>Modify the "width" and "height" attributes.</p> <p>By default, the width is "500" and the height is "600"</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Direct users to a specific Queue Topic or Topic Group</p> </td> 
           <td> <p>Add the "path" parameter to the src URL. You can find the path parameter by navigating to the desired Queue Topic or Topic Group in the non-embedded form and inspecting the URL.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Show and allow users to change the pre-configured Topic Group drop-down list</p> </td> 
           <td> <p>Use the "path" parameter by adding the <code>showPreSelectedOptions=true</code> parameter to the <code>src URL</code>.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Detect when the form has been submitted</p> </td> 
           <td> <p>Add a "message" event listener to your web page's window and checking if <code>event.data.type</code> is <code>requestSubmitted</code>. <code>event.data.newIssueID</code> will be set to the ID of the created issue.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **Request Types:** Select from the default options below.

     The Workfront administrator can rename the default request types. For more information about renaming the request types, see [Customize default issue types](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

      * Bug Report
      * Change Order
      * Issue
      * Request

        This is a required field and you must select at least one option.

     >[!NOTE]
     >
     >Request Types display as a selection in the Requests area only if the Request Type is selected in both the Queue Details and the Queue Topic pages. For information about setting up the Queue Details area of a project, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Each type selected here will be available on the form (you can select more than one). Selecting more than one type can help organize multiple requests coming in.  
     For example, if you are using the form on a request queue for an IT project, the following request types can come in to the queue: hardware, software, bug fixes, and issues.

   * **Default Duration:** The default duration is the length of time it typically takes to complete an issue. This becomes the default for all incoming issues and can be modified manually. Duration is generally set in hours, days, or weeks. The Default Duration of an issue is the same as the Planned Hours on the issue. The Planned Completion Date of the issue calculates based on this field.  
     The default for the issue Duration is 1 day or 8 hours. If your Workfront administrator set the Typical Hours per Work Day as less than 8 hours, the Default Duration for issues is still 8 hours. For example, if the Typical Hours per Work Day is set to 7 hours, the Default Duration for issues is 1.14 Days or 8 hours. For more information about how to set up the system Typical Hours per Work Day, see the "Timeline Calculations" section in the article [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).
   
   * **People from the same company will inherit the same permissions for all requests.:** When selected, all requests submitted to the queue are visible for users in the same company. Users can view these requests in the All Requests  section , located within the Requests area. At the time that this setting is enabled or disabled, it impacts all future requests; it does not retroactively impact information. 
   * **When someone makes a request, automatically grant:** When a user makes a request to the request queue, the user is automatically granted the level of permission that you choose to that request. Select from the following permissions levels: 

      * **View Access** 
      * **Contribute Access**. This is the default selection.
      * **Manage Access**

     For information about the Workfront permissions model, see [Overview of sharing permissions on objects](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).   
     Setting permissions here saves time, rather than having to grant permissions for each individual incoming request. Choosing this option impacts all future requests, but does not retroactively impact existing requests. 
   
   * **Default Approval**: Associate an approval process with this request queue. Only Issue Approval Processes are visible in this drop-down menu. All issues submitted to this queue will be associated with this approval process. Your Workfront administrator must define system-level approval processes before you can associate them with request queues. Users with administrative access to Approval processes can also create group-specific approval processes.

     >[!IMPORTANT]
     >
     >If the group of the project changes, the group-specific approval process attached to existing issues becomes a single-use approval process. For more information about how changes to the group of the project or changes in the approval process affect approval settings, see [How group and approval process changes affect assigned approval processes](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     If you have multiple queue topics associated with a request queue, we recommend that you associate approval processes with the queue topics instead. For more information about creating queue topics, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md). 
   
     Consider the following when adding approval processes to request queues:

      * Only active approval processes display in the list. 
      * System-wide and group-specific approval processes display in the list. An approval process associated with a group other than that of the project does not display in the list.

   * **Default Route**: Associate a Routing Rule with this request queue. Use Routing Rules to automatically assign new issues submitted to a Request Queue to the correct resource (user, job role, or team), and to the correct project. All issues submitted to this queue will be associated with this Routing Rule. You must configure Routing Rules before they display in the Queue Details section and before you can associate them with request queue.  
     If you have multiple queue topics associated with a request queue, we recommend that you associate routing rules with the queue topics instead. For more information about creating routing rules, see [Create Routing Rules](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).
   
   * **New Issue Fields:** In the **Show the following selected fields to all users** section, select any fields that you want to be visible to all users who submit a request to the project or add an issue to the project or the tasks.

     >[!TIP]
     >
     >New Issue Fields selected in the Queue Details section are also associated with any new issue added to the project <!--this is confusing: or to the tasks in the Issues section-->.

<!--     When you enable any of the Assigned to, Job Role, or the Team fields, they are always renamed to Assignments in the request form, but you can only specify the type of assignment selected here.

      >[!NOTE]
      >
      >If you selected Assigned To in the Queue Details area, you can enter only users in the Assignments field on the request form. In this case, you cannot enter job roles or a team. 
   
   * **Documents**: If you select to display the Documents section in the new request form, select where the document uploading section should be positioned. Select from the following:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">After custom forms</td> 
        <td><span>The Documents section displays at the bottom of the request form.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Before custom forms</td> 
        <td> <p><span>The Documents section displays between the Workfront fields and the custom fields of the request form.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>   
   
     ![New issue fields area with documents](assets/nwe-new-issue-fields-area-with-documents-350x167.png)

   * **Show all selected and unselected fields to:** Select which users you want to see all the fields on the new request form. The following options control the access to the fields on the form.
    
      |Which users can see all fields on the request form | Description|  
      |---|---| 
      | All Users (Plan Licenses) |All users who have a Plan license can see the selected as well as the unselected fields. |
      | People with view access to this project (Plan License) |Those users with a Plan license that also have View rights to this project can see the selected as well as the unselected fields. The rest of the users who can submit requests to this project can see just the selected fields. |
      | No Users |No users can see the unselected fields. All users who can submit requests to this project can only see the fields selected.  |
  
   * **Custom Forms**: Select a custom form to associate with the Request Queue. Only Issue Custom Forms are available to select from this drop-down menu. All issues submitted to the Request Queue will have the selected forms associated with them. You must create issue custom forms before you can see them displayed in the Queue Details section. 
     If you have multiple Queue Topics associated with a Request Queue, we recommend that you associate custom forms with the Queue Topics instead. For more information about creating sub-sections for the Request Queue, see [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![Custom forms on Queue Details](assets/custom-forms-on-queue-details.png)

     If you have multiple custom forms associated with the Request Queue, drag and drop the forms to sort them in the desired order, in the **Reorder Forms** section.

     >[!TIP]
     >
     >Custom forms added to the Queue Details section are also associated with any new issue added to the project <!--this is confusiong: or the tasks in the Issues  section-->.

<!--1. Continue selecting information for the settings in the **Email Queue Settings** area, to allow users to email requests to the request queue project. 

    For more information, see [Enable users to email an issue into a Request Queue project](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. Click **Save**.  
   Your project has now been configured to be a Request Queue and users can now add requests to it. 

1. (Optional) To enhance the Request Queue functionality, build additional sub-sections for your queue, as well as rules to route the incoming requests to the correct team, assignee or project.

   * For information about creating sub-sections for the Request Queue, see the articles [Create Queue Topics](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md) and [Create Topic Groups](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).  
   * For information about routing the requests to the appropriate assignee, team, and appropriate project, see [Create Routing Rules](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   -->


### Anfrage-Warteschlange erstellen

Wenn Sie ein Projekt als Anfrage-Warteschlange einrichten, muss der Projektstatus Aktuell sein, damit er im Bereich Anfragen von Workfront angezeigt wird.

>[!TIP]
>
>Ihr Workfront- oder Gruppen-Administrator kann Ihnen eine benutzerdefinierte Layout-Vorlage zuweisen, die möglicherweise nicht alle der in den folgenden Schritten beschriebenen Abschnitte enthält.

So erstellen Sie eine Anfrage-Warteschlange:

1. Wechseln Sie zu dem Projekt, das Sie als Anfrage-Warteschlange einrichten möchten.
1. (Optional) Klicken Sie **linken Bereich auf****Projektdetails) und fügen Sie dem Projekt** Bereich **Übersicht** eine Beschreibung hinzu. Diese Informationen werden bei allen neuen Anfragen angezeigt.
1. Klicken Sie **linken Bedienfeld** Warteschlangendetails“. Möglicherweise müssen Sie auf **Weitere anzeigen** und dann auf **Warteschlangendetails** klicken.

   Dadurch wird der Abschnitt Warteschlangendetails geöffnet.

   ![Abschnitt „Warteschlangentyp“ im Bereich „Warteschlangendetails“](assets/unshimmed-queue-type-section-queue-details-area.png)

1. Geben Sie die folgenden Informationen an:

   * **Als Warteschlange für Hilfeanfragen veröffentlichen**: Wählen Sie diese Option, um dieses Projekt als Anfragewarteschlange zu identifizieren. Alle eingehenden Anfragen werden als Anfragen betrachtet.\
     Wenn diese Option nicht ausgewählt ist, verhält sich das Projekt wie ein Standardprojekt in Workfront, und alle eingehenden Probleme sind Probleme.

   * **Wer kann dieser Warteschlange Anforderungen hinzufügen?**: Wählen Sie aus, welche Benutzer Zugriff haben, um Anfragen zu dieser Warteschlange hinzuzufügen. Sie können den folgenden Personengruppen erlauben, die Anfrage-Warteschlange in ihrem Anfragebereich der globalen Navigationsleiste anzuzeigen, wenn sie eine neue Anfrage hinzufügen:

     | Wer Anfragen eingeben kann | Beschreibung |
     |---|---|
     | Jeder | Jeder Workfront-Benutzer mit einem aktiven Konto kann diese Anfrage-Warteschlange einsehen und ihr Anfragen hinzufügen |
     | Benutzer mit Ansichtszugriff auf dieses Projekt | Benutzende mit Anzeigeberechtigungen für das Projekt können Anfragen anzeigen und zu dieser Warteschlange hinzufügen |
     | Personen im Unternehmen dieses Projekts | Benutzer, die zu dem Unternehmen gehören, das mit diesem Projekt verknüpft ist, können Anfragen anzeigen und zu dieser Warteschlange hinzufügen. Wenn dem Projekt eine Firma zugeordnet ist, wird der Name der Firma nach dieser Einstellung in Klammern aufgeführt. |
     | Personen in der Gruppe dieses Projekts | Benutzer, die zu der mit diesem Projekt verknüpften Gruppe gehören, können Anfragen anzeigen und zu dieser Warteschlange hinzufügen. Wenn mit dem Projekt eine Gruppe verknüpft ist, wird der Name der Gruppe nach dieser Einstellung in Klammern in grauer Schriftart aufgeführt. |

     {style="table-layout:auto"}

   * Verwenden Sie die folgenden Optionen, um Benutzern außerhalb von Workfront oder Workfront-Benutzern mithilfe einer eingebetteten externen Seite direkten Zugriff auf die Anfrage-Warteschlange und die damit verbundenen Formulare bereitzustellen.

   Informationen zum Einbetten einer Anfrage-Warteschlange in ein Dashboard als externe Seite finden Sie unter [Anfrage-Warteschlange in ein Dashboard einbetten](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-request-queue-dashboard.md).

   Benutzer müssen zunächst über Berechtigungen für die Anfrage-Warteschlange verfügen, um direkten Zugriff zu erhalten. Durch die Verwendung einer der hier beschriebenen Optionen wird Benutzenden nicht automatisch Zugriff gewährt.

   >[!TIP]
   >
   >Anwender müssen sich zuerst bei Workfront anmelden, bevor sie Zugriff auf die Anfrage-Warteschlange erhalten, wenn sie von einem anderen Programm aus auf die Seite „Anfrage-Warteschlange“ zugreifen.

   * **Direktzugriff-URL:** Wenn ein Benutzer über einen Browser auf diese URL zugreift, wird der Benutzer direkt zum Abschnitt „Neue Anfrage“ im Bereich „Anfragen“ geleitet und diese Anfrage ist standardmäßig für ihn ausgewählt.

     ![Neues Anfragefeld von Direct URL Share](assets/new-request-box-from-direct-url-share.png)

     >[!NOTE]
     >
     >Sie können eine Anfrage-Warteschlange in einem Dashboard als externe Seite anzeigen. In diesem Fall ist die Anfragewarteschlange vorausgewählt, Sie können jedoch eine beliebige andere Anfragewarteschlange aus dem Feld Anfragetyp auswählen. Benutzer, die die Anfrage senden, können einen anderen Anfragetyp auswählen. Themengruppen und Warteschlangenthemen werden ebenfalls angezeigt.

   * **Einbettungs-Code:** Verwenden Sie diesen HTML-Code, um das Formular für die Anfrage-Warteschlange als iframe in eine beliebige HTML-Seite einzubetten.\
     Wenn Benutzende nicht bereits bei Workfront authentifiziert sind, wenn sie die Seite aufrufen, auf der der Code eingebettet ist, wird das Workfront-Anmeldedialogfeld angezeigt. Nachdem sich Benutzer angemeldet haben, wird das Formular Anfrage-Warteschlange angezeigt.

     >[!NOTE]
     >
     >Wenn eine Anfrage-Warteschlange in einem IFrame angezeigt wird, wird nur das Anfrage-Formular angezeigt, und der Name der Anfrage ist vorab ausgewählt und abgeblendet. Der Benutzer kann den Anfragetyp nicht ändern. Navigationskomponenten des Bereichs Anfragen werden nicht angezeigt.

     Damit das Formular für die Anfrage-Warteschlange bei Verwendung dieses Einbettungs-Codes angezeigt wird, muss der Workfront-Administrator die Einstellung „Einbetten von Workfront in einen iframe zulassen“ im Bereich „System-Setup“ aktivieren.

     Weitere Informationen zum Aktivieren der Einbettung von Workfront in einen iframe finden Sie unter [Systemsicherheitseinstellungen konfigurieren](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md). Wenn diese Einstellung nicht aktiviert ist, wird der IFrame als leer angezeigt.

     Sie können verschiedene Aspekte der Anzeige des eingebetteten Formulars wie folgt anpassen:

     <table border="1" cellspacing="15"> 
         <col> 
         <col> 
         <thead> 
          <tr> 
           <th> <p><strong>Funktionalität</strong> </p> </th> 
           <th> <p><strong>Lösung</strong> </p> </th> 
          </tr> 
         </thead> 
         <tbody> 
          <tr> 
           <td> <p>Anpassen der Rahmengröße</p> </td> 
           <td> <p>Ändern Sie die Attribute „width“ und „height“.</p> <p>Standardmäßig ist die Breite „500“ und die Höhe „600“</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Benutzer zu einem bestimmten Warteschlangenthema oder einer bestimmten Themengruppe weiterleiten</p> </td> 
           <td> <p>Fügen Sie den Parameter „path“ zur src-URL hinzu. Sie können den Pfadparameter finden, indem Sie zum gewünschten Warteschlangenthema oder zur gewünschten Themengruppe im nicht eingebetteten Formular navigieren und die URL überprüfen.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Anzeigen und Zulassen, dass Benutzer die vorkonfigurierte Dropdown-Liste Themengruppe ändern</p> </td> 
           <td> <p>Verwenden Sie den Parameter „path“, indem Sie dem <code>src URL</code> den Parameter <code>showPreSelectedOptions=true</code> hinzufügen.</p> </td> 
          </tr> 
          <tr> 
           <td> <p>Erkennen, wann das Formular gesendet wurde</p> </td> 
           <td> <p>Fügen Sie einen Ereignis-Listener „Nachricht“ zum Fenster Ihrer Web-Seite hinzu und überprüfen Sie, ob <code>event.data.type</code> <code>requestSubmitted</code> ist. <code>event.data.newIssueID</code> wird auf die ID des erstellten Problems gesetzt.</p> </td> 
          </tr> 
         </tbody> 
        </table>

   * **Anfragetypen:** Wählen Sie im Abschnitt **Warteschlangeneigenschaften** eine der folgenden Optionen aus:

   * Fehlerbericht
   * Änderungsanforderung
   * Problem
   * Anfrage

   Dies ist ein Pflichtfeld, und Sie müssen mindestens eine Option auswählen.

   Der Workfront-Administrator kann die Standardanfragetypen umbenennen. Weitere Informationen zum Umbenennen der Anfragetypen finden Sie unter [Anpassen von Standardanfragetypen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

   >[!NOTE]
   >
   >Wenn Benutzer über den Bereich Anfragen auf die Anfrage-Warteschlange zugreifen, werden die Anfragetypen nur dann als Auswahl angezeigt, wenn der Anfragetyp sowohl auf der Seite Warteschlangendetails als auch auf der Seite Warteschlangenthema ausgewählt ist.
   >
   >Informationen zum Einrichten des Bereichs Warteschlangenthemen eines Projekts finden Sie unter [Warteschlangenthemen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

   Jeder hier ausgewählte Typ ist im Formular verfügbar (Sie können mehrere Typen auswählen). Die Auswahl mehrerer Typen kann dabei helfen, mehrere eingehende Anfragen zu organisieren.\
   Wenn Sie das Formular beispielsweise in einer Anfrage-Warteschlange für ein IT-Projekt verwenden, können die folgenden Anfragetypen in die Warteschlange aufgenommen werden: Hardware, Software, Fehlerbehebungen und Probleme.

   * **Standarddauer:** Sie eine Zahl für die Dauer ein und wählen Sie dann aus dem Dropdown-Menü eine der folgenden Einheiten für die Dauer aus:

      * Tage
      * Stunden
      * Minuten
      * Wochen

   Die Standarddauer ist die Zeit, die normalerweise benötigt wird, um ein an diese Anfrage-Warteschlange gesendetes Problem zu beheben. Dies wird zur Standardeinstellung für alle eingehenden Probleme und kann manuell geändert werden.
Die Standarddauer eines Problems entspricht den für das Problem geplanten Stunden. Das geplante Abschlussdatum der Anfrage wird auf Grundlage dieses Felds berechnet.\
   Wenn sie unverändert gelassen wird, beträgt der Standardwert für die Problemdauer 1 Tag oder 8 Stunden.
Wenn Ihr Workfront-Administrator im Bereich „Setup“ für jeden Arbeitstag einen Wert von unter 8 Stunden festgelegt hat, beträgt die Standarddauer für Probleme weiterhin 8 Stunden.
Wenn beispielsweise die Standardstundenzahl pro Arbeitstag im Bereich Setup von Workfront auf 7 Stunden festgelegt ist, beträgt die Standarddauer für Probleme 1,14 Tage oder 8 Stunden.
Weitere Informationen zum Einrichten des Systems „Typische Stunden pro Arbeitstag“ finden Sie im Abschnitt „Zeitleistenberechnungen“ im Artikel [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   * **Personen aus demselben Unternehmen erben dieselben Berechtigungen für alle Anfragen.**: Wenn diese Option aktiviert ist, sind alle an die Warteschlange gesendeten Anfragen für Benutzer im selben Unternehmen sichtbar. Benutzer können diese Anfragen im Abschnitt Alle Anfragen anzeigen, der sich im Bereich Anfragen befindet. Zum Zeitpunkt der Aktivierung oder Deaktivierung dieser Einstellung wirkt sich dies nicht rückwirkend auf die Informationen aus, sondern auf alle zukünftigen Anfragen.
   * **Wenn jemand eine Anfrage stellt, automatisch erteilen…** Wenn ein Benutzer eine Anfrage an die Anfrage-Warteschlange sendet, wird dem Benutzer automatisch die Berechtigungsstufe gewährt, die Sie für diese Anfrage auswählen. Klicken Sie auf die Schaltfläche Zugriff , um aus den folgenden Berechtigungsebenen auszuwählen:

      * **Ansichtszugriff**
      * **Beitragszugriff**. Dies ist die Standardauswahl und der Name der Schaltfläche „Zugriff“.
      * **Zugriff verwalten**

     Weitere Informationen zum Workfront-Berechtigungsmodell finden Sie unter [Übersicht über Freigabeberechtigungen für Objekte](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).\
     Wenn Sie hier Berechtigungen festlegen, sparen Sie Zeit, da Sie für jede eingehende Anfrage nicht einzeln Berechtigungen erteilen müssen. Die Auswahl dieser Option wirkt sich auf alle zukünftigen Anfragen aus, hat jedoch keine rückwirkenden Auswirkungen auf bestehende Anfragen.

   * **Standardgenehmigung**: Klicken Sie auf das Dropdown-Menü, um einen Genehmigungsprozess für diese Anfrage-Warteschlange auszuwählen. In diesem Dropdown-Menü werden nur Problemgenehmigungsprozesse angezeigt. Alle an diese Warteschlange gesendeten Probleme werden mit diesem Genehmigungsprozess verknüpft. Ihr Workfront-Administrator muss Genehmigungsprozesse auf Systemebene definieren, bevor Sie sie mit Anfragewarteschlangen verknüpfen können. Benutzende mit administrativem Zugriff auf Genehmigungsprozesse können auch gruppenspezifische Genehmigungsprozesse erstellen.

     >[!IMPORTANT]
     >
     >Wenn sich die Gruppe des Projekts ändert, wird der gruppenspezifische Genehmigungsprozess, der an vorhandene Probleme angehängt ist, zu einem einmaligen Genehmigungsprozess. Weitere Informationen darüber, wie sich Änderungen an der Projektgruppe oder Änderungen im Genehmigungsprozess auf die Genehmigungseinstellungen auswirken, finden Sie unter [Wie sich Änderungen an Gruppen- und Genehmigungsprozessen auf zugewiesene Genehmigungsprozesse auswirken](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/how-changes-affect-group-approvals.md).

     Wenn mehrere Warteschlangenthemen mit einer Anfrage-Warteschlange verknüpft sind, empfehlen wir, stattdessen Genehmigungsprozesse mit den Warteschlangenthemen zu verknüpfen.

     Weitere Informationen zum Erstellen von Warteschlangenthemen finden Sie unter [Warteschlangenthemen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     Beachten Sie beim Hinzufügen von Genehmigungsprozessen zu Anfrage-Warteschlangen Folgendes:

      * In der Liste werden nur aktive Problemgenehmigungsprozesse angezeigt.
      * In der Liste werden systemweite und gruppenspezifische Problemgenehmigungsprozesse angezeigt. Ein Genehmigungsprozess, der mit einer anderen Gruppe als der des Projekts verknüpft ist, wird nicht in der Liste angezeigt.

   * **Standardroute**: Klicken Sie auf das Dropdown-Menü, um eine Routing-Regel für diese Anfrage-Warteschlange auszuwählen. Routing-Regeln weisen automatisch neue Probleme zu, die an eine Anfrage-Warteschlange gesendet wurden, an die richtige Ressource (Benutzer, Aufgabengebiet oder Team) und an das richtige Projekt. Alle an diese Warteschlange gesendeten Probleme werden dieser Routingregel zugeordnet. Sie müssen Routing-Regeln konfigurieren, bevor sie im Abschnitt Warteschlangendetails angezeigt werden und bevor Sie sie mit der Anfrage-Warteschlange verknüpfen können.\
     Wenn mehrere Warteschlangenthemen mit einer Anfrage-Warteschlange verknüpft sind, empfehlen wir, stattdessen Routing-Regeln mit den Warteschlangenthemen zu verknüpfen. Weitere Informationen zum Erstellen von Routingregeln finden Sie unter [Routingregeln erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

   * **Neue Problemfelder:** Wählen Sie im Abschnitt **Die folgenden ausgewählten Felder für alle Benutzer anzeigen** die Felder aus, die für alle Benutzer sichtbar sein sollen, die eine Anfrage an das Projekt senden oder ein Problem zu diesem Projekt oder den Aufgaben des Projekts hinzufügen.

     >[!NOTE]
     >
     >* Wenn Sie eines der Felder Zugewiesen an, Aufgabengebiet oder Team aktivieren, werden sie im Anfrageformular immer in Zuweisungen umbenannt, wenn Benutzer die Anfrage senden. Sie können den Typ der Zuweisung nur im Bereich Warteschlangendetails angeben.
     >
     >* Wenn Sie im Bereich „Warteschlangendetails“ die Option „Zugewiesen an“ ausgewählt haben, können Sie im Anforderungsformular nur Benutzer in das Feld „Zuweisungen“ eingeben. In diesem Fall können Sie keine Aufgabengebiete oder ein Team eingeben.

   * **Dokumente**: Wählen Sie diese Option, um den Abschnitt Dokumente im neuen Anfrageformular anzuzeigen, und wählen Sie dann aus, wo der Abschnitt Dokument hochladen positioniert werden soll. Wählen Sie aus den folgenden Optionen aus:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Nach benutzerdefinierten Formularen</td> 
        <td><span>Der Abschnitt Dokumente wird unten im Anfrageformular angezeigt.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Vor benutzerdefinierten Formularen</td> 
        <td> <p><span>Der Abschnitt Dokumente wird zwischen den Workfront-Feldern und den benutzerdefinierten Feldern des Anfrageformulars angezeigt.</span> </p> </td> 
       </tr> 
      </tbody> 
     </table>

     ![Neue Problemfelder und Dokumente in Warteschlangendetails](assets/new-issue-fields-and-documents-on-queue-details.png)

   * **Alle ausgewählten und nicht ausgewählten Felder anzeigen für** Wählen Sie aus, welchen Benutzern alle Felder im neuen Anfrageformular angezeigt werden sollen. Die folgenden Optionen steuern den Zugriff auf die Felder im Formular.

     | Benutzer, die alle Felder im Anfrageformular sehen können | Beschreibung |
     |---|---| 
     | Alle Benutzer (Planlizenzen) | Alle Benutzer, die über eine Planlizenz verfügen, können die ausgewählten sowie die nicht ausgewählten Felder sehen. |
     | Personen mit Ansichtszugriff auf dieses Projekt (Planlizenz) | Benutzer mit einer Planlizenz, die auch über Ansichtsrechte für dieses Projekt verfügen, können die ausgewählten sowie die nicht ausgewählten Felder sehen. Der Rest der Benutzer, die Anfragen an dieses Projekt senden können, kann nur die ausgewählten Felder sehen. |
     | Keine Benutzer | Die nicht ausgewählten Felder können nicht von Benutzenden angezeigt werden. Alle Benutzer, die Anfragen an dieses Projekt senden können, können nur die ausgewählten Felder sehen. Dies ist die Standardauswahl. |

   * **Benutzerdefinierte Forms**: Wählen Sie aus dem Dropdown-Menü ein benutzerdefiniertes Formular aus, das mit der Anfrage-Warteschlange verknüpft werden soll. Sie können mehrere Formulare auswählen und sie dann per Drag-and-Drop in der Reihenfolge ablegen, in der sie im Anfrageformular angezeigt werden sollen.
In diesem Dropdown-Menü stehen nur benutzerdefinierte Problemformulare zur Auswahl. Allen Problemen, die an diese Anfrage-Warteschlange gesendet und dem Projekt oder seinen Aufgaben hinzugefügt werden, werden die ausgewählten Formulare zugeordnet.
Sie müssen benutzerdefinierte Anfrageformulare erstellen, bevor Sie sie im Abschnitt Warteschlangendetails anzeigen können.
Wenn mehrere Warteschlangenthemen mit einer Anfrage-Warteschlange verknüpft sind, empfehlen wir, stattdessen benutzerdefinierte Formulare mit den Warteschlangenthemen zu verknüpfen.
Weitere Informationen finden Sie unter [Warteschlangenthemen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md).

     ![Benutzerdefiniertes Formular-Feld in Warteschlangendetails](assets/custom-forms-box-on-queue-details.png)

1. Wählen Sie weiterhin Informationen für die Einstellungen im Bereich **E-Mail-Warteschlangeneinstellungen** aus, damit Benutzer E-Mail-Anfragen an das Projekt für die Anfrage-Warteschlange senden können.

   Weitere Informationen finden Sie unter [Benutzer können ein Problem per E-Mail an ein Anfrage-Warteschlangenprojekt senden](../../../manage-work/requests/create-requests/enable-email-issues-into-projects.md).

1. Klicken Sie auf **Speichern**.\
   Ihr Projekt wurde jetzt als Anfrage-Warteschlange konfiguriert, und Benutzer können ihm jetzt Anforderungen hinzufügen.

1. (Optional) Um die Funktionalität für die Anfrage-Warteschlange zu verbessern, erstellen Sie zusätzliche Unterabschnitte für Ihre Warteschlange sowie Regeln für die Weiterleitung der eingehenden Anfragen an das richtige Team, den richtigen Verantwortlichen oder das richtige Projekt.

   * Informationen zum Erstellen von Unterabschnitten für die Anfrage-Warteschlange finden Sie in den folgenden Artikeln
   * [Warteschlangenthemen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)
   * [Themengruppen erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-topic-groups.md).

     Weitere Informationen zum Weiterleiten der Anfragen an den entsprechenden Verantwortlichen, das entsprechende Team und das entsprechende Projekt finden Sie unter [Routing-Regeln erstellen](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

