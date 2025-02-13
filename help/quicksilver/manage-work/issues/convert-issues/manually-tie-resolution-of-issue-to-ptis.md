---
product-area: projects
navigation-topic: convert-issues
title: Die Lösung eines Problems manuell mit anderen Problemen, Aufgaben oder Projekten verknüpfen
description: Sie können die Lösung eines Problems manuell mit der Lösung eines Projekts, einer Aufgabe oder eines Problems verknüpfen, ohne das Problem zu konvertieren. Das Problem wird zu einem der lösbaren Objekte des ausgewählten Projekts, der ausgewählten Aufgabe oder des ausgewählten Problems. Dabei ändert sich durch eine Statusänderung des Projekts, der Aufgabe oder des Problems der Trigger des ursprünglichen Problems.
author: Alina
feature: Work Management
exl-id: f57f67cb-60b3-4a95-9963-fa339e542551
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

# Die Lösung eines Problems manuell mit anderen Problemen, Aufgaben oder Projekten verknüpfen

Sie können die Lösung eines Problems manuell mit der Lösung eines Projekts, einer Aufgabe oder eines Problems verknüpfen, ohne das Problem zu konvertieren. Das Problem wird zu einem der lösbaren Objekte des ausgewählten Projekts, der ausgewählten Aufgabe oder des ausgewählten Problems. Dabei ändert sich durch eine Statusänderung des Projekts, der Aufgabe oder des Problems der Trigger des ursprünglichen Problems.

>[!TIP]
>
>Wenn Sie die Lösung eines Problems mit der Lösung eines anderen Objekts verknüpfen, können Sie den Status des ursprünglichen Problems nicht mehr manuell bearbeiten.

Weitere Informationen zum Auflösen und Auflösen von Objekten finden Sie unter [Übersicht über das Auflösen und Auflösen von Objekten](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Anfrage oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Probleme, Aufgaben und Projekte bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten Sie Berechtigungen für das Problem, das Sie mit einem anderen Problem, einer anderen Aufgabe oder einem anderen Projekt verknüpfen</p> <p>Zeigen Sie Berechtigungen für das Problem, die Aufgabe oder das Projekt, das Sie dem vorhandenen Problem hinzufügen, an oder erhöhen Sie diese</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie Folgendes tun:

* Problem haben, dessen Lösung mit der Lösung eines anderen Problems, einer anderen Aufgabe oder eines anderen Projekts verknüpft werden soll

* Ein zusätzliches Problem, eine zusätzliche Aufgabe oder ein zusätzliches Projekt haben

## Binden Sie die Lösung eines Problems an die Lösung eines anderen Problems, einer anderen Aufgabe oder eines anderen Projekts

1. Navigieren Sie zu einem Problem, dessen Lösung Sie mit der Lösung eines anderen Problems oder mit der Lösung einer Aufgabe oder eines Projekts verknüpfen möchten.
1. Klicken Sie im linken Bereich auf **Problemdetails** und erweitern Sie dann den Bereich **Übersicht**.

   ![Symbol „Problemdetails“](assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png)

1. Klicken Sie auf **Feld** Aufgelöst von“ und wählen Sie aus den folgenden Typen von aufzulösenden Objekten:

   * **Projekt**
   * **Aufgabe**
   * **Probleme**

   Je nach ausgewähltem Objekt werden die folgenden Felder angezeigt:

   * **Projekt wird aufgelöst**
   * **Aufgabe wird gelöst**
   * **Problem wird gelöst**

1. Geben Sie den Namen eines bestimmten Projekts, einer bestimmten Aufgabe oder eines bestimmten Problems in das Feld **Projekt wird gelöst**, **Aufgabe** oder **Problem** ein und klicken Sie dann auf den Namen, wenn er in der Liste angezeigt wird.

   >[!NOTE]
   >
   >Sie können die Lösung eines Problems nicht mit der Aufgabe oder dem Projekt verknüpfen, in dem sich das Problem befindet. Die Aufgabe oder das Projekt des Problems wird nicht in den Feldern zur Lösungsaufgabe oder zur Lösungsaufgabe angezeigt.


1. Klicken Sie auf **Änderungen speichern**.

   Das ursprüngliche Problem wird zum lösbaren Objekt für das Projekt, die Aufgabe oder das Problem, das bzw. das Sie in Schritt 4 und 5 ausgewählt haben. Das bedeutet, dass das ursprüngliche Problem abgeschlossen ist, wenn das Lösungsobjekt (das Projekt, die Aufgabe oder das Problem, mit dem bzw. der Sie es verknüpft haben) abgeschlossen ist.

   >[!NOTE]
   >
   >Ein Projekt, eine Aufgabe oder ein Problem kann mehrere Probleme als lösbare Objekte haben.
