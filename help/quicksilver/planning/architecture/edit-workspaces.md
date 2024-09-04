---
title: Arbeitsbereiche bearbeiten
description: Sie können die Informationen eines vorhandenen Arbeitsbereichs bearbeiten, z. B. um ihn umzubenennen.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
source-git-commit: bd202821687453288c96147933331c8a7a6b3acb
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---


# Arbeitsbereiche bearbeiten

{{planning-important-intro}}

In der Adobe Workfront-Planung sind Arbeitsbereiche zentrale Standorte für Teams zur Arbeitsplanung.

Ein Arbeitsbereich ist eine Sammlung von Datensatztypen, die von einem Team verwendet werden und den Arbeitslebenszyklus des Teams darstellen. Sie können die Arbeitsbereiche in der Adobe Workfront-Planung vollständig anpassen.

Informationen zum Erstellen von Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

Alle Änderungen, die Sie an einem Arbeitsbereich vornehmen, sind für alle sichtbar, die mindestens über Anzeigeberechtigungen für den Arbeitsbereich verfügen.

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
<p>Weitere Informationen zu den Funktionen der einzelnen Workfront-Planungspläne erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
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
   <td><p> Standard</p>
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
   <td>  <p>Berechtigungen für den Arbeitsbereich verwalten </p>   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

1. (Bedingt) Wenn Sie Workfront-Administrator sind, klicken Sie auf **Arbeitsbereiche, die ich verwende, um auf die erstellten Arbeitsbereiche zuzugreifen, oder auf** Andere Arbeitsbereiche **, um auf Arbeitsbereiche zuzugreifen, die für Sie freigegeben wurden.**

<!--***********Replace the steps from the next below till the "Update the following information in the Edit workspace box:" (but keep this last step)*******-->

1. (Optional) Klicken Sie auf **Alle anzeigen** , um weitere Arbeitsbereiche anzuzeigen. Der Link **Alle anzeigen** wird nur angezeigt, wenn Sie mehr als zwei Zeilen Workspace-Karten haben.
1. (Optional) Klicken Sie auf K **Anzeigen weniger** , um die Anzahl der auf dem Bildschirm angezeigten Arbeitsbereiche zu begrenzen.
1. Führen Sie einen der folgenden Schritte aus, um einen Arbeitsbereich zu bearbeiten:

   * Bewegen Sie den Mauszeiger über die Workspace-Karte und klicken Sie dann oben rechts auf der Karte auf das Menü **Mehr** ![](assets/more-menu.png) .
Oder
   * Klicken Sie auf eine Workspace-Karte, um den Arbeitsbereich zu öffnen, und klicken Sie dann auf das Menü **Mehr** rechts neben dem Arbeitsbereichnamen.![](assets/more-menu.png)
1. Klicken Sie auf **Bearbeiten**.

   Das Feld **Arbeitsbereich bearbeiten** wird angezeigt.

   ![](assets/edit-workspace-box.png)

1. Aktualisieren Sie die folgenden Informationen im Feld **Arbeitsbereich bearbeiten** :

   * Fügen Sie einen Namen für den Arbeitsbereich hinzu. <!--did they add a label for this field?-->
   * **Beschreibung**: Fügen Sie Informationen zum Arbeitsbereich hinzu.
   * Wählen Sie ein Symbol aus, das mit dem Arbeitsbereich verknüpft werden soll.

1. Klicken Sie auf **Speichern** , um das Feld &quot;Arbeitsbereich bearbeiten&quot;zu schließen und Ihre Änderungen anzuwenden.

1. (Optional) Führen Sie einen der folgenden Schritte aus, um einen neuen Workspace-Abschnitt hinzuzufügen:

   * Klicken Sie unten im Arbeitsbereich auf **Abschnitt hinzufügen** .
   * Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie auf das Menü **Mehr** ![](assets/more-menu.png) und klicken Sie dann auf **Abschnitt über** hinzufügen oder auf **Abschnitt unter** hinzufügen .

1. (Optional) Führen Sie einen der folgenden Schritte aus, um den Speicherort eines Abschnitts zu ändern:

   * Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie auf das Symbol **Grab** ![](assets/grab-icon.png) und ziehen Sie es dann an die rechte Stelle.
   * Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie auf das Menü **Mehr** ![](assets/more-menu.png) und klicken Sie dann auf **Nach oben verschieben** oder **Nach unten**. Der Abschnitt wird innerhalb des Arbeitsbereichs nach oben oder unten verschoben.

1. (Optional) Gehen Sie wie folgt vor, um einen Arbeitsbereich zu löschen:

   1. Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie dann auf das Menü **Mehr** ![](assets/more-menu.png) und dann auf **Löschen**. <!--add screen shot when UI is final?-->
   1. Wählen Sie einen neuen Abschnitt aus, um alle Datensatztypen darauf zu verschieben, und klicken Sie dann auf **Löschen** <!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->.

      Alle Datensatztypen werden in den Auswahlabschnitt verschoben und der Abschnitt wird gelöscht.

1. (Optional) Klicken Sie auf **Hinzufügen des Datensatztyps** , um dem Arbeitsbereich Datensatztypen hinzuzufügen.

   Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

1. (Optional) Bewegen Sie den Mauszeiger über eine Karte vom Typ &quot;Record&quot;, klicken Sie oben rechts auf das Menü **Mehr** ![](assets/more-menu.png) und klicken Sie dann auf **Bearbeiten** , um das Erscheinungsbild eines Datensatztyps zu ändern.

   Weitere Informationen finden Sie unter [Bearbeiten von Datensatztypen](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Optional) Bewegen Sie den Mauszeiger über eine Karte vom Typ &quot;Record&quot;, klicken Sie oben rechts auf das Menü **Mehr** ![](assets/more-menu.png) und dann auf **Löschen** , um einen Datensatztyp zu löschen.

   Weitere Informationen finden Sie unter [Löschen von Datensatztypen](/help/quicksilver/planning/architecture/delete-record-types.md).

1. (Optional) Klicken Sie auf eine Karte vom Typ Datensatz, um sie zu ziehen und an einer neuen Stelle abzulegen. Sie können Datensatztypen per Drag-and-Drop von einem Arbeitsbereich in einen anderen Arbeitsbereich ziehen.

   ![](assets/drag-and-drop-record-types-in-a-workspace.png)

1. (Optional) Klicken Sie oben rechts im Arbeitsbereich auf **Freigeben** , um den Arbeitsbereich für andere freizugeben.

   Weitere Informationen finden Sie unter [Freigeben von Arbeitsbereichen](/help/quicksilver/planning/access/share-workspaces.md).
