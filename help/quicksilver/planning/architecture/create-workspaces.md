---
title: Erstellen von Arbeitsbereichen
description: Ein Arbeitsbereich ist eine Sammlung von Datensatztypen, die von einem Team verwendet werden und den Arbeitslebenszyklus des Teams darstellen. Sie können die Arbeitsbereiche in der Adobe Workfront-Planung vollständig anpassen. Die Typen von Datensätzen sind nach Abschnitten in einem Arbeitsbereich organisiert.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Erstellen von Arbeitsbereichen

{{planning-important-intro}}

In der Adobe Workfront-Planung sind Arbeitsbereiche zentrale Standorte für Teams zur Arbeitsplanung.

Ein Arbeitsbereich ist eine Sammlung von Datensatztypen, die von einem Team verwendet werden und den Arbeitslebenszyklus des Teams darstellen. Sie können die Arbeitsbereiche in der Adobe Workfront-Planung vollständig anpassen.

Allgemeine Informationen zu Arbeitsbereichen finden Sie unter [Arbeitsbereiche - Übersicht](/help/quicksilver/planning/architecture/workspaces-overview.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Workfront-Planung anzuzeigen.

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
   <td><p> Standard </p>
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
   <td>   <p>Sie erhalten Verwaltungsberechtigungen für die von Ihnen erstellten Arbeitsbereiche. </p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

Sie können einen Arbeitsbereich erstellen und ihm Datensatztypen hinzufügen, um Ihre Objekte in der Workfront-Planung zu organisieren. Weitere Informationen zum Bearbeiten eines Arbeitsbereichs finden Sie unter [Arbeitsbereiche bearbeiten](/help/quicksilver/planning/architecture/edit-workspaces.md).

{{step1-to-planning}}

1. Klicken Sie auf **Arbeitsbereich erstellen**

   Das Feld Arbeitsbereich erstellen wird angezeigt. Sie können einen Arbeitsbereich von Grund auf neu erstellen oder mithilfe einer der verfügbaren Vorlagen erstellen.

1. (Optional und bedingt) Klicken Sie in einer der folgenden vordefinierten Workspace-Vorlagen auf **Vorschau** :

   * Allgemein: Marketing-Management
   * Erweitert: Marketing-Management
   * Unternehmen: Marketing-Management
   * Vertriebsmanagement
   * Produktverwaltung

   Das Vorlagenvorschaufeld wird geöffnet.

   Es gibt einen Hinweis darauf, welche operationellen Datensatztypen, Taxonomien und wie viele Felder mit jeder Vorlage verknüpft sind.

   ![](assets/previewing-a-workspace-template.png)

   Weitere Informationen zu Workfront Planning Workspace-Vorlagen finden Sie unter [Liste der Workspace-Vorlagen](/help/quicksilver/planning/architecture/workspace-templates.md).

1. Klicken Sie im Vorlagenvorschaufeld auf **Vorlage verwenden** , um mit der Erstellung des Arbeitsbereichs aus der ausgewählten Vorlage zu beginnen.

   Oder

   Klicken Sie auf **Zurück** und dann auf **Neuer Arbeitsbereich** , um einen neuen Arbeitsbereich zu erstellen.

   Eine für die folgenden Arten von Arbeitsbereichen wird erstellt:

   * Ein leerer Arbeitsbereich mit dem Namen **Unbenannter Workspace** , in dem Sie Datensatztypen manuell hinzufügen können, wenn Sie einen neuen Arbeitsbereich erstellen.
   * Ein Arbeitsbereich mit dem Namen nach der ausgewählten Vorlage, der mit Beispieldatensatztypen gefüllt ist. Sie können die Datensatztypen und den Arbeitsbereich weiter anpassen.

   Für Workfront-Administratoren wird der neue Arbeitsbereich auf der Registerkarte **Arbeitsbereiche, die ich verwende** angezeigt.

   Für alle anderen Benutzer, die Arbeitsbereiche erstellen können, wird der neue Arbeitsbereich im Bereich **Arbeitsbereiche** angezeigt.

1. Klicken Sie in den Namen des Arbeitsbereichs in der Kopfzeile des neuen Arbeitsbereichs, um ihn umzubenennen, und drücken Sie dann die Eingabetaste.

1. (Optional und bedingt) Wenn Sie den Arbeitsbereich aus einer Vorlage erstellt haben, klicken Sie in den Namen der Abschnitte **Typen für operative Datensätze** oder **Taxonomien** .

   Oder

   Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie dann auf das Menü **Mehr** ![](assets/more-menu.png) und dann auf **Umbenennen** , um den Abschnitt umzubenennen.

   >[!TIP]
   >
   >Sie können jeden Abschnitt aus einem beliebigen Arbeitsbereich umbenennen, auch wenn Sie den Abschnitt nicht erstellt haben.

   Weitere Informationen zum Bearbeiten von Arbeitsbereichen, einschließlich der Bearbeitung von Arbeitsbereichen, finden Sie unter [Arbeitsbereiche bearbeiten](/help/quicksilver/planning/architecture/edit-workspaces.md).

1. (Optional) Klicken Sie auf **Hinzufügen des Datensatztyps** , um dem Arbeitsbereich in einem beliebigen Abschnitt Datensatztypen hinzuzufügen.

   Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md).

   Weitere Informationen zum Bearbeiten und Löschen von Datensatztypen in einem Arbeitsbereich finden Sie unter [Arbeitsbereiche bearbeiten](/help/quicksilver/planning/architecture/edit-workspaces.md).


