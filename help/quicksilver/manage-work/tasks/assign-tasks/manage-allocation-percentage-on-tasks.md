---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Verwalten des Prozentsatzes der Benutzer- oder Rollenzuweisung bei Aufgaben
description: Der Zuordnungsprozentsatz gibt an, wie lange eine zugewiesene Ressource an einem Tag an einem Vorgang arbeiten soll. Er ist der Prozentsatz eines Arbeitstages (gemäß dem Benutzer- oder Projektzeitplan), an dem eine Ressource während der gesamten Dauer des Vorgangs zugewiesen wird.
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 830ad0411084844ace1e1e543c3ebefcb558af80
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 1%

---

# Verwalten des Prozentsatzes der Benutzer- oder Rollenzuweisung bei Aufgaben

Der Zuordnungsprozentsatz gibt an, wie lange eine zugewiesene Ressource an einem Tag an einem Vorgang arbeiten soll. Er ist der Prozentsatz eines Arbeitstages (gemäß dem Benutzer- oder Projektzeitplan), an dem eine Ressource während der gesamten Dauer des Vorgangs zugewiesen wird.

>[!NOTE]
>
>Wenn Sie Benutzende einer Arbeit zuweisen, wirkt sich ihre Verfügbarkeit entsprechend den Zeitplänen auf die geplanten und erwarteten Termine von Aufgaben und Problemen aus. Weitere Informationen zu Zeitplänen finden Sie unter [Erstellen eines Zeitplans](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <td> <p>Neu: Standard</p> 
   <p>Aktuell: Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Contribute oder höhere Berechtigungen für die Aufgabe</p> <p>Bearbeiten Sie die Berechtigungen, um den Zuordnungsprozentsatz im Feld Aufgabe bearbeiten zu aktualisieren</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen finden Sie unter [Zugriffsanforderungen für Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zur Änderung der prozentualen Zuteilungen für Aufgaben

* Benutzern wird standardmäßig ein gleicher Prozentsatz der Zeit für Aufgaben zugewiesen, denen sie zugewiesen sind.
* Sie können den Zuordnungsprozentsatz für Benutzer und Aufgabengebiete, die Aufgaben zugewiesen sind, nur dann manuell ändern, wenn der Dauertyp der Aufgabe „Berechnet“, „Arbeit“ oder „Arbeitsaufwand“ ist.

  Weitere Informationen finden Sie unter [Übersicht über Aufgabendauer und -typ](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Die prozentuale Zuordnung für Teams, die Aufgaben zugewiesen sind, kann nicht geändert werden.
* Die prozentuale Zuordnung für Benutzende und den Problemen zugewiesenen Aufgabengebieten kann nicht geändert werden.

## Ändern der prozentualen Zuordnung des Benutzers oder der Funktion für eine Aufgabe

1. Wechseln Sie zu einem Vorgang, für dessen Ressourcen Sie die prozentuale Zuordnung ändern.
1. Klicken Sie auf das **Mehr**-![](assets/qs-more-icon-on-an-object.png) neben dem Namen der Aufgabe und dann auf **Bearbeiten**.

   Oder

   Klicken Sie in **Aufgabenkopfzeile auf den** „Arbeitsaufträge“ und dann auf **Erweitert**.

1. Stellen Sie sicher **dass der** Dauertyp“ der Aufgabe einer der folgenden ist:

   * Berechnete Arbeit
   * Leistungsgesteuert

   >[!TIP]
   >
   >* Für den Typ „Berechnete Zuweisungsdauer“ verwendet Workfront die folgende Formel, um den Zuordnungsprozentsatz jedes Empfängers zu berechnen: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* Für den Typ Einfache Dauer können Sie die jeder Ressource zugewiesenen Stunden schätzen, nicht den Zuordnungsprozentsatz.

1. Klicken Sie **Arbeitsaufträge** und ändern Sie dann **Zuweisungen** für jeden Aufgabenzugewiesenen.

   Sie können nur den Zuordnungsprozentsatz für Benutzer- und Aufgabenrollenzuweisungen ändern.

   Sie können den Zuordnungsprozentsatz für ein Team, das einer Aufgabe zugewiesen ist, nicht ändern.

   ![Ändern des Zuordnungsprozentsatzes](assets/advanced-assignments-allocation-percentage.png)

1. Klicken Sie auf **Speichern**.
