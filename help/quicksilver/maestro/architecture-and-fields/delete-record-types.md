---
title: Löschen von Datensatztypen
description: Sie können betriebliche Datensatztypen oder Taxonomie-Datensatztypen löschen, wenn sie nicht mehr relevant sind.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav:
---
title: Delete record types
description: You can delete operational record types or taxonomy record types when they are no longer relevant. 
author: Alina
feature: Work Management
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->

# Löschen von Datensatztypen

>[!IMPORTANT]
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

Sie können betriebliche Datensatztypen oder Taxonomie-Datensatztypen löschen, wenn sie nicht mehr relevant sind.

Informationen zu Datensatztypen und Taxonomien finden Sie unter [Übersicht über Datensatztypen und Taxonomien](../architecture-and-fields/overview-of-record-types-and-taxonomies.md).

Es wird empfohlen, die Felder und Datensätze, die mit dem Datensatztyp oder der Taxonomie verknüpft sind, die Sie löschen möchten, in einem anderen Datensatztyp neu zu erstellen, bevor Sie sie löschen.

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-Abkommen</p></td>
   <td>
<p>Ihr Unternehmen muss am Adobe Maestro Closed-Beta-Programm teilnehmen. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Abo</p></td>
   <td>
<p>Beliebig</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td>
   <td>
   <p>Beliebig</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">Zugriffsebene</td>
   <td> <p>Beliebig</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layout-Vorlage</td>
   <td> <p>Ihr Systemadministrator muss den Maestro-Bereich in Ihre Layoutvorlage einfügen. Weitere Informationen finden Sie unter <a href="../access/grant-access.md">Zugriff auf Adobe Maestro gewähren</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Überlegungen zum Löschen von Datensatztypen

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Sie können jeden Datensatztyp oder jede Taxonomie löschen, den Sie oder andere Mitarbeiter in Ihrem Unternehmen erstellt haben. <!--this will change with access levels and permissions-->
* Durch das Löschen von Datensatztypen werden alle mit ihnen verknüpften Informationen entfernt, einschließlich Feldern und Datensätzen dieses Typs.
* Gelöschte Datensatztypen und ihre Informationen können nicht abgerufen werden.

## Löschen von Datensatztypen

Das Löschen von Taxonomie-Datensatztypen ist mit dem Löschen betrieblicher Datensatztypen identisch.

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-workfront.png) in der oberen rechten Ecke von Workfront, <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> Klicken Sie dann auf **Maestro** ![](assets/maestro-icon.png).

   Der zuletzt aufgerufene Arbeitsbereich sollte standardmäßig geöffnet werden.

1. (Optional) Erweitern Sie den nach unten zeigenden Pfeil rechts neben einem vorhandenen Workspace-Namen und wählen Sie den Arbeitsbereich aus, für den Sie Datensatztypen löschen möchten.

   Der Arbeitsbereich wird geöffnet und die damit verbundenen Datensatztypen und Taxonomien werden angezeigt.
1. Klicken Sie auf die Karte für den Datensatztyp oder die Taxonomie, die Sie löschen möchten.

   Dadurch wird die Seite des Datensatztyps geöffnet.
1. Klicken Sie auf **Mehr** Menü ![](assets/more-menu.png) rechts neben dem Namen des Datensatztyps klicken Sie auf **Löschen**.
1. Klicks **Löschen** zur Bestätigung.

   Der ausgewählte Datensatztyp oder die ausgewählte Taxonomie sowie die zugehörigen Felder und Datensätze werden gelöscht.