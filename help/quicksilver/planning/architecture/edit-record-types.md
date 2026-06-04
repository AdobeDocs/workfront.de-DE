---
title: Datensatztypen bearbeiten
description: Datensatztypen können nach ihrem Speichern bearbeitet werden. Datensatztypen sind die Objekttypen von Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/PNC5GvQItDhcmQ0TSup8vbJJ3uWn2k-v-lKBZJBhakw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 611
ht-degree: 4%

---

# Bearbeiten von Eintragstypen

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Datensatztypen sind die Objekttypen von Adobe Workfront Planning. Sie können das Erscheinungsbild von Datensatztypen bearbeiten, die Sie oder eine andere Person erstellt haben. Informationen zum Erstellen von Workfront Planning-Datensatztypen finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

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
<p>Beliebiges Workfront- und Planungspaket</p>
<p><b>NOTIZ</b></p>
<p>So konfigurieren Sie verbindbare Datensatztypen: </p>
<ul> 
<li><p>Jedes Workfront-Paket und jedes Planungspaket</p></li>
ODER
<li><p>Beliebiger Workflow und ein Planning Prime- oder Ultimate-Paket</p></li></ul>


<p>So konfigurieren Sie globale Datensatztypen:</p>

<ul> 
<li><p>Beliebiges Workfront-Paket und Planning Plus-Paket</p></li>
ODER
<li><p>Beliebiger Workflow und ein Planning Prime- oder Ultimate-Paket</p></li></ul>
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

## Bearbeiten von Eintragstypen

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatztypen Sie bearbeiten möchten.

   Die Workspace-Seite wird geöffnet und die Datensatztypen werden angezeigt.
1. Führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über die Karte eines Datensatztyps und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) in der oberen rechten Ecke der Karte Datensatztyp und klicken Sie dann auf **Bearbeiten** oder **Einstellungen**
oder
   * Klicken Sie auf eine Karte für den Datensatztyp, um die Seite für den Datensatztyp zu öffnen. Klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und dann auf **Bearbeiten** oder **Einstellungen**.

   ![Weitere Menüoptionen auf der Karte „Datensatztyp“ mit Einstellungen](assets/more-menu-options-from-record-type-card-with-settings-link.png)

1. Im Feld **Datensatztyp bearbeiten** wird standardmäßig die Registerkarte **Erscheinungsbild** geöffnet.

   ![Registerkarte „Erscheinungsbild des Felds „Datensatztyp bearbeiten“ ](assets/edit-record-type-box-appearance-tab.png)

   Aktualisieren Sie die folgenden Informationen auf der Registerkarte **Erscheinungsbild**:

   * Bearbeiten Sie bei Bedarf den Namen des Datensatztyps. <!--did they add a field label for this?-->
   * **Beschreibung**: Bearbeiten oder fügen Sie eine Beschreibung für den Datensatztyp mit weiteren Informationen hinzu.
   * Bearbeiten Sie die Farbe und Form des Symbols, das mit dem Datensatztyp verknüpft ist. Gehen Sie folgendermaßen vor:
      * Farbe zur Identifizierung des Datensatztyps auswählen. Dies ist die Farbe des Symbols für den Datensatztyp.
      * Wählen Sie ein Symbol aus der Liste aus oder geben Sie den Namen eines Symbols ein, um zu beschreiben, was es darstellt, und wählen Sie es dann aus, wenn es angezeigt wird. Dies ist das Symbol des Datensatztyps. Standardmäßig ist ein Dateisymbol ausgewählt.

1. (Optional und bedingt) Wenn Sie Systemadministrator sind, klicken Sie auf die Registerkarte **Arbeitsbereichsübergreifende Einstellungen** und aktualisieren Sie die Informationen zu den arbeitsbereichsübergreifenden Funktionen des Datensatztyps.

   Weitere Informationen finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

   ![Feld „Datensatztyp bearbeiten“ mit der Registerkarte „Arbeitsbereich-übergreifende Einstellungen“](assets/edit-record-type-box-advanced-settings-tab.png)

1. Klicken Sie auf **Speichern**.

   Wenn Sie ausgewählt haben, diesen Datensatz von anderen Arbeitsbereichen zu verbinden, wird das Symbol **Verbindbarer Datensatz** (Symbol ![ Verbindung von anderen ](assets/connect-from-other-workspaces-icon.png)) auf der Datensatzkarte angezeigt.

   Wenn Sie ausgewählt haben, dass dieser Datensatz anderen Arbeitsbereichen hinzugefügt werden kann, wird **Symbol „Globaler**&quot; ![Symbol „Globaler Datensatztyp](assets/global-icon.png) auf der Datensatzkarte angezeigt.

1. (Optional) Klicken Sie im Arbeitsbereich auf die Karte Datensatztyp , um die Seite des Datensatztyps zu öffnen, und benennen Sie dann den Datensatztyp in der Kopfzeile um.

1. (Optional) Zum Bearbeiten eines anderen Datensatztyps erweitern Sie auf der Seite „Datensatztyp“ den nach unten zeigenden Pfeil rechts neben dem Namen eines Datensatztyps, suchen Sie nach einem Datensatztyp und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.

   ![Dropdown-Liste „Datensatztyp“ auf der Seite „Datensatztyp“ mit Suchfeld](assets/record-type-drop-down-on-record-type-page-with-search-box.png)

   >[!TIP]
   >
   >Sie können die folgende Tastaturkombination verwenden, um das globale Suchfeld von jeder Workfront-Planungs -Seite aus zu öffnen und nach Datensatztypen zu suchen:
   >
   >* STRG+K für Windows
   >* ⌘+K für Mac
   >
   >![Globales Suchfeld](assets/global-search-box.png)
