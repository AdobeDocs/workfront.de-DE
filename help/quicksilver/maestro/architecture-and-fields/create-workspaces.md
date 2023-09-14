---
title: Erstellen von Arbeitsbereichen
description: Ein Arbeitsbereich ist eine Sammlung operativer Datensatztypen und Taxonomien, die von einem Team verwendet werden und den Arbeitslebenszyklus des Teams darstellen. Sie können die Arbeitsbereiche in Maestro vollständig anpassen.
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '489'
ht-degree: 1%

---


<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Erstellen von Arbeitsbereichen

>[!IMPORTANT]
>
>Derzeit ist Adobe Maestro Teil eines Betaprogramms, das für eine begrenzte Anzahl von Kunden geöffnet ist.
>
>Wenden Sie sich an Ihren Kundenbetreuer, um weitere Informationen zum Betaprogramm für Maestro zu erhalten.
>
>Weitere Informationen finden Sie unter [Übersicht über Adobe Maestro](../maestro-overview.md).

In Adobe Maestro sind Arbeitsbereiche zentrale Standorte für Teams zur Arbeitsplanung.

Ein Arbeitsbereich ist eine Sammlung operativer Datensatztypen und Taxonomien, die von einem Team verwendet werden und den Arbeitslebenszyklus des Teams darstellen. Sie können die Arbeitsbereiche in Maestro vollständig anpassen.

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

## Überlegungen zu Arbeitsbereichen

* Sie können Arbeitsbereiche für bestimmte Organisationseinheiten in Ihrer Organisation erstellen, die der einzigartigen Funktionsweise jeder Einheit entsprechen.
* Die in einem Arbeitsbereich enthaltenen Datensatztypen und Taxonomien sollten den Arbeitszyklus einer Organisationseinheit widerspiegeln.
* Wenn Sie einen Arbeitsbereich erstellen, kann jeder in Ihrer Organisation ihn anzeigen, bearbeiten oder löschen.  <!--this will change with access levels and permissions-->
* Sie können maximal 1.000 Arbeitsbereiche in Ihrem Unternehmen haben.
* Arbeitsbereiche enthalten Datensatztypen, die für jeden Arbeitsbereich eindeutig sind. <!--this might change-->

## Erstellen eines Arbeitsbereichs

1. (Bedingt) Wenn Ihr System keine Arbeitsbereiche enthält, klicken Sie auf die Schaltfläche **Hauptmenü** icon ![](assets/main-menu-workfront.png) in der oberen rechten Ecke von Workfront, <!--or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> Klicken Sie dann auf **Maestro** ![](assets/maestro-icon.png).

   Oder klicken Sie in einem vorhandenen Arbeitsbereich auf den nach unten zeigenden Pfeil rechts neben dem Workspace-Namen und klicken Sie dann auf **Arbeitsbereich erstellen**.

   ![](assets/workspace-drop-down-right-menu.png)

   Dadurch wird der Arbeitsbereich von Maestro geöffnet.
1. (Optional und bedingt) Klicken Sie auf **Vorschau** in einer der folgenden vordefinierten Arbeitsbereichsvorlagen:

   * Marketing-Management
   * Vertriebsmanagement
   * Produktverwaltung

   Es gibt einen Hinweis darauf, welche operationellen Datensatztypen, Taxonomien und wie viele Felder mit jeder Vorlage verknüpft sind.

   ![](assets/previewing-a-workspace-template.png)

   Weitere Informationen zu Maestro Workspace-Vorlagen finden Sie unter [Liste der Workspace-Vorlagen](../architecture-and-fields/workspace-templates.md).

1. Klicks **Vorlage verwenden** , um den Arbeitsbereich aus der ausgewählten Vorlage zu erstellen

   Oder

   Klicks **Arbeitsbereich erstellen** , um einen neuen Arbeitsbereich zu erstellen.

   Eine für die folgenden Arten von Arbeitsbereichen wird erstellt:

   * Ein leerer Arbeitsbereich, in dem Sie Datensatztypen manuell hinzufügen können.
   * Ein Arbeitsbereich mit Beispieldatensatztypen, die Sie weiter anpassen können.

1. Klicken Sie in den Namen des Arbeitsbereichs in der Kopfzeile des neuen Arbeitsbereichs, um ihn umzubenennen, und drücken Sie dann die Eingabetaste

   Oder

   Klicken Sie auf **Mehr** Menü ![](assets/more-menu.png)rechts neben dem Workspace-Namen in der Kopfzeile klicken Sie auf **Umbenennen**.

1. (Optional) Klicken Sie auf **Datensatztyp hinzufügen** , um dem Arbeitsbereich Datensatztypen hinzuzufügen.

   Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](../architecture-and-fields/create-record-types.md).

1. (Optional) Klicken Sie auf **Taxonomie hinzufügen** , um dem Arbeitsbereich Taxonomien hinzuzufügen.

   Weitere Informationen finden Sie unter [Erstellen von Taxonomien](../architecture-and-fields/create-a-taxonomy.md).