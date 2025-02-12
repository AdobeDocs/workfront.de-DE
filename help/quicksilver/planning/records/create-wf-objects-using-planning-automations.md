---
title: Erstellen von Workfront-Objekten mithilfe von Adobe Workfront Planning-Datensatzautomatisierungen
description: Sie können Automatisierungen in Adobe Workfront Planning konfigurieren, die, wenn sie aktiviert sind, Objekte in Workfront oder Datensätze in Workfront Planning erstellen. Die erstellten Objekte und Datensätze werden automatisch mit den vorhandenen Planungsdatensätzen verbunden. In diesem Artikel wird beschrieben, wie Sie Automatisierungen verwalten können, einschließlich der Bearbeitung, Deaktivierung, Löschung und des Triggers zum Erstellen von Objekten und Datensätzen.
hide: true
hidefromtoc: true
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: 0a7bb953e7e02e24857bfb7ff671538e184bda17
workflow-type: tm+mt
source-wordcount: '1479'
ht-degree: 2%

---

# Erstellen von Objekten mithilfe von Adobe Workfront Planning-Datensatzautomatisierungen

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->
<!--when you make this public, add this to the metadata above (and take the "hide" tags out):

feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog

-->

<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Sie können Automatisierungen in Adobe Workfront Planning konfigurieren, die, wenn sie aktiviert sind, Objekte in Workfront erstellen oder Datensätze in Workfront Planning aufnehmen, wenn sie durch einen Planungsdatensatz ausgelöst werden. Die erstellten Objekte oder Datensätze werden automatisch mit den Datensätzen verbunden, für die Sie die Automatisierung auslösen.

Sie können die Automatisierung auf der Seite des Datensatzes in Workfront Planning konfigurieren und aktivieren. Das erstellte verbundene Objekt wird im verbundenen Feld des Datensatztyps platziert, von dem aus die Automatisierung ausgeführt wird.

Sie können beispielsweise eine Automatisierung erstellen, die eine Workfront Planning-Kampagne benötigt und in Workfront ein Projekt erstellt, um den Fortschritt dieser Kampagne zu verfolgen. Das Projekt wird mit der Workfront Planning-Kampagne im Feld Verbundenes Projekt der Kampagne verbunden.

Weitere Informationen zu verbundenen Datensätzen finden Sie unter [Übersicht über verbundene Datensätze](/help/quicksilver/planning/records/connected-records-overview.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für Workfront Planning anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produkte</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront-Planung<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Plan*</p></td> 
   <td> 
<p>Einer der folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Erstklassig</li> 
<li>Ultimativ</li></ul> 
<p>Workfront Planning ist nicht für ältere Workfront-Pläne verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td> 
   <td> 
<p>Beliebig </p> 
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen erhalten Sie von Ihrem Workfront Account Manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Um auf alle Funktionen von Workfront zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td> Standard
   <p>Workfront Planning ist nicht für ältere Workfront-Lizenzen verfügbar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p> 
   <p>Bearbeitungszugriff in Workfront für die Objekttypen, die Sie erstellen möchten (Projekte, Portfolios, Programme). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td> <p>Verwalten Sie die Berechtigungen für den Arbeitsbereich, dem Sie Datensätze hinzufügen möchten. </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>
   <p>Verwalten Sie Berechtigungen für Workfront-Objekte (Portfolios), um untergeordnete Objekte (Projekte) hinzuzufügen.</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutvorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü enthält </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Überlegungen zum Erstellen von Objekten und Datensätzen mithilfe einer Automatisierung

* Bei neuen Workfront-Objekten ist der neue Objektname mit dem Datensatznamen identisch, aus dem Sie ihn erstellen.
* Bei neuen Planungsdatensätzen können Sie angeben, welches ursprüngliche Datensatzfeld verwendet werden soll, um den Namen des neuen Datensatzes zu bestimmen.
* Neue Objekte oder Datensätze überschreiben nicht vorhandene im selben Feld. Durch das mehrfache Auslösen derselben Automatisierung für dieselben Datensätze werden die neuen Objekte oder Datensätze im selben verbundenen Feld des ursprünglichen Datensatzes zusätzlich zu den zuvor erstellten hinzugefügt.
* Durch die Automatisierung werden zusätzliche Objekte nur in den Feldern Viele zu viele oder Eins zu viele Verbindungstypen hinzugefügt. In allen anderen Fällen erstellt die Automatisierung das Objekt, verbindet es jedoch nicht mit dem ursprünglichen Datensatz, von dem aus die Automatisierung ausgelöst wird.

## Automatisierung in Workfront Planning konfigurieren

Sie müssen in Workfront Planning eine Automatisierung für einen Datensatztyp konfigurieren, bevor Sie ihn zum Erstellen von Objekten verwenden können.

{{step1-to-planning}}

1. Klicken Sie auf eine Karte für den Datensatztyp und dann auf den Namen eines Datensatzes.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. Klicken Sie auf **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und dann auf **Automatisierungen verwalten**.

   Die Liste der verfügbaren Automatisierungen für den ausgewählten Datensatztyp wird geöffnet.

1. Klicken Sie **Neue Automatisierung** in der oberen rechten Ecke des Bildschirms. Das Feld **Neue**&quot; wird geöffnet.
1. Aktualisieren Sie die folgenden Felder:

   * Ersetzen **Nicht benannte Automatisierung** durch den Text, der auf der Schaltfläche „Automatisierung“ angezeigt werden soll. Benutzer klicken auf diese Schaltfläche, wenn sie die Automatisierung zum Erstellen eines Workfront-Objekts oder eines Planungsdatensatzes verwenden.
   * **Beschreibung**: Fügen Sie eine Beschreibung hinzu, um den Zweck der Automatisierung anzugeben.
1. Klicken Sie **Speichern**.
Die Seite mit den Automatisierungsdetails wird geöffnet.

1. Aktualisieren Sie auf der Detailseite der Automatisierung die folgenden Felder im Abschnitt **Trigger**:

   * **Trigger**: Wählen Sie die Aktion aus, durch die die Automatisierung Trigger werden soll. Wählen Sie beispielsweise **Schaltflächen-Klick** aus. <!--update this step with a list of all possible triggers; right not only Button click is available-->

1. Aktualisieren Sie die folgenden Felder im Abschnitt **Aktionen**: <!--submitted bugs for these fields - see if they need changing here-->
   * **Objekttyp**: Wählen Sie das Objekt aus, das die Automatisierung erstellen soll. Dies ist ein Pflichtfeld.

     Sie können die folgenden Objekte aus Workfront Planning-Datensätzen erstellen:

      * Projekt
      * Portfolio
      * Programm
      * Gruppe
      * Eintrag

     >[!TIP]
     >
     >Nachdem Sie die Automatisierung gespeichert haben, können Sie den Objekttyp in diesem Feld nicht mehr ändern.

1. (Bedingt) Aktualisieren Sie je nachdem, welchen Objekttyp Sie erstellen möchten, die folgenden Felder:


   * **Projekt**:
      * **Verbundenes Feld, in dem das Objekt erstellt wird**: Dies ist das verbundene Feld, in dem das neue Projekt angezeigt wird. Dies ist ein Pflichtfeld.
      * **Vorlage, aus der das Projekt erstellt werden soll**: Wählen Sie eine Projektvorlage aus, die Workfront zum Erstellen des Projekts verwenden soll.
   * **Portfolio**:
      * **Verbundenes Feld, in dem das Objekt erstellt wird**: Dies ist das verbundene Feld, in dem das neue Portfolio angezeigt wird. Dies ist ein Pflichtfeld.
      * **Benutzerdefiniertes Formular, das an das neue Portfolio angehängt werden soll**: Wählen Sie ein benutzerdefiniertes Formular aus, das an das neue Portfolio angehängt werden soll. Sie müssen ein benutzerdefiniertes Portfolio-Formular erstellen, bevor Sie es auswählen können.
   * **Programm**:
      * **Verbundenes Feld, in dem das Objekt erstellt wird**: Dies ist das verbundene Feld, in dem das neue Programm angezeigt wird. Dies ist ein Pflichtfeld.
      * **Programm-**: Wählen Sie ein Portfolio aus, in dem das neue Programm hinzugefügt werden soll. Dies ist ein Pflichtfeld.
      * **Benutzerdefiniertes Formular, das an das neue Programm angehängt werden soll**: Wählen Sie ein benutzerdefiniertes Formular aus, das an das neue Programm angehängt werden soll. Sie müssen ein benutzerdefiniertes Programmformular erstellen, bevor Sie es auswählen können.
   * **Gruppe**:
      * **Verbundenes Feld, in dem das Objekt erstellt wird**: Dies ist das verbundene Feld, in dem die neue Gruppe angezeigt wird. Dies ist ein Pflichtfeld.
      * **Benutzerdefiniertes Formular, das an die neue Gruppe angehängt werden soll**: Wählen Sie ein benutzerdefiniertes Formular aus, das an das neue Programm angehängt werden soll. Sie müssen ein benutzerdefiniertes Programmformular erstellen, bevor Sie es auswählen können.
   * **Eintrag**:
      * **Verbundener Datensatztyp**: Wählen Sie den Datensatztyp aus, den Sie erstellen möchten.
      * **Verbundenes Feld, in dem der Datensatz erstellt wird**: Dies ist das verbundene Feld, in dem der neue Datensatz angezeigt wird. Dies ist ein Pflichtfeld. <!--this might need revision as right now it shows the field on the connected record table where the current record will display; submitted a bug to correct this label-->
      * **Felder zuordnen**
         * **Übertragen von**: Wählen Sie Felder aus dem Datensatztyp aus, für den die Automatisierung erstellt wird, um sie den Feldern des verbundenen Datensatztyps zuzuordnen.
      * **Übertragen an**: Wählen Sie Felder aus dem neu erstellten Datensatz aus, die mit Informationen aus dem Datensatz gefüllt werden, für den Sie die Automatisierung ausführen.
1. (Optional und bedingt) Wenn Sie ausgewählt haben, einen Datensatz zu erstellen, klicken Sie auf **Felder hinzufügen**, um zusätzliche Suchfelder von einem Datensatz einem anderen zuzuordnen.
1. (Optional und bedingt) Wenn Sie kein Verbindungsfeld für einen Workfront-Objekttyp haben, klicken Sie auf das Symbol **Verbindungsfeld erstellen** (Symbol ![Verbindungsfeld erstellen](assets/create-a-connection-field-icon.png), um ein Feld hinzuzufügen.

   Das neue Feld wird automatisch erstellt und mit **Verbunden &lt; Workfront-Objektname >** benannt. Wenn beispielsweise ein mit einem Portfolio verbundenes Feld für den Datensatz erstellt wird, wird es „Verbundenes Portfolio“ genannt.

1. Klicken **oben** auf der Seite mit den Automatisierungsdetails auf „Speichern“.

   Die Automatisierung wird in der Liste der Automatisierungen angezeigt und kann in Datensätzen verwendet werden.
1. (Optional) Gehen Sie wie folgt vor, um eine Automatisierung zu bearbeiten, zu deaktivieren oder zu löschen:

   1. Bewegen Sie in der Automatisierungsliste den Mauszeiger über den Namen einer gespeicherten Automatisierung und klicken Sie dann auf das Menü **Mehr** ![Mehr](assets/more-menu.png).

   1. Klicken Sie **Bearbeiten**, um Informationen über Felder in der Automatisierung zu aktualisieren und sie zu konfigurieren.
   1. Klicken Sie auf **Deaktivieren**, um die Automatisierung aus der Tabellenansicht zu entfernen und zu verhindern, dass Benutzer sie zum Erstellen von Datensätzen oder Objekten verwenden. Um sie wieder verfügbar zu machen, klicken Sie erneut auf das **Mehr** Menü ![Mehr](assets/more-menu.png) und dann auf **Aktivieren**.
   1. Klicken Sie **Löschen**, um die Automatisierung zu löschen. Eine gelöschte Automatisierung kann nicht wiederhergestellt werden. Datensätze, die mithilfe der Automatisierung erstellt wurden, bleiben mit dem ursprünglich ausgewählten Datensatz verbunden.

## Verwenden einer Workfront Planning-Automatisierung, um ein Objekt oder einen Datensatz zu erstellen

1. Öffnen Sie in Workfront Planning die Seite „Datensatztyp“, die die Datensätze enthält, die Sie zum Erstellen von Workfront-Objekten oder Planning-Datensätzen verwenden möchten.
1. Öffnen Sie die Tabellenansicht.
1. Einen oder mehrere Datensätze auswählen.

   Unten in der Tabelle wird ein blauer Balken mit zusätzlichen Schaltflächen, einschließlich Automatisierungsschaltflächen, angezeigt.
1. Klicken Sie auf die Schaltfläche Automatisierung in der rechten unteren Ecke des Bildschirms.

   ![Schaltfläche „Automatisierung](assets/automation-custom-button.png)

   Wenn die Automatisierung ein Objekt oder einen Datensatz erfolgreich erstellt hat, wird unten im Bildschirm eine Bestätigungsmeldung angezeigt.

   Das neue Objekt wird in dem verbundenen Feld angezeigt, das Sie beim Einrichten der Automatisierungsschaltfläche angegeben haben. Möglicherweise müssen Sie die Seite aktualisieren, bevor Sie das neue Objekt anzeigen.

   >[!NOTE]
   >
   >Es wird empfohlen zu überprüfen, ob das Objekt erwartungsgemäß erstellt und verbunden wurde.

1. (Optional) Klicken Sie auf das neue Objekt im verbundenen Feld. Die Seite „Objekt“ wird geöffnet, und Sie können zusätzliche Änderungen am neuen Objekt vornehmen.

<!--you might need to add something about notifications and emails?!-->


<!--****************************************FUTURE ARTICLE AFTER THE RELEASE TO PREVIEW ON FEBRUARY 20:*****************************************************  

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. The created objects or records are automatically connected to the records you are triggering the automation from. 

You can configure and activate the automation in the record's page in Workfront Planning. The connected object that is created is placed in the connected field of the record type you run the automation from. 

For example, you could create an automation that takes a Workfront Planning campaign and creates a project in Workfront to track that campaign's progress. The project would be connected to the Workfront Planning campaign in the Connected Project field on the campaign.

For more information on connected records, see [Connected records overview](/help/quicksilver/planning/records/connected-records-overview.md).

## Access requirements

+++ Expand to view access requirements for Workfront Planning. 

You must have the following access to perform the steps in this article:  

 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access all the capabilities of Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace you want to add records to. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Planning area in the Main Menu </p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).   

+++


## Considerations about creating objects and records using an automation

* For new Workfront objects, the new object name is the same as the record name from which you create it. 
* For new Planning records, you can indicate what original record field should be used to determine the new record's name. 
* New objects or records don't override existing ones in the same field. Triggering the same automation multiple times for the same record adds the new objects or records in the same connected field of the original record, in addition to the ones created before. 
* The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered. 

## Configure an automation in Workfront Planning

You must configure an automation for a record type in Workfront Planning before you can use it to create objects.

{{step1-to-planning}}

1. Click a record type card, then click the name of a record. 

   The record type page opens. 
1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Manage automations**. 

   The list of available automations for the selected record type opens.

1. Click **New automation** in the upper-right corner of the screen. The **New automation** box opens.
1. Update the following fields:

   * Replace **Untitled automation** with the text that you want to appear on the automation button. Users will click this button when using the automation to create a Workfront object or a Planning record.
   * **Description**: Add a description to identify the purpose of the automation.
1. Click **Save**.
   The automation details page opens. 

1. On the automation's details page, update the following fields in the **Triggers** section: 

   * **Trigger**: Select the action that will trigger the automation. For example, select **Button click**. *************update this step with a list of all possible triggers; right now only Button click is available*********

1. Update the following fields in the **Actions** section: **********submitted bugs for these fields - see if they need changing here***********
   * **Actions**: Select the action that you want Workfront to perform when triggering the automation. This is a required field. 
   Select one of the following actions: 

      * Create group
      * Create program
      * Create portfolio
      * Create project
      * Create record

      >[!TIP]
      >
      >After you saved the automation, you can no longer change the action selected in this field.

1. (Conditional) Depending on what action you selected, update the following fields:

   * **Create project**: 
      * **Connected field where the object is created**: This is the connected field where the new project will display. This is a required field. 
      * **Project template**: Select a project template that Workfront will use to create the project.  
   * **Create portfolio**:
      * **Connected field where the object is created**: This is the connected field where the new portfolio will display. This is a required field.
      * **Custom form to attach to the new portfolio**: Select a custom form to attach to the new portfolio. You must create a portfolio custom form before you can select it. 
   * **Create program**: 
      * **Connected field where the object is created**: This is the connected field where the new program will display. This is a required field.
      * **Program portfolio**: Select a portfolio where the new program will be added. This is a required field.
      * **Custom form to attach to the new program**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Create group**:
      * **Connected field where the object is created**: This is the connected field where the new group will display. This is a required field.
      * **Custom form to attach to the new group**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Create record**: 
      * **Record type**: Select the record type you want to create. 

      The **Settings** sub-section displays. Update the following fields in the **Settings** sub-section: 

      * **Field on the connected record type where the current record will show**: This is the connected field on the record type selected for the action where the current record will display. 
      
      For example, if you are creating an automation for campaigns to connect Product records from, this is the connected field on the Product record type where the campaigns will display, after the products are created using the automation. 
      
      This is a required field. 
      
      ******submitted a change in functionality and UI text for this - revise?? *******
      * **Map fields**
         * **Transfer from**: Select fields from the record type the automation is created for to map them to the fields of the connected record type. 
      * **Transfer to**: Select fields from the newly created record that will populate with information from the record you are running the automation from. 

      >[!TIP]
      >
      >The field types from the original record type must match the field types from the newly created record type.

1. (Optional and conditional) If you selected to create a record, click **Add fields** to map additional lookup fields from one record to another.
1. (Conditional) If you selected to create a record and there are no connection fields between the original record type and the record type selected in the **Actions** area, click the question mark icon to the right of the **Field on the connected record type where the current record will show** field, then click the **Add** icon ![Create a connection field icon](assets/create-a-connection-field-icon.png) to add a connection field. 

   The new field is automatically created for the record type you selected in the **Actions** area, and named **Connected Record**. 
   
   A connected field for the selected record type is also created on the original record type from where you are configuring the automation. 
1. (Optional and conditional) If you selected to create a Workfront object and don't have a connection field for the selected Workfront object type, click the question mark icon to the right of the **Connected field where the < Workfront object type name > is created** field, and click the **Add** icon ![Create a connection field icon](assets/create-a-connection-field-icon.png) to add a connection field. 

   ![](assets/question-mark-icon-to-add-connected-fields-in-automations-with-workfront.png)

   The new field is automatically created and named **Connected < Workfront object name >**. For example, when a portfolio connected field is created for the record, it is named "Connected portfolio." 

1. Click **Save** in the upper-right corner of the automation details page. 

   The automation displays on the list of automations, and is available to use in records.

## Manage existing automations

{{step1-to-planning}}

1. Click a record type card, then click the name of a record. 

   The record type page opens. 
1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Manage automations**. 

   The list of available automations for the selected record type opens.

1. (Optional) To edit, disable, or delete an automation, do one of the following:

   1. From the list of automations, hover over the name of a saved automation, then click the **More** menu ![More menu](assets/more-menu.png).

   1. Click **Edit** to update information about and configure fields on the automation.

      >[!TIP]
      >
      >   You cannot change the action you originally selected for an automation. 
   

   1. Click **Disable** to remove the automation from the record's table view and prevent users from using it to create records or objects. 

   Records that have been created using a disabled automation remain connected to the record originally selected.
   
   To make it available again, click the **More** menu ![More menu](assets/more-menu.png) again, then click **Activate**.
   1. Click **Delete** to delete the automation. A deleted automation cannot be recovered. 
   
   Records that have been created using a deleted automation remain connected to the record originally selected.  

## Use a Workfront Planning automation to create an object or a record

1. In Workfront Planning, open the record type page that contains the automation you want to use to autoamtically create and connect records or objects. 
1. Open the table view. 
1. Select one or more records.
   
   A blue bar displays at the bottom of the table with additional buttons, including automation buttons. 
1. Click the automation button near the lower-right corner of the screen. 

   ![Automation button](assets/automation-custom-button.png)

   The following things occur: 

   * A confirmation message displays at the bottom of the screen, if the automation successfully created an object or a record. 

   * The new object displays in the connected field you indicated in the setup of the automation button. You might need to refresh your page before viewing the new object. 

   * The record you are triggering the automation from is added to the connected field of the new record.

   >[!NOTE]
   >
   >We recommend checking that the objects or records were created and the connected as expected.

1. (Optional) Click the new object in the connected field. The object page opens and you can make additional changes to the new object. 

***********you might need to add something about notifications and emails?!*************

-->