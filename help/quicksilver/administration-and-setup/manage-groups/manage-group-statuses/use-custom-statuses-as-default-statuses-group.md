---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Benutzerdefinierten Status als Standardstatus für eine Gruppe verwenden
description: Als Gruppenadministrator können Sie einen benutzerdefinierten Status als Standardstatus für eine von Ihnen verwaltete Gruppe oder Untergruppe konfigurieren. Dies ist nützlich, wenn das System einem Projekt, einer Aufgabe oder einem Problem automatisch einen Workfront-Status zuweisen muss. Bei einem Projekt, einer Aufgabe oder einem Problem wird immer der benutzerdefinierte Status angezeigt, den Sie als Standardstatus festlegen, anstatt den Workfront-Status anzuzeigen, dem es entspricht.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51018635-cd9a-402d-a136-c5bec4707cda
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '727'
ht-degree: 0%

---

# Benutzerdefinierten Status als Standardstatus für eine Gruppe verwenden

Als Gruppenadministrator können Sie einen benutzerdefinierten Status als Standardstatus für eine von Ihnen verwaltete Gruppe oder Untergruppe konfigurieren. Dies ist nützlich, wenn das System einem Projekt, einer Aufgabe oder einem Problem automatisch einen Workfront-Status zuweisen muss. Bei einem Projekt, einer Aufgabe oder einem Problem wird immer der benutzerdefinierte Status angezeigt, den Sie als Standardstatus festlegen, anstatt den Workfront-Status anzuzeigen, dem es entspricht.

Der Status, den Sie konfigurieren, kann ein beliebiger benutzerdefinierter Status sein, der für die Gruppe erstellt, von einer Gruppe über der Gruppe übernommen oder von der Systemebene übernommen wurde.

Wenn es Gruppen über der von Ihnen verwalteten Gruppe gibt, können deren Administratoren dies auch für Ihre Gruppe tun. Dasselbe gilt für Workfront-Administratoren (für jede Gruppe).

>[!INFO]
>
>**Beispiel:** Sie können einen benutzerdefinierten Status mit dem Namen Abgeschlossen erstellen und ihn als Standardstatus mit dem Workfront-Status Abgeschlossen festlegen.
>
>Für Aufgaben, die auf den Status Abgeschlossen geändert werden, wenn sie 100 % erreichen, wird der Status als Abgeschlossen anstelle von Abgeschlossen angezeigt.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen, um die Schritte in diesem Artikel durchzuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-Plan*</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> <p>Sie müssen Gruppenadministrator der Gruppe oder Workfront-Administrator sein. Weitere Informationen finden Sie unter <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppenadministratoren</a> und <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenn Sie herausfinden möchten, welchen Plan oder welchen Lizenztyp Sie haben, wenden Sie sich an Ihren Workfront-Administrator.

## Problemstatus

Wenn der benutzerdefinierte Status ein Problemstatus ist, müssen alle vier Ausgabetypen dafür aktiviert sein (Fehlerbericht, Änderungsreihenfolge, Problem und Anfrage). Beispielsweise kann der Status Neu geöffnet im unten gezeigten Problemstatus nicht als Standardstatus verwendet werden, da der Problemtyp Reihenfolge ändern nicht ausgewählt ist:

![](assets/all-4-issue-types-enabled.png)

## Benutzerdefinierten Status als Standardstatus für eine Gruppe festlegen

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).
1. Klicken Sie im linken Bereich auf **Gruppen** ![](assets/groups-icon.png)und klicken Sie dann auf den Namen der Gruppe, in der Sie Status erstellen oder anpassen möchten.
1. Klicken Sie im linken Bereich auf **Status** ![](assets/gear-icon-settings.png).
1. Öffnen Sie die **Projekt**, **Aufgaben** oder **Probleme** -Tab, abhängig vom Statustyp, den Sie als Standardstatus festlegen möchten.
1. Klicken **Festlegen von Standardstatus** in der Nähe der oberen rechten Ecke.
1. Wählen Sie im angezeigten Dropdown-Bereich neben dem Status, für den Sie den Standardstatus festlegen möchten, den Standardstatus aus, den Sie festlegen möchten.
1. Klicken Sie auf **Speichern**.

   Der Status ist jetzt als Standardstatus für die Verwendung mit Projekten verfügbar, die mit der Gruppe verknüpft sind.

1. Verknüpfen Sie den benutzerdefinierten Status mit dem Projekt, in dem Sie es verwenden möchten.

   Sie verknüpfen den Status mit dem Projekt, indem Sie die Gruppe, in der sich der Status befindet, mit dem Projekt verknüpfen. Benutzer können den benutzerdefinierten Status nur verwenden, wenn die Gruppe, in der sich der Status befindet, mit dem Projekt verknüpft ist.

   >[!NOTE]
   >
   >Wenn Sie das Projekt einer anderen Gruppe zuweisen, wird der Projektstatus neu geladen und kann sich ändern.

   1. Wechseln Sie zu dem Projekt, in dem Sie den benutzerdefinierten Status verwenden möchten.
   1. Klicken Sie auf das Menü Mehr . ![](assets/more-icon.png)Klicken Sie auf **Bearbeiten**.
   1. Im **Projekt bearbeiten** -Feld, das im **Gruppe** Feld unter **Projektverknüpfung** wählen Sie die Gruppe aus, der der benutzerdefinierte Status zugeordnet ist.

   1. Klicken **Änderungen speichern**.

## Gruppen übernehmen Standardstatuskonfigurationen

Nachdem ein Workfront-Administrator einen benutzerdefinierten Status als Standardstatus konfiguriert hat, übernehmen neue erstellte Gruppen diese Konfiguration.

Entsprechend übernehmen neue Untergruppen, die direkt unterhalb der Gruppe erstellt werden, nachdem ein Gruppenadministrator einen benutzerdefinierten Status als Standardstatus festgelegt hat.

Weitere Informationen finden Sie unter [Vererben von Status durch Gruppen](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

## Wenn ein Standardstatus ausgeblendet wird

Wenn Sie einen Standardstatus ausblenden (indem Sie die Option Status ausblenden aktivieren), versucht das System stattdessen, einen anderen Status des entsprechenden Typs als Standard festzulegen.

Wenn der Status des entsprechenden Typs nicht verfügbar ist, wird der Statustyp als **Ausgeblendet** und ist nicht für Arbeitselemente verfügbar.

![](assets/when-hide-default-status-no-equivalent.png)
