---
title: Datensatztypen löschen
description: Sie können Datensatztypen löschen, wenn sie nicht mehr relevant sind. Durch das Löschen von Datensatztypen werden auch alle mit den Datensatztypen verknüpften Informationen gelöscht, z. B. ihre Datensätze, Felder und Ansichten.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 7d37481fc5b468f6f8ea1fce6ccd7ae064f00251
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 2%

---


<!--keep the global record type reference in yellow till January 2026-->

# Datensatztypen löschen

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Sie können Datensatztypen löschen, wenn sie nicht mehr relevant sind.

Beim Löschen von Datensatztypen werden jedoch auch alle mit den Datensatztypen verknüpften Informationen gelöscht. Weitere Informationen finden Sie im Abschnitt [Überlegungen beim Löschen von Datensatztypen](#considerations-when-deleting-record-types) in diesem Artikel.

Weitere Informationen zu Datensatztypen finden Sie unter [Datensatztypen - Übersicht](/help/quicksilver/planning/architecture/overview-of-record-types.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen. 

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
<li>Prime</li> 
<li>Ultimate</li></ul> 
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
   <td><p> Standard</p>
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
   <td>   <p>Verwalten der Berechtigungen für einen Arbeitsbereich und Datensatztyp</p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p></td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


## Überlegungen beim Löschen von Datensatztypen

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Sie können nur Datensatztypen aus Arbeitsbereichen löschen, für die Sie über Verwaltungsberechtigungen verfügen.
* Durch das Löschen von Datensatztypen werden die folgenden mit ihnen verknüpften Informationen entfernt:

   * Alle Datensätze dieses Typs.
   * Alle mit dem Datensatztyp verknüpften Felder.
   * Alle Ansichten (einschließlich Filtern, Gruppierungen und Sortierkriterien) des Datensatztyps.
* Der Datensatztyp wird aus allen Benutzern entfernt, die auf den Arbeitsbereich zugreifen.
* Gelöschte Datensatztypen oder deren Informationen können nicht wiederhergestellt werden.
* Es wird empfohlen, die Felder und die mit dem Datensatztyp verknüpften Datensätze, die Sie löschen möchten, in einem anderen Datensatztyp neu zu erstellen, bevor Sie sie löschen.

<!--

<div class="preview">

* You cannot delete a global record type that has been added to other workspaces. 
   
   You must first delete it from the secondary workspaces where it's been added, before you can delete it from its original workspace. 

   Deleting a global record type from their secondary workspaces only remove them, their records, and that workspace's fields from the secondary workspace. It does not delete the global record type from its original workspace.

   For information, see the section "Delete a global record type from a secondary workspace" in the article [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md). 

</div>
-->

## Datensatztypen löschen

{{step1-to-planning}}

1. Klicken Sie auf den Arbeitsbereich, dessen Datensatztypen Sie löschen möchten.

   Oder

   Erweitern Sie in einem Arbeitsbereich den nach unten zeigenden Pfeil rechts neben einem vorhandenen Arbeitsbereichsnamen, suchen Sie nach einem Arbeitsbereich und wählen Sie ihn aus, wenn er in der Liste angezeigt wird.

   Der Arbeitsbereich wird geöffnet und die Datensatztypen werden angezeigt.
1. Führen Sie einen der folgenden Schritte aus:

   * Zeigen Sie mit der Maus auf die Karte für den Datensatztyp und klicken Sie auf das Menü **Mehr** und dann auf **Löschen**.
   * Klicken Sie auf die Karte für den Datensatztyp, den Sie löschen möchten, und klicken Sie auf der Seite Datensatztyp auf das Menü **Mehr** ![Mehr](assets/more-menu.png) rechts neben dem Namen des Datensatztyps und dann auf **Löschen**.

   ![Datensatztyp-Bestätigung dauerhaft löschen](assets/permanently-delete-record-type-confirmation.png)

   <!--[!TIP]
   >
   ><span class="preview">You cannot delete global record types added to other workspaces. First, delete the global record types form their secondary workspaces before deleting them from the original workspace.</span>-->


1. Geben Sie **Bestätigungsfeld** Löschen“ ein und klicken Sie dann auf **Dauerhaft löschen**. Hierbei wird nicht zwischen Groß- und Kleinschreibung unterschieden.

   Der ausgewählte Datensatztyp wird zusammen mit den zugehörigen Feldern, zugehörigen Datensätzen und Ansichten gelöscht und kann nicht wiederhergestellt werden.


