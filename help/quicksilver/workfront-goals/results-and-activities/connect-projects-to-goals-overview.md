---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Hinzufügen von Projekten zu Zielen in Adobe Workfront Goals
description: Sie können Projekte mit Zielen verbinden, um den Fortschritt des Ziels basierend auf dem tatsächlichen Fortschritt des Projekts anzugeben. Das Projekt wird zu einem Fortschrittsindikator für das Ziel.
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: 45c71a8106bdb8eeaa38f2fb83ff0312e48183d0
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 1%

---

# Hinzufügen von Projekten zu Zielen in Adobe Workfront Goals

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

Sie können Projekte mit Zielen verbinden, um den Fortschritt des Ziels basierend auf dem tatsächlichen Fortschritt des Projekts anzugeben. Das Projekt wird zu einem Fortschrittsindikator für das Ziel.

Indem Sie Projekte mit Zielen verbinden, können Sie die strategische Planung (Ziele) Ihres Unternehmens mit der tatsächlichen Arbeit verknüpfen, die Ihre Mitarbeiter täglich ausführen und abschließen (Projekte).

>[!IMPORTANT]
>
>Ziele auf Projektebene, die im Business-Case-Bereich eines Projekts erstellt wurden, sind nicht mit strategischen Zielen verbunden, die in Workfront-Zielen erstellt wurden. Informationen zu Business Case-Projektzielen finden Sie unter [Erstellen von Business Case-Zielen](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


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
   <p>Für die neue Plan- und Lizenzstruktur:
  <ul><li>Ein Ultimate-Plan </li></ul>
   </p>
<p>Für die aktuelle Plan- und Lizenzstruktur: 
<ul><li> Ein Profi oder höher </li>
  <li>Eine Adobe Workfront-Ziellizenz zusätzlich zu einer Workfront-Lizenz.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront-Lizenz*</td>
 <td>
 <p>Neue Lizenz: Mitwirkende oder höher</p>
 Oder
 <p>Aktuelle Lizenz: Anfrage oder höher</p> <p>Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Übersicht über Adobe Workfront-Lizenzen</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Produkt*</td>
 <td>
 <p> Neue Produktanforderung, eine der folgenden: </p>
<ul>
<li>Einen ausgewählten oder Prime Adobe Workfront-Plan und eine zusätzliche Adobe Workfront Goals-Lizenz.</li>
<li>Ein Ultimate Workfront-Plan, der standardmäßig Workfront-Ziele enthält. </li></ul>
 <p>Oder</p>
 <p>Aktuelle Produktanforderung: Ein Workfront-Plan und eine zusätzliche Lizenz für Adobe Workfront Goals. </p> <p>Weitere Informationen finden Sie unter <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Voraussetzungen für die Verwendung von Workfront-Zielen</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Zugriffsebene</td>
 <td> <p>Zugriff auf Ziele bearbeiten</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Objektberechtigungen</td>
 <td>
  <div>
  <p>Anzeigen von oder höheren Berechtigungen für das Ziel, um es anzuzeigen</p>
  <p>Verwalten von Berechtigungen für das Ziel, um es zu bearbeiten</p>
  <p>Informationen zum Freigeben von Zielen finden Sie <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Freigeben eines Ziels in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layoutvorlage</p></td>
   <td> <p>Allen Benutzenden, einschließlich Workfront-Administratoren, muss eine Layout-Vorlage zugewiesen werden, die den Bereich Ziele im Hauptmenü enthält. </p>  
</td>
  </tr>
</tbody>
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Überlegungen zum Verbinden von Projekten mit Zielen

* Sie können ein Projekt, das die folgenden Kriterien erfüllt, zu einem Ziel hinzufügen:

   * Sie müssen mindestens über die Berechtigung zum Anzeigen verfügen.

     >[!NOTE]
     >
     >Wenn Sie Ihre Berechtigungen zum Anzeigen des Projekts verlieren, nachdem Sie das Projekt an das Ziel angehängt haben, können Sie weiterhin Projektinformationen zum Ziel anzeigen, Sie können jedoch nicht mehr auf das Projekt zugreifen.

   * Das Projekt darf nicht den Status „Eingestellt“ haben.

* Sie können mehrere Projekte mit einem Ziel verknüpfen.
* Sie können dasselbe Projekt mit mehreren Zielen verknüpfen.
* Sie können den Fortschritt eines Projekts nicht manuell von dem Ziel aus aktualisieren, an das das Projekt angehängt ist. Stattdessen berechnet Workfront den Prozentsatz der Fertigstellung des Projekts und Workfront Goals berechnet den Zielfortschritt mithilfe dieses Prozentsatzes der Fertigstellung. Dadurch wird das Ziel in Echtzeit nach den prozentualen Aktualisierungen des Projekts aktualisiert.
* Die Projektdauer kann außerhalb des Zeitraums eines Ziels liegen. Wenn ein Projekt länger als die Frist für das Ziel dauert, können Sie Ihr Ziel immer noch schließen und als abgeschlossen betrachten, aber das Ziel in Prozent abgeschlossen ist nicht 100 %. Der Prozentwert der Fertigstellung des Projekts wird nicht mehr auf dem Ziel aktualisiert.

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![Goal closed](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* Wenn Sie ein Projekt löschen, das an ein Ziel angehängt ist, wird das Projekt auch aus dem Ziel gelöscht.

  >[!CAUTION]
  >
  >Wenn das Ziel vor dem Löschen des Projekts aktiv war und es keine anderen Fortschrittsanzeigen für das Ziel gibt, wird das Ziel inaktiv.


## Projekte zu Zielen hinzufügen

1. Klicken Sie auf **Hauptmenü** ![Hauptmenüsymbol](assets/main-menu-icon.png) (entwerfen Sie diese für Shell: oder klicken Sie auf das **Hauptmenü** ![Hauptmenüzeilen](assets/three-line-main-menu-icon.png) in der oberen linken Ecke, falls verfügbar.) , dann **Ziele**.
1. Klicken Sie in der Liste Ziel auf den Namen eines Ziels, um die Seite Ziel zu öffnen.
1. Klicken Sie **linken Bereich** Fortschrittsanzeigen“.
1. Klicken Sie **Dropdown-Menü** Neue Fortschrittsanzeige“ auf **Vorhandenes Projekt hinzufügen**.

   Das Feld Projekte zum Ziel hinzufügen wird angezeigt.
1. (Optional) Aktualisieren Sie **Ansicht**, **Filter** oder **Gruppierung**, indem Sie auf die entsprechenden Symbole in der rechten oberen Ecke der Liste klicken, um die Anzeige der Projektliste zu ändern.
1. (Optional) Klicken Sie auf das Symbol **Suchen** ![Suchsymbol](assets/search-icon.png) und geben Sie den Namen eines Projekts ein, um es schnell in der Liste zu finden.
1. Wählen Sie die Projekte aus, die Sie zum Ziel hinzufügen möchten, und klicken Sie dann auf **Hinzufügen**.

   Die ausgewählten Projekte werden zum Ziel hinzugefügt und im Abschnitt Fortschrittsanzeigen der Zielseite unter der Gruppierung **Projekt** angezeigt.

   Nach der Aktivierung des Ziels wird der Fortschritt des Ziels automatisch aktualisiert, wenn der Fortschritt eines Projekts aktualisiert wird. Informationen zum Aktivieren eines Ziels finden Sie unter [Aktivieren von Zielen in Adobe Workfront](../goal-management/activate-goals.md).

## Suchen von Projektinformationen für Ziele

<p>
Die folgenden Projektinformationen sind auf der Zielebene im Abschnitt Fortschrittsanzeigen auf der Zielseite sichtbar:

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
   <td>Alle Änderungen am Projektbesitzer werden auch im verbundenen Projekt übernommen.
   </td>
  </tr>
    <tr>
   <td>Tatsächlicher Fortschritt
   </td>
   <td> <p>Der Prozentsatz der Fertigstellung des Projekts. Sie können den abgeschlossenen Projekt-Prozentsatz nicht manuell vom Ziel aktualisieren. Workfront berechnet sie automatisch anhand des Prozentsatzes der abgeschlossenen Aufgaben. </p>
   </td>
  </tr>
  <tr>
   <td>Fortschritt
   </td>
   <td>Der Prozentsatz der Fertigstellung des Projekts, dargestellt durch einen Balken. Jede Änderung des Prozentsatzes der Fertigstellung des Projekts aktualisiert automatisch den Zielfortschritt, es sei denn, das Ziel ist geschlossen.
   </td>
  </tr>

</table>

## Suchen von Zielinformationen in Projekten

Die folgenden Zielinformationen sind in einer Projektliste oder einem Bericht sichtbar:

| Informationen zum Ziel | Beschreibung |
|---|---|
| Ziele | Eine Liste aller Ziele, denen ein Projekt zugeordnet ist. |
| Zielhierarchie | Die Hierarchie, zu der ein Ziel gehört. In diesem Feld werden nur die übergeordneten Elemente des Ziels und des Ziels angezeigt. Untergeordnete Ziele werden nicht angezeigt. |
| Anzahl verknüpfter Ziele | Die Anzahl der mit einem Projekt verknüpften Ziele. |
