---
title: Gelöschte Einträge wiederherstellen
description: Sie können gelöschte Datensätze aus dem kürzlich gelöschten Bereich in Adobe Workfront Planning wiederherstellen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Gelöschte Einträge wiederherstellen

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> -->

{{planning-important-intro}}

Sie können gelöschte Datensätze aus dem kürzlich gelöschten Bereich in Adobe Workfront Planning wiederherstellen.

Informationen zum Löschen von Datensätzen finden Sie unter [Löschen von Datensätzen](/help/quicksilver/planning/records/delete-records.md).

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
Oder
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
   <td>   <p>Beitragen von oder höhere Berechtigungen für einen Arbeitsbereich und einen Datensatztyp  </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p> </td> 
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
   <td><p> Standard</p>
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
   <td>   <p>Contribute or higher permissions to a workspace and record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->

## Überlegungen zum Wiederherstellen gelöschter Datensätze

* Sie können Datensätze wiederherstellen, die Sie oder andere Benutzer gelöscht haben.
* Datensätze werden 30 Tage lang im kürzlich gelöschten Bin gespeichert. Nach 30 Tagen werden die Datensätze dauerhaft aus Workfront Planning gelöscht.
* Wenn die gelöschten Datensätze mit anderen Datensätzen verknüpft sind, werden die verknüpften Datensätze nicht gelöscht, aber die Informationen aus dem gelöschten Datensatz werden ebenfalls gelöscht. Beim Wiederherstellen der gelöschten Datensätze werden die Informationen aus den verbundenen Datensätzen wiederhergestellt.
* Sie können Einträge stapelweise wiederherstellen.
* Wenn die Datensätze gelöscht werden, werden die folgenden Informationen im zuletzt gelöschten Bin gespeichert:
   * **Name**: Dies sind die Informationen im Primären Feld des Datensatzes. Weitere Informationen zu Primären Datensatzfeldern finden Sie unter Übersicht über Primäre Felder [&#128279;](/help/quicksilver/planning/fields/primary-field-overview.md).
   * **Löschdatum**: Uhrzeit und Datum, an dem der Datensatz gelöscht wurde.
   * **Zeit in kürzlich gelöschten**: Die Zeit seit dem Löschen des Datensatzes. Datensätze, die mehr als 30 Tage vor dem aktuellen Datum gelöscht wurden, werden nicht im kürzlich gelöschten Bin angezeigt.
   * **Gelöscht von**: Der Name des Benutzers, der den Datensatz gelöscht hat.

## Gelöschte Einträge wiederherstellen

1. Navigieren Sie zur Seite „Datensatztyp“, auf der Sie Datensätze gelöscht haben.
1. Klicken Sie auf **Rückgängig**-Symbol ![Rückgängig](assets/undo-icon.png) in der oberen rechten Ecke einer beliebigen Seitenansicht des Datensatztyps und dann auf **Zuletzt gelöscht**.

   Das Feld **Kürzlich gelöscht** wird angezeigt.

   ![Kürzlich gelöschtes Feld](assets/recently-deleted-box.png)

1. Wählen Sie die zu löschenden Datensätze aus und klicken Sie dann auf **Wiederherstellen** > **Wiederherstellen**. Sie können mehrere Datensätze auswählen.

   Wenn die Wiederherstellung erfolgreich war, erhalten Sie eine Erfolgsbenachrichtigung am unteren Bildschirmrand.
1. Wechseln Sie zur Tabellenansicht und überprüfen Sie die wiederhergestellten Datensätze.
