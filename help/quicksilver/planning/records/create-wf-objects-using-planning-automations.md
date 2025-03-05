---
title: Erstellen von Workfront-Objekten mithilfe von Adobe Workfront Planning-Datensatzautomatisierungen
description: Sie können Automatisierungen in Adobe Workfront Planning konfigurieren, die, wenn sie aktiviert sind, Objekte in Workfront oder Datensätze in Workfront Planning erstellen. Die erstellten Objekte und Datensätze werden automatisch mit den vorhandenen Planungsdatensätzen verbunden. In diesem Artikel wird beschrieben, wie Sie Automatisierungen verwalten können, einschließlich der Bearbeitung, Deaktivierung, Löschung und des Triggers zum Erstellen von Objekten und Datensätzen.
hide: true
hidefromtoc: true
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: c669217a-40e2-471f-951d-93157a34f1ee
source-git-commit: bddd0dcd2263bd65420a17e4b9cc74336877719f
workflow-type: tm+mt
source-wordcount: '1802'
ht-degree: 2%

---

# Erstellen von Objekten mithilfe von Adobe Workfront Planning-Datensatzautomatisierungen

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->

<!--you might need to add something about notifications and emails?!-->
<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Sie können Automatisierungen in Adobe Workfront Planning konfigurieren, die, wenn sie aktiviert sind, Objekte in Workfront erstellen oder Datensätze in Workfront Planning aufnehmen, wenn sie durch einen Planungsdatensatz ausgelöst werden. Die erstellten Objekte oder Datensätze werden automatisch mit den Datensätzen verbunden, für die Sie die Automatisierung auslösen.

Sie können die Automatisierung auf der Seite „Datensatztyp“ in Workfront Planning konfigurieren und aktivieren. Das erstellte verbundene Objekt wird im verbundenen Feld des Datensatztyps platziert, von dem aus die Automatisierung ausgeführt wird.

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
   <td> <p>Tragen Sie Berechtigungen oder höhere Berechtigungen zu dem Arbeitsbereich bei, dem Sie Datensätze hinzufügen möchten. </p>  
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

* Der Name des von einer Automatisierung erstellten Objekts oder Datensatzes entspricht dem Namen des Datensatzes, aus dem Sie ihn erstellen.
* Neue Objekte oder Datensätze überschreiben nicht vorhandene im selben Feld. Durch das mehrfache Auslösen derselben Automatisierung für denselben Datensatz werden die neuen Objekte oder Datensätze im selben verbundenen Feld des ursprünglichen Datensatzes zusätzlich zu den zuvor erstellten hinzugefügt.

<!--hide this for now; they are trying to remove this militation: * The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered.-->

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

   * **Trigger**: Wählen Sie die Aktion aus, durch die die Automatisierung Trigger werden soll. Wählen Sie beispielsweise **Schaltflächen-Klick** aus. <!--update this step with a list of all possible triggers; right now only Button click is available-->

1. Aktualisieren Sie die folgenden Felder im Abschnitt **Aktionen**: <!--submitted bugs for these fields - see if they need changing here-->
   * **Aktionen**: Wählen Sie die Aktion aus, die Workfront beim Auslösen der Automatisierung ausführen soll. Dies ist ein Pflichtfeld.
Eine der folgenden Aktionen auswählen:

      * Gruppe erstellen
      * Programm erstellen
      * Portfolio erstellen
      * Projekt erstellen
      * Eintrag erstellen

     >[!TIP]
     >
     >Nachdem Sie die Automatisierung gespeichert haben, können Sie die in diesem Feld ausgewählte Aktion nicht mehr ändern.

1. (Bedingt) Aktualisieren Sie je nach ausgewählter Aktion die folgenden Felder:

   * **Projekt erstellen**:
      * **Verbundenes Feld, in dem das Objekt erstellt wird**: Dies ist das verbundene Feld, in dem das neue Projekt angezeigt wird. Dies ist ein Pflichtfeld.
      * **Projektvorlage**: Wählen Sie eine Projektvorlage aus, die Workfront zum Erstellen des Projekts verwenden wird.
   * **Portfolio erstellen**:
      * **Verbundenes Feld, in dem das Objekt erstellt wird**: Dies ist das verbundene Feld, in dem das neue Portfolio angezeigt wird. Dies ist ein Pflichtfeld.
      * **Benutzerdefiniertes Formular, das an das neue Portfolio angehängt werden soll**: Wählen Sie ein benutzerdefiniertes Formular aus, das an das neue Portfolio angehängt werden soll. Sie müssen ein benutzerdefiniertes Portfolio-Formular erstellen, bevor Sie es auswählen können.
   * **Programm erstellen**:
      * **Verbundenes Feld, in dem das Objekt erstellt wird**: Dies ist das verbundene Feld, in dem das neue Programm angezeigt wird. Dies ist ein Pflichtfeld.
      * **Programm-**: Wählen Sie ein Portfolio aus, in dem das neue Programm hinzugefügt werden soll. Dies ist ein Pflichtfeld.
      * **Benutzerdefiniertes Formular, das an das neue Programm angehängt werden soll**: Wählen Sie ein benutzerdefiniertes Formular aus, das an das neue Programm angehängt werden soll. Sie müssen ein benutzerdefiniertes Programmformular erstellen, bevor Sie es auswählen können.
   * **Gruppe erstellen**:
      * **Verbundenes Feld, in dem das Objekt erstellt wird**: Dies ist das verbundene Feld, in dem die neue Gruppe angezeigt wird. Dies ist ein Pflichtfeld.
      * **Benutzerdefiniertes Formular, das an die neue Gruppe angehängt werden soll**: Wählen Sie ein benutzerdefiniertes Formular aus, das an das neue Programm angehängt werden soll. Sie müssen ein benutzerdefiniertes Programmformular erstellen, bevor Sie es auswählen können.
   * **Datensatz erstellen**:
      * **Datensatztyp**: Wählen Sie den Datensatztyp aus, den Sie erstellen möchten.

     Der Unterabschnitt **Einstellungen** wird angezeigt. Aktualisieren Sie die folgenden Felder **Unterabschnitt** Einstellungen“:

      * **Feld für den verbundenen Datensatztyp, der für den aktuellen Datensatz angezeigt wird**: Dies ist das verbundene Feld für den Datensatztyp, der für die Aktion ausgewählt wurde, für die der aktuelle Datensatz angezeigt wird.

     Wenn Sie beispielsweise eine Automatisierung für Kampagnen erstellen, über die Produktdatensätze verbunden werden sollen, ist dies das verbundene Feld auf dem Produktdatensatztyp, in dem die Kampagnen angezeigt werden, nachdem die Produkte mithilfe der Automatisierung erstellt wurden.

     Dies ist ein Pflichtfeld.

     <!--submitted a change in functionality and UI text for this - revise??-->
      * **Felder zuordnen**
         * **Übertragen von**: Wählen Sie Felder aus dem Datensatztyp aus, für den die Automatisierung erstellt wird, um sie den Feldern des verbundenen Datensatztyps zuzuordnen.
         * **Übertragen an**: Wählen Sie Felder aus dem neu erstellten Datensatz aus, die mit Informationen aus dem Datensatz gefüllt werden, für den Sie die Automatisierung ausführen.

     >[!TIP]
     >
     >Die Feldtypen vom ursprünglichen Datensatztyp müssen mit den Feldtypen vom neu erstellten Datensatztyp übereinstimmen.

1. (Optional und bedingt) Wenn Sie ausgewählt haben, einen Datensatz zu erstellen, klicken Sie auf **Felder hinzufügen**, um zusätzliche Suchfelder von einem Datensatz einem anderen zuzuordnen.
1. (Bedingt) Wenn Sie die Erstellung eines Datensatzes ausgewählt haben und es keine Verbindungsfelder zwischen dem ursprünglichen Datensatztyp und dem im Bereich **Aktionen** ausgewählten Datensatztyp gibt, klicken Sie auf das Fragezeichen-Symbol rechts neben **Feld auf dem verbundenen Datensatztyp, auf dem der aktuelle Datensatz angezeigt werden soll** und dann auf das Symbol **Hinzufügen** ![Verbindungsfeld erstellen](assets/create-a-connection-field-icon.png), um ein Verbindungsfeld hinzuzufügen.

   Das neue Feld wird automatisch für den Datensatztyp erstellt, den Sie im Bereich **Aktionen** ausgewählt haben, und heißt **Verbundener Datensatz**.

   Ein verbundenes Feld für den ausgewählten Datensatztyp wird auch für den ursprünglichen Datensatztyp erstellt, von dem aus Sie die Automatisierung konfigurieren.
1. (Optional und bedingt) Wenn Sie ein Workfront-Objekt erstellen möchten und kein Verbindungsfeld für den ausgewählten Workfront-Objekttyp haben, klicken Sie auf das Fragezeichen-Symbol rechts neben dem Feld **Verbunden, in dem der &lt; Workfront-Objekttyp Name > erstellt wird** und klicken Sie auf das Symbol **Hinzufügen** ![Verbindungsfeld erstellen](assets/create-a-connection-field-icon.png), um ein Verbindungsfeld hinzuzufügen.

   ![](assets/question-mark-icon-to-add-connected-fields-in-automations-with-workfront.png)

   Das neue Feld wird automatisch erstellt und mit **Verbunden &lt; Workfront-Objektname >** benannt. Wenn beispielsweise ein mit einem Portfolio verbundenes Feld für den Datensatz erstellt wird, wird es „Verbundenes Portfolio“ genannt.

1. Klicken **oben** auf der Seite mit den Automatisierungsdetails auf „Speichern“.

   Die Automatisierung wird in der Liste der Automatisierungen angezeigt und kann in Datensätzen verwendet werden.

## Verwalten vorhandener Automatisierungen

{{step1-to-planning}}

1. Klicken Sie auf eine Karte für den Datensatztyp und dann auf den Namen eines Datensatzes.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. Klicken Sie auf **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und dann auf **Automatisierungen verwalten**.

   Die Liste der verfügbaren Automatisierungen für den ausgewählten Datensatztyp wird geöffnet.

1. (Optional) Führen Sie einen der folgenden Schritte aus, um eine Automatisierung zu bearbeiten, zu deaktivieren oder zu löschen:

   1. Bewegen Sie in der Automatisierungsliste den Mauszeiger über den Namen einer gespeicherten Automatisierung und klicken Sie dann auf das Menü **Mehr** ![Mehr](assets/more-menu.png).

   1. Klicken Sie **Bearbeiten**, um Informationen über Felder in der Automatisierung zu aktualisieren und sie zu konfigurieren.

      >[!TIP]
      >
      >   Die Aktion, die Sie ursprünglich für eine Automatisierung ausgewählt haben, kann nicht geändert werden.


   1. Klicken Sie auf **Deaktivieren**, um die Automatisierung aus der Tabellenansicht des Datensatzes zu entfernen und zu verhindern, dass Benutzer sie zum Erstellen von Datensätzen oder Objekten verwenden.

   Datensätze, die mit einer deaktivierten Automatisierung erstellt wurden, bleiben mit dem ursprünglich ausgewählten Datensatz verbunden.

   Um sie wieder verfügbar zu machen, klicken Sie erneut auf das **Mehr** Menü ![Mehr](assets/more-menu.png) und dann auf **Aktivieren**.
   1. Klicken Sie **Löschen**, um die Automatisierung zu löschen. Eine gelöschte Automatisierung kann nicht wiederhergestellt werden.

   Datensätze, die mithilfe einer gelöschten Automatisierung erstellt wurden, bleiben mit dem ursprünglich ausgewählten Datensatz verbunden.

## Verwenden einer Workfront Planning-Automatisierung, um ein Objekt oder einen Datensatz zu erstellen

1. Öffnen Sie in Workfront Planning die Seite „Datensatztyp“, die die Automatisierung enthält, mit der Sie automatisch Datensätze oder Objekte erstellen und verbinden möchten.
1. Öffnen Sie die Tabellenansicht.
1. Einen oder mehrere Datensätze auswählen.

   Unten in der Tabelle wird ein blauer Balken mit zusätzlichen Schaltflächen, einschließlich Automatisierungsschaltflächen, angezeigt.
1. Klicken Sie auf die Schaltfläche Automatisierung in der rechten unteren Ecke des Bildschirms.

   ![Schaltfläche „Automatisierung](assets/automation-custom-button.png)

   Folgendes geschieht:

   * Wenn die Automatisierung ein Objekt oder einen Datensatz erfolgreich erstellt hat, wird unten im Bildschirm eine Bestätigungsmeldung angezeigt.

   * Das neue Objekt wird in dem verbundenen Feld angezeigt, das Sie beim Einrichten der Automatisierungsschaltfläche angegeben haben. Möglicherweise müssen Sie die Seite aktualisieren, bevor Sie das neue Objekt anzeigen.

   * Der Datensatz, dessen Automatisierung Sie auslösen, wird dem verbundenen Feld des neuen Datensatzes hinzugefügt.

   >[!NOTE]
   >
   >Es wird empfohlen zu überprüfen, ob die Objekte oder Datensätze erwartungsgemäß erstellt und verbunden wurden.

1. (Optional) Klicken Sie auf das neue Objekt im verbundenen Feld. Die Seite „Objekt“ wird geöffnet, und Sie können zusätzliche Änderungen am neuen Objekt vornehmen.

<!--ORIGINAL AUTOMATION FUNCTIONALITY - BEFORE FEB. 20, 2025

You can configure automations in Adobe Workfront Planning that, when activated, create objects in Workfront or records in Workfront Planning when triggered from a Planning record. The created objects or records are automatically connected to the records you are triggering the automation from. 

You can configure and activate the automation in the record type's page in Workfront Planning. The connected object that is created is placed in the connected field of the record type you run the automation from. 

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

* The new object or record name is the same as the record name from which you create it. 
* New objects or records don't override existing ones in the same field. Triggering the same automation multiple times for the same records adds the new objects or records in the same connected field of the original record, in addition to the ones created before. 
* The automation adds additional objects only in the Many to many or One to many connection type fields. In the all other cases, the automation creates the object, but it does not connect it to the original record from which the automation is triggered. 

## Configure an automation in Workfront Planning

You must configure an automation for a record type in Workfront Planning, before you can use it to create objects.

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

   * **Trigger**: Select the action that will trigger the automation. For example, select **Button click**. (********update this step with a list of all possible triggers; right not only Button click is available***********)

1. Update the following fields in the **Actions** section: <********submitted bugs for these fields - see if they need changing here*********)
   * **Object type**: Select the object that you want the automation to create. This is a required field.
      
      You can create the following objects from Workfront Planning records: 

      * Project
      * Portfolio
      * Program
      * Group
      * Record

      >[!TIP]
      >
      >After you saved the automation, you can no longer change the object type in this field.

1. (Conditional) Depending on what type of object you want to create, update the following fields:


   * **Project**: 
      * **Connected field where the object is created**: This is the connected field where the new project will display. This is a required field. 
      * **Template from which to create the project**: Select a project template that Workfront will use to create the project.  
   * **Portfolio**:
      * **Connected field where the object is created**: This is the connected field where the new portfolio will display. This is a required field.
      * **Custom form to attach to the new portfolio**: Select a custom form to attach to the new portfolio. You must create a portfolio custom form before you can select it. 
   * **Program**: 
      * **Connected field where the object is created**: This is the connected field where the new program will display. This is a required field.
      * **Program portfolio**: Select a portfolio where the new program will be added. This is a required field.
      * **Custom form to attach to the new program**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Group**:
      * **Connected field where the object is created**: This is the connected field where the new group will display. This is a required field.
      * **Custom form to attach to the new group**: Select a custom form to attach to the new program. You must create a program custom form before you can select it. 
   * **Record**: 
      * **Connected record type**: Select the record type you want to create. 
      * **Connected field where the record is created**: This is the connected field where the new record will display. This is a required field. (******this might need revision as right now it shows the field on the connected record table where the current record will display; submitted a bug to correct this label*********)
      * **Map fields**
         * **Transfer from**: Select fields from the record type the automation is created for to map them to the fields of the connected record type. 
      * **Transfer to**: Select fields from the newly created record that will populate with information from the record you are running the automation from. 
1. (Optional and conditional) If you selected to create a record, click **Add fields** to map additional lookup fields from one record to another.
1. (Optional and conditional) If you don't have a connection field for a Workfront object type, click the **Create a connection field** icon ![Create a connection field icon](assets/create-a-connection-field-icon.png) to add a field.

   The new field is automatically created and named **Connected < Workfront object name >**. For example, when a portfolio connected field is created for the record, it is named "Connected portfolio." 

1. Click **Save** in the upper-right corner of the automation details page. 

   The automation displays on the list of automations, and is available to use in records.
1. (Optional) To edit, disable, or delete an automation, do the following:

   1. From the list of automations, hover over the name of a saved automation, then click the **More** menu ![More menu](assets/more-menu.png).

   1. Click **Edit** to update information about and configure fields on the automation.
   1. Click **Disable** to remove the automation from the table view and prevent users from using it to create records or objects. To make it available again, click the **More** menu ![More menu](assets/more-menu.png) again, then click **Activate**.
   1. Click **Delete** to delete the automation. A deleted automation cannot be recovered. Records that have been created using the automation remain connected to the record originally selected.  

## Use a Workfront Planning automation to create an object or a record

1. In Workfront Planning, open the record type page that contains the records you want to use to create Workfront objects or Planning records. 
1. Open the table view. 
1. Select one or more records.
   
   A blue bar displays at the bottom of the table with additional buttons, including automation buttons. 
1. Click the automation button near the lower-right corner of the screen. 

   ![Automation button](assets/automation-custom-button.png)

   A confirmation message displays at the bottom of the screen, if the automation successfully created an object or a record. 

   The new object displays in the connected field you indicated in the setup of the automation button. You might need to refresh your page before viewing the new object. 

   >[!NOTE]
   >
   >We recommend checking that the object was created and connected as expected.

1. (Optional) Click the new object in the connected field. The object page opens and you can make additional changes to the new object. 

-->

