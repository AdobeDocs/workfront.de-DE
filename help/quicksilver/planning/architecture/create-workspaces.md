---
title: Erstellen von Arbeitsbereichen
description: Ein Arbeitsbereich ist eine Sammlung von Datensatztypen, die von einem Team verwendet werden und den Arbeitszyklus des Teams darstellen. Sie können Arbeitsbereiche in Adobe Workfront Planning vollständig anpassen. Datensatztypen sind in einem Arbeitsbereich nach Abschnitten organisiert.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 609396b2eb6413c8f6e84361757f00c2cc5e3ad6
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Erstellen von Arbeitsbereichen

{{planning-important-intro}}

In Adobe Workfront Planning sind Arbeitsbereiche zentrale Orte, an denen Teams ihre Arbeit planen.

Ein Arbeitsbereich ist eine Sammlung von Datensatztypen, die von einem Team verwendet werden und den Arbeitszyklus des Teams darstellen. Sie können Arbeitsbereiche in Adobe Workfront Planning vollständig anpassen.

Allgemeine Informationen zu Arbeitsbereichen finden Sie unter [Arbeitsbereiche - Übersicht](/help/quicksilver/planning/architecture/workspaces-overview.md).

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
   <td>   <p>Sie erhalten Verwaltungsberechtigungen für die von Ihnen erstellten Arbeitsbereiche. </p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layoutvorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!---
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
   Or
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
   <td> <p>You receive Manage permissions to the workspaces you create. </p>  
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

## Arbeitsbereich erstellen

Sie können einen Arbeitsbereich erstellen und Datensatztypen hinzufügen, um Ihre Objekte in Workfront Planning zu organisieren. Weitere Informationen zum Bearbeiten eines Arbeitsbereichs finden Sie unter [Bearbeiten von Arbeitsbereichen](/help/quicksilver/planning/architecture/edit-workspaces.md).

{{step1-to-planning}}

1. Klicken Sie auf **Arbeitsbereich erstellen**

   Das Feld Arbeitsbereich erstellen wird angezeigt. Sie können einen Arbeitsbereich von Grund auf neu erstellen oder ihn mit einer der verfügbaren Vorlagen erstellen.

1. (Optional und bedingt) Klicken Sie **Vorschau** innerhalb einer der folgenden vordefinierten Arbeitsbereichsvorlagen:

   * Einfach: Marketing-Verwaltung
   * Erweitert: Marketing-Verwaltung
   * Unternehmen: Marketing-Management
   * Vertriebsleitung
   * Produkt-Management

   Das Vorschaufeld für Vorlagen wird geöffnet.

   Es gibt einen Hinweis darauf, welche operativen Datensatztypen, Taxonomien und wie viele Felder mit jeder Vorlage verknüpft sind.

   ![Vorschau einer Workspace-Vorlage](assets/previewing-a-workspace-template.png)

   Weitere Informationen zu Workfront Planning Workspace-Vorlagen finden Sie unter [Liste der Workspace-Vorlagen](/help/quicksilver/planning/architecture/workspace-templates.md).

1. Klicken Sie im Vorlagenvorschaufeld auf **Vorlage verwenden**, um den Arbeitsbereich aus der ausgewählten Vorlage zu erstellen

   Oder

   Klicken Sie auf **Zurück** und dann auf **Neuer Arbeitsbereich**, um einen neuen Arbeitsbereich zu erstellen.

   Es wird einer für die folgenden Typen von Arbeitsbereichen erstellt:

   * Ein leerer Arbeitsbereich mit dem **Nicht benannter Workspace** in dem Sie manuell mit dem Hinzufügen von Datensatztypen beginnen können, wenn Sie einen Arbeitsbereich von Grund auf neu erstellen.
   * Ein Arbeitsbereich, der nach der ausgewählten Vorlage benannt und mit Beispieldatensatztypen gefüllt ist. Sie können die Datensatztypen und den Arbeitsbereich weiter anpassen.

   Für Workfront-Administratoren wird der neue Arbeitsbereich auf der Registerkarte **Arbeitsbereiche, an denen ich mitwirke** angezeigt.

   Für alle anderen Benutzer, die Arbeitsbereiche erstellen können, wird der neue Arbeitsbereich im Bereich **Arbeitsbereiche** angezeigt.

1. Klicken Sie in den Namen des Arbeitsbereichs in der Kopfzeile des neuen Arbeitsbereichs, um ihn umzubenennen, und drücken Sie dann die Eingabetaste.

1. (Optional und bedingt) Wenn Sie den Arbeitsbereich über eine Vorlage erstellt haben, klicken Sie in den Namen der Abschnitte **Operative Datensatztypen** oder **Taxonomien** .

   Oder

   Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie dann auf das Menü **Mehr** ![Mehr](assets/more-menu.png) und anschließend auf **Umbenennen**, um den Abschnitt umzubenennen.

   >[!TIP]
   >
   >Sie können jeden Abschnitt in jedem Arbeitsbereich umbenennen, auch wenn Sie den Abschnitt nicht erstellt haben.

   Weitere Informationen zum Bearbeiten von Arbeitsbereichen, einschließlich der Abschnitte zum Bearbeiten von Arbeitsbereichen, finden Sie unter [Bearbeiten von Arbeitsbereichen](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Optional) Klicken Sie auf **Datensatztyp hinzufügen**, um Datensatztypen zu dem Arbeitsbereich in einem beliebigen Abschnitt hinzuzufügen.

   Weitere Informationen finden Sie [Datensatztypen erstellen](/help/quicksilver/planning/architecture/create-record-types.md).

   Weitere Informationen zum Bearbeiten und Löschen von Datensatztypen in einem Arbeitsbereich finden Sie unter [Bearbeiten von Arbeitsbereichen](/help/quicksilver/planning/architecture/edit-workspaces.md).


