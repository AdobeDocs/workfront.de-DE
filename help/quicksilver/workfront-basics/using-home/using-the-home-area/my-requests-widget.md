---
product-area: projects
navigation-topic: use-the-home-area
title: Verwenden des Widgets „Meine Anfragen“
description: Sie können Anfragen im Widget Meine Anfragen senden. Sie können das Widget auch mit Filtern und Spalten anpassen.
author: Alina, Courtney
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
source-git-commit: a9cc76139c0f542e4b27e8e3591a40bf626342f4
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 11%

---

# Verwenden des Widgets „Meine Anfragen“

>[!IMPORTANT]
>
>In diesem Artikel wird das neue Widget „Meine Anfragen“ beschrieben. Das neue anfragende Erlebnis muss aktiviert sein, damit das neue Widget angezeigt wird.
>Sie können das neue Anfrageerlebnis in Ihrem Anfragebereich aktivieren.

Das Widget Meine Anfragen zeigt von Ihnen gesendete Anfragen an. Sie können die Anfragen filtern, nach bestimmten Anfragen suchen oder die Spaltenreihenfolge und Sichtbarkeit anpassen. Sie können auch über das Widget Meine Anfragen eine neue Anfrage erstellen.

>[!NOTE]
>
>* Wenn das Widget Meine Anfragen geladen wird, werden bis zu 50 Anfragen angezeigt. Um weitere Anfragen anzuzeigen, scrollen Sie in der Liste nach unten.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Beliebiges Workfront- oder Workflow-Paket</p>
   <p>Ein beliebiges Workfront-Planungspaket für den Zugriff auf Workfront-Planungsanfragen und die zugehörigen erstellten Objekte</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Lizenz</strong></td> 
   <td> <p>Mitwirkende oder höher</p>
   <p>Anfragende oder höher</p> </td> 
  </tr> 
  <tr> 
   <!--
   <tr> 
   <td role="rowheader"><strong>Additional products</strong></td> 
   <td> You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
   <td role="rowheader"><strong>Konfiguration der Zugriffsebene</strong></td> 
   <td> <p>Anzeigen oder höherer Zugriff auf Objekte, für die Sie in einer Konversation getaggt sind oder eine Genehmigung auflösen müssen (Projekte, Aufgaben, Probleme, Dokumente)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektberechtigungen</strong></td> 
   <td> <p>[!UICONTROL Anzeigen] Berechtigungen oder höher für Projekte, Aufgaben, Probleme, Dokumente, bei denen Sie in einer Konversation getaggt sind oder eine Genehmigung auflösen müssen</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Erstellen einer Anfrage

Sie können eine Anfrage direkt über das Widget Meine Anfragen erstellen.

Anweisungen finden Sie im Abschnitt [Erstellen einer Anfrage](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md/#create-a-request) im Artikel [Erstellen von Arbeitselementen und Projekten im Bereich „Startseite“](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

## Anfrage kopieren

Sie können eine Anfrage im Widget Meine Anfragen kopieren, bearbeiten und als neue Anfrage senden.

Anweisungen finden Sie unter [Kopieren und Senden von Anfragen](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Informationen in der Anfragenliste im Widget „Meine Anfragen“ verwalten

<!--
The My Requests widget features a customizable filter that allows you to control which requests appear in the widget. You can configure this filter for different fields and values, and can stack conditions using AND and OR operators.

To configure the filter in the My Requests widget:
-->

1. Klicken Sie oben links auf **[!UICONTROL Hauptmenü]** ![Hauptmenüsymbol](assets/lines-main-menu.png) und dann auf **[!UICONTROL Home]**.
1. (Bedingt) So fügen Sie das Widget **Meine Anfragen** zu Ihrem Startbildschirm hinzu. Klicken Sie auf **Anpassen**, suchen Sie nach **Meine Anfragen** und klicken Sie dann darauf, um sie zu &quot;**&quot;**.
1. (Optional) Um zu verwalten, wie die Informationen in der Anfragenliste angezeigt werden, aktualisieren Sie die folgenden Ansichtselemente für die Liste:

   * Ansicht
   * Filter
   * Spalten

   <!--
   <div class="preview">
      * Group
   * Format cells
   * Row height
      </div>
   -->

   Weitere Informationen zum Verwalten von Informationen in der Anfragenliste finden Sie unter [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


<!-- Removed all these sections because this is common to ALL the Glists/ enhanced lists. So, we will update that article with all the specific steps: 
1. Select the field that you want to filter by. Available options are:

   * Workspace
   * Object type
   * Entry date
   * Request form
   * Status
   * Entered by
   * Custom fields from the request or from the created object   

1. In the next field, select the operator that you want to use for this filter condition. Available operators depend on the chosen field.
1. (Conditional) If a field appears to the right of the operator, select the value that you want to filter by.
1. (Optional) To add another filter condition, click **Add condition** and repeat steps 4-6.
1. (Optional and conditional) If you have multiple conditions, switch the And or Or value by clicking **And** or **Or** to the left of the condition.


The filter is saved automatically.

-->

>[!TIP]
>
>Wenn Ihr Unternehmen Workfront Planning zusätzlich zu Adobe Workfront erworben hat, enthält das Widget Meine Anfragen sowohl Workfront- als auch Workfront-Planungsanfragen.
> 
>* Um nur nach Workfront-Anfragen zu filtern, setzen Sie den Filter auf **Objekttyp** > **Hat beliebige von** > **Probleme**.
>* Um nur nach Workfront Planning-Anfragen zu filtern, setzen Sie den Filter auf **Objekttyp** > **Hat keine von** > **Probleme**.

<!--

## Adjust or add columns

You can choose which of the available columns appear on the My Requests widget, and set their order.

Available columns include:

* Subject
* Created object
* Object type
* Status
* Request form
* Entry date
* Entered by

To adjust the columns on the My Requests widget:

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. (Conditional) To add the **My Requests** widget to your home screen. Click **Customize**, and find **My Requests**, then click it to add it to **Home**. 
1. In the **My Requests** widget, click **Columns**.
1. (Optional) To reorder columns, click the drag handle ![drag handle](assets/drag-handle.png) of the column you want to move and drag it to the desired locations. The column at the top of the list appears in the My Requests widget as the first column.
1. (Optional) Use the toggle to hide or show the column in the requests list.
1. To add a custom field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list, and click the plus icon next to the custom field that you want to add as a column to the widget.

   Custom fields on forms attached to the object in the list are available to add as columns.

Column preferences are saved automatically.

-->

<!--

## Create a view

You can create views in the My Requests widget to change the way the information displays in the request list. 

Consider the following when working with views in the My Requests widget:

* A view in the My Requests widget contains the columns and filters applied to the view.
* You can create views and share them with others. The filters and columns you select for the view before you share it are included in the views you share. 
* The following is a system view which you cannot edit, share, or delete: 

   * Widget Unified Requests Default View
* Creating and editing a view in the My Requests widget is similar to enhanced lists. For information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). 

-->

## Suchanfragen

So suchen Sie im Widget „Meine Anfragen“ nach bestimmten Anfragen:

1. Klicken Sie oben rechts auf **[!UICONTROL Hauptmenü]** ![Hauptmenüsymbol](assets/main-menu-icon.png) und dann auf **[!UICONTROL Startseite]**.
1. (Bedingt) So fügen Sie das Widget **Meine Anfragen** zu Ihrem Startbildschirm hinzu. Klicken Sie auf **Anpassen**, suchen Sie nach **Meine Anfragen** und klicken Sie dann darauf, um sie zu &quot;**&quot;**.
1. Geben Sie in der Suchleiste rechts oben im Widget Meine Anfragen den Begriff ein, nach dem Sie suchen möchten.

   Anfragen, die den Begriff enthalten, sind orange hervorgehoben.

1. (Optional) Um zu den hervorgehobenen Anfragen zu springen, klicken Sie in der Suchleiste auf die Pfeile nach oben oder unten.

## Navigieren Sie zu einem durch eine Anfrage erstellten Objekt

Objekte, die durch eine Anfrage erstellt wurden, finden Sie im Widget Meine Anfragen .

>[!NOTE]
>
>Links zu erstellten Objekten sind in der neuen anfordernden Version nur für Planungsanfragen verfügbar, wenn die Anfrage selbst ein Objekt erstellt hat. Wenn eine Workfront-Anfrage in ein Projekt oder ein anderes Objekt konvertiert wird, ist in der Anfrageliste im neuen Anfrageerlebnis kein Link zu diesem konvertierten Objekt verfügbar.

1. Klicken Sie oben rechts auf **[!UICONTROL Hauptmenü]** ![Hauptmenüsymbol](assets/main-menu-icon.png) und dann auf **[!UICONTROL Startseite]**.
1. (Bedingt) So fügen Sie das Widget **Meine Anfragen** zu Ihrem Startbildschirm hinzu. Klicken Sie auf **Anpassen**, suchen Sie nach **Meine Anfragen** und klicken Sie dann darauf, um sie zu &quot;**&quot;**.
1. Suchen Sie die Anfrage, die das -Objekt erstellt hat.
1. Klicken Sie auf den Objektnamen in der Spalte **Erstelltes Objekt** für diese Anfrage.

   Die Seite des -Objekts wird geöffnet.

