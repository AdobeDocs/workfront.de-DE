---
title: Arbeitsbereiche löschen
description: Sie können Arbeitsbereiche löschen, wenn sie nicht mehr relevant sind.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/yzpirNfY0Hsp0cbClQA8dFqhgqbpK8ZryIyeq4tBAgw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 9053a824ecec4feb35a612b26aebb91904ef2546
workflow-type: tm+mt
source-wordcount: 499
ht-degree: 4%

---

# Löschen von Arbeitsbereichen

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

In Adobe Workfront Planning sind Arbeitsbereiche zentrale Orte, an denen Teams ihre Arbeit planen. Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

Sie können nicht mehr relevante Arbeitsbereiche löschen.

Es wird empfohlen, einige oder alle Datensatztypen, Datensätze, Felder und Ansichten, die mit dem Workspace verknüpft sind und in einem anderen Workspace gelöscht werden sollen, neu zu erstellen, bevor Sie ihn löschen.

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
<ul> 
<li><p>Beliebiges Workfront und beliebiges Planungspaket</p></li>
ODER
<li><p>Beliebiger Workflow und beliebiges Planungspaket</p></li></ul>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
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
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table>
-->

## Überlegungen zum Löschen von Arbeitsbereichen

* Wenn Sie Arbeitsbereiche löschen, werden alle Datensatztypen, Datensätze, deren Felder und Ansichten ebenfalls gelöscht.
* Gelöschte Arbeitsbereiche und die darin enthaltenen Informationen können nicht wiederhergestellt werden.

## Löschen eines Arbeitsbereichs

{{step1-to-planning}}

1. (Bedingt) Wenn Sie Workfront-Administrator sind, klicken Sie auf eine der folgenden Optionen:

   * **Workspaces I&#39;m on**, um auf von Ihnen erstellte Workspaces zuzugreifen
   * **Alle Arbeitsbereiche**, um auf für Sie freigegebene Arbeitsbereiche oder von Ihnen erstellte Arbeitsbereiche zuzugreifen

   >[!NOTE]
   >
   ><span class="preview">Sie können die Arbeitsbereiche auf der Registerkarte **Beispiel-Arbeitsbereiche** nicht löschen. Es wird empfohlen, das Vorlagenpaket für mehrere Arbeitsbereiche zu verwenden, um Arbeitsbereiche zu erstellen, die denen auf der Registerkarte Beispielarbeitsbereich ähneln. Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).</span>

1. (Optional) Klicken Sie auf **Alle anzeigen**, um zusätzliche Arbeitsbereiche anzuzeigen. Der **Alle anzeigen** wird nur angezeigt, wenn Sie mehr als zwei Zeilen Arbeitsbereichskarten haben.
1. (Optional) Klicken Sie auf **Weniger anzeigen**, um die Anzahl der Arbeitsbereiche zu begrenzen, die auf dem Bildschirm angezeigt werden.
1. Führen Sie einen der folgenden Schritte aus, um einen Arbeitsbereich zu löschen:

   * Bewegen Sie den Mauszeiger über die Arbeitsbereichskarte und klicken Sie dann auf **Mehr** Menü ![Mehr](assets/more-menu.png) in der oberen rechten Ecke der Karte
ODER
   * Klicken Sie auf **search**-Symbol ![search-Symbol](assets/search-icon.png) in der rechten oberen Ecke der Seite „Workspace“, um nach einem Workspace anhand des Namens zu suchen, und klicken Sie auf eine Workspace-Karte, um den Workspace zu öffnen. Klicken Sie dann auf das **More**-Menü ![More-Menü](assets/more-menu.png) rechts neben dem Workspace-Namen.

   >[!TIP]
   >
   >Sie können die folgende Tastaturkombination verwenden, um das globale Suchfeld von einer beliebigen Workfront-Planungsseite aus zu öffnen und nach Arbeitsbereichen zu suchen:
   >
   >* STRG+K für Windows
   >* ⌘+K für Mac

1. Klicken Sie auf **Löschen**.

   ![Arbeitsbereich-Bestätigung dauerhaft löschen](assets/permanently-delete-workspace-confirmation.png)

1. Geben Sie &quot;**delete**&quot; in das bereitgestellte Feld ein und klicken Sie dann auf **Permanent delete**. Hierbei wird nicht zwischen Groß- und Kleinschreibung unterschieden.

   Der Arbeitsbereich wurde gelöscht und kann nicht wiederhergestellt werden. Alle Datensatztypen, Datensätze, Felder und Ansichten, die mit ihnen verknüpft sind, werden ebenfalls gelöscht. <!--ensure this is right at or before GA-->


