---
title: Gelöschte Einträge wiederherstellen
description: Sie können gelöschte Datensätze aus dem kürzlich gelöschten Bereich in Adobe Workfront Planning wiederherstellen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 8b6df633-eb05-4d3e-bfe6-76cedabdb76d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/6F-GarlW1gY0gHEZIC-CgSiN75EMd2RcZZUGgyOgqxU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 455
ht-degree: 3%

---

# Wiederherstellen gelöschter Einträge


<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


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
<p>Beliebiges Workfront und beliebiges Planungspaket</p> <p>Beliebiger Workflow und beliebiges Planungspaket</p>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Tragen Sie Berechtigungen oder höhere Berechtigungen zu einem Arbeitsbereich, einem Datensatztyp und <span class="preview">Verwalten von Berechtigungen für einen Datensatz) </span> </p>    
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p> </td> 
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
</table>
-->

## Überlegungen zum Wiederherstellen gelöschter Datensätze

* Sie können Datensätze wiederherstellen, die Sie oder andere Benutzer gelöscht haben.
* Datensätze werden 30 Tage lang im kürzlich gelöschten Bin gespeichert. Nach 30 Tagen werden die Datensätze dauerhaft aus Workfront Planning gelöscht.
* Wenn die gelöschten Datensätze mit anderen Datensätzen verknüpft sind, werden die verknüpften Datensätze nicht gelöscht, aber die Informationen aus dem gelöschten Datensatz werden ebenfalls gelöscht. Beim Wiederherstellen der gelöschten Datensätze werden die Informationen aus den verbundenen Datensätzen wiederhergestellt.
* Sie können Einträge stapelweise wiederherstellen.
* Wenn die Datensätze gelöscht werden, werden die folgenden Informationen im zuletzt gelöschten Bin gespeichert:
   * **Name**: Dies sind die Informationen im Primären Feld des Datensatzes. Weitere Informationen zu Primären Datensatzfeldern finden Sie unter Übersicht über Primäre Felder [](/help/quicksilver/planning/fields/primary-field-overview.md).
   * **Löschdatum**: Uhrzeit und Datum, an dem der Datensatz gelöscht wurde.
   * **Zeit in kürzlich gelöschten**: Die Zeit seit dem Löschen des Datensatzes. Datensätze, die mehr als 30 Tage vor dem aktuellen Datum gelöscht wurden, werden nicht im kürzlich gelöschten Bin angezeigt.
   * **Gelöscht von**: Der Name des Benutzers, der den Datensatz gelöscht hat.

## Wiederherstellen gelöschter Einträge

1. Navigieren Sie zur Seite „Datensatztyp“, auf der Sie Datensätze gelöscht haben.
1. Klicken Sie auf **Rückgängig**-Symbol ![Rückgängig](assets/undo-icon.png) in der oberen rechten Ecke einer beliebigen Seitenansicht des Datensatztyps und dann auf **Zuletzt gelöscht**.

   Das Feld **Kürzlich gelöscht** wird angezeigt.

   ![Kürzlich gelöschtes Feld](assets/recently-deleted-box.png)

1. Wählen Sie die zu löschenden Datensätze aus und klicken Sie dann auf **Wiederherstellen** > **Wiederherstellen**. Sie können mehrere Datensätze auswählen.

   Wenn die Wiederherstellung erfolgreich war, erhalten Sie eine Erfolgsbenachrichtigung am unteren Bildschirmrand.
1. Wechseln Sie zur Tabellenansicht und überprüfen Sie die wiederhergestellten Datensätze.
