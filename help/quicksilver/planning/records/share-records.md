---
title: Freigeben von Datensätzen über einen Link
description: Sie können Datensätze für andere freigeben, um die Zusammenarbeit zu verbessern.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Ct6I5wnivCVr3V86Zj4F7stm2IVUJVH50yvTRyWFuUA
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: b186900d58f6a422c787cef881a4d06d6cd7feed
workflow-type: tm+mt
source-wordcount: 677
ht-degree: 2%

---

<!--should this move to the Access folder when we have sharing for ALL the objects???-->

# Freigeben von Einträgen über einen Link

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Um mit anderen Benutzern zusammenzuarbeiten, können Sie Datensätze für andere freigeben.

Sie können einen Adobe Workfront Planning-Datensatz wie folgt freigeben:

* Kopieren Sie den Link der Datensatzseite aus Ihrem Browser, wenn die Seite geöffnet ist.

* Kopieren Sie bei der Anzeige von Datensätzen in der Tabellenansicht des Datensatztyps einen Link auf die Seite des Datensatzes.

In diesem Artikel wird beschrieben, wie Sie Datensätze freigeben können, indem Sie einen Link freigeben.

Darüber hinaus können Sie Datensätze auf folgende Arten freigeben:

* Geben Sie alle Datensätze in einem Arbeitsbereich für andere Benutzer frei, indem Sie den Arbeitsbereich und den Datensatztyp freigeben. Standardmäßig werden alle Datensätze auch für dieselben Benutzer freigegeben.

  Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Freigeben eines Arbeitsbereichs](/help/quicksilver/planning/access/share-workspaces.md)

   * [Datensatztyp freigeben](/help/quicksilver/planning/access/share-record-types.md)

* Sie können einzelne Datensätze für Personen, Teams, Rollen, Gruppen oder Unternehmen freigeben, indem Sie die geerbten Berechtigungen deaktivieren, wenn die Datensätze für Arbeitsbereiche oder Datensatztypen freigegeben werden.

  Weitere Informationen finden Sie unter [Freigeben von Datensätzen](/help/quicksilver/planning/access/share-records.md).


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
   <td><p>Mitwirkende oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>  <p>Anzeigen von oder höheren Berechtigungen für einen Arbeitsbereich und einen Datensatztyp, um einen Datensatz über einen Link freizugeben</p>
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
</table>
-->


## Freigeben von Datensatz-Links aus der Tabellenansicht vom Typ Datensatz

{{step1-to-planning}}

Der zuletzt aufgerufene Arbeitsbereich wird geöffnet.

1. Klicken Sie auf eine Karte vom Typ Datensatz.

   Die Seite mit dem Datensatztyp wird geöffnet.

1. (Bedingt) Wählen Sie **Dropdownmenü** Ansicht“ oben rechts in der Tabelle eine Tabellenansicht aus. Dies sollte die Standardansicht sein, es sei denn, Sie haben den Datensatztyp in der Zeitleisten -Ansicht zum Zeitpunkt des letzten Zugriffs angezeigt.

   Die mit dem ausgewählten Datensatztyp verknüpften Datensätze werden in der Tabellenansicht angezeigt.

1. Rechtsklick auf eine Datensatzzeile

   ODER

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

Datensatztypen und Datensätze erben standardmäßig dieselben Berechtigungen vom Arbeitsbereich.

Nur Benutzer mit der Berechtigung Verwalten für einen Arbeitsbereich können ihn für andere freigeben.

Weitere Informationen finden Sie unter [Freigeben eines Arbeitsbereichs](/help/quicksilver/planning/access/share-workspaces.md).

## Freigabe aller Datensätze in einem Datensatztyp durch Freigabe des Datensatztyps

Standardmäßig erben Datensätze Berechtigungen vom Datensatztyp.

Standardmäßig erben Datensatztypen Berechtigungen vom Arbeitsbereich.

Sie können jedoch einen der folgenden Schritte ausführen:

* Deaktivieren Sie geerbte Berechtigungen aus dem Arbeitsbereich für einen Datensatztyp. Dadurch werden höhere Berechtigungen für die Datensätze entfernt, aber die Anzeigeberechtigungen für den Arbeitsbereich, den Datensatztyp und die Datensätze werden beibehalten.
* Benutzern manuell Berechtigungen für einen Datensatztyp erteilen, selbst wenn sie keine Berechtigungen für den Arbeitsbereich haben. Dadurch erhalten sie automatisch Ansichtsberechtigungen für den Arbeitsbereich. Dadurch erhalten Benutzende standardmäßig Anzeigeberechtigungen für die Datensätze.

Nur Benutzer mit der Berechtigung Verwalten für einen Arbeitsbereich können seine Datensatztypen und Datensätze für andere freigeben.

Weitere Informationen finden Sie unter [Freigeben von Datensatztypen](/help/quicksilver/planning/access/share-record-types.md).

## Freigeben einzelner Datensätze

Benutzer erben standardmäßig die Datensatzberechtigungen vom Arbeitsbereich und vom Datensatztyp.

Um nur ausgewählten Benutzern mit Berechtigungen für Datensatztypen Berechtigungen zum Verwalten nur bestimmter Datensätze zu erteilen, können Sie geerbte Berechtigungen für ausgewählte Datensätze deaktivieren und nur diesen Benutzern den Zugriff auf diese Datensätze verwalten gewähren.

Sie können die Berechtigungen für einen Datensatz oder für mehrere Datensätze gleichzeitig stapelweise anpassen.

Weitere Informationen finden Sie unter [Freigeben von Datensätzen](/help/quicksilver/planning/access/share-records.md).



