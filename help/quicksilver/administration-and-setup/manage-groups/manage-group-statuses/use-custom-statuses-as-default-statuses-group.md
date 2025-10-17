---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Benutzerdefinierten Status als Standardstatus für eine Gruppe verwenden
description: Als Gruppenadministrator können Sie einen benutzerdefinierten Status als Standardstatus für eine von Ihnen verwaltete Gruppe oder Untergruppe konfigurieren.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51018635-cd9a-402d-a136-c5bec4707cda
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 1%

---

# Benutzerdefinierten Status als Standardstatus für eine Gruppe verwenden

Als Gruppenadministrator können Sie einen benutzerdefinierten Status als Standardstatus für eine von Ihnen verwaltete Gruppe oder Untergruppe konfigurieren. Dies ist nützlich, wenn das System einem Projekt, einer Aufgabe oder einem Problem automatisch einen Workfront-Status zuweisen muss. Ein Projekt, eine Aufgabe oder ein Problem zeigt immer den benutzerdefinierten Status an, den Sie als Standardstatus festgelegt haben, anstatt den entsprechenden Workfront-Status anzuzeigen.

Der konfigurierte Status kann ein beliebiger benutzerdefinierter Status sein, der für die Gruppe erstellt wurde, von einer Gruppe über der Gruppe übernommen wurde oder von der Systemebene übernommen wurde.

Wenn es Gruppen oberhalb der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

>[!INFO]
>
>**Beispiel** Sie können einen benutzerdefinierten Status mit dem Namen Beendet erstellen und ihn als Standardstatus festlegen, der mit dem Workfront-Status Fertig entspricht.
>
>Für Aufgaben, die auf den Status Abgeschlossen gesetzt werden, wenn sie 100 % erreichen, wird dann der Status als Abgeschlossen anstelle von Abgeschlossen angezeigt.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p>
   <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>Sie müssen Gruppenadministrator der Gruppe oder Systemadministrator sein.</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Status ausgeben

Wenn der benutzerdefinierte Status ein Problemstatus ist, müssen alle vier Problemtypen dafür aktiviert sein (Fehlerbericht, Änderungsauftrag, Problem und Anfrage). Im folgenden Problemstatus kann beispielsweise der Status Erneut geöffnet nicht als Standardstatus verwendet werden, da der Problemtyp „Änderungsanforderung“ nicht ausgewählt ist:

![Alle Problemtypen aktiviert](assets/all-4-issue-types-enabled.png)

## Festlegen eines benutzerdefinierten Status als Standardstatus für eine Gruppe

{{step-1-to-setup}}

1. Klicken Sie im linken Bereich auf **Gruppen** ![Gruppen](assets/groups-icon.png) und klicken Sie dann auf den Namen der Gruppe, in der Sie Status erstellen oder anpassen möchten.
1. Klicken Sie im linken Bedienfeld auf **Status** ![Zahnradeinstellungssymbol](assets/gear-icon-settings.png).
1. Öffnen Sie **Registerkarte**, **Aufgaben** oder **Probleme** je nach dem Typ des Status, den Sie als Standardstatus festlegen möchten.
1. Klicken **oben rechts auf** Standardstatus festlegen“.
1. Wählen Sie in dem angezeigten Dropdown-Bereich neben dem Status, für den Sie den Standardstatus festlegen möchten, den Standardstatus aus, den Sie festlegen möchten.
1. Klicken Sie auf **Speichern**.

   Der Status ist jetzt als Standardstatus für die Verwendung mit Projekten verfügbar, die mit der Gruppe verknüpft sind.

1. Verknüpfen Sie den benutzerdefinierten Status mit dem Projekt, in dem Sie ihn verwenden möchten.

   Sie verknüpfen den Status mit dem Projekt, indem Sie die Gruppe, in der sich der Status befindet, mit dem Projekt verknüpfen. Benutzende können den benutzerdefinierten Status nur verwenden, wenn die Gruppe, in der sich der Status befindet, mit dem Projekt verknüpft ist.

   >[!NOTE]
   >
   >Wenn Sie das Projekt einer anderen Gruppe zuweisen, wird der Projektstatus neu geladen und kann sich ändern.

   1. Wechseln Sie zu dem Projekt, in dem Sie den benutzerdefinierten Status verwenden möchten.
   1. Klicken Sie auf das Menü Mehr ![Mehr-Symbol](assets/more-icon.png) und dann auf **Bearbeiten**.
   1. Wählen Sie in dem **Projekt bearbeiten** angezeigten Feld **Gruppe** unter **Projektverknüpfung** die Gruppe aus, mit der der benutzerdefinierte Status verknüpft ist.

   1. Klicken Sie auf **Änderungen speichern**.

## Gruppen übernehmen Standardstatuskonfigurationen

Nachdem ein Workfront-Administrator einen benutzerdefinierten Status als Standardstatus konfiguriert hat, übernehmen neu erstellte Gruppen diese Konfiguration.

Wenn ein Gruppenadministrator bzw. eine Gruppenadministratorin einen benutzerdefinierten Status als Standardstatus festgelegt hat, übernehmen auch neue Untergruppen, die direkt unterhalb der Gruppe erstellt wurden, diese Konfiguration.

Weitere Informationen finden Sie unter [So erben Gruppen Status](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

## Wenn ein Standardstatus ausgeblendet ist

Wenn Sie einen Standardstatus ausblenden (indem Sie die Option „Status ausblenden“ aktivieren), versucht das System stattdessen, einen anderen Status des entsprechenden Typs als Standard festzulegen.

Wenn kein verfügbarer Status des entsprechenden Typs vorhanden ist, wird der Statustyp als **Ausgeblendet** und ist nicht für Arbeitselemente verfügbar.

![Kein verfügbarer Status](assets/when-hide-default-status-no-equivalent.png)
