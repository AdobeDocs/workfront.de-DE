---
title: Hinzufügen vorhandener Datensatztypen
description: Datensatztypen sind die Objekttypen von Adobe Workfront Planning. In Workfront Planning können Sie einen vorhandenen Datensatztyp aus einem anderen Arbeitsbereich importieren.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 976810c8cedc5d3c5afd8333fdbace4fe8d0ccda
workflow-type: tm+mt
source-wordcount: '584'
ht-degree: 1%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Hinzufügen vorhandener Datensatztypen

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Als Workspace-Manager können Sie einen vorhandenen Datensatztyp in einen anderen Workspace importieren oder hinzufügen.

Sie müssen zunächst einen Datensatztyp als zentralisierten Arbeitsbereich festlegen, bevor Workspace-Manager ihn in andere Arbeitsbereiche importieren können.

Sie können einen Datensatztyp beim Erstellen oder Bearbeiten als zentralisiert festlegen, während Sie seine arbeitsbereichsübergreifenden Einstellungen definieren.

Weitere Informationen finden Sie unter [Konfigurieren von arbeitsbereichsübergreifenden Funktionen für Datensatztypen](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

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
   <td role="rowheader"><p>Adobe Workfront-Paket*</p></td> 
   <td> 
<ul><li><p>Beliebiges Workfront-Paket</p></li>
Und
<li><p>Planning Plus-Paket</p></li></ul>
Oder:
<ul><li><p>Beliebiges Workflow-Paket</p> </li>
Und
<li><p>Planen eines Prime- oder Ultimate-Pakets</p></li></ul>
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen erhalten Sie von Ihrem Workfront Account Manager. </p> 
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

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Übersicht über zentralisierte Datensatztypen

Überlegungen beim Hinzufügen vorhandener Datensatztypen aus einem anderen Arbeitsbereich

* Wenn keine Datensatztypen zum Hinzufügen zu einem anderen Arbeitsbereich konfiguriert sind, wird beim Erstellen eines Datensatztyps die Option zum Importieren aus einem anderen Arbeitsbereich nicht angezeigt. <!--add this a tip in the steps below, and/ or add a Conditional step that this is possible only when these record types are first enabled-->
* Nachdem Sie den Datensatztyp aus einem anderen Arbeitsbereich hinzugefügt haben, werden auch die folgenden Informationen aus dem vorhandenen Datensatztyp hinzugefügt:

   * Felder
   * Verbindungen aufzeichnen

* Sie können Datensätze, die von anderen Arbeitsbereichen hinzugefügt wurden, nur anzeigen, wenn Sie über Berechtigungen für diese Arbeitsbereiche verfügen.

* Sie können den Datensatztyp einschließlich der Felder nur im ursprünglichen Arbeitsbereich bearbeiten. Sie können sie nicht in den Arbeitsbereichen bearbeiten, in denen sie hinzugefügt wurde.
* Die aus allen Arbeitsbereichen hinzugefügten Datensätze sind für alle Benutzer sichtbar, die in allen Arbeitsbereichen auf sie zugreifen, auch wenn sie in einem Arbeitsbereich erstellt wurden, in dem sie keine Berechtigungen haben.

## Erstellen eines Datensatztyps aus einem vorhandenen Datensatztyp

1. Beginnen Sie mit der Erstellung eines Datensatztyps, wie im Artikel [Erstellen von Datensatztypen](/help/quicksilver/planning/architecture/create-record-types.md) beschrieben, und klicken Sie dann auf **Vorhandene hinzufügen**. <!--check this - the option might have been renamed in the UI-->

   ![Modal zum Hinzufügen eines Datensatztyps mit der Option zum Importieren aus einem anderen Arbeitsbereich](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. Klicken Sie auf **Fortfahren**.
1. Klicken **im Feld „Datensatztyp auswählen** auf die Karte für den Datensatztyp, den Sie aus einem vorhandenen Arbeitsbereich hinzufügen möchten, und klicken Sie dann auf **Hinzufügen**.

   Der Datensatztyp wird dem ausgewählten Arbeitsbereich hinzugefügt und Folgendes geschieht:

   * Das Symbol **Arbeitsbereichsübergreifender Datensatztyp** ![Symbol für arbeitsbereichsübergreifende ](assets/global-icon.png)) wird der Karte des importierten Datensatztyps hinzugefügt.
   * Das schreibgeschützte Feld **Workspace** wird zum importierten Datensatztyp hinzugefügt. Das Feld zeigt an, in welchem Arbeitsbereich die einzelnen Datensätze erstellt wurden.

     >[!NOTE]
     >
     >* Der importierte Datensatztyp oder seine Felder können nicht bearbeitet werden. Sie können den Datensatztyp und dessen Felder über den ursprünglichen Arbeitsbereich bearbeiten.

1. (Optional) Klicken Sie auf das Menü **Mehr** ![Mehr](assets/more-menu.png) auf der Karte des importierten Datensatztyps oder rechts neben dem Namen des Datensatztyps auf seiner Seite und klicken Sie dann auf **Löschen**.
1. (Bedingt) Geben Sie **Löschen** in das bereitgestellte Feld ein und klicken Sie dann auf **Dauerhaft löschen**.

   Dadurch wird der importierte Datensatztyp aus dem ausgewählten Arbeitsbereich entfernt. Der ursprüngliche Datensatztyp und seine Felder verbleiben im ursprünglichen Arbeitsbereich.

   <!--**************************ASK LILIT ON THIS ONE, NOT SURE IF THIS IS TRUE: Any records added in the current workspace are saved in the original workspace.**********-->



