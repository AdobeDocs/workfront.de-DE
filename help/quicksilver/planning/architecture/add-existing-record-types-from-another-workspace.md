---
title: Hinzufügen vorhandener Datensatztypen aus einer anderen Workspace
description: Datensatztypen sind die Objekttypen von Adobe Workfront Planning. In Workfront Planning können Sie einen vorhandenen Datensatztyp hinzufügen, der in einem anderen Workspace erstellt wurde.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: bfb0fd2956ffb9384a09882864668d5dba33a53b
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Hinzufügen vorhandener Datensatztypen aus einem anderen Arbeitsbereich

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Als Workspace-Manager können Sie einen Datensatztyp, der in einem Workspace vorhanden ist, zu einem Workspace hinzufügen, den Sie in Adobe Workfront Planning verwalten.

Sie müssen zunächst einen Datensatztyp als zentralisierten Workspace-Typ festlegen, bevor Workspace-Manager ihn als vorhandenen Datensatztyp in andere Workspaces einfügen können.

Sie können einen Datensatztyp beim Erstellen oder Bearbeiten als zentralisiert festlegen, während Sie seine arbeitsbereichsübergreifenden Einstellungen definieren.

Weitere Informationen finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

Bevor Sie einem Arbeitsbereich Datensätze aus einem zentralisierten Datensatztyp hinzufügen, lesen Sie den Artikel [Übersicht über arbeitsbereich-übergreifende Datensatztypen](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

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
<ul><li><p>Beliebiges Workfront-Paket</p></li>
Und
<li><p>Planning Plus-Paket</p></li></ul>
<!--Or:
<ul><li><p>Any Workflow package</p> </li>
And
<li><p>Planning Prime or Ultimate package</p></li></ul>-->
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront Account Manager. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Erstellen eines Datensatztyps aus einem vorhandenen Datensatztyp

1. Beginnen Sie mit der Erstellung eines Datensatztyps, wie im Artikel [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md) beschrieben, und klicken Sie dann auf **Vorhandene hinzufügen**. <!--check this - the option might have been renamed in the UI-->

   ![Modal zum Hinzufügen eines Datensatztyps mit der Option zum Hinzufügen aus einem anderen Arbeitsbereich](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. Klicken Sie auf **Fortfahren**.
1. Klicken **im Feld „Datensatztyp auswählen** auf die Karte für den Datensatztyp, den Sie aus einem vorhandenen Arbeitsbereich hinzufügen möchten, und klicken Sie dann auf **Hinzufügen**.

   Der Datensatztyp wird dem ausgewählten Arbeitsbereich hinzugefügt.

   >[!TIP]
   >
   >Wenn keine Datensatztypen zum Hinzufügen zu einem anderen Arbeitsbereich konfiguriert sind, wird beim Erstellen eines Datensatztyps nicht die Option zum Hinzufügen aus einem anderen Arbeitsbereich angezeigt.

   Folgendes geschieht:

   * Darüber hinaus werden die folgenden Informationen aus dem vorhandenen zentralisierten Datensatztyp hinzugefügt:

      * Alle Originalfelder
      * Alle Datensatzverbindungen
   * Sie können Datensätze, die von anderen Arbeitsbereichen hinzugefügt wurden, nur anzeigen, wenn Sie mindestens über die Berechtigung Anzeigen für diese Arbeitsbereiche verfügen.
   * Das Symbol **zentralisierter Datensatztyp** ![Symbol für zentralisierten Datensatztyp](assets/global-icon.png) wird der Karte des neuen Datensatztyps hinzugefügt.
   * Das schreibgeschützte Feld **Workspace** wird der neuen Tabellenansicht vom Typ Datensatz hinzugefügt. Das Feld zeigt an, in welchem Arbeitsbereich die einzelnen Datensätze erstellt wurden.

     >[!NOTE]
     >
     >* Das Erscheinungsbild, die erweiterten Einstellungen oder die ursprünglichen Felder des neuen Datensatztyps können nicht bearbeitet werden. Sie können den Datensatztyp und alle zugehörigen Originalfelder und -einstellungen nur über den ursprünglichen Arbeitsbereich bearbeiten.

1. (Optional) Klicken Sie auf und ziehen Sie den neu hinzugefügten Datensatztyp dann per Drag-and-Drop in einen beliebigen Abschnitt im Arbeitsbereich.

<!--This will be released later with another epic: 1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.-->

1. (Optional) Klicken Sie auf die Karte **Mehr** Menü ![Mehr](assets/more-menu.png) auf der Karte des neuen Datensatztyps oder rechts neben dem Namen des Datensatztyps auf seiner Seite und klicken Sie dann auf **Löschen**.
1. (Bedingt) Geben Sie **Löschen** in das bereitgestellte Feld ein und klicken Sie dann auf **Dauerhaft löschen**.

   Folgendes geschieht:

   * Der aus einem zentralisierten Datensatztyp erstellte Datensatztyp wird aus dem ausgewählten Arbeitsbereich entfernt.
   * Der ursprüngliche Datensatztyp und seine Felder verbleiben im ursprünglichen Arbeitsbereich.
   * Der Datensatztyp verbleibt in allen anderen Arbeitsbereichen, in denen er hinzugefügt wurde.
   * Die Datensätze, die dem Datensatztyp aus dem aktuellen Arbeitsbereich hinzugefügt wurden, werden gelöscht. Alle anderen Datensätze, die aus zusätzlichen Arbeitsbereichen hinzugefügt wurden, in denen der zentralisierte Datensatztyp hinzugefügt wurde, bleiben erhalten.





