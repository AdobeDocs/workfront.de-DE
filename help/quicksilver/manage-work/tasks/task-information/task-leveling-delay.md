---
product-area: projects
navigation-topic: task-information
title: Abgleichsverzögerung für Aufgabe aktualisieren
description: Manchmal kann es zu Konflikten zwischen Aufgabenplänen für ein Projekt kommen. Sie können Ressourcen abgleichen oder Ressourcenkonflikte beheben, indem Sie Ressourcen und Vorgänge neu planen, sodass alle Vorgänge innerhalb eines realistischen Zeitplans abgeschlossen werden können. Weitere Informationen zu Abgleichsaufgaben finden Sie unter Abgleichsressourcen im Gantt-Diagramm .
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 3%

---

# Abgleichsverzögerung für Aufgabe aktualisieren

Manchmal kann es zu Konflikten zwischen Aufgabenplänen für ein Projekt kommen. Sie können Ressourcen abgleichen oder Ressourcenkonflikte beheben, indem Sie Ressourcen und Vorgänge neu planen, sodass alle Vorgänge innerhalb eines realistischen Zeitplans abgeschlossen werden können. Weitere Informationen zu Abgleichsaufgaben finden Sie [Ressourcen abgleichen im Gantt-Diagramm](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

Als Projektmanager oder Aufgabenbearbeiter können Sie auch eine Abgleichsverzögerung für einzelne Vorgänge hinzufügen, um Ressourcen- oder Terminkonflikte zu berücksichtigen. Mit anderen Worten: Eine Aufgabe kann verzögert geplant werden, um sicherzustellen, dass beim Abgleichen der Aufgaben durch Adobe Workfront ein realistischerer Zeitplan Ressourcenkonflikte überwindet.

Durch Hinzufügen einer Abgleichsverzögerung zu einer Aufgabe wird das voraussichtliche Abschlussdatum der Aufgabe angepasst. Informationen zum voraussichtlichen Abschlussdatum finden Sie unter [Übersicht über das voraussichtliche Abschlussdatum für Projekte, Aufgaben und Probleme](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für Aufgaben </p> <p>Contribute oder höhere Berechtigungen für Projekte</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Abgleichsverzögerung zu einer Aufgabe hinzufügen

1. Gehe zu einer Aufgabe, für die du eine Abgleichsverzögerung hinzufügen möchtest.
1. Klicken Sie auf **Mehr** rechts neben dem Aufgabennamen und dann auf **Bearbeiten**.

1. Klicken Sie **Einstellungen**.

   ![](assets/leveling-delay-edit-task-nwe-350x345.png)

1. Geben Sie die **Abgleichsverzögerung** in Stunden an und wählen Sie dann eine Zeiteinheit aus.\
   Dies ist der Zeitpunkt, zu dem der Start der Aufgabe aufgrund von Ressourcenkonflikten verzögert wird.

   Wählen Sie für Zeiteinheiten aus den folgenden Optionen aus:

   * Minuten
   * Stunden. Dies ist der Standardwert.
   * Tag(e)
   * Wochen
   * Monate
   * Verstrichene Minuten
   * Verstrichene Stunden
   * Verstrichene Tage
   * Verstrichene Wochen
   * Verstrichene Monate

   >[!TIP]
   >
   >Verstrichene Zeit ist eine Zeiteinheit für die Dauer einer Aufgabe. Dies ist die Zeit zwischen dem geplanten Startdatum und dem geplanten Abschlussdatum einer Aufgabe, die Feiertage, Wochenenden und Ausfallzeiten umfasst. Mit anderen Worten: Verstrichene Zeit ist der Ablauf von Kalendertagen.

1. Klicken Sie **Speichern**. 

 
