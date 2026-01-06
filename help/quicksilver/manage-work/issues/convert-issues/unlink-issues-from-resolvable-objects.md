---
product-area: projects
navigation-topic: convert-issues
title: Aufheben der Verknüpfung von Problemen mit Lösungsobjekten
description: Wenn Sie ein Projekt oder eine Aufgabe erstellen, indem Sie ein Problem in das Projekt oder die Aufgabe konvertieren, haben Sie die Möglichkeit, das ursprüngliche Problem beizubehalten. Ihr Adobe Workfront-Administrator muss diese Voreinstellung aktivieren, damit Sie diese Option während der Konvertierung des Problems erhalten. Weitere Informationen zum Konvertieren von Problemen in Projekte und Aufgaben finden Sie unter Übersicht über das Konvertieren von Problemen in Adobe Workfront.
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 3%

---

# Aufheben der Verknüpfung von Problemen mit Lösungsobjekten

<!--Audited: 08/2025-->

Wenn Sie ein Projekt oder eine Aufgabe erstellen, indem Sie ein Problem in das Projekt oder die Aufgabe konvertieren, haben Sie die Möglichkeit, das ursprüngliche Problem beizubehalten. Ihr Adobe Workfront-Administrator muss diese Voreinstellung aktivieren, damit Sie diese Option während der Konvertierung des Problems erhalten.\
Weitere Informationen zum Konvertieren von Problemen in Projekte und Aufgaben finden Sie unter [Übersicht über das Konvertieren von Problemen in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Wenn Sie sich entscheiden, das Problem, das in das Projekt oder die Aufgabe konvertiert wurde, beizubehalten, ist die Lösung des Problems an das Projekt oder die Aufgabe gebunden. Das Problem wird zum lösbaren Objekt des Projekts oder der Aufgabe. Das Projekt oder die Aufgabe sind die Lösungsobjekte des Problems.

Sie können ein Problem auch manuell mit einem anderen Problem verknüpfen. Das zweite Problem wird in diesem Fall zum Lösungsobjekt für das erste Problem.\
Weitere Informationen zum Auflösen von Objekten finden Sie unter [Übersicht über das Auflösen und das Auflösen von Objekten](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

>[!TIP]
>
>Der Problemstatus kann nicht geändert werden, da er sich automatisch mit dem Status des Lösungsobjekts ändert.

Sie können die Verknüpfung zwischen der Lösung eines Problems und der eines Projekts, einer Aufgabe oder eines Problems aufheben, indem Sie das Projekt, die Aufgabe oder das Problem aus dem Problem entfernen.

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
   <td> <p>Mitwirkender oder höher</p>
   <p>Anfrage oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfiguration der Zugriffsebene</td> 
   <td> <p>Zugriff auf Anfragen bearbeiten</p> <p>Anzeigen des Zugriffs auf Aufgaben und Projekte</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Problem</p> <p>Anzeigen von Berechtigungen für die Aufgabe oder das Projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Issues</p> <p>View access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the issue</p> <p>View permissions on the task or project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Verknüpfung eines Problems mit einem Projekt, einer Aufgabe oder einem Problem aufheben

1. Navigieren Sie zu dem Problem, das mit einem Projekt, einer Aufgabe oder einem Problem verknüpft ist.
1. Klicken Sie auf **Abschnitt &quot;**&quot;.
1. Navigieren Sie zum **Überblick** des Abschnitts **Problemdetails**.
1. Entfernen **im Feld „Auflösbar**&quot; den Typ „Auflösbares Objekt“.\
   Ein Problem kann durch ein Projekt, eine Aufgabe oder ein Problem gelöst werden.

   Dadurch wird das anfragelösende Objekt entfernt.

1. Klicken Sie **Speichern** **Änderungen**.\
   Das Problem ist nicht mehr mit einem Projekt, einer Aufgabe oder einem Problem verknüpft, und Sie können das Problem jetzt unabhängig lösen.
