---
title: Arbeitsbereiche löschen
description: Sie können Arbeitsbereiche löschen, wenn sie nicht mehr relevant sind.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '423'
ht-degree: 1%

---


# Arbeitsbereiche löschen

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

In Adobe Workfront Planning sind Arbeitsbereiche zentrale Orte, an denen Teams ihre Arbeit planen. Weitere Informationen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

Sie können nicht mehr relevante Arbeitsbereiche löschen.

Es wird empfohlen, einige oder alle Datensatztypen, Datensätze, Felder und Ansichten, die mit dem Workspace verknüpft sind und in einem anderen Workspace gelöscht werden sollen, neu zu erstellen, bevor Sie ihn löschen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

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
<p>Um auf Workfront Planning zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning ist nicht für ältere Workfront-Lizenzen verfügbar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Löschen von Arbeitsbereichen

* Wenn Sie Arbeitsbereiche löschen, werden alle Datensatztypen, Datensätze, deren Felder und Ansichten ebenfalls gelöscht.
* Gelöschte Arbeitsbereiche und die darin enthaltenen Informationen können nicht wiederhergestellt werden.

## Löschen eines Arbeitsbereichs

{{step1-to-planning}}

1. (Bedingt) Wenn Sie Workfront-Administrator sind, klicken Sie auf **Arbeitsbereiche, an denen ich**, um auf von Ihnen erstellte Arbeitsbereiche zuzugreifen, oder auf **Andere Arbeitsbereiche**, um auf Arbeitsbereiche zuzugreifen, die von anderen für Sie freigegeben wurden.

1. (Optional) Klicken Sie auf **Alle anzeigen**, um zusätzliche Arbeitsbereiche anzuzeigen. Der **Alle anzeigen** wird nur angezeigt, wenn Sie mehr als zwei Zeilen Arbeitsbereichskarten haben.
1. (Optional) Klicken Sie auf **Weniger anzeigen**, um die Anzahl der Arbeitsbereiche zu begrenzen, die auf dem Bildschirm angezeigt werden.
1. Führen Sie einen der folgenden Schritte aus, um einen Arbeitsbereich zu löschen:

   * Bewegen Sie den Mauszeiger über die Arbeitsbereichskarte und klicken Sie dann auf **Mehr** Menü ![Mehr](assets/more-menu.png) in der oberen rechten Ecke der Karte
oder
   * Klicken Sie auf eine Arbeitsbereichskarte, um den Arbeitsbereich zu öffnen, und klicken Sie dann auf **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Arbeitsbereichsnamen.
1. Klicken Sie **Löschen**.

   ![Arbeitsbereich-Bestätigung dauerhaft löschen](assets/permanently-delete-workspace-confirmation.png)

1. Geben Sie &quot;**delete**&quot; in das bereitgestellte Feld ein und klicken Sie dann auf **Permanent delete**. Hierbei wird nicht zwischen Groß- und Kleinschreibung unterschieden.

   Der Arbeitsbereich wurde gelöscht und kann nicht wiederhergestellt werden. Alle Datensatztypen, Datensätze, Felder und Ansichten, die mit ihnen verknüpft sind, werden ebenfalls gelöscht. <!--ensure this is right at or before GA-->
