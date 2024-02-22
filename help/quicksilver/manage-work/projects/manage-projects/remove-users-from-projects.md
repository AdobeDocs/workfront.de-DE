---
product-area: projects;user-management
navigation-topic: manage-projects
title: Entfernen von Benutzern aus Projekten
description: Sie können Benutzer aus einem Projekt entfernen, wenn sie nicht mehr an der Bearbeitung des Projekts beteiligt sind.
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: afbf2e2fbfcc2c527223da008518bc7632872c23
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# Entfernen von Benutzern aus Projekten

Sie können Benutzer aus einem Projekt entfernen, wenn sie nicht mehr an der Bearbeitung des Projekts beteiligt sind. Das Entfernen von Benutzern aus Projekten wirkt sich auf Aufgaben- und Problemzuweisungen sowie auf Projektrollen aus. Entfernte Benutzer erhalten keine Benachrichtigungen mehr, die für das Projektteam vorgesehen sind. Weitere Informationen zu Benachrichtigungen für die Projektteams finden Sie unter [Typen von Ereignisbenachrichtigungen](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

Die mit einem Projekt verknüpften Benutzer werden im Bereich Personen eines Projekts aufgelistet. Sie vertreten das Projektteam. Weitere Informationen zum Projektteam finden Sie unter [Übersicht über das Projektteam](../../../manage-work/projects/planning-a-project/project-team-overview.md).

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für das Projekt verwalten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Auswirkungen des Entfernens eines Benutzers auf bestehende Aufgaben, Probleme und Projekte

Wenn ein Benutzer aus einem Projekt entfernt wird, können alle ihm zugewiesenen Aufgaben oder Probleme davon betroffen sein, je nachdem, ob die Aufgabe oder das Problem beim Entfernen des Benutzers abgeschlossen wurde:

* **Wenn das Element beim Entfernen des Benutzers nicht abgeschlossen ist:** Das Element wird einer Auftragsrolle erneut zugewiesen, wenn bereits eine Auftragsrolle zugewiesen wurde, oder es wird der Auftragsrolle zugewiesen, die der Benutzer für das Element ausgeführt hat. Wenn dem Element oder dem Benutzer keine Auftragsrolle zugewiesen wurde, müssen Sie das Element manuell neu zuweisen.
* **Wenn das Element beim Entfernen des Benutzers abgeschlossen ist:** Der Name des entfernten Benutzers verbleibt im Element.
* **Wenn der entfernte Benutzer auch der Ersteller eines Projekts ist:** Das Projekt wird nicht aus dem **Projekte, an denen ich arbeite** Liste im Bereich &quot;Projekte&quot;. Das Projekt wird für alle anderen Benutzer, die nach diesem Projekt filtern, durch das Feld &quot;Eingegeben von&quot;aus den Listen entfernt.
* **Wenn der Benutzer Eigentümer oder Sponsor des Projekts ist:** Der Benutzer bleibt in seiner Rolle als Sponsor oder Eigentümer des Projekts.

## Entfernen von Benutzern aus einem Projekt und einem Projektteam

Sie können Benutzer aus einem Projekt entfernen, indem Sie sie aus dem Projektteam entfernen.

Wenn Benutzer Rollen in einem Projekt erfüllen, werden sie Teil des Projektteams.

Wenn Sie Benutzer aus ihren Rollen im Projekt entfernen, bleiben sie Teil des Projektteams.

Informationen zu den Benutzerrollen in einem Projekt finden Sie unter [Verwalten des Projektteams](../planning-a-project/manage-project-team.md).

So entfernen Sie Benutzer aus dem Projektteam:

1. Wechseln Sie zu dem Projekt, aus dem Sie die Benutzer entfernen möchten.

1. Klicks **Personen** Wählen Sie im linken Bereich die Benutzer aus, die Sie entfernen möchten. Möglicherweise müssen Sie auf **Mehr anzeigen**, dann **Personen**.

1. Klicken Sie auf **Entfernen** icon  ![Element entfernen](assets/remove-icon---x-in-circle.png) oben in der Liste der Benutzer.

1. Klicks **Ja, ausgewählte Benutzer entfernen** zur Bestätigung der Entfernung.

   Die Benutzer werden aus dem Projektteam entfernt und von unvollständigen Aufgaben oder Problemen, denen sie möglicherweise zugewiesen sind. Sie erhalten keine Benachrichtigungen mehr für das Projektteam.
