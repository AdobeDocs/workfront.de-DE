---
product-area: projects
navigation-topic: task-information
title: Zeitverzögerung für Aufgabenebene aktualisieren
description: Manchmal kann es bei einem Projekt zu Konflikten zwischen Aufgabenzeitplänen kommen. Sie können Ressourcen einschränken oder Ressourcenkonflikte beheben, indem Sie Ressourcen und Aufgaben neu planen, damit alle Aufgaben innerhalb eines realistischen Zeitplans ausgeführt werden können. Weitere Informationen zum Einteilen von Aufgaben finden Sie unter Level-Ressourcen im Gantt-Diagramm .
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 3%

---

# Zeitverzögerung für Aufgabenebene aktualisieren

Manchmal kann es bei einem Projekt zu Konflikten zwischen Aufgabenzeitplänen kommen. Sie können Ressourcen einschränken oder Ressourcenkonflikte beheben, indem Sie Ressourcen und Aufgaben neu planen, damit alle Aufgaben innerhalb eines realistischen Zeitplans ausgeführt werden können. Weitere Informationen zum Leveln von Aufgaben finden Sie unter [Level-Ressourcen im Gantt-Diagramm](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md).

Als Projektmanager oder Aufgabenverantwortlicher können Sie für einzelne Aufgaben auch eine Zeitverzögerung hinzufügen, um alle Ressourcen- oder Zeitplankonflikte zu berücksichtigen. Anders ausgedrückt: Eine Aufgabe kann mit einer Verzögerung geplant werden, um sicherzustellen, dass Ressourcenkonflikte bei der Stufe der Adobe Workfront-Aufgabenniveaus realistischer werden.

Durch das Hinzufügen einer Zeitverzögerung zu einer Aufgabe wird das geplante Abschlussdatum der Aufgabe angepasst. Informationen zum geplanten Abschlussdatum finden Sie unter [Überblick über das voraussichtliche Abschlussdatum für Projekte, Aufgaben und Probleme](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben und Projekte bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für Aufgaben verwalten </p> <p>Contribute oder höhere Berechtigungen für Projekte</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Einer Aufgabe eine Verzögerung auf Stufe hinzufügen

1. Gehen Sie zu einer Aufgabe, für die Sie eine Zeitverzögerung hinzufügen möchten.
1. Klicken Sie auf das Symbol &quot;**Mehr&quot;** rechts neben dem Aufgabennamen und dann auf &quot;**Bearbeiten**&quot;.

1. Klicken Sie auf **Einstellungen**.

   ![](assets/leveling-delay-edit-task-nwe-350x345.png)

1. Geben Sie die **Verzögerung bei der Leerung** in Stunden an und wählen Sie dann eine Zeiteinheit aus.\
   Dies ist der Zeitpunkt, zu dem die Ressource aufgrund von Ressourcenkonflikten beim Starten der Aufgabe verzögert wird.

   Wählen Sie aus den folgenden Optionen für Zeiteinheiten aus:

   * Minuten
   * Stunden. Dies ist die Standardeinstellung.
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
   >Die verstrichene Zeit ist eine Zeiteinheit für die Dauer einer Aufgabe. Dies ist die Zeit zwischen dem geplanten Startdatum und dem geplanten Abschlussdatum einer Aufgabe, die Feiertage, Wochenenden und eine Verspätung umfasst. Mit anderen Worten, vergangene Zeit ist der Durchgang von Kalendertagen.

1. Klicken Sie auf **Speichern**. 

 
