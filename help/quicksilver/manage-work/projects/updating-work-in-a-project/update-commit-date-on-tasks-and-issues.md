---
product-area: projects
navigation-topic: update-work-in-a-project
title: Aktualisieren der Daten zum Bestätigen von Aufgaben und Problemen
description: Sie können das Übermittlungsdatum einer Aufgabe oder eines Problems, dem Sie zugewiesen sind, manuell aktualisieren. Weitere Informationen zu den Zusendedaten in Adobe Workfront finden Sie unter Übersicht über das Datum der Übermittlung .
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: ac5e56a2881d589c9a737d5e7115d82ee5c11ea6
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---


# Aktualisieren der Daten zum Bestätigen von Aufgaben und Problemen

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau-Umgebung für alle Kunden oder in der Produktionsumgebung für Kunden verfügbar, die schnelle Versionen aktiviert haben.</span>

<span class="preview">Informationen zu schnellen Versionen finden Sie unter [Schnellversionen für Ihr Unternehmen aktivieren oder deaktivieren](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)</span>.

<span class="preview">Weitere Informationen zur aktuellen Version finden Sie unter [Übersicht über die Version 2024 im dritten Quartal 2024](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

Sie können das Übermittlungsdatum einer Aufgabe oder eines Problems, dem Sie zugewiesen sind, manuell aktualisieren. Weitere Informationen zu den Zusendedaten in Adobe Workfront finden Sie unter [Übersicht über das Veröffentlichungsdatum](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md).

## Zugriffsanforderungen

<!--Audited: 01/2024-->

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

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
   Für die neuen Lizenzen:
   <ul>
   <li><p>Standard für Aufgaben</p> </li>
   <li><p>Beitragende oder höher für Probleme</p></li>
   </ul>
   Für aktuelle Lizenzen:
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

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben. Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Voraussetzungen

Bevor Sie das Übermittlungsdatum einer Aufgabe oder eines Problems bearbeiten können, müssen Sie der Aufgabe oder dem Problem zugewiesen sein, deren Übermittlungsdatum Sie aktualisieren müssen.

## Aktualisieren der Daten zum Bestätigen von Aufgaben und Problemen


In den folgenden Bereichen von Workfront können Sie das Übermittlungsdatum einer Aufgabe oder eines Problems aktualisieren:

* Der Bereich Details einer Aufgabe oder eines Problems
* <span class="preview">Die Aufgaben- oder Problemkopfzeile</span>

  <span class="preview">Ihr Workfront- oder Gruppenadministrator muss der Aufgaben- oder Problemüberschrift Ihrer Layoutvorlage das &quot;Datum festlegen&quot;hinzufügen, um es auf der Aufgaben- oder Problemseite anzuzeigen.
Weitere Informationen finden Sie unter [Anpassen von Objektüberschriften mithilfe einer Layoutvorlage](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).</span>

Die Aktualisierung des Veröffentlichungsdatums ist für Aufgaben und Probleme identisch.

>[!NOTE]
>
>Sie können Ihren System- oder Gruppenadministrator bitten, das Feld &quot;Commit Date&quot;zu Ihrem Zusammenfassungsbereich hinzuzufügen, um die Aktualisierung in verschiedenen Bereichen von Workfront zu vereinfachen.
>
>Weitere Informationen finden Sie in den folgenden Artikeln:
>
>* [Überblick über die Zusammenfassung](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [Passen Sie die Startseite und die Zusammenfassung mit einer Layoutvorlage an](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).


1. Wechseln Sie zu einer Aufgabe oder einem Problem, der Sie als **Inhaber** zugewiesen sind.

   Weitere Informationen dazu, wer der Aufgabeneigentümer für ein Problem oder eine Aufgabe ist, finden Sie im Abschnitt [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments) im Artikel [Aufgaben bearbeiten](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

1. <span class="preview">(Bedingt und optional) Wenn Ihr Workfront- oder Gruppenadministrator das Datum für die Übermittlung zu Ihrer Aufgaben- oder Problemüberschrift hinzugefügt hat, klicken Sie in der Kopfzeile auf das Feld **Veröffentlichungsdatum** und wählen Sie dann ein Datum aus dem Kalender aus. Wenn sich das Datum des Versands nicht in der Kopfzeile befindet, fahren Sie mit den folgenden Schritten fort. </span>

   <span class="preview">![](assets/commit-date-task-header.png)</span>

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