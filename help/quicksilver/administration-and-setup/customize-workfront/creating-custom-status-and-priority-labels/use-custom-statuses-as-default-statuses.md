---
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Benutzerdefinierte Status als Standardstatus verwenden
description: Wenn ein benutzerdefinierter Status als Standardstatus festgelegt wird, wird der neue Standardstatus im gesamten System auf verschiedene Arten verwendet. Die Verwendungsmöglichkeiten hängen davon ab, ob es sich um einen Standardstatus auf Systemebene oder einen Standardstatus auf Gruppenebene handelt.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5b137cee-e03a-4176-a683-b77f2b27f5ce
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# Benutzerdefinierte Status als Standardstatus verwenden

Wenn ein benutzerdefinierter Status als Standardstatus festgelegt wird, wird der neue Standardstatus im gesamten System auf verschiedene Arten verwendet. Die Verwendungsmöglichkeiten hängen davon ab, ob es sich um einen Standardstatus auf Systemebene oder einen Standardstatus auf Gruppenebene handelt.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
     <p>Neu: Standard</p>
     <p>oder</p>
     <p>Aktuell: Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Benutzerdefinierte Standardstatus auf Systemebene

Wenn Sie einen benutzerdefinierten Status als Standardsystemstatus festlegen, erben alle neuen Gruppen, die im System erstellt werden, diesen Status.

Gruppen, die bereits vorhanden waren, als Sie den neuen standardmäßigen Systemstatus festgelegt haben, übernehmen ihn nicht automatisch.

Angenommen, in Ihrer Adobe Workfront-Umgebung wurden bereits zwei Gruppen erstellt (Marketing und Vertrieb). Sie erstellen einen neuen benutzerdefinierten Status, der dem aktuellen entspricht, und rufen den Status In Bearbeitung auf. Jetzt erstellen Sie eine neue Gruppe mit dem Namen Engineering. In diesem Szenario übernimmt die Engineering-Gruppe den neuen Standardstatus. Die Marketing- und Vertriebsgruppen übernehmen ihn nicht.

## Benutzerdefinierte Standardstatus auf Gruppenebene

Ein benutzerdefinierter Status, den Sie als Standardgruppenstatus festlegen, wird unter folgenden Umständen verwendet:

* **Wenn das Workfront-System automatisch einen Status auswählt, wird der Standardgruppenstatus verwendet:** Der benutzerdefinierte Status, den Sie als Standardgruppenstatus festlegen, wird verwendet, wenn das Workfront-System einem Objekt automatisch einen Status zuweist.

  Beispielsweise kann eine Aufgabe so konfiguriert werden, dass sie automatisch in den Status Abgeschlossen wechselt, wenn der abgeschlossene Prozentwert 100 % erreicht. Wenn Sie einen benutzerdefinierten Status erstellen, der mit Abgeschlossen übereinstimmt, und diesen benutzerdefinierten Status als Standardstatus festlegen, ändert Workfront den Status der Aufgabe in den neuen Standardstatus.

  Benutzerdefinierte Status werden auf diese Weise nur mit Gruppenstatus verwendet, die mit einer Aufgabe oder einem Problem verknüpft sind. Benutzerdefinierte Status können auf diese Weise nicht für Status verwendet werden, die mit einem Projekt verknüpft sind.

* Der **Status eines Projekts wird durch die mit dem Projekt verknüpfte Gruppe bestimmt**: Wenn sich die mit einem bestimmten Projekt verknüpfte Gruppe ändert, ändert sich der Status des Projekts in Abhängigkeit von den für die Gruppe definierten Standardstatus. (Eine Gruppe kann bei der Bearbeitung des Projekts über das Feld Gruppen mit einem Projekt verknüpft werden.)

  Wenn sich diese Gruppe ändert, ändert sich der Status des Projekts, wenn für die neue Gruppe ein anderer Standardstatus definiert ist, der dem aktuellen Status des Projekts entspricht.

  Beispielsweise kann ein Projekt mit der Marketing-Gruppe verknüpft werden und der Status des Projekts ist „Planung“. Das Projekt wird so bearbeitet, dass es jetzt mit der Vertriebsgruppe verknüpft ist. Die Verkaufsgruppe hat einen benutzerdefinierten Standardgruppenstatus mit der Bezeichnung Denken (dieser Status entspricht Planung). Da die Gruppe im Projekt geändert wurde, ändert sich der Status des Projekts jetzt in „Denken“.

Wenn Sie Gruppenadministrator sind, lesen Sie [Festlegen eines Status als Standardstatus für eine Gruppe](/help/quicksilver/administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Status ausgeben

Wenn der benutzerdefinierte Status ein Problemstatus ist, müssen alle vier Problemtypen dafür aktiviert sein (Fehlerbericht, Änderungsauftrag, Problem und Anfrage). Im folgenden Problemstatus kann beispielsweise der Status Erneut geöffnet nicht als Standardstatus verwendet werden, da der Problemtyp „Änderungsanforderung“ nicht ausgewählt ist:

![Alle Problemtypen aktiviert](assets/all-4-issue-types-enabled.png)

## Festlegen eines benutzerdefinierten Status als Standardstatus

{{step-1-to-setup}}

1. Klicken Sie im linken Bedienfeld auf **Projektvoreinstellungen** > **Status**.
1. (Bedingt) Wenn Sie einen Standardstatus für eine Gruppe festlegen, geben Sie den Namen der Gruppe in das Menü oben rechts ein und wählen Sie ihn aus, wenn er angezeigt wird.
1. Öffnen Sie **Registerkarte**, **Aufgaben** oder **Probleme** je nach dem Typ des Status, den Sie als Standardstatus festlegen möchten.
1. Klicken Sie auf **Dropdown** Menü Standardstatus festlegen .
1. Wählen Sie in dem angezeigten Dropdown-Bereich neben dem Status, für den Sie den Standardstatus festlegen möchten, den gewünschten Standardstatus aus.
1. Klicken Sie auf **Speichern**.
1. Verknüpfen Sie das Projekt mit der Gruppe, in der sich der Status befindet.

   >[!NOTE]
   >
   >Wenn Sie den benutzerdefinierten Status für eine Gruppe festlegen und das Projekt später einer anderen Gruppe zuweisen, wird der Projektstatus neu geladen und kann sich ändern.

   1. Wechseln Sie zu dem Projekt, in dem Sie den benutzerdefinierten Status verwenden möchten.
   1. Klicken Sie auf das Menü Mehr ![Mehr-Symbol](assets/more-icon.png) und dann auf **Bearbeiten**.
   1. Wählen Sie in dem **Projekt bearbeiten** angezeigten Feld im Feld **Gruppe** unter **Projektverknüpfung** die Gruppe aus, in der sich der Status befindet.
   1. Klicken Sie auf **Änderungen speichern**.
