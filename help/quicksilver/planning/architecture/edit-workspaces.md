---
title: Arbeitsbereiche bearbeiten
description: Sie können die Informationen eines vorhandenen Arbeitsbereichs bearbeiten, z. B. umbenennen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
source-git-commit: 609396b2eb6413c8f6e84361757f00c2cc5e3ad6
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 0%

---


# Arbeitsbereiche bearbeiten

{{planning-important-intro}}

In Adobe Workfront Planning sind Arbeitsbereiche zentrale Orte, an denen Teams ihre Arbeit planen.

Ein Arbeitsbereich ist eine Sammlung von Datensatztypen, die von einem Team verwendet werden und den Arbeitszyklus des Teams darstellen. Sie können Arbeitsbereiche in Adobe Workfront Planning vollständig anpassen.

Informationen zum Erstellen von Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

Alle Änderungen, die Sie an einem Arbeitsbereich vornehmen, sind für alle sichtbar, die zumindest über Anzeigeberechtigungen für den Arbeitsbereich verfügen.

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
<p>Um auf alle Funktionen von Workfront zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
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
   <td>  <p>Verwalten von Berechtigungen für den Arbeitsbereich </p>   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutvorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--OLD

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
   <td> <p>There are no access level controls for Workfront Planning</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to the workspace </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>You must add the Planning area to your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

For more information about access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## Bearbeiten eines Arbeitsbereichs

{{step1-to-planning}}

1. (Bedingt) Wenn Sie Workfront-Administrator sind, klicken Sie auf **Arbeitsbereiche, an denen ich**, um auf von Ihnen erstellte Arbeitsbereiche zuzugreifen, oder auf **Andere Arbeitsbereiche**, um auf Arbeitsbereiche zuzugreifen, die von anderen für Sie freigegeben wurden.

<!--***********Replace the steps from the next below till the "Update the following information in the Edit workspace box:" (but keep this last step)*******-->

1. (Optional) Klicken Sie auf **Alle anzeigen**, um zusätzliche Arbeitsbereiche anzuzeigen. Der **Alle anzeigen** wird nur angezeigt, wenn Sie mehr als zwei Zeilen Arbeitsbereichskarten haben.
1. (Optional) Klicken Sie auf **Weniger anzeigen**, um die Anzahl der Arbeitsbereiche zu begrenzen, die auf dem Bildschirm angezeigt werden.
1. Führen Sie einen der folgenden Schritte aus, um einen Arbeitsbereich zu bearbeiten:

   * Bewegen Sie den Mauszeiger über die Arbeitsbereichskarte und klicken Sie dann auf **Mehr** Menü ![Mehr](assets/more-menu.png) in der oberen rechten Ecke der Karte
oder
   * Klicken Sie auf eine Arbeitsbereichskarte, um den Arbeitsbereich zu öffnen, und klicken Sie dann auf **Mehr** Menü ![Mehr](assets/more-menu.png) rechts neben dem Arbeitsbereichsnamen.
1. Klicken Sie **Bearbeiten**.

   Das **Arbeitsbereich bearbeiten** wird angezeigt.

   ![Feld Arbeitsbereich bearbeiten](assets/edit-workspace-box.png)

1. Aktualisieren Sie die folgenden Informationen im Feld **Arbeitsbereich bearbeiten**:

   * Fügen Sie einen Namen für den Arbeitsbereich hinzu. <!--did they add a label for this field?-->
   * **Beschreibung**: Fügen Sie Informationen über den Arbeitsbereich hinzu.
   * Wählen Sie ein Symbol aus, das mit dem Arbeitsbereich verknüpft werden soll.

1. Klicken Sie **Speichern**, um das Feld Arbeitsbereich bearbeiten zu schließen und Ihre Änderungen anzuwenden.

1. (Optional) Führen Sie einen der folgenden Schritte aus, um einen neuen Arbeitsbereich hinzuzufügen:

   * Klicken **unten** Arbeitsbereich auf „Abschnitt hinzufügen“.
   * Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) und klicken Sie dann **Abschnitt hinzufügen oben** oder **Abschnitt hinzufügen unten**.

1. (Optional) Führen Sie einen der folgenden Schritte aus, um die Position eines Abschnitts zu ändern:

   * Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie auf das **grab**-Symbol ![grab icon](assets/grab-icon.png) und ziehen Sie ihn dann an die rechte Stelle.
   * Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) und klicken Sie dann auf **Nach oben** oder **Nach unten**. Der Abschnitt wird innerhalb des Arbeitsbereichs nach oben oder unten verschoben.

1. (Optional) Gehen Sie wie folgt vor, um einen Workspace-Abschnitt zu löschen:

   1. Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie dann auf das Menü **Mehr** ![Mehr](assets/more-menu.png) und anschließend auf **Löschen** <!--add screen shot when UI is final?-->
   1. Wählen Sie einen neuen Abschnitt aus, in den alle Datensatztypen verschoben werden sollen, und klicken Sie auf **Löschen**. <!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      Alle Datensatztypen werden in den Auswahlabschnitt verschoben, und der Abschnitt wird gelöscht.

1. (Optional) Klicken Sie auf **Datensatztyp hinzufügen**, um Datensatztypen zum Arbeitsbereich hinzuzufügen.

   Weitere Informationen finden Sie [Datensatztypen erstellen](/help/quicksilver/planning/architecture/create-record-types.md).

1. (Optional) Zeigen Sie mit der Maus auf eine Karte für den Datensatztyp und klicken Sie oben rechts auf **Mehr** Menü ![Mehr](assets/more-menu.png) und dann auf **Bearbeiten**, um das Erscheinungsbild eines Datensatztyps zu ändern.

   Weitere Informationen finden Sie [Datensatztypen bearbeiten](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Optional) Zeigen Sie mit der Maus auf eine Karte für den Datensatztyp und klicken Sie oben rechts auf **Mehr** Menü ![Mehr](assets/more-menu.png) und dann auf **Löschen**, um einen Datensatztyp zu löschen.

   Weitere Informationen finden Sie [Löschen von Datensatztypen](/help/quicksilver/planning/architecture/delete-record-types.md).

1. (Optional) Klicken Sie auf eine Karte vom Typ Datensatz, um sie per Drag-and-Drop an eine neue Position zu ziehen. Sie können Datensatztypen per Drag-and-Drop von einem Workspace-Abschnitt in einen anderen ziehen.

   ![Datensatztypen per Drag-and-Drop in einen Arbeitsbereich ziehen](assets/drag-and-drop-record-types-in-a-workspace.png)

1. (Optional) Klicken Sie **Freigeben** in der oberen rechten Ecke des Arbeitsbereichs, um den Arbeitsbereich für andere freizugeben.

   Weitere Informationen finden Sie unter [Freigeben von Arbeitsbereichen](/help/quicksilver/planning/access/share-workspaces.md).
