---
title: Hinzufügen vorhandener Datensatztypen aus einer anderen Workspace
description: Datensatztypen sind die Objekttypen von Adobe Workfront Planning. In Workfront Planning können Sie einen vorhandenen Datensatztyp hinzufügen, der in einem anderen Workspace erstellt wurde.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '619'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Hinzufügen vorhandener Datensatztypen aus einem anderen Arbeitsbereich

{{planning-important-intro}}

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Als Workspace-Manager können Sie einen Datensatztyp, der in einem anderen Workspace vorhanden ist, zu einem Workspace hinzufügen, den Sie in Adobe Workfront Planning verwalten.

Ein Workspace-Manager muss zunächst einen Datensatztyp als globalen Datensatztyp festlegen, bevor Sie ihn Arbeitsbereichen hinzufügen können, die Sie als vorhandenen Datensatztyp verwalten. Workspace-Manager können einen Datensatztyp beim Erstellen oder Bearbeiten als „global“ festlegen, indem sie die arbeitsbereichsübergreifenden Einstellungen des Datensatztyps definieren.

Weitere Informationen finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

Dieser Artikel beschreibt, wie Sie einen Datensatztyp aus einem vorhandenen hinzufügen können.

Bevor Sie einem Arbeitsbereich Datensätze aus einem globalen Datensatztyp hinzufügen, lesen Sie auch den Artikel [Übersicht über arbeitsbereich-übergreifende Datensatztypen](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).


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
<ul><li><p>Beliebiges Workfront-Paket und Planning Plus-Paket</p></li>
<p>Oder</p>
<li><p>Workflow- und Planungspakete für Prime und Ultimate</p></p></li></ul>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Verwalten von Berechtigungen für einen Arbeitsbereich</p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:
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
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul><li><p>Any Workfront package</p></li>
<p>And</p>
<li><p>Any Planning package to create connectable record types</p></li>
<li><p>A Planning Plus package to create global record types</p></li>
</ul>
Or:
<ul><li><p>A Prime or Ultimate Workflow package</p> </li>
And
<li><p>A Planning Prime or Ultimate package</p></li></ul>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
   </td> 

  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and to the record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table>-->

## Erstellen eines Datensatztyps durch Hinzufügen eines vorhandenen Datensatztyps aus einem anderen Arbeitsbereich

>[!NOTE]
>
>Stellen Sie sicher, dass in mindestens einem anderen Arbeitsbereich mindestens ein Datensatztyp als „global“ festgelegt ist.

1. Beginnen Sie mit der Erstellung eines Datensatztyps, wie im Artikel [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md) beschrieben, und klicken Sie dann auf **Vorhandene hinzufügen**. <!--check this - the option might have been renamed in the UI-->

   ![Modal zum Hinzufügen eines Datensatztyps mit der Option zum Hinzufügen aus einem anderen Arbeitsbereich](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

   >[!TIP]
   >
   >Wenn keine Datensatztypen zum Hinzufügen zu anderen Arbeitsbereichen in Ihrem System konfiguriert sind, wird die Option **Vorhandene hinzufügen** nicht angezeigt.

1. Klicken Sie auf **Fortfahren**.
1. Klicken **im Feld &quot;** auswählen“ auf die Karte für den Datensatztyp, den Sie aus einem vorhandenen Arbeitsbereich hinzufügen möchten, und klicken Sie dann auf **Hinzufügen**.

   Der Datensatztyp wird dem ausgewählten Arbeitsbereich hinzugefügt und das Symbol **globaler Datensatztyp** wird ![](assets/global-icon.png) auf der Karte des Datensatztyps angezeigt.

   Folgendes geschieht:

   * Die folgenden Informationen werden auch aus dem vorhandenen globalen Datensatztyp hinzugefügt:

      * Alle Originalfelder
      * Alle Datensatzverbindungen
   * Sie können Datensätze, die von anderen Arbeitsbereichen mit demselben globalen Datensatztyp hinzugefügt wurden, nur anzeigen, wenn Sie mindestens über die Berechtigung zum Anzeigen dieser Arbeitsbereiche verfügen.
   * Das schreibgeschützte Feld **Workspace** wird der neuen Tabellenansicht vom Typ Datensatz hinzugefügt. Das Feld zeigt den Arbeitsbereich an, in dem die einzelnen Datensätze erstellt wurden.

     >[!NOTE]
     >
     >Das Erscheinungsbild, zusätzliche Einstellungen oder ursprüngliche Felder des neuen Datensatztyps können nicht bearbeitet werden. Sie können den Datensatztyp und alle zugehörigen Originalfelder und -einstellungen nur über den ursprünglichen Arbeitsbereich bearbeiten.

1. (Optional) Klicken Sie auf und ziehen Sie den neu hinzugefügten Datensatztyp dann per Drag-and-Drop in einen beliebigen Abschnitt im Arbeitsbereich.
1. (Optional) Klicken Sie auf der Karte des neuen Datensatztyps **das Menü** Mehr oder rechts neben dem Namen des Datensatztyps auf seiner Seite und klicken Sie dann auf **Löschen**.

   Weitere Informationen finden Sie im Abschnitt „Löschen globaler Datensatztypen“ im Artikel [Löschen von Datensatztypen](/help/quicksilver/planning/architecture/delete-record-types.md).

<!--This will be released later with another epic: 
1. In the table view, click the **+** icon in the upper-right corner to add new fields. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.
-->

&lt;!—Mit Lilit prüfen, ob wir Automatisierungen hinzufügen oder Formulare an sekundäre globale RTs anfordern können??—Schritt mit Links zu diesen Artikeln hinzufügen, wenn/ wenn ja—>







