---
product-area: requests
navigation-topic: create-requests
title: Erstellen und Verwalten von Ansichten im Bereich „Anfragen“
description: Wenn Sie das neue anfordernde Erlebnis verwenden, können Sie Ansichten für den Bereich Anfragen erstellen und speichern.
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 59a9725e7697a81be2a827a902ee3d23085a2ecd
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 9%

---


# Erstellen und Verwalten von Ansichten im Bereich „Anfragen“

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


Wenn Sie das neue anfragende Erlebnis in Adobe Workfront verwenden, können Sie Ansichten für den Bereich Anfragen erstellen und speichern. Zu diesen Ansichten gehören Filter sowie Spaltenanordnungen <span class="preview"> Gruppierungen.</span>


>[!IMPORTANT]
>
>* Diese Funktion ist nur in der neuen anfragenden -Version im Bereich Anfragen verfügbar.
>* Anzeigeeinstellungen sind auch im Widget Meine Anfragen auf der Startseite verfügbar. Die Ansichten aus dem Bereich Anfragen sind jedoch von denen aus dem Widget Meine Anfragen getrennt.
>* Die Anfragenliste im Bereich „Anfragen“ und im Widget „Meine Arbeit“ verwendet die erweiterte Liste in Workfront. Weitere Informationen finden Sie unter [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebiges Workfront- oder Workflow-Paket</p>
   <p>Eine beliebige Workfront Planning-Lizenz, um Workfront Planning-Anfragen in Anfragelisten anzuzeigen</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Mitwirkende oder höher</p>
   <p>Anfragende oder höher</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Anfragen bearbeiten</p>  <p>Sie müssen Workfront-Administrator sein, um Ansichten Layoutvorlagen hinzufügen zu können</td> 
  </tr> 
  <!--
  <tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<div class="preview">

## Systemansichten für Anfragen

>[!NOTE]
>
>Systemansichten sind in Ihrer Vorschau-Umgebung möglicherweise nicht verfügbar. Sie werden am 16. April 2026 in der Produktion für alle Kunden verfügbar sein.

Zusätzlich zu den Ansichten, die Sie selbst erstellen können, bietet Workfront die folgenden Systemansichten für den Bereich Anfragen und das Widget Meine Anfragen auf der Startseite:

* **Alle Anfragen**: Alle Anfragen, die Sie oder eine andere Person in Warteschlangen oder Arbeitsbereichen gesendet haben, für die Sie über Anzeigeberechtigungen verfügen. Dies ist nicht für das Widget Meine Anfragen verfügbar.
* **Meine Anfragen**: Von Ihnen gesendete Anfragen, unabhängig vom Status.
* **Meine offenen Anfragen**: Von Ihnen gesendete und noch offene Anfragen.
* **Meine Entwürfe**: Entwürfe Ihrer Quests, die noch nicht eingereicht wurden.
* **Offene Anfragen**: Anfragen, die Sie oder eine andere Person in Warteschlangen oder für Arbeitsbereiche gesendet haben, für die Sie über Anzeigeberechtigungen verfügen und die noch offen sind. Dies ist nicht für das Widget Meine Anfragen verfügbar.

Sie können keine Systemansichten bearbeiten. Sie können die Elemente ändern und dann die Ansicht kopieren und die Kopie bearbeiten oder freigeben.

</div>

## Ansicht für Anfragen erstellen

Sie können eine Ansicht im Bereich Anfragen von Workfront erstellen, wenn Sie das neue Anfrageerlebnis verwenden. Nach der Aktivierung und dem Erlebnis „Neue Anfragen“ können Sie auf der Startseite auch Ansichten für das Widget „Meine Anfragen“ erstellen.

1. So greifen Sie auf die **Anfragen**-Liste zu:

   {{step1-to-requests}}

   1. Stellen Sie sicher **dass die Einstellung** Neues Erlebnis verwenden“ aktiviert ist.

1. So greifen Sie auf der **auf das Widget** Meine Anfragen“ zu:

   {{step1-to-home}}

   1. Fügen Sie das Widget „Meine **&quot; hinzu oder wechseln Sie**.

1. Klicken Sie in der Liste der Anfragen auf das Dropdown **Menü** Ansichten![&#x200B; und &#x200B;](assets/view-icon-requests.png) auf **Neue Ansicht**.

   <!-- 
   
   replace the screen shot with release
   ![New view](assets/create-new-view.png)

   -->

1. Geben Sie einen Namen für die neue Ansicht ein und klicken Sie auf **Erstellen**.
1. Fahren Sie fort [Ansicht für Anfragen bearbeiten](#edit-a-view-for-requests).

## Ansicht für Anfragen bearbeiten

Sie können vorhandene Ansichten bearbeiten, einschließlich der Ansichten, die Sie gerade im Bereich Anfragen oder im Widget Meine Anfragen auf der Startseite erstellt haben.

Durch Bearbeiten einer Ansicht können Sie die folgenden Elemente der Ansicht ändern:

* Name
* Filter
* Spalten

<div class="preview">

* Gruppierung
* Zellen formatieren
* Zeilenhöhe

</div>

Weitere Informationen finden Sie unter [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

<!-- 
hide these details - all the information is in "Use enhanced lists" - we need one point of messaging for this feature: 

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to edit from the **Views** dropdown menu ![Views dropdown](assets/view-icon-requests.png).

1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and click the three-dot menu next to the view, select **Rename**, then type in the new name for the view.
1. Press Enter to save the new name. 
1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and select the view you want to edit.
1. To add a field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list. 

   The **Column manager** opens.
1. Click the plus icon next to the field that you want to add as a column to the view, then click **Save**.

   Fields associated with the objects in the list are available to add as columns. <!-keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future->

   >[!TIP]
   >
   >Fields you add to the columns must exist before they are available in the **Column manager**.

1. (Optional) Click **Columns** to open the **Fields visibility and order** box. 
1. Turn on the setting for each field  you want to show in the list, turn it off to hide it, or drag and drop the fields in a different order.

1. (Optional) Click **Filters** and start adding conditions for what requests you want to view. 

    You can filter by the following request fields:  

    * **Workspace**: The workspace the request form is associated with.
    * **Object type**: The record type the request form is associated with.
    * **Entry date**: The date when the request was submitted.
    * **Request form**: The name of the request form used to submit the request.
    * **Status**: The status of the request.
    * **Entered by**: The name of the user who added the request. If the request was added by someone outside of Workfront, the **Entered by** field shows `N/A`.

    You can also filter by any fields that have been added to the view for any object visible in the view.

    You can have multiple filters joined by either **And** or **Or**.
    The request list is filtered automatically, as you add the filter conditions. 
-->

<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * Änderungen an Ansichten werden automatisch gespeichert.
> * Änderungen an Ansichten sind für alle Benutzer sichtbar, die die Ansicht verwenden <span class="preview">nur, wenn Sie eine neue Kopie der Ansicht freigeben, nachdem Sie Änderungen daran vorgenommen haben.</span>
> * Verwenden Sie den **Me (angemeldeter Benutzer),** den Platzhalter in jedem Feld zu filtern, das Benutzer als Wert enthält.

## Hinzufügen der Anfrageansicht zu einer Layout-Vorlage

Ein Workfront-Administrator kann Layoutvorlagen im Bereich Anfragen eine neue Ansicht hinzufügen.

Anweisungen finden Sie unter [Anpassen von Filtern, Ansichten und Gruppierungen mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

## Ansicht freigeben

Sie können von Ihnen erstellte Ansichten für andere Benutzer, Teams, Gruppen oder Unternehmen freigeben.

Nach der Freigabe einer Ansicht können andere Benutzer die aktualisierten Ansichtselemente anzeigen, die Sie für die Ansicht bearbeitet haben, bevor sie sie freigeben.

<span class="preview">Wenn sie die Ansicht aktualisieren, sind ihre Änderungen für andere nicht sichtbar, es sei denn, sie erstellen eine Kopie derselben Ansicht und behalten ihre Änderungen bei, bevor sie die Kopie freigeben.

Weitere Informationen finden Sie unter [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>

<!--
Let's just redirect to Use enhanced lists so we avoid duplicating information. 

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to share.
1. Hover over the view that you want to share, then click on the three-dot menu to the right of the view name, then click  **Share**.
1. In the **Share** box, enter the people, teams, roles, groups, or companies that you want to share the view with, then select them from the list when they appear.
1. Click **Save**.

   The view is shared with the entities you indicate. 
-->