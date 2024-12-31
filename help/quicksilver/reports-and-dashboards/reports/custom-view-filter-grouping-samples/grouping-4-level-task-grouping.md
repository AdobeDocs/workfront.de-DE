---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Gruppierung: 4-stufige Aufgabengruppierung für Portfolio-Verantwortliche, Programm-Verantwortliche, Projekt-Verantwortliche und Projektstatus'
description: Diese Aufgabengruppierung bietet vier Gruppierungsebenen. In diesem Fall werden die Aufgaben nach Portfolio-Verantwortlicher, Programm-Verantwortlicher, Projekt-Verantwortlicher und Projektstatus gruppiert. Sie können über die Standardschnittstelle nur bis zu drei Gruppierungsebenen haben. Um eine vierte Ebene hinzuzufügen, müssen Sie den Textmodus verwenden. Es ist nicht möglich, Berichte nach mehr als vier Kriterien gleichzeitig zu gruppieren.
author: Nolan
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 0%

---

# Gruppierung: 4-stufige Aufgabengruppierung für Portfolio-Verantwortliche, Programm-Verantwortliche, Projekt-Verantwortliche und Projektstatus

<!--Audited: 10/2024-->

Diese Aufgabengruppierung bietet vier Gruppierungsebenen. In diesem Fall werden die Aufgaben nach Portfolio-Verantwortlicher, Programm-Verantwortlicher, Projekt-Verantwortlicher und Projektstatus gruppiert. Sie können über die Standardschnittstelle nur bis zu drei Gruppierungsebenen haben. Um eine vierte Ebene hinzuzufügen, müssen Sie den Textmodus verwenden. Es ist nicht möglich, Berichte nach mehr als vier Kriterien gleichzeitig zu gruppieren.

![four_tier_grouping_for_tasks.png](assets/four-tier-grouping-for-tasks-350x239.png)

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
    <p>Neu:</p>
   <ul><li><p>Mitwirkender zum Ändern eines Filters </p></li>
   <li><p>Standard zum Ändern eines Berichts</p></li> </ul>

<p>Aktuell:</p>
   <ul><li><p>Filter ändern </p></li>
   <li><p>Planen der Änderung eines Berichts</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Berichte, Dashboards und Kalender bearbeiten, um einen Bericht zu ändern</p> <p>Zugriff auf Filter, Ansichten, Gruppierungen bearbeiten, um einen Filter zu ändern</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für einen Bericht</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Erstellen Sie eine 4-stufige Aufgabengruppe für Portfolio-Inhaber, Programm-Inhaber, Projekt-Inhaber und Projektstatus

Um diese Gruppierung anzuwenden:

1. Zu einer Aufgabenliste gehen.
1. Wählen Sie **Dropdown-Menü** Gruppierung“ **Neue Gruppierung** aus.

1. Klicken Sie **In Textmodus wechseln**.
1. Entfernen Sie den Text im Bereich **Bericht gruppieren**.
1. Ersetzen Sie den Text in dem angezeigten Feld durch den folgenden Code:
   <pre>group.0.linkedname=project<br>group.0.name=Portfolio Owner<br>group.0.notime=false<br>group.0.valueField=project:portfolio:owner:name<br>group.0.valueFormat=string<br>group.1.linkedname=project<br>group.1.name=Program Besitzer<br>Gruppe.1.notime=false<br>group.1.valueField=Projekt:program:Inhaber:name<br>group.1.valueFormat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgrouingparsedmethod=nested(project).nested(owner).string(name)<br>group.2.namekey=projectownermm<br>group.2.notime=false<br>group.2.valueField=projectOwnerMM:nameName<br>group.2.valuegroup.proeform=umeform 3.nameKeyArgKey.0=project<br>eygroup.3.nameArgKey.1=status<br>group.3.notime=false<br><br> <br> <br> <br> <br> group.3.valueField=project:statusGroup.3.valueFormat=val</pre>

1. Klicken Sie **Fertig** und dann **Gruppierung speichern**.
1. (Optional) Aktualisieren Sie den Namen für die Gruppierung und klicken Sie dann auf **Gruppierung speichern**.
