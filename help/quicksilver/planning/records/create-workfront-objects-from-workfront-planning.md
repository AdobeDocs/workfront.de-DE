---
title: Erstellen von Workfront-Objekten aus Workfront Planning, während Sie sie mit Datensätzen verbinden
description: Sie können Workfront-Objekttypen erstellen, während Sie sie aus anderen Datensätzen in Workfront Planning verbinden.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 1f9a0e6064f83c6f0947e3c7ef596e96c934a687
workflow-type: tm+mt
source-wordcount: '1271'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Erstellen von Workfront-Objekten aus Workfront Planning, während Sie sie mit Datensätzen verbinden

<!-- remove preview and production at release time-->

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Sie können Adobe Workfront-Objekte aus Workfront Planning wie folgt erstellen:

* Beim Verbinden von Workfront-Objekten aus Planungsdatensätzen

  In diesem Artikel wird beschrieben, wie Sie Workfront-Objekte aus Workfront Planning erstellen, während Sie sie aus Planning-Datensätzen verbinden.
* Wenn Sie Automatisierungen von der Datensatzseite aus verwenden.

  Informationen zum Erstellen von Workfront-Objekten mithilfe von Automatisierungen finden Sie unter [Erstellen von Objekten mithilfe von Adobe Workfront Planning-Datensatzautomatisierungen](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

>[!IMPORTANT]
>
>Sie können die folgenden Workfront-Objekte aus Workfront Planning erstellen, wenn Sie sie mit Planungsdatensätzen verbinden:
>
>* Projekte
>* Portfolios
>* Programme
>
>Sie können die folgenden Workfront-Objekte mit Planungsdatensätzen verbinden, sie jedoch nicht im Verbindungsprozess erstellen:
>
>* Gruppen
>* Firmen
>

Beachten Sie beim Verbinden und Erstellen von Workfront-Objekten mit Workfront-Planungsdatensätzen Folgendes:

* Sie können Workfront-Projekte, -Portfolios, -Programme, -Gruppen und -Unternehmen über ein Verbindungsfeld aus den folgenden Bereichen von Workfront Planning verbinden:

   * Die Tabellenansicht eines Datensatztyps
   * Die Detailseite oder das Vorschaufeld eines Datensatzes
   * Registerkarte „Verbindungen“ eines Datensatzes

* Sie können Projekte aus den folgenden Bereichen von Workfront Planning erstellen:

   * Die Tabellenansicht eines Datensatztyps
   * Der Detailbereich eines Datensatzes im Verbindungsfeld
   * Die Seite „Verbundener Datensatz“ eines Datensatzes im Bereich Details

* Sie können Portfolios und Programme aus den folgenden Bereichen von Workfront Planning erstellen:

   * Die Tabellenansicht eines Datensatztyps
   * Der Detailbereich eines Datensatzes im Verbindungsfeld

Informationen zum Verbinden von Planning-Datensätzen mit Workfront-Objekten finden Sie unter [Verbinden von Datensätzen](/help/quicksilver/planning/records/connect-records.md).

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
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p> 
   <p>Bearbeiten Sie den Zugriff mit dem Zugriff auf Erstellen von Objekten in Workfront für die Objekttypen, die Sie erstellen möchten (Projekte, Portfolios, Programme). </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td> <p>Tragen Sie Berechtigungen oder höhere Berechtigungen zum Arbeitsbereich und Datensatztyp bei, dem Sie Datensätze hinzufügen möchten. </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>
   <p>Verwalten Sie Berechtigungen für Workfront-Objekte (Portfolios), um untergeordnete Objekte (Projekte) hinzuzufügen.</p>
   </td> 
  </tr>   
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

<!--Old:

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
   <td> <p>Manage permissions to the workspace and record type where you want to add records. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).  -->


## Voraussetzungen für das Erstellen von Workfront-Objekten beim Verbinden dieser Objekte mit Datensätzen aus Workfront Planning

Sie müssen über Folgendes verfügen, bevor Sie neue Projekte oder Portfolios hinzufügen können, indem Sie sie mit vorhandenen Datensätzen verbinden:

* Datensatztypen, die mit Workfront-Projekten, -Portfolios oder -Programmen verbunden sind. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
* Datensätze für die mit Workfront-Objekten verbundenen Datensatztypen. Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).
* Die richtigen Zugriffsberechtigungen in Workfront Planning und Workfront, wie im Abschnitt [Zugriffsanforderungen“ in &#x200B;](#access-requirements) Artikel beschrieben.

## Erstellen Sie Projekte, während Sie sie mit Datensätzen aus Workfront Planning verbinden

Sie können in Workfront Planning in den folgenden Bereichen von Workfront Planning Projekte erstellen, während Sie sie mit Datensätzen verbinden:

* Die Tabellenansicht eines Datensatztyps oder der Bereich Details eines Datensatzes im Verbindungsfeld
* Die Seite „Verbundener Datensatz“ eines Datensatzes im Bereich „Details“ eines Datensatzes

### Erstellen von Projekten im Bereich „Details“ eines Datensatzes oder in der Tabellenansicht eines Datensatztyps

So erstellen Sie Projekte, während Sie sie mit anderen Datensätzen verbinden:

1. Wechseln Sie zur Detailseite eines Datensatzes oder zur Tabelle des Datensatztyps und verbinden Sie Workfront Planning-Datensätze mit Workfront-Projekten, wie im Artikel [Verbinden von Datensätzen](/help/quicksilver/planning/records/connect-records.md) beschrieben.

1. (Bedingt) Klicken Sie auf **Projekt hinzufügen**
oder
Geben Sie den Namen eines Projekts ein und klicken Sie dann auf **Projekt hinzufügen**, wenn Sie es nicht finden können. Auf die Schaltfläche Hinzufügen folgt der von Ihnen eingegebene Projektname.

   ![Projekt hinzufügen beim Verbinden über ein Verbindungsfeld](assets/add-project-when-connecting-it-from-connection-field.png)

   Das **Projekt erstellen** wird geöffnet.

1. (Optional) Aktualisieren Sie den **Projektnamen**. Standardmäßig wird das Projekt nach dem benannt, was Sie beim Verbinden aus dem Datensatz als Suchelement hinzugefügt haben.
1. (Optional) Wählen Sie eine **Projektvorlage** aus. Wenn Sie keine Vorlage auswählen, erstellt Workfront ein leeres Projekt ohne Aufgaben.
1. Klicken Sie auf **Erstellen**.
1. (Bedingt) Wenn Sie ausgewählt haben, ein Projekt aus einer Vorlage zu erstellen, befolgen Sie die Schritte im Artikel [Erstellen eines Projekts mit einer Vorlage](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md), um das Hinzufügen des Projekts abzuschließen.

   Das neue Projekt wird erstellt und dem verbundenen Feld des ausgewählten Datensatzes hinzugefügt.

1. (Optional) Klicken Sie in Workfront Planning auf den Namen des neuen Projekts, um die Projektseite in Workfront zu öffnen und zusätzliche Aktualisierungen am Projekt vorzunehmen.

### Erstellen von Projekten über die Seite „Verbundene Datensätze“ eines Datensatzes

1. Verbinden Sie den Projektobjekttyp mit einem Workfront Planning-Datensatztyp in der Tabellenansicht.

   Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes. Das Vorschaufeld Details wird geöffnet.

1. Fügen Sie eine **Seite „Verbundene Datensätze** für Projekte hinzu.

   Weitere Informationen finden Sie im Abschnitt „Hinzufügen einer verbundenen Datensatzseite zu einem Datensatz“ im Artikel [Verwalten des Datensatzseitenlayouts](/help/quicksilver/planning/records/manage-the-record-page.md).

   Die Seite Verbundene Datensätze wird in der Tabellenansicht angezeigt. Verbundene Projekte werden in der Tabelle angezeigt.

   ![Tabellenansicht „Projekte“ auf der Seite „Verbundene Datensätze“](assets/projects-connected-records-page-table.png)

1. Klicken Sie **Neue Zeile** in der Projekttabelle, um ein Projekt hinzuzufügen.

   Sie können in diesem Bereich nur ein leeres Projekt hinzufügen. Sie können kein Projekt mit einer Vorlage hinzufügen.
1. (Optional) Klicken Sie auf den Namen des Projekts in der Tabellenansicht, um das Projekt in Workfront zu öffnen und weitere Informationen hinzuzufügen.

## Erstellen Sie Portfolios, während Sie sie mit Datensätzen aus Workfront Planning verbinden

Sie können Portfolios aus der Tabellenansicht eines Datensatztyps oder der Detailseite eines Datensatzes erstellen.

So erstellen Sie Portfolios, während Sie sie mit Planungsdatensätzen verbinden:

1. Wechseln Sie zur Detailseite eines Datensatzes oder zur Tabelle des Datensatztyps und verbinden Sie Workfront Planning-Datensätze mit Workfront-Portfolios, wie im Artikel [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md) beschrieben.

1. (Bedingt) Klicken Sie auf **Portfolio hinzufügen**

   Oder

   Geben Sie den Namen eines Portfolios ein und klicken Sie auf **Portfolio hinzufügen** wenn Sie es nicht finden können. Auf die Schaltfläche Hinzufügen folgt der von Ihnen eingegebene Portfolioname.

   ![Portfolio beim Verbinden über ein Verbindungsfeld hinzufügen](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   Das Portfolio wird erstellt und zum Verbindungsfeld des ausgewählten Datensatzes hinzugefügt.

1. (Optional) Klicken Sie in Workfront Planning auf den Namen des neuen Portfolios, um die Portfolioseite in Workfront zu öffnen und zusätzliche Aktualisierungen am Portfolio vorzunehmen.

## Erstellen Sie Programme, während Sie sie mit Datensätzen aus Workfront Planning verbinden

Sie können Programme aus der Tabellenansicht eines Datensatztyps oder der Detailseite eines Datensatzes erstellen.

So erstellen Sie Programme, während Sie sie aus Planungsdatensätzen verbinden:

1. Wechseln Sie zur Detailseite eines Datensatzes oder zur Tabelle des Datensatztyps und verbinden Sie Workfront Planning-Datensätze mit Workfront-Portfolios, wie im Artikel [Datensätze verbinden](/help/quicksilver/planning/records/connect-records.md) beschrieben.

1. Klicken Sie **Programm hinzufügen**

   Oder

   Geben Sie den Namen eines Programms ein und klicken Sie auf **Programm hinzufügen**, wenn Sie es nicht finden können. Auf die Schaltfläche Hinzufügen folgt der von Ihnen eingegebene Programmname.

   ![Fügen Sie das Workfront-Programm hinzu, wenn Sie es über das Verbindungsfeld verbinden](assets/add-wf-program-when-connecting-it-from-connection-field.png)

   Das **Programm erstellen** wird geöffnet.

1. Aktualisieren Sie den **Programmnamen**. Dies ist ein Pflichtfeld.
1. Wählen Sie eine **Portfolio** aus der Dropdown-Liste aus oder tippen Sie den Namen eines Portfolios und wählen Sie es aus, wenn es in der Liste angezeigt wird. Dies ist ein Pflichtfeld.
1. Klicken Sie auf **Erstellen**.

   Das Programm wird erstellt und dem Feld Verbindung des ausgewählten Datensatzes hinzugefügt.

1. (Optional) Klicken Sie in Workfront Planning auf den Namen des neuen Programms, um die Programmseite in Workfront zu öffnen und zusätzliche Aktualisierungen vorzunehmen.

