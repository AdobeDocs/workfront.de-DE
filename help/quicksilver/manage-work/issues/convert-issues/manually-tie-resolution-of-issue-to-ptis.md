---
product-area: projects
navigation-topic: convert-issues
title: Manuelles Verbinden der Lösung eines Problems mit anderen Problemen, Aufgaben oder Projekten
description: Sie können die Lösung eines Problems manuell mit der Lösung eines Projekts, einer Aufgabe oder eines Problems verknüpfen, ohne das Problem zu konvertieren. Das Problem wird zu einem der auflösbaren Objekte des ausgewählten Projekts, der Aufgabe oder des Problems. Wenn Sie dies tun, wird durch eine Änderung des Projektstatus, der Aufgabe oder eine Ausgabe eine Änderung des Status des ursprünglichen Problems Trigger.
author: Alina
feature: Work Management
exl-id: f57f67cb-60b3-4a95-9963-fa339e542551
source-git-commit: ea430157da539507c11a559a4dce6b24aca9e5a6
workflow-type: tm+mt
source-wordcount: '553'
ht-degree: 1%

---

# Manuelles Verbinden der Lösung eines Problems mit anderen Problemen, Aufgaben oder Projekten

Sie können die Lösung eines Problems manuell mit der Lösung eines Projekts, einer Aufgabe oder eines Problems verknüpfen, ohne das Problem zu konvertieren. Das Problem wird zu einem der auflösbaren Objekte des ausgewählten Projekts, der Aufgabe oder des Problems. Wenn Sie dies tun, wird durch eine Änderung des Projektstatus, der Aufgabe oder eine Ausgabe eine Änderung des Status des ursprünglichen Problems Trigger.

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
   <td> <p>Anforderung oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Probleme, Aufgaben, Projekte bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten von Berechtigungen für das Problem, das Sie mit einem anderen Problem, einer anderen Aufgabe oder einem anderen Projekt verknüpfen</p> <p>Anzeigen oder höherer Berechtigungen für das Problem, die Aufgabe oder das Projekt, das/das Sie zum bestehenden Problem hinzufügen</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Bevor Sie beginnen, müssen Sie:

* Sie haben ein Problem, dessen Lösung Sie mit der Lösung eines anderen Problems, einer anderen Aufgabe oder eines anderen Projekts verknüpfen möchten.

* Zusätzliche Probleme, Aufgaben oder Projekte haben

## Verknüpfen der Lösung eines Problems mit der Lösung eines anderen Problems, einer anderen Aufgabe oder eines anderen Projekts

1. Navigieren Sie zu einem Problem, dessen Lösung Sie mit der Lösung eines anderen Problems, einer Aufgabe oder eines Projekts verknüpfen möchten.
1. Klicken Sie auf **Problemdetails** > **Übersicht** Bereich.

   ![](assets/qs-issue-details-icon-expanded-with-overview-section-350x462.png)

1. Navigieren Sie zu **Übersicht** -Gebiet **Problemdetails** Abschnitt.
1. Klicken Sie auf **Gelöst von** und wählen Sie aus den folgenden Arten auflösender Objekte aus:

   * **Projekt**
   * **Aufgabe**
   * **Probleme**

   Je nach ausgewähltem Objekt werden die folgenden Felder angezeigt:

   * **Projekt wird gelöst**
   * **Aufgabe wird gelöst**
   * **Problem wird gelöst**


1. Beginnen Sie mit der Eingabe des Namens eines bestimmten Projekts, einer bestimmten Aufgabe oder eines bestimmten Problems im **Auflösen des Projekts**, **Aufgabe** oder **Problem** und klicken Sie dann auf das Feld, wenn es in der Liste angezeigt wird.

   >[!NOTE]
   >
   >Sie können die Lösung eines Problems nicht mit der Aufgabe oder dem Projekt verknüpfen, in dem sich das Problem befindet. Die Aufgabe oder das Projekt des Problems werden nicht in den Feldern &quot;Aufgabe auflösen&quot;oder &quot;Aufgabe auflösen&quot;angezeigt.


1. Klicken **Änderungen speichern**.

   Das ursprüngliche Problem wird zum auflösbaren Objekt für das Projekt, die Aufgabe oder das Problem, das/das Sie in den Schritten 4 und 5 ausgewählt haben. Das bedeutet, dass das ursprüngliche Problem behoben wird, wenn das aufgelöste Objekt (das Projekt, die Aufgabe oder das Problem, mit dem Sie es verknüpft haben) abgeschlossen ist.

   >[!NOTE]
   >
   >Ein Projekt, eine Aufgabe oder ein Problem kann mehrere Probleme als auflösbare Objekte haben.
