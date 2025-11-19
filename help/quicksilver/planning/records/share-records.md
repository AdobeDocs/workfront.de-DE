---
title: Freigeben von Datensätzen über einen Link
description: Sie können Datensätze für andere freigeben, um die Zusammenarbeit zu verbessern.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: 15ffe027c281782bcaa4df229badc134d91195a0
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 1%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

<!--take out preview and production references at release-->

# Freigeben von Datensätzen über einen Link

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->

{{planning-important-intro}}

Um mit anderen Benutzern zusammenzuarbeiten, können Sie Datensätze für andere freigeben.

Sie können einen Adobe Workfront Planning-Datensatz wie folgt freigeben:

* Kopieren Sie den Link der Datensatzseite aus Ihrem Browser, wenn die Seite geöffnet ist.

* Kopieren Sie bei der Anzeige von Datensätzen in der Tabellenansicht des Datensatztyps einen Link auf die Seite des Datensatzes.

* Sie können alle Datensätze in einem Arbeitsbereich für andere Benutzer freigeben, indem Sie den Arbeitsbereich und den Datensatztyp freigeben.

  Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Freigeben eines Arbeitsbereichs](/help/quicksilver/planning/access/share-workspaces.md)

   * [Datensatztyp freigeben](/help/quicksilver/planning/access/share-record-types.md)

<!--When we release record-level permissions, replace the bullets above with these:

You can share an Adobe Workfront Planning record in the following ways: 

* Copy the link of the record page from your browser when the page is open. 

* Copy a link to the record's page when viewing records in the record type's table view.   

* In the Production environment: 

   * You can share all records in a workspace with other users by sharing the workspace and the record type.

      For more information see the following articles:

      * [Share a workspace](/help/quicksilver/planning/access/share-workspaces.md)

      * [Share a record type](/help/quicksilver/planning/access/share-record-types.md)

<div class="preview">

* In the Preview environment: 

   * You can share individual records with people, teams, roles, groups, or companies.

</div>
-->

<!--take out the sentence below when we release record-level sharing-->

In diesem Artikel wird beschrieben, wie Sie einen Link zur Datensatzseite aus der Tabellenansicht eines Datensatztyps kopieren können.

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
   <td><p>Mitwirkender oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>  <p>Anzeigen von oder höheren Berechtigungen für einen Arbeitsbereich und einen Datensatztyp, um einen Datensatz über einen Link freizugeben</p>
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> Benutzenden mit einer Light- oder Contributor-Lizenz muss eine Layout-Vorlage zugewiesen werden, die Planning enthält.
   <p>Für Standardbenutzer und Systemadministratoren sind die Planungsbereiche standardmäßig aktiviert.</p></div></li></ul>
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
   <td><p> Contributor or higher license </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  <p>View or higher permissions to a workspace and record typeto share   a record using a link </p>
   <p>Manage permissions to a workspace and record type to share the records in the workspace </p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table> -->


## Freigeben von Datensatz-Links aus der Tabellenansicht vom Typ Datensatz

{{step1-to-planning}}

Der zuletzt aufgerufene Arbeitsbereich wird geöffnet.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. (Bedingt) Wählen Sie **Dropdownmenü** Ansicht“ oben rechts in der Tabelle eine Tabellenansicht aus. Dies sollte die Standardansicht sein, es sei denn, Sie haben den Datensatztyp in der Zeitleisten -Ansicht zum Zeitpunkt des letzten Zugriffs angezeigt.

   Die mit dem ausgewählten Datensatztyp verknüpften Datensätze werden in der Tabellenansicht angezeigt.

1. Rechtsklick auf eine Datensatzzeile

   Oder

   Bewegen Sie den Mauszeiger über den Namen eines Datensatzes und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) und dann auf **Link kopieren**.

   ![Kontextmenü für Datensatzzeile](assets/contextual-menu-for-record-row.png)

   Der Link wird in die Zwischenablage kopiert.

1. Fügen Sie den Link in ein E-Mail- oder Chat-Fenster ein, um ihn für andere Benutzer freizugeben. Wenn Benutzende den Link erhalten, wird die Datensatzseite geöffnet.

   >[!TIP]
   >
   >Die Felder auf der Datensatzseite sind dieselben Felder, die auch in der Tabellenansicht des Datensatzes verfügbar sind.


   <!--add there when it will be available: if they have access to this record-->

## Freigeben aller Datensätze in einem Arbeitsbereich durch Freigeben des Arbeitsbereichs

Sie können alle Datensätze in einem Arbeitsbereich freigeben, wenn Sie den Arbeitsbereich für andere freigeben.

Datensatztypen und Datensätze übernehmen dieselben Berechtigungen vom Arbeitsbereich.

Nur Benutzer mit der Berechtigung Verwalten für einen Arbeitsbereich können ihn für andere freigeben.

Weitere Informationen finden Sie unter [Freigeben eines Arbeitsbereichs](/help/quicksilver/planning/access/share-workspaces.md).

## Freigabe aller Datensätze in einem Datensatztyp durch Freigabe des Datensatztyps

Datensätze erben Berechtigungen vom Datensatztyp.

Standardmäßig erben Datensatztypen Berechtigungen vom Arbeitsbereich.

Sie können jedoch einen der folgenden Schritte ausführen:

* Deaktivieren Sie geerbte Berechtigungen aus dem Arbeitsbereich für einen Datensatztyp. Dadurch werden höhere Berechtigungen für die Datensätze entfernt, aber die Anzeigeberechtigungen für den Arbeitsbereich, den Datensatztyp und die Datensätze werden beibehalten.
* Benutzern manuell Berechtigungen für einen Datensatztyp erteilen, selbst wenn sie keine Berechtigungen für den Arbeitsbereich haben. Dadurch erhalten sie automatisch Ansichtsberechtigungen für den Arbeitsbereich. Dadurch erhalten Benutzende Berechtigungen für die Datensätze.

Nur Benutzer mit der Berechtigung Verwalten für einen Arbeitsbereich können seine Datensatztypen und Datensätze für andere freigeben.

Weitere Informationen finden Sie unter [Freigeben von Datensatztypen](/help/quicksilver/planning/access/share-record-types.md).

