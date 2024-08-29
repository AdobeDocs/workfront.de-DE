---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Hinzufügen von Projekten zu Zielen in Adobe Workfront-Zielen
description: Sie können Projekte mit Zielen verknüpfen, um basierend auf dem tatsächlichen Fortschritt des Projekts anzugeben, wie das Ziel voranschreitet. Das Projekt wird zu einem Fortschrittsanzeiger für das Ziel.
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 1%

---

# Hinzufügen von Projekten zu Zielen in Adobe Workfront-Zielen

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

Sie können Projekte mit Zielen verknüpfen, um basierend auf dem tatsächlichen Fortschritt des Projekts anzugeben, wie das Ziel voranschreitet. Das Projekt wird zu einem Fortschrittsanzeiger für das Ziel.

Indem Sie Projekte mit Zielen verbinden, können Sie die strategische Planung (Ziele) Ihrer Organisation mit der tatsächlichen Arbeit verbinden, die Ihre Mitarbeiter täglich leisten und abschließen (Projekte).

>[!IMPORTANT]
>
>Ziele auf Projektebene, die im Geschäftsfallbereich eines Projekts erstellt wurden, sind nicht mit strategischen Zielen verknüpft, die in Workfront-Zielen erstellt wurden. Weitere Informationen zu den Projektzielen von Business Case finden Sie unter [Ziele für Geschäftsfälle erstellen](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> 
   <p>Für den neuen Plan und die Lizenzstruktur:
  <ul><li>Ein ultimativer Plan </li></ul>
   </p>
<p>Für den aktuellen Plan und die Lizenzstruktur: 
<ul><li> A Pro oder höher </li>
  <li>Eine Adobe Workfront Goals-Lizenz zusätzlich zu einer Workfront-Lizenz.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-Lizenz*</td>
 <td>
 <p>Neue Lizenz: Mitarbeiter oder höher</p>
 Oder
 <p>Aktuelle Lizenz: Anfrage oder höher</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produkt*</td>
 <td>
 <p> Neue Produktanforderungen, eine der folgenden: </p>
<ul>
<li>Ein Select- oder Prime-Adobe Workfront-Plan und eine zusätzliche Adobe Workfront Goals-Lizenz.</li>
<li>Ein Ultimate Workfront-Plan, der standardmäßig Workfront-Ziele enthält. </li></ul>
 <p>Oder</p>
 <p>Aktuelle Produktanforderungen: Ein Workfront-Plan und eine zusätzliche Lizenz für Adobe Workfront Goals. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Voraussetzungen für die Verwendung von Workfront-Zielen</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Zugriffsebene</td>
 <td> <p>Zugriff auf Ziele bearbeiten</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektberechtigungen</td>
 <td>
  <div>
  <p>Anzeigen oder Anzeigen höherer Berechtigungen zum Ziel</p>
  <p>Berechtigungen für das Ziel verwalten</p>
  <p>Informationen zum Freigeben von Zielen finden Sie unter <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront-Zielen</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Überlegungen zum Verbinden von Projekten mit Zielen

* Sie können einem Ziel ein Projekt hinzufügen, das die folgenden Kriterien erfüllt:

   * Sie müssen mindestens über die Berechtigungen zum Anzeigen verfügen.

     >[!NOTE]
     >
     >Wenn Sie die Berechtigung zum Anzeigen des Projekts verlieren, nachdem Sie das Projekt an das Ziel angehängt haben, können Sie weiterhin Projektinformationen zum Ziel sehen, aber Sie können nicht mehr auf das Projekt zugreifen.

   * Das Projekt darf nicht den Status &quot;Tot&quot;haben.

* Sie können mehrere Projekte mit einem Ziel verknüpfen.
* Sie können dasselbe Projekt mit mehreren Zielen verknüpfen.
* Sie können den Fortschritt eines Projekts nicht manuell über das Ziel aktualisieren, an das das Projekt angehängt ist. Stattdessen berechnet Workfront den prozentualen Abschluss des Projekts und Workfront Goals berechnet den Zielfortschritt anhand dieses Prozentsatzes. Dadurch wird das Ziel in Echtzeit aktualisiert, nachdem der Prozentsatz des Projekts aktualisiert wurde.
* Die Projektdauer kann außerhalb des Zeitraums eines Ziels liegen. Wenn ein Projekt länger dauert als der Zieltermin, können Sie Ihr Ziel dennoch schließen und es als abgeschlossen betrachten. Der Zielprozentsatz für die Fertigstellung beträgt jedoch nicht 100 %. Der prozentuale Abschluss des Projekts aktualisiert das Ziel nicht mehr.

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* Wenn Sie ein an ein Ziel angehängtes Projekt löschen, wird das Projekt auch aus dem Ziel gelöscht.

  >[!CAUTION]
  >
  >Wenn das Ziel aktiv war, bevor Sie das Projekt gelöscht haben, und es keine weiteren Fortschrittsanzeigen für das Ziel gibt, wird das Ziel inaktiv.


## Hinzufügen von Projekten zu Zielen

1. Klicken Sie auf das **Hauptmenü** ![](assets/main-menu-icon.png) (Entwurf für Shell: oder klicken Sie auf das **Hauptmenü** ![](assets/three-line-main-menu-icon.png) in der oberen linken Ecke, falls verfügbar.) und dann auf **Ziele**.
1. Klicken Sie in der Zielliste auf den Namen eines Ziels, um die Zielseite zu öffnen.
1. Klicken Sie im linken Bereich auf **Fortschrittsanzeigen** .
1. Klicken Sie im Dropdownmenü **Neuer Fortschrittsanzeige** auf **Vorhandenes Projekt hinzufügen**.

   Das Feld Projekte zum Ziel hinzufügen wird angezeigt.
1. (Optional) Aktualisieren Sie die **Ansicht**, den **Filter** oder die **Gruppierung**, indem Sie auf die entsprechenden Symbole oben rechts in der Liste klicken, um die Anzeige der Projektliste zu ändern.
1. (Optional) Klicken Sie auf das Symbol **Suchen** ![](assets/search-icon.png) und geben Sie den Namen eines Projekts ein, um es schnell in der Liste zu finden.
1. Wählen Sie die Projekte aus, die Sie zum Ziel hinzufügen möchten, und klicken Sie dann auf **Hinzufügen**.

   Die ausgewählten Projekte werden zum Ziel hinzugefügt und im Abschnitt Fortschrittsanzeigen der Zielseite unter der Gruppe **Projekt** angezeigt.

   Nachdem Sie das Ziel aktiviert haben, wird der Fortschritt des Ziels automatisch aktualisiert, sobald der Fortschritt eines Projekts aktualisiert wird. Informationen zum Aktivieren eines Ziels finden Sie unter [Ziele in Adobe Workfront aktivieren](../goal-management/activate-goals.md).

## Suchen Sie nach Projektinformationen zu Zielen

<p>
Die folgenden Projektinformationen sind auf der Zielebene im Abschnitt Fortschrittsindikatoren auf der Seite eines Ziels sichtbar:

</p>

<table>
  <tr>
   <td>Projektname
   </td>
   <td>Alle Änderungen am Projektnamen werden auch im verbundenen Projekt übernommen.
   </td>
  </tr>
  <tr>
   <td>Projektbesitzer
   </td>
   <td>Alle Änderungen im Projekteigentümer werden auch im verbundenen Projekt übernommen.
   </td>
  </tr>
    <tr>
   <td>Tatsächlicher Fortschritt
   </td>
   <td> <p>Der prozentuale Abschluss des Projekts. Sie können den Prozentsatz des Projekts, der vom Ziel abgeschlossen wurde, nicht manuell aktualisieren. Workfront berechnet sie automatisch anhand des Prozentsatzes, in dem die Aufgaben abgeschlossen sind. </p>
   </td>
  </tr>
  <tr>
   <td>Fortschritt
   </td>
   <td>Der prozentuale Abschluss des Projekts, dargestellt durch einen Balken. Jede Änderung des Prozentsatzes für den Abschluss des Projekts aktualisiert automatisch den Zielfortschritt, es sei denn, das Ziel ist geschlossen.
   </td>
  </tr>

</table>

## Zielinformationen zu Projekten suchen

Die folgenden Zielinformationen sind in einer Projektliste oder einem Bericht sichtbar:

| Zielinformation | Beschreibung |
|---|---|
| Ziele | Eine Liste aller Ziele, denen ein Projekt zugeordnet ist. |
| Zielhierarchie | Die Hierarchie, zu der ein Ziel gehört. Nur die übergeordneten Elemente des Ziels und des Ziels werden in diesem Feld angezeigt. Untergeordnete Ziele werden nicht angezeigt. |
| Anzahl verknüpfter Ziele | Die Anzahl der mit einem Projekt verknüpften Ziele. |
