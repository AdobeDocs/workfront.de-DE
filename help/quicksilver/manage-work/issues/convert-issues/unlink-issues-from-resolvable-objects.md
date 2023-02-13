---
product-area: projects
navigation-topic: convert-issues
title: Aufheben der Verknüpfung von Problemen mit den aufgelösten Objekten
description: Wenn Sie ein Projekt oder eine Aufgabe erstellen, indem Sie ein Problem in das Projekt oder die Aufgabe konvertieren, haben Sie die Möglichkeit, das ursprüngliche Problem beizubehalten. Ihr Adobe Workfront-Administrator muss diese Voreinstellung aktivieren, damit Sie diese Option während der Konvertierung des Problems nutzen können. Weitere Informationen zum Konvertieren von Problemen in Projekte und Aufgaben finden Sie unter Übersicht über Konvertierungsprobleme in Adobe Workfront.
author: Alina
feature: Work Management
exl-id: c18160e5-9f95-4575-a1b3-b4f7e5334844
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 0%

---

# Aufheben der Verknüpfung von Problemen mit den aufgelösten Objekten

Wenn Sie ein Projekt oder eine Aufgabe erstellen, indem Sie ein Problem in das Projekt oder die Aufgabe konvertieren, haben Sie die Möglichkeit, das ursprüngliche Problem beizubehalten. Ihr Adobe Workfront-Administrator muss diese Voreinstellung aktivieren, damit Sie diese Option während der Konvertierung des Problems nutzen können.\
Weitere Informationen zum Konvertieren von Problemen in Projekte und Aufgaben finden Sie unter [Übersicht über Konvertierungsprobleme in Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Wenn Sie sich dafür entscheiden, das in das Projekt oder die Aufgabe konvertierte Problem beizubehalten, ist die Lösung des Problems an das Projekt oder die Aufgabe gebunden. Das Problem wird zum auflösbaren Objekt des Projekts oder der Aufgabe. Das Projekt oder die Aufgabe sind die Auflösungsobjekte des Problems.

Sie können ein Problem auch manuell mit einem anderen Problem verknüpfen. Das zweite Problem wird in diesem Fall zum Auflösungsobjekt für das erste Problem.\
Weitere Informationen zum Auflösen von Objekten finden Sie unter [Übersicht über das Auflösen und Auflösen von Objekten](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

>[!TIP]
>
>Der Problemstatus kann nicht geändert werden, da er sich automatisch mit dem Status des aufgelösten Objekts ändert.

Sie können die Verknüpfung zwischen der Lösung eines Problems und dem eines Projekts, einer Aufgabe oder eines Problems aufheben, indem Sie das Projekt, die Aufgabe oder das Problem aus dem Problem entfernen.

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
   <td> <p>Anforderung oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene*</td> 
   <td> <p>Zugriff auf Probleme bearbeiten</p> <p>Zugriff auf Aufgaben und Projekte anzeigen</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen zum Problem verwalten</p> <p>Berechtigungen für die Aufgabe oder das Projekt anzeigen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Aufheben der Verknüpfung eines Problems mit einem Projekt, einer Aufgabe oder einem Problem

1. Gehen Sie zu dem Problem, das mit einem Projekt, einer Aufgabe oder einem Problem verknüpft ist.
1. Klicken Sie auf **Problemdetails** Abschnitt.
1. Navigieren Sie zu **Übersicht** der **Problemdetails** Abschnitt.
1. Im **Gelöst von** -Feld den auflösbaren Objekttyp entfernen.\
   Ein Problem kann durch ein Projekt, eine Aufgabe oder ein Problem behoben werden.

   Dadurch wird das aufgelöste Objekt aus dem Problem entfernt.

1. Klicken **Speichern** **Änderungen**.\
   Das Problem ist nicht mehr mit einem Projekt, einer Aufgabe oder einem Problem verknüpft und Sie können das Problem jetzt unabhängig voneinander lösen.
