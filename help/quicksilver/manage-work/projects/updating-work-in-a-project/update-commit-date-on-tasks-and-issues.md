---
product-area: projects
navigation-topic: update-work-in-a-project
title: Commit-Daten für Aufgaben und Probleme aktualisieren
description: Sie können das Commit-Datum einer Aufgabe oder eines Problems, der bzw. dem Sie zugewiesen sind, manuell aktualisieren. Weitere Informationen zu Commit-Datumsangaben in Adobe Workfront finden Sie unter Übersicht über das Commit-Datum .
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 170edee352f1219986057dbb7d77228f84d855b1
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---


# Aktualisieren von Commit-Terminen für Aufgaben und Probleme

<!--Audited: 07/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

Sie können das Commit-Datum einer Aufgabe oder eines Problems, der bzw. dem Sie zugewiesen sind, manuell aktualisieren. Weitere Informationen zu Commit-Daten in Adobe Workfront finden Sie unter [Übersicht über Commit-Datum](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Zugriffsanforderungen

<!--Audited: 01/2024-->

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
   Neu:
   <ul>
   <li><p>Standard für Aufgaben</p> </li>
   <li><p>Mitwirkender oder höher für Probleme</p></li>
   </ul>
   Aktuell:
<ul>
   <li><p>Arbeit oder höher für Aufgaben</p></li> 
   <li><p>Anfrage oder höher für Probleme</p></li>
</ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Probleme bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für die Aufgabe oder das Problem verwalten</p>
   <p> Sie müssen der Aufgabe oder dem Problem zugewiesen sein, um das Commit-Datum zu aktualisieren </p>
    </td> 
  </tr> 
 </tbody> 
</table>

* Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie das Commit-Datum einer Aufgabe oder eines Problems bearbeiten können, müssen Sie der Aufgabe oder dem Problem zugewiesen sein, deren Commit-Datum Sie aktualisieren müssen.

## Aktualisieren von Commit-Terminen für Aufgaben und Probleme


Sie können das Commit-Datum einer Aufgabe oder eines Problems in den folgenden Bereichen von Workfront aktualisieren:

* Der Abschnitt Details einer Aufgabe oder eines Problems
* Die Kopfzeile der Aufgabe oder des Problems

  Ihr Workfront- oder Gruppen-Administrator muss das Commit-Datum zur Aufgaben- oder Problem-Kopfzeile Ihrer Layout-Vorlage hinzufügen, um es auf der Aufgaben- oder Problem-Seite anzuzeigen.
Weitere Informationen finden Sie unter [Anpassen von Objektkopfzeilen mithilfe einer Layout-Vorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

Die Aktualisierung des Commit-Datums ist für Aufgaben und Probleme identisch.

>[!NOTE]
>
>Sie können Ihren System- oder Gruppenadministrator bitten, das Feld Übertragungsdatum zu Ihrem Zusammenfassungsbereich hinzuzufügen, um die Aktualisierung in verschiedenen Bereichen von Workfront zu vereinfachen.
>
>Weitere Informationen finden Sie in den folgenden Artikeln:
>
>* [Übersicht](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Passen Sie das Bedienfeld Zusammenfassung mithilfe einer Layout-Vorlage ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


1. Navigieren Sie zu einer Aufgabe oder einem Problem, der bzw. dem Sie als &quot;**&quot; zugewiesen**.

   Weitere Informationen dazu, wer der Aufgabenbesitzer für ein Problem oder eine Aufgabe ist, finden Sie im Abschnitt [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) im Artikel [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. (Bedingt und optional) Wenn der Workfront- oder Gruppen-Administrator bzw. die Gruppenadministratorin das Commit-Datum zu Ihrer Aufgaben- oder Problem-Kopfzeile hinzugefügt hat, klicken Sie auf das Feld **Commit-Datum** in der Kopfzeile und wählen Sie dann ein Datum aus dem Kalender aus. Wenn das Commit-Datum nicht in der Kopfzeile enthalten ist, fahren Sie mit den folgenden Schritten fort.

   ![](assets/commit-date-task-header.png)

1. Klicken Sie **linken Bedienfeld auf** Aufgabendetails **oder** Problemdetails“.
1. Klicken Sie auf **Übersicht**, um sie zu erweitern.
1. Aktualisieren Sie das Feld **Commit-**).

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. Klicken Sie auf **Änderungen speichern**.

   Nach dieser Änderung geschieht Folgendes:

   * Das Commit-Datum und das geplante Abschlussdatum der Aufgabe oder Anfrage sind nicht mehr identisch.

     Stattdessen werden das Commit-Datum und das voraussichtliche Abschlussdatum der Aufgabe oder des Problems identisch.

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * Der Projektbesitzer wird in einer Workfront-In-App-Benachrichtigung darüber benachrichtigt, dass Sie ein neues Commit-Datum für die Aufgabe oder das Problem vorgeschlagen haben.
   * Der Projektbesitzer wird im Abschnitt Aktualisierungen darüber informiert, dass Sie ein neues Commit-Datum vorgeschlagen haben. Er kann zu diesem Zeitpunkt das geplante Abschlussdatum der Aufgabe oder Anfrage aktualisieren, sodass es dem von Ihnen vorgeschlagenen Commit-Datum entspricht.

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)


     <!--![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)-->

     Informationen zu den Benachrichtigungen und Aktualisierungen, die durch diese Änderung ausgelöst werden, finden Sie im Abschnitt „Benachrichtigungen und Aktualisierungen, die durch die Änderung des Commit-Datums ausgelöst werden“ im Artikel [Übersicht über das Commit-Datum](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->