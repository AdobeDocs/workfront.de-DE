---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aktualisierung der Zusagedaten zu Aufgaben und Problemen
description: Sie können das Übermittlungsdatum einer Aufgabe oder eines Problems, dem Sie zugewiesen sind, manuell aktualisieren. Weitere Informationen zu den Zusendedaten in Adobe Workfront finden Sie unter Übersicht über das Datum der Übermittlung .
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: 2def8297fe606adaeaef6cc079b718531377919d
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---


# Aktualisieren der Daten zum Bestätigen von Aufgaben und Problemen

<!--Audited: 07/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

Sie können das Übermittlungsdatum einer Aufgabe oder eines Problems, dem Sie zugewiesen sind, manuell aktualisieren. Weitere Informationen zu den Zusendedaten in Adobe Workfront finden Sie unter [Übersicht über das Veröffentlichungsdatum](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Zugriffsanforderungen

<!--Audited: 01/2024-->

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> 
   Neu:
   <ul>
   <li><p>Standard für Aufgaben</p> </li>
   <li><p>Beitragende oder höher für Probleme</p></li>
   </ul>
   Aktuell:
<ul>
   <li><p>Arbeit oder höher für Aufgaben</p></li> 
   <li><p>Anfrage oder höher für Probleme</p></li>
</ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben und Probleme bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für Aufgaben oder Probleme verwalten</p> </td> 
  </tr> 
 </tbody> 
</table>

* Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Bevor Sie das Übermittlungsdatum einer Aufgabe oder eines Problems bearbeiten können, müssen Sie der Aufgabe oder dem Problem zugewiesen sein, deren Übermittlungsdatum Sie aktualisieren müssen.

## Aktualisieren der Daten zum Bestätigen von Aufgaben und Problemen


In den folgenden Bereichen von Workfront können Sie das Übermittlungsdatum einer Aufgabe oder eines Problems aktualisieren:

* Der Bereich Details einer Aufgabe oder eines Problems
* Aufgaben- oder Problemkopfzeile

  Ihr Workfront- oder Gruppenadministrator muss der Aufgaben- oder Problemüberschrift Ihrer Layoutvorlage das Datum &quot;Bestätigen&quot;hinzufügen, um es auf der Aufgaben- oder Problemseite anzuzeigen.
Weitere Informationen finden Sie unter [Anpassen von Objektüberschriften mithilfe einer Layoutvorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

Die Aktualisierung des Veröffentlichungsdatums ist für Aufgaben und Probleme identisch.

>[!NOTE]
>
>Sie können Ihren System- oder Gruppenadministrator bitten, das Feld &quot;Commit Date&quot;zu Ihrem Zusammenfassungsbereich hinzuzufügen, um die Aktualisierung in verschiedenen Bereichen von Workfront zu vereinfachen.
>
>Weitere Informationen finden Sie in den folgenden Artikeln:
>
>* [Überblick über die Zusammenfassung](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Passen Sie den Zusammenfassungsbereich mithilfe einer Layoutvorlage an](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


1. Wechseln Sie zu einer Aufgabe oder einem Problem, der Sie als **Inhaber** zugewiesen sind.

   Weitere Informationen dazu, wer der Aufgabeneigentümer für ein Problem oder eine Aufgabe ist, finden Sie im Abschnitt [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) im Artikel [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. (Bedingt und optional) Wenn Ihr Workfront- oder Gruppenadministrator Ihrer Aufgaben- oder Problemüberschrift das Datum der Übermittlung hinzugefügt hat, klicken Sie in der Kopfzeile auf das Feld **Datum der Übermittlung** und wählen Sie dann ein Datum aus dem Kalender aus. Wenn sich das Datum des Versands nicht in der Kopfzeile befindet, fahren Sie mit den folgenden Schritten fort.

   ![](assets/commit-date-task-header.png)

1. Klicken Sie im linken Bereich auf **Aufgabendetails** oder **Problemdetails** .
1. Klicken Sie auf **Überblick** , um es zu erweitern.
1. Aktualisieren Sie das Feld **Datum für die Übermittlung**.

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. Klicken Sie auf **Änderungen speichern**.

   Nach dieser Änderung geschieht Folgendes:

   * Das Datum der Übermittlung und das geplante Abschlussdatum der Aufgabe bzw. des Problems sind nicht mehr dasselbe.

     Stattdessen werden das Bestätigungsdatum und das geplante Abschlussdatum der Aufgabe oder des Problems identisch.

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * Der Projekteigentümer wird in einer In-App-Benachrichtigung von Workfront darüber benachrichtigt, dass Sie ein neues Veröffentlichungsdatum für die Aufgabe oder das Problem vorgeschlagen haben.
   * Der Projekteigentümer wird im Abschnitt Updates darüber benachrichtigt, dass Sie ein neues Veröffentlichungsdatum vorgeschlagen haben. Zu diesem Zeitpunkt kann er das geplante Abschlussdatum der Aufgabe oder des Problems entsprechend dem von Ihnen vorgeschlagenen Zustimmungsdatum aktualisieren.

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)


     <!--![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)-->

     Informationen zu den Benachrichtigungen und Aktualisierungen, die durch diese Änderung ausgelöst werden, finden Sie im Abschnitt &quot;Benachrichtigungen und Aktualisierungen, die durch Änderung des Zustimmungsdatums ausgelöst werden&quot;im Artikel [Übersicht über das Veröffentlichungsdatum](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->