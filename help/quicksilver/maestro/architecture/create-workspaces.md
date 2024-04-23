---
title: Erstellen von Arbeitsbereichen
description: Ein Arbeitsbereich ist eine Sammlung von Datensatztypen, die von einem Team verwendet werden und den Arbeitslebenszyklus des Teams darstellen. Sie können die Arbeitsbereiche in der Adobe Workfront-Planung vollständig anpassen. Die Typen von Datensätzen sind nach Abschnitten in einem Arbeitsbereich organisiert.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
source-git-commit: 6bea34403e45c2b50986f79272f7a46959d67c6d
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Erstellen von Arbeitsbereichen

{{maestro-important-intro}}

In der Adobe Workfront-Planung sind Arbeitsbereiche zentrale Standorte für Teams zur Arbeitsplanung.

Ein Arbeitsbereich ist eine Sammlung von Datensatztypen, die von einem Team verwendet werden und den Arbeitslebenszyklus des Teams darstellen. Sie können die Arbeitsbereiche in der Adobe Workfront-Planung vollständig anpassen.

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
<p>Ihr Unternehmen muss in das geschlossene Betaprogramm für die Adobe-Arbeitsplanung aufgenommen werden. Wenden Sie sich an Ihren Kundenbetreuer, um sich über dieses neue Angebot zu informieren. </p>
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
   Oder
   <p>Aktuell: Plan</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td>
   <td> <p>Für die Adobe Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Berechtigungen</p></td>
   <td> <p>Sie erhalten Verwaltungsberechtigungen für die von Ihnen erstellten Arbeitsbereiche. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Sie müssen den Planungsbereich zu Ihrer Layoutvorlage hinzufügen. Weitere Informationen finden Sie unter <a href="../access/access-overview.md">Zugriffsübersicht</a>. </p>  
</td>
  </tr>

</tbody>
</table>

Weitere Informationen zu Zugriffsanforderungen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Überlegungen zu Arbeitsbereichen

* Sie können Arbeitsbereiche für bestimmte Organisationseinheiten in Ihrer Organisation erstellen, die der einzigartigen Funktionsweise jeder Einheit entsprechen.
* Die in einem Arbeitsbereich enthaltenen Datensatztypen sollten den Arbeitszyklus einer Organisationseinheit widerspiegeln.
* Wenn Sie einen Arbeitsbereich erstellen, haben nur Sie die Berechtigung, auf Ihren Arbeitsbereich zuzugreifen und ihn zu verwalten. Sie müssen es für andere Benutzer freigeben, damit sie mit Ihnen an derselben Stelle zusammenarbeiten können. Weitere Informationen finden Sie unter [Freigeben eines Arbeitsbereichs](/help/quicksilver/maestro/access/share-workspaces.md). Systemadministratoren können alle Arbeitsbereiche verwalten, auch die, die sie nicht erstellt haben.
* Sie können über Folgendes verfügen:

   * Bis zu 50 Abschnitte in einem Arbeitsbereich.
   * Bis zu 1.000 Datensatztypen aus allen Bereichen eines Arbeitsbereichs. Alle Datensatztypen sind für jeden Arbeitsbereich eindeutig. <!--this might change-->
   * Bis zu 1.000 Arbeitsbereiche in der Workfront-Instanz Ihres Unternehmens.


## Erstellen eines Arbeitsbereichs

Sie können einen Arbeitsbereich erstellen und ihm Datensatztypen hinzufügen, um Ihre Objekte in der Workfront-Planung zu organisieren. Weitere Informationen zum Bearbeiten eines Arbeitsbereichs finden Sie unter [Arbeitsbereiche bearbeiten](/help/quicksilver/maestro/architecture/edit-workspaces.md).

{{step1-to-maestro}}

Dadurch wird der Arbeitsbereich für die Workfront-Planung geöffnet.

1. (Bedingt) Wenn Ihre Umgebung keine Arbeitsbereiche enthält, klicken Sie auf **Arbeitsbereich erstellen**

   Oder klicken Sie in einem vorhandenen Arbeitsbereich auf den nach unten zeigenden Pfeil rechts neben dem Workspace-Namen und klicken Sie dann auf **Arbeitsbereich erstellen**.

   ![](assets/workspace-drop-down-right-menu.png)


1. (Optional und bedingt) Klicken Sie auf **Vorschau** in einer der folgenden vordefinierten Arbeitsbereichsvorlagen:

   * Marketing-Management
   * Vertriebsmanagement
   * Produktverwaltung

   Es gibt einen Hinweis darauf, welche operationellen Datensatztypen, Taxonomien und wie viele Felder mit jeder Vorlage verknüpft sind.

   ![](assets/previewing-a-workspace-template.png)

   Weitere Informationen zu Vorlagen für Workfront Planning Workspace finden Sie unter [Liste der Workspace-Vorlagen](../architecture/workspace-templates.md).

1. Klicks **Vorlage verwenden** , um den Arbeitsbereich aus der ausgewählten Vorlage zu erstellen

   Oder

   Klicks **Arbeitsbereich erstellen** , um einen neuen Arbeitsbereich zu erstellen.

   Eine für die folgenden Arten von Arbeitsbereichen wird erstellt:

   * Ein leerer Arbeitsbereich mit dem Namen **Unbenannter Arbeitsbereich** wo Sie beim Erstellen eines neuen Arbeitsbereichs manuell mit dem Hinzufügen von Datensatztypen beginnen können.
   * Ein Arbeitsbereich mit dem Namen nach der ausgewählten Vorlage, der mit Beispieldatensatztypen gefüllt ist. Sie können die Datensatztypen und den Arbeitsbereich weiter anpassen.

1. Klicken Sie in den Namen des Arbeitsbereichs in der Kopfzeile des neuen Arbeitsbereichs, um ihn umzubenennen, und drücken Sie dann die Eingabetaste.

1. (Optional und bedingt) Wenn Sie den Arbeitsbereich aus einer Vorlage erstellt haben, klicken Sie in den Namen der **Operative Datensatztypen** oder **Taxonomien** Abschnitte

   Oder

   Bewegen Sie den Mauszeiger über den Namen eines Abschnitts und klicken Sie auf die Schaltfläche **Mehr** Menü ![](assets/more-menu.png)Klicken Sie auf **Umbenennen** , um den Abschnitt umzubenennen.

   >[!TIP]
   >
   >Sie können jeden Abschnitt aus einem beliebigen Arbeitsbereich umbenennen, auch wenn Sie den Abschnitt nicht erstellt haben.

   Weitere Informationen zum Bearbeiten von Arbeitsbereichen, einschließlich Arbeitsbereichsabschnitten, finden Sie unter [Arbeitsbereiche bearbeiten](/help/quicksilver/maestro/architecture/edit-workspaces.md).

1. (Optional) Klicken Sie auf **Datensatztyp hinzufügen** , um dem Arbeitsbereich in einem beliebigen Abschnitt Datensatztypen hinzuzufügen.

   Weitere Informationen finden Sie unter [Erstellen von Datensatztypen](../architecture/create-record-types.md).

   Weitere Informationen zum Bearbeiten und Löschen von Datensatztypen in einem Arbeitsbereich finden Sie unter [Arbeitsbereiche bearbeiten](/help/quicksilver/maestro/architecture/edit-workspaces.md).


