---
title: Konfigurieren von Adobe Workfront Planning Automations
description: Sie können Automatisierungen in Adobe Workfront Planning konfigurieren, die, wenn sie aktiviert sind, Objekte in Workfront oder Datensätze in Workfront Planning erstellen. Die erstellten Objekte und Datensätze werden automatisch mit den vorhandenen Planungsdatensätzen verbunden. In diesem Artikel wird beschrieben, wie Sie Automatisierungen verwalten können, einschließlich ihrer Bearbeitung, Deaktivierung oder Löschung.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: cde20e5a-15a2-413a-8de4-ccf6eeb4395f
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/GgrkobfJEMRxHMsZF8mXAuH2xEoe-i4GTArk3S8O6fE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 1758
ht-degree: 4%

---

# Konfigurieren von Automatisierungen für Adobe Workfront-Planung

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

<!--add screen shots when UI is finalized AND redo all the steps - some things got changed and moved around-->

<!--you might need to add something about notifications and emails?!-->
<!--add a new section to this article to mention a new way to create objects: help/quicksilver/planning/records/create-records.md-->
<!-- add a new section to this article to mention a new way to create WF objects from Planning: help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md-->

<!-- if they give access to use the automation to people with LESS than Manage permissions to a workspace, split this article in two: the Configure section should be for admins and the "Use a Workfront Planning automation to create an object" should be for all other users-->

Sie können Automatisierungen in Adobe Workfront Planning konfigurieren, die, wenn sie aktiviert sind, Objekte in Workfront erstellen oder Datensätze in Workfront Planning aufnehmen, wenn sie durch einen Planungsdatensatz ausgelöst werden. Die erstellten Objekte oder Datensätze werden automatisch mit den Datensätzen verbunden, für die Sie die Automatisierung auslösen.

Sie können die Automatisierung auf der Seite „Datensatztyp“ in Workfront Planning konfigurieren und aktivieren.

Sie können beispielsweise eine Automatisierung erstellen, die eine Workfront Planning-Kampagne benötigt und in Workfront ein Projekt erstellt, um den Fortschritt dieser Kampagne zu verfolgen.

In diesem Artikel wird beschrieben, wie Sie Automatisierungen verwalten können, einschließlich der Bearbeitung, Deaktivierung, Löschung und des Triggers zum Erstellen von Objekten und Datensätzen.

Informationen zum Erstellen von Datensätzen oder Objekten mithilfe einer bestehenden Automatisierung finden Sie unter [Erstellen von Objekten mithilfe von Adobe Workfront Planning-Datensatzautomatisierungen](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<p>Beliebiges Workfront und beliebiges Planungspaket</p> <p>Beliebiger Workflow und beliebiges Planungspaket</p>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   <p>Systemadministrator hat Zugriff auf die Konfiguration von Automatisierungen basierend auf der Änderung des Feldwerts</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td> <p>Verwalten Sie die Berechtigungen für den Arbeitsbereich und den Datensatztyp, für den Sie Automatisierungen erstellen möchten. </p>
   <p>Systemadministratoren haben Verwaltungsberechtigungen für alle Arbeitsbereiche, einschließlich der Arbeitsbereiche, die sie nicht erstellt haben</p>
   </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--
Old:
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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
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
   <p>Edit access with access to Create objects in Workfront for the object types that you want to create (projects, portfolios, programs). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Manage permissions to the workspace and to the record type where you want to create automations. </p>
   <p>System Administrators have Manage permissions to all workspaces, including the ones they did not create</p>
   </td> 
  </tr> 
</tbody> 
</table>
-->

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

1. Wählen Sie auf der Detailseite der Automatisierung im Abschnitt **Trigger eine der folgenden Optionen**:

   * **Trigger**: Wählen Sie eine Aktion aus, durch die die Automatisierung in Trigger gesetzt werden soll:

      * Klick auf Schaltfläche
      * Änderung des Feldwerts

1. (Bedingt) Wenn Sie **Schaltflächen-Klick** ausgewählt haben, gehen Sie zu Schritt 9 unten, der den Bereich **Aktionen** beschreibt. <!--ensure this number stays accurate-->

1. (Bedingt) Wenn Sie **Feldwertänderung** ausgewählt haben, gehen Sie im Abschnitt **Einstellungen** wie folgt vor:

   1. Wählen Sie ein Feld aus dem Dropdown-Menü aus. Dies sind Felder, die mit dem ausgewählten Datensatztyp verknüpft sind.
   1. Definieren Sie weitere Bedingungen für das ausgewählte Feld.
   1. Klicken Sie **Bedingung hinzufügen**, um bis zu 5 Felder hinzuzufügen und ihre Bedingung zu definieren.

      Sie können einen der folgenden Feldtypen hinzufügen:

      * Einzelauswahl
      * Mehrfachauswahl
      * Einzeiliger Text
      * Absatz
      * Zahl
      * Kontrollkästchen
      * Datum

      Workfront Planning erstellt Objekte automatisch, wenn die Bedingungen erfüllt sind.

      ![Trigger zum Ändern des Feldwerts ausgewählt](assets/field-value-change-trigger-selected.png)

      >[!TIP]
      >
      >Der Modifikator in jeder Bedingung ändert sich mit dem ausgewählten Feldtyp.

1. Aktualisieren Sie die folgenden Felder im Abschnitt **Aktionen**: <!--submitted bugs for these fields - see if they need changing here-->
   * **Aktionen**: Wählen Sie die Aktion aus, die Workfront beim Auslösen der Automatisierung ausführen soll. Dies ist ein Pflichtfeld.
Eine der folgenden Aktionen auswählen:

      * Erstellen mehrerer Projekte
      * Einzelnes Projekt erstellen
      * Erstellen eines Projekts
      * Eintrag erstellen
      * Programm erstellen
      * Portfolio erstellen
      * Gruppe erstellen

     >[!TIP]
     >
     >Nachdem Sie die Automatisierung gespeichert haben, können Sie die in diesem Feld ausgewählte Aktion nicht mehr ändern.

1. (Bedingt) Aktualisieren Sie je nach ausgewählter Aktion die folgenden Felder:

   * **Erstellen eines einzelnen Projekts**: <!--replace to the left: Create a single project-->
      * **Verbundenes Feld, in dem das Projekt erstellt wird**: Dies ist das verbundene Feld, in dem das neue Projekt angezeigt wird. Dies ist ein Pflichtfeld.
      * **Projektvorlage**: Wählen Sie eine Projektvorlage aus, die Workfront zum Erstellen des Projekts verwenden wird.

   * **Erstellen mehrerer Projekte**:
      * **Verbundenes Feld, in dem das Projekt erstellt wird**: Dies ist das verbundene Feld, in dem das neue Projekt angezeigt wird. Dies ist ein Pflichtfeld.
      * **Feld, durch dessen Auswahl die Datensätze erstellt werden**: Wählen Sie ein Mehrfachauswahlfeld oder ein Einzelauswahlfeld aus dem ausgewählten Datensatztyp aus. Workfront erstellt ein Projekt für jedes Feld, das derzeit im Datensatz ausgewählt ist, aus dem Sie die Automatisierung Trigger haben.

     >[!TIP]
     >
     >Ein Projekt wird nur für die Optionen erstellt, die derzeit im Mehrfachauswahl- oder Einzelauswahlfeld des Datensatzes ausgewählt sind, für den die Automatisierung ausgeführt wird, und nicht für alle möglichen Optionen für dieses Feld.
     >

      * **Dieselbe Vorlage verwenden**: Wählen Sie diese Option, um für jedes neue Projekt dieselbe Vorlage zu verwenden. Wenn die Option nicht ausgewählt ist, wählen **für jede Feldauswahl eine** Projektvorlage) aus.
      * **Projektvorlage**: Wenn Sie die Option **Dieselbe Vorlage verwenden** ausgewählt haben, wählen Sie eine Projektvorlage aus, die Workfront zum Erstellen der Projekte verwenden wird.

   * **Portfolio erstellen**:
      * **Verbundenes Feld, in dem das Portfolio erstellt wird**: Dies ist das verbundene Feld, in dem das neue Portfolio angezeigt wird. Dies ist ein Pflichtfeld.
      * **Benutzerdefiniertes Formular, das an das neue Portfolio angehängt werden soll**: Wählen Sie ein benutzerdefiniertes Formular aus, das an das neue Portfolio angehängt werden soll. Sie müssen ein benutzerdefiniertes Portfolio-Formular erstellen, bevor Sie es auswählen können.
   * **Programm erstellen**:
      * **Verbundenes Feld, in dem das Programm erstellt wird**: Dies ist das verbundene Feld, in dem das neue Programm angezeigt wird. Dies ist ein Pflichtfeld.
      * **Programm-**: Wählen Sie ein Portfolio aus, in dem das neue Programm hinzugefügt werden soll. Dies ist ein Pflichtfeld.
      * **Benutzerdefiniertes Formular, das an das neue Programm angehängt werden soll**: Wählen Sie ein benutzerdefiniertes Formular aus, das an das neue Programm angehängt werden soll. Sie müssen ein benutzerdefiniertes Programmformular erstellen, bevor Sie es auswählen können.
   * **Gruppe erstellen**:
      * **Verbundenes Feld, in dem die Gruppe erstellt wird**: Dies ist das verbundene Feld, in dem die neue Gruppe angezeigt wird. Dies ist ein Pflichtfeld.
      * **Benutzerdefiniertes Formular, das an die neue Gruppe angehängt werden soll**: Wählen Sie ein benutzerdefiniertes Formular aus, das an das neue Programm angehängt werden soll. Sie müssen ein benutzerdefiniertes Programmformular erstellen, bevor Sie es auswählen können.
   * **Datensatz erstellen**:
      * **Datensatztyp**: Wählen Sie den Datensatztyp aus, den Sie erstellen möchten.

        Der Unterabschnitt **Einstellungen** wird angezeigt. Aktualisieren Sie die folgenden Felder **Unterabschnitt** Einstellungen“:

         * **Feld für den verbundenen Datensatztyp, der für den aktuellen Datensatz angezeigt wird**: Dies ist das verbundene Feld für den Datensatztyp, der für die Aktion ausgewählt wurde, für die der aktuelle Datensatz angezeigt wird.

        Wenn Sie beispielsweise eine Automatisierung für Kampagnen erstellen, über die Produktdatensätze verbunden werden sollen, ist dies das verbundene Feld auf dem Produktdatensatztyp, in dem die Kampagnen angezeigt werden, nachdem die Produkte mithilfe der Automatisierung erstellt wurden.

        Dies ist ein Pflichtfeld.

        <!--submitted a change in functionality and UI text for this - revise??-->
Aktualisieren Sie **Bereich** Zuordnungsfelder“ die folgenden Informationen:

         * **Übertragen von**: Wählen Sie Felder aus dem Datensatztyp aus, für den die Automatisierung erstellt wird, um sie den Feldern des verbundenen Datensatztyps zuzuordnen.
         * **Übertragen an**: Wählen Sie Felder aus dem neu erstellten Datensatz aus, die mit Informationen aus dem Datensatz gefüllt werden, für den Sie die Automatisierung ausführen.

        >[!TIP]
        >
        >* Die Feldtypen vom ursprünglichen Datensatztyp müssen mit den Feldtypen vom neu erstellten Datensatztyp übereinstimmen.
        >* Wenn Sie keine Felder auswählen, lauten die Namen der neuen Datensätze **Unbenannter Datensatz**.

1. (Optional und bedingt) Wenn Sie ausgewählt haben, einen Datensatz zu erstellen, klicken Sie auf **Felder hinzufügen**, um zusätzliche Suchfelder von einem Datensatz einem anderen zuzuordnen.
1. (Bedingt) Wenn keine Verbindungsfelder zwischen dem ursprünglichen Datensatztyp und dem im Feld „Datensatztyp“ ausgewählten Datensatztyp vorhanden sind **klicken Sie** Verbundenes Feld hinzufügen **&#x200B;**.

   ![Automatisierungseinstellungen zum Erstellen eines Datensatzes](assets/automation-setup-create-record.png)

   Die beiden folgenden Felder werden erstellt:

   * Ein neues Verbindungsfeld mit dem Namen **Verbundener Datensatz** wird für den Datensatztyp erstellt, den Sie im Feld **Datensatztyp** angegeben haben.
   * Für den Datensatztyp, für den Sie die Automatisierung konfigurieren **wird ein neues Verbindungsfeld mit demselben Namen wie** Feld „Datensatztyp“ erstellt.

     Wenn Sie beispielsweise eine Automatisierung für Kampagnen konfigurieren, um automatisch einen anderen Datensatztyp namens Marken zu erstellen, und auf **Verbundenes Feld hinzufügen** klicken, werden die folgenden Felder erstellt:

      * Das **Verbundener Datensatz** Verbindungsfeld wird für den Datensatztyp **Marken** erstellt.
      * Das **Marken** Verbindungsfeld wird für den Datensatztyp **Kampagnen** erstellt.

1. (Optional) Wenn keine Verbindungsfelder zwischen dem ursprünglichen Datensatztyp und dem im Bereich Aktionen ausgewählten Workfront-Objekt vorhanden sind, klicken Sie auf **Verbundenes Feld hinzufügen**.

   ![Automatisierungseinstellungen zum Erstellen mehrerer Projekte](assets/automation-setup-create-multiple-projects.png)

   Folgendes wird erstellt:

   * Ein neues Verbindungsfeld mit dem Namen **Verbunden &lt; Name des Workfront-Objekts >** wird für den Datensatztyp erstellt, für den Sie die Automatisierung erstellen. Beispiel: Wenn Sie **Projekt automatisch erstellen, wird** Feld „Verbundenes Projekt“ für den Datensatztyp erstellt, für den Sie die Automatisierung erstellen.
   * Im Planungsabschnitt eines Workfront-Projekts wird in Workfront eine neue Karte für den Datensatztyp mit dem Namen des Datensatztyps hinzugefügt, für den Sie die Automatisierung konfigurieren.

1. Klicken **oben** auf der Seite mit den Automatisierungsdetails auf „Speichern“.

   Die Automatisierung wird in der Liste der Automatisierungen angezeigt und kann in Datensätzen verwendet werden.

## Verwalten vorhandener Automatisierungen

{{step1-to-planning}}

1. Klicken Sie auf eine Karte für den Datensatztyp und dann auf den Namen eines Datensatzes.

   Die Seite mit dem Datensatztyp wird geöffnet.
1. Klicken Sie auf **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und dann auf **Automatisierungen verwalten**.

   Die Liste der verfügbaren Automatisierungen für den ausgewählten Datensatztyp wird geöffnet.

1. (Optional) Um eine Automatisierung anzuzeigen, zu deaktivieren oder zu löschen, klicken Sie in einer Liste von Automatisierungen auf das Menü **Mehr** ![Mehr](assets/more-menu.png) rechts neben dem Namen einer Automatisierung und führen Sie dann einen der folgenden Schritte aus:

   * Klicken Sie bei einer Automatisierung der Feldwertänderung auf **Anzeigen**, um die Einstellungen der Automatisierung anzuzeigen.

     >[!TIP]
     >
     >Wenn die Automatisierung durch eine Änderung eines Feldwerts ausgelöst wird, können die Einstellungen einer Automatisierung nach dem Speichern nicht mehr bearbeitet werden.

   * Klicken Sie bei einer Schaltflächen-Klick-Automatisierung auf **Bearbeiten**, um die folgenden Informationen zu aktualisieren:

      * Geben Sie den Namen der Automatisierung ein, indem Sie auf **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Automatisierungsnamen und dann **Bearbeiten** klicken.
      * Beliebiges Feld in der Automatisierung, mit Ausnahme des Felds **Aktionen**.

     >[!TIP]
     >
     >Die Aktion, die Sie ursprünglich für eine Automatisierung ausgewählt haben, kann nicht geändert werden.

   * Klicken Sie auf **Deaktivieren**, um die Automatisierung aus der Tabellenansicht des Datensatzes zu entfernen und zu verhindern, dass Benutzer sie zum Erstellen von Datensätzen oder Objekten verwenden.

     Datensätze, die mit einer deaktivierten Automatisierung erstellt wurden, bleiben mit dem ursprünglich ausgewählten Datensatz verbunden.

     Um sie wieder verfügbar zu machen, klicken Sie erneut auf das **Mehr** Menü ![Mehr](assets/more-menu.png) und dann auf **Aktivieren**.
   * Klicken Sie **Löschen**, um die Automatisierung zu löschen. Eine gelöschte Automatisierung kann nicht wiederhergestellt werden.

     Datensätze, die mithilfe einer gelöschten Automatisierung erstellt wurden, bleiben mit dem ursprünglich ausgewählten Datensatz verbunden.
