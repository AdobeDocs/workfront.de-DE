---
product-area: projects;user-management
navigation-topic: manage-projects
title: Benutzer aus Projekten entfernen
description: Sie können Benutzer aus einem Projekt entfernen, wenn sie nicht mehr an der Fertigstellung der Arbeit am Projekt beteiligt sind.
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 0%

---

# Benutzer aus Projekten entfernen

Sie können Benutzer aus einem Projekt entfernen, wenn sie nicht mehr an der Fertigstellung der Arbeit am Projekt beteiligt sind. Das Entfernen von Benutzern aus Projekten wirkt sich auf Aufgaben- und Problemzuweisungen sowie auf Projektrollen aus. Entfernte Benutzer erhalten keine Benachrichtigungen mehr, die für das Projekt-Team vorgesehen sind. Weitere Informationen zu Benachrichtigungen für die Projekt-Teams finden Sie unter [Ereignistypen](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Die mit einem Projekt verknüpften Benutzer werden im Bereich Personen eines Projekts aufgelistet. Sie repräsentieren das Projektteam. Weitere Informationen über das Projektteam finden Sie unter [Übersicht über das Projektteam](../../../manage-work/projects/planning-a-project/project-team-overview.md).

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Projekt</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Wie sich das Entfernen eines Benutzers auf vorhandene Aufgaben, Probleme und Projekte auswirkt

Wenn ein(e) Benutzende(r) aus einem Projekt entfernt wird, können alle ihm/ihr zugewiesenen Aufgaben oder Probleme betroffen sein, je nachdem, ob die Aufgabe oder das Problem beim Entfernen des/r Benutzenden abgeschlossen wurde:

* **Wenn das Element nicht abgeschlossen ist, wenn der Benutzer entfernt wird:** Das Element wird einem Aufgabengebiet erneut zugewiesen, wenn bereits ein Aufgabengebiet zugewiesen wurde, oder es wird dem Aufgabengebiet zugewiesen, das der Benutzer für das Element erfüllt hat. Wenn dem Element oder dem Benutzer kein Aufgabengebiet zugewiesen war, müssen Sie das Element manuell neu zuweisen.
* **Wenn das Element abgeschlossen ist, wenn der Benutzer entfernt wird:** Der Name des entfernten Benutzers bleibt auf dem Element.
* **Wenn der entfernte Benutzer auch der Ersteller eines Projekts ist:** Das Projekt wird nicht aus der Liste **Projekte, an denen ich**) im Bereich Projekte entfernt. Das Projekt wird für alle anderen Benutzer aus den Listen entfernt, die über das Feld Eingegeben von nach diesem Projekt filtern.
* **Wenn der Benutzer Projekteigentümer oder Sponsor ist** bleibt der Benutzer in seiner Rolle als Sponsor oder Eigentümer des Projekts.

## Entfernen von Benutzern aus einem Projekt- und Projektteam

Sie können Benutzer aus einem Projekt entfernen, indem Sie sie aus dem Projektteam entfernen.

Wenn Benutzer Rollen in einem Projekt erfüllen, werden sie Teil des Projektteams.

Wenn Sie Benutzer aus ihren Rollen im Projekt entfernen, bleiben sie Teil des Projektteams.

Informationen zu Benutzerrollen in einem Projekt finden Sie unter [Verwalten des Projektteams](../planning-a-project/manage-project-team.md).

So entfernen Sie Benutzer aus dem Projektteam:

1. Wechseln Sie zu dem Projekt, in dem Sie die Benutzer entfernen möchten.

1. Klicken Sie **linken** auf „Personen“ und wählen Sie dann die Benutzer aus, die Sie entfernen möchten.

1. Klicken Sie auf **Entfernen**-Symbol ![Element entfernen](assets/remove-icon---x-in-circle.png) oben in der Benutzerliste.

1. Klicken Sie auf **Ja, ausgewählte Benutzer entfernen**, um die Entfernung zu bestätigen.

   Die Benutzer werden aus dem Projektteam und aus allen unvollständigen Aufgaben oder Problemen entfernt, denen sie möglicherweise zugewiesen sind. Sie erhalten keine Benachrichtigungen mehr, die für das Projektteam bestimmt sind.
