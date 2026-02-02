---
product-area: projects
navigation-topic: task-information
title: Abgleichsverzögerung für Aufgabe aktualisieren
description: Manchmal kann es zu Konflikten zwischen Aufgabenplänen für ein Projekt kommen. Sie können Ressourcen abgleichen oder Ressourcenkonflikte beheben, indem Sie Ressourcen und Vorgänge neu planen, sodass alle Vorgänge innerhalb eines realistischen Zeitplans abgeschlossen werden können. Weitere Informationen zu Abgleichsaufgaben finden Sie unter Abgleichsressourcen im Gantt-Diagramm .
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 9%

---

# Abgleichsverzögerung für Aufgabe aktualisieren

Manchmal kann es zu Konflikten zwischen Aufgabenplänen für ein Projekt kommen. Sie können Ressourcen abgleichen oder Ressourcenkonflikte beheben, indem Sie Ressourcen und Vorgänge neu planen, sodass alle Vorgänge innerhalb eines realistischen Zeitplans abgeschlossen werden können. Weitere Informationen zu Abgleichsaufgaben finden Sie [Ressourcen abgleichen im Gantt-Diagramm](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

Als Projektmanager oder Aufgabenbearbeiter können Sie auch eine Abgleichsverzögerung für einzelne Vorgänge hinzufügen, um Ressourcen- oder Terminkonflikte zu berücksichtigen. Mit anderen Worten: Eine Aufgabe kann verzögert geplant werden, um sicherzustellen, dass beim Abgleichen der Aufgaben durch Adobe Workfront ein realistischerer Zeitplan Ressourcenkonflikte überwindet.

Durch Hinzufügen einer Abgleichsverzögerung zu einer Aufgabe wird das voraussichtliche Abschlussdatum der Aufgabe angepasst. Informationen zum voraussichtlichen Abschlussdatum finden Sie unter [Übersicht über das voraussichtliche Abschlussdatum für Projekte, Aufgaben und Probleme](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> <p>Standard</p>
   <p>Work oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für Aufgaben </p> <p>Mitwirken an oder höhere Berechtigungen für Projekte</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to Tasks </p> <p>Contribute or higher permissions to Projects</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Abgleichsverzögerung zu einer Aufgabe hinzufügen

1. Gehe zu einer Aufgabe, für die du eine Abgleichsverzögerung hinzufügen möchtest.
1. Klicken Sie auf **Mehr** rechts neben dem Aufgabennamen und dann auf **Bearbeiten**.

1. Klicken Sie auf **Einstellungen**.

   ![Abgleichsverzögerung beim Bearbeiten einer Aufgabe](assets/leveling-delay-edit-task-nwe-350x345.png)

1. Geben Sie die **Abgleichsverzögerung** in Stunden an und wählen Sie dann eine Zeiteinheit aus.\
   Dies ist der Zeitpunkt, zu dem der Start der Aufgabe aufgrund von Ressourcenkonflikten verzögert wird.

   Wählen Sie für Zeiteinheiten aus den folgenden Optionen aus:

   * Minutes
   * Stunden. Dies ist der Standardwert.
   * Days
   * Weeks
   * Months
   * Verstrichene Minuten
   * Verstrichene Stunden
   * Verstrichene Tage
   * Verstrichene Wochen
   * Verstrichene Monate

   >[!TIP]
   >
   >Verstrichene Zeit ist eine Zeiteinheit für die Dauer einer Aufgabe. Dies ist die Zeit zwischen dem geplanten Startdatum und dem geplanten Abschlussdatum einer Aufgabe, die Feiertage, Wochenenden und Ausfallzeiten umfasst. Mit anderen Worten: Verstrichene Zeit ist der Ablauf von Kalendertagen.

1. Klicken Sie auf **Speichern**.


