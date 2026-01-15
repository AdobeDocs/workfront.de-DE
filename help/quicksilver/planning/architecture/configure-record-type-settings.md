---
title: Konfigurieren des Einstellungsbereichs eines Datensatztyps
description: Datensatztypen können nicht nur im Feld Datensatztyp bearbeiten bearbeitet werden, sondern auch auf der Seite Einstellungen .
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 5d326776b9c5b4d9d24e802375df4630508c8bd0
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 3%

---


# Konfigurieren des Bereichs Einstellungen eines Datensatztyps

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Sie können zusätzliche Einstellungen für einen Datensatztyp konfigurieren, nachdem sie in Adobe Workfront Planning gespeichert wurden.

Je nachdem, welche Funktionen Sie für einen Datensatztyp definieren möchten, können Sie zusätzliche Einstellungen konfigurieren, indem Sie einen der folgenden Schritte ausführen:

<!--the above will need to be reworded when we add automations and manage request forms to this area-->

* Bearbeiten

  Weitere Informationen finden Sie [Datensatztypen bearbeiten](/help/quicksilver/planning/architecture/edit-record-types.md).

* Konfigurieren der Seite „Einstellungen“ eines Datensatztyps.

  In diesem Artikel wird beschrieben, wie Sie einen Datensatztyp bearbeiten können, indem Sie seine Einstellungsseite konfigurieren.

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
<p>Beliebiges Workfront- und Planungspaket</p>
<p>Beliebiges Workflow- und Planungspaket</p>

<p><b>NOTIZ</b></p>

<p>So konfigurieren Sie verbindbare Datensatztypen:</p>

<ul> 
<li><p>Beliebiges Workfront- und Planungspaket</p></li>
ODER
<li><p>Ein beliebiges Workflow-Paket und ein Planning Prime- oder Ultimate-Paket</p></li></ul>

<p>So konfigurieren Sie globale Datensatztypen:</p>

<ul> 
<li><p>Beliebiges Workfront-Paket und Planning Plus-Paket</p></li>
ODER
<li><p>Ein beliebiges Workflow-Paket und ein Planning Prime- oder Ultimate-Paket</p></li></ul>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p>

</td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich</p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
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
   <td><p> Standard </p>
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
   <td>   <p>Manage permissions to a workspace and record type </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p> </td> 
  </tr> 

</tbody> 
</table> 

-->

## Konfigurieren Sie die Informationen zum Datensatztyp auf der Seite Einstellungen .

Sie können Workspace-übergreifende Funktionen für einen Datensatztyp definieren, indem Sie Informationen auf der Seite Einstellungen konfigurieren.

<!--the intro above will change when we can configure more in this area -->

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatztypen Sie bearbeiten möchten.

   Die Workspace-Seite wird geöffnet und die Datensatztypen werden angezeigt.
1. Führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über die Karte eines Datensatztyps und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) in der oberen rechten Ecke der Karte Datensatztyp und klicken Sie dann auf **Einstellungen**

     ![Weitere Menüoptionen auf der Karte „Datensatztyp“](assets/more-menu-options-from-record-type-card-with-settings-link.png)

     ODER

   * Klicken Sie auf eine Karte für den Datensatztyp, um die Seite für den Datensatztyp zu öffnen, klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und klicken Sie dann auf **Einstellungen**.

   <!--update screen shot at prod??-->

   ![Arbeitsbereichsübergreifende Einstellungen auf der Seite „Einstellungen“](assets/settings-page-cross-workspace-settings.png)

1. Der **Arbeitsbereich-übergreifende Einstellungen** ist standardmäßig ausgewählt.
1. Schalten Sie eine der folgenden Einstellungen ein oder aus:

   * **Zulassen, dass dieser Datensatztyp anderen Arbeitsbereichen hinzugefügt**, um anzugeben, dass es sich um einen globalen Datensatztyp handelt
   * **Verbindung zu diesem Datensatztyp in anderen Arbeitsbereichen zulassen** um anzugeben, dass es sich um einen verbindbaren Datensatztyp handelt.

   Die Einstellungen sind standardmäßig deaktiviert.

   Weitere Informationen finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)