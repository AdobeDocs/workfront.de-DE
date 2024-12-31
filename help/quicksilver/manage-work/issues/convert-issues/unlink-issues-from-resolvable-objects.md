---
product-area: projects
navigation-topic: convert-issues
title: Aufheben der Verknüpfung von Problemen mit Lösungsobjekten
description: Wenn Sie ein Projekt oder eine Aufgabe erstellen, indem Sie ein Problem in das Projekt oder die Aufgabe konvertieren, haben Sie die Möglichkeit, das ursprüngliche Problem beizubehalten. Ihr Adobe Workfront-Administrator muss diese Voreinstellung aktivieren, damit Sie diese Option während der Konvertierung des Problems erhalten. Weitere Informationen zum Konvertieren von Problemen in Projekte und Aufgaben finden Sie unter Übersicht über das Konvertieren von Problemen in Adobe Workfront.
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Aufheben der Verknüpfung von Problemen mit Lösungsobjekten

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
   <td> <p>Anfrage oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene*</td> 
   <td> <p>Zugriff auf Anfragen bearbeiten</p> <p>Anzeigen des Zugriffs auf Aufgaben und Projekte</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Problem</p> <p>Anzeigen von Berechtigungen für die Aufgabe oder das Projekt</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Verknüpfung eines Problems mit einem Projekt, einer Aufgabe oder einem Problem aufheben

1. Navigieren Sie zu dem Problem, das mit einem Projekt, einer Aufgabe oder einem Problem verknüpft ist.
1. Klicken Sie auf **Abschnitt &quot;**&quot;.
1. Navigieren Sie zum **Überblick** des Abschnitts **Problemdetails**.
1. Entfernen **im Feld „Auflösbar**&quot; den Typ „Auflösbares Objekt“.\
   Ein Problem kann durch ein Projekt, eine Aufgabe oder ein Problem gelöst werden.

   Dadurch wird das anfragelösende Objekt entfernt.

1. Klicken Sie **Speichern** **Änderungen**.\
   Das Problem ist nicht mehr mit einem Projekt, einer Aufgabe oder einem Problem verknüpft, und Sie können das Problem jetzt unabhängig lösen.
