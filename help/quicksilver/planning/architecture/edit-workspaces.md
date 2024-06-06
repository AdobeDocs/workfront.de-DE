---
title: Arbeitsbereiche bearbeiten
description: Sie können die Informationen eines vorhandenen Arbeitsbereichs bearbeiten, z. B. um ihn umzubenennen.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
source-git-commit: 3a819fc18e0b5f438a55265ea0c5c9679ef0fdd6
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Arbeitsbereiche bearbeiten

{{planning-important-intro}}

In der Adobe Workfront-Planung sind Arbeitsbereiche zentrale Standorte für Teams zur Arbeitsplanung.

Ein Arbeitsbereich ist eine Sammlung von Datensatztypen, die von einem Team verwendet werden und den Arbeitslebenszyklus des Teams darstellen. Sie können die Arbeitsbereiche in der Adobe Workfront-Planung vollständig anpassen.

Informationen zum Erstellen von Arbeitsbereichen finden Sie unter [Erstellen von Arbeitsbereichen](/help/quicksilver/planning/architecture/create-workspaces.md).

Alle Änderungen, die Sie an einem Arbeitsbereich vornehmen, sind für alle sichtbar, die mindestens über Anzeigeberechtigungen für den Arbeitsbereich verfügen.

## Zugriffsanforderungen

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
   <p> Produkt</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront-Abkommen</p></td>
   <td>
<p>Ihr Unternehmen muss in der Phase des frühen Zugriffs für die Workfront-Planung eingeschrieben sein </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Abo</p></td>
   <td>
<p>Alle</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td>
   <td>
   <p>Neu: Standard</p>
   <p>Aktuell: Plan</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td>
   <td> <p>Für die Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Berechtigungen für den Arbeitsbereich verwalten </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Sie müssen den Planungsbereich zu Ihrer Layoutvorlage hinzufügen. Weitere Informationen finden Sie unter <a href="/help/quicksilver/planning/access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Weitere Informationen zu Zugriffsanforderungen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## Bearbeiten eines Arbeitsbereichs

{{step1-to-planning}}

1. Klicken Sie in den Namen des Arbeitsbereichs in der Kopfzeile des neuen Arbeitsbereichs, um ihn umzubenennen, und drücken Sie dann die Eingabetaste **Eingabe**.
1. Klicken Sie auf **Mehr** Menü ![](assets/more-menu.png)rechts neben dem Workspace-Namen in der Kopfzeile klicken Sie auf **Bearbeiten**.

   ![](assets/edit-workspace-box.png)

   Aktualisieren Sie die folgenden Informationen in der **Arbeitsbereich bearbeiten** Feld:

   * Fügen Sie einen Namen für den Arbeitsbereich hinzu. <!--did they add a label for this field?-->
   * **Beschreibung**: Fügen Sie Informationen zum Arbeitsbereich hinzu.
   * Wählen Sie ein Symbol aus, das mit dem Arbeitsbereich verknüpft werden soll.

1. Klicks **Speichern** , um das Feld &quot;Arbeitsbereich bearbeiten&quot;zu schließen und Ihre Änderungen anzuwenden.

1. (Optional) Führen Sie einen der folgenden Schritte aus, um einen neuen Workspace-Abschnitt hinzuzufügen:

   * Klicks **Abschnitt hinzufügen** unten im Arbeitsbereich.
   * Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie auf **Mehr** Menü ![](assets/more-menu.png)Klicken Sie auf **Abschnitt oben hinzufügen** oder **Abschnitt unten hinzufügen**.

1. (Optional) Führen Sie einen der folgenden Schritte aus, um den Speicherort eines Abschnitts zu ändern:

   * Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie auf **Grab** icon ![](assets/grab-icon.png)und ziehen Sie sie per Drag-and-Drop an die richtige Stelle.
   * Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie auf **Mehr** Menü ![](assets/more-menu.png)Klicken Sie auf **Nach oben** oder **Nach unten**. Der Abschnitt wird innerhalb des Arbeitsbereichs nach oben oder unten verschoben.

1. (Optional) Gehen Sie wie folgt vor, um einen Arbeitsbereich zu löschen:

   1. Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie auf die Schaltfläche **Mehr** Menü ![](assets/more-menu.png)Klicken Sie auf **Löschen**. <!--add screen shot when UI is final?-->
   1. Wählen Sie einen neuen Abschnitt aus, um alle Datensatztypen dorthin zu verschieben, und klicken Sie dann auf **Löschen**. <!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      Alle Datensatztypen werden in den Auswahlabschnitt verschoben und der Abschnitt wird gelöscht.

1. (Optional) Klicken Sie auf **Datensatztyp hinzufügen** , um dem Arbeitsbereich Datensatztypen hinzuzufügen.

   Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

1. (Optional) Bewegen Sie den Mauszeiger über eine Karte vom Typ &quot;Record&quot;, klicken Sie auf die **Mehr** Menü ![](assets/more-menu.png) in der oberen rechten Ecke und klicken Sie auf **Bearbeiten** , um das Erscheinungsbild eines Datensatztyps zu ändern.

   Weitere Informationen finden Sie unter [Datensatztypen bearbeiten](/help/quicksilver/planning/architecture/edit-record-types.md).

1. (Optional) Bewegen Sie den Mauszeiger über eine Karte vom Typ &quot;Record&quot;, klicken Sie auf die **Mehr** Menü ![](assets/more-menu.png) in der oberen rechten Ecke und klicken Sie auf **Löschen** , um einen Datensatztyp zu löschen.

   Weitere Informationen finden Sie unter [Löschen von Datensatztypen](/help/quicksilver/planning/architecture/delete-record-types.md)).

1. (Optional) Klicken Sie auf eine Karte vom Typ Datensatz, um sie zu ziehen und an einer neuen Stelle abzulegen. Sie können Datensatztypen per Drag-and-Drop von einem Arbeitsbereich in einen anderen Arbeitsbereich ziehen.

   ![](assets/drag-and-drop-record-types-in-a-workspace.png)

1. (Optional) Klicken Sie auf **Freigeben** in der oberen rechten Ecke des Arbeitsbereichs, um den Arbeitsbereich für andere freizugeben.

   Weitere Informationen finden Sie unter [Freigeben von Arbeitsbereichen](/help/quicksilver/planning/access/share-workspaces.md).
