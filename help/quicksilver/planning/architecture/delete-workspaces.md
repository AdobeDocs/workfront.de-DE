---
title: Löschen von Arbeitsbereichen
description: Sie können Arbeitsbereiche löschen, die nicht mehr relevant sind.
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: 83c716dea3815ed9a2ce4c3d0598ef42b128de87
workflow-type: tm+mt
source-wordcount: '445'
ht-degree: 1%

---


# Löschen von Arbeitsbereichen

{{planning-important-intro}}

In der Adobe Workfront-Planung sind Arbeitsbereiche zentrale Standorte für Teams zur Arbeitsplanung. Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

Sie können nicht mehr relevante Arbeitsbereiche löschen.

Es wird empfohlen, einige oder alle Datensatztypen, Datensätze, Felder und Ansichten, die mit dem Arbeitsbereich verknüpft sind, den Sie löschen möchten, neu zu erstellen, bevor Sie ihn löschen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Workfront-Planung anzuzeigen.

Für den Zugriff auf die Workfront-Planung benötigen Sie Folgendes:

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
<p>Die folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Erstklassig</li> 
<li>Ultimativ</li></ul> 
<p>Die Workfront-Planung ist für veraltete Workfront-Pläne nicht verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungsplan*</p></td> 
   <td> 
<p>Alle </p> 
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen finden Sie unter <a href="https://business.adobe.com/products/workfront/pricing.html">Preise und Verpackung für Adobe Workfront</a>. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Die Workfront-Instanz Ihres Unternehmens muss in das Adobe Unified Experience integriert sein, damit Sie auf alle Funktionen der Workfront-Planung zugreifen können.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard </p>
   <p>Für ältere Workfront-Lizenzen ist die Workfront-Planung nicht verfügbar.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Für die Adobe Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Berechtigungen für einen Arbeitsbereich verwalten</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--
OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
    
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information about access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->


## Überlegungen zum Löschen von Arbeitsbereichen

* Beim Löschen von Arbeitsbereichen werden auch alle Datensatztypen, Datensätze, Felder und Ansichten gelöscht.
* Gelöschte Arbeitsbereiche und die darin enthaltenen Informationen können nicht wiederhergestellt werden.

## Löschen eines Arbeitsbereichs

{{step1-to-planning}}

1. (Bedingt) Wenn Sie Workfront-Administrator sind, klicken Sie auf **Arbeitsbereiche, die ich verwende, um auf die erstellten Arbeitsbereiche zuzugreifen, oder auf** Andere Arbeitsbereiche **, um auf Arbeitsbereiche zuzugreifen, die für Sie freigegeben wurden.**

1. (Optional) Klicken Sie auf **Alle anzeigen** , um weitere Arbeitsbereiche anzuzeigen. Der Link **Alle anzeigen** wird nur angezeigt, wenn Sie mehr als zwei Zeilen Workspace-Karten haben.
1. (Optional) Klicken Sie auf K **Anzeigen weniger** , um die Anzahl der auf dem Bildschirm angezeigten Arbeitsbereiche zu begrenzen.
1. Um einen Arbeitsbereich zu löschen, führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie den Mauszeiger über die Workspace-Karte und klicken Sie dann oben rechts auf der Karte auf das Menü **Mehr** ![](assets/more-menu.png) .
Oder
   * Klicken Sie auf eine Workspace-Karte, um den Arbeitsbereich zu öffnen, und klicken Sie dann auf das Menü **Mehr** rechts neben dem Arbeitsbereichnamen.![](assets/more-menu.png)
1. Klicken Sie auf **Löschen**.

   ![](assets/permanently-delete-workspace-confirmation.png)

1. Geben Sie &quot;**delete**&quot;in den verfügbaren Bereich ein und klicken Sie dann auf **Permanentes Löschen**. Dabei wird nicht zwischen Groß- und Kleinschreibung unterschieden.

   Der Arbeitsbereich wird gelöscht und kann nicht wiederhergestellt werden. Alle Datensatztypen, Datensätze, Felder und Ansichten, die mit ihnen verknüpft sind, werden ebenfalls gelöscht. <!--ensure this is right at or before GA-->
