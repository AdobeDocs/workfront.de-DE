---
product-area: projects
navigation-topic: create-projects
title: Erstellen von Projekt-Baselines
description: Eine Baseline ist eine Projekt-Momentaufnahme, die wichtige Informationen darstellt, die im ursprünglichen Projektplan oder zu einem bestimmten Zeitpunkt während der Laufzeit des Projekts enthalten sind.
author: Alina
feature: Work Management
exl-id: 422bd7a5-d7a0-4c24-8624-bd0fe6e79d7b
source-git-commit: 49bd393af77a67aa1e3a443c4189569178e99ada
workflow-type: tm+mt
source-wordcount: '757'
ht-degree: 0%

---

# Erstellen von Projekt-Baselines

<!-- Audited: 12/2023 -->

Eine Baseline ist eine Projekt-Momentaufnahme, die wichtige Informationen darstellt, die im ursprünglichen Projektplan oder zu einem bestimmten Zeitpunkt während der Laufzeit des Projekts enthalten sind.

Sie können Baseline verwenden, um diese Informationen aus dem aktuellen Plan mit dem ursprünglichen Plan oder einem anderen Zeitpunkt zu vergleichen, um Problemaufgaben, Umfangsänderung und andere Trends im Zeitverlauf zu identifizieren.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<!--
drafted for P&P:

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
   <td> <p>Current license: Standard </p> 
   Or
   <p>Legacy license: Plan </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher to view baselines</p> <p>Manage permissions to the project to create baselines</p> <p> For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

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
    <td><p>Neu: Standard</p>
        <p>oder</p>
        <p>Aktuell: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Zugriffsebene</td> 
   <td> <p>Zugriff auf Projekte bearbeiten</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von Berechtigungen für das Projekt oder höher zum Anzeigen von Baselines</p> <p>Verwalten von Berechtigungen für das Projekt, um Baselines zu erstellen</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zum Arbeiten mit Baselines

* Sie können mehrmals während der Lebensdauer des Projekts einen Schnappschuss des Fortschritts in einem Projekt erfassen und so mehrere Baselines erstellen.
* Sie können die in den Baselines eines Projekts enthaltenen Informationen anzeigen, indem Sie einen Baseline-Bericht erstellen oder einen Baseline-Bericht erstellen.
* Wenn Sie eine Baseline erstellen, werden die Aufgabeninformationen auch in den Baseline-Aufgaben dieser Baseline erfasst.
* Sie können die Informationen zu den grundlegenden Aufgaben anzeigen, indem Sie einen Bericht zu den grundlegenden Aufgaben erstellen.

>[!IMPORTANT]
>
>Eine Baseline erstellt eine Momentaufnahme des Namens, der Daten und der Finanzinformationen des Projekts. Die Baseline enthält nicht die Werte von benutzerdefinierten Feldern im Projekt. Informationen zu den in der Baseline enthaltenen Finanzinformationen finden Sie unter [Projektfinanzen in Projektbaselines enthalten](../../../manage-work/projects/project-finances/project-finances-included-in-project-baselines.md).

## Erstellen einer Baseline

Sie können eine Baseline wie folgt erstellen:

* **Automatisch**: Ihr Workfront-Administrator oder ein Gruppenadministrator legt die Projektvoreinstellung für Workfront fest, damit automatisch eine Grundlinie erstellt wird, wenn ein Projekt „Aktuell“ wird. Wenn diese Einstellung aktiviert ist, wird eine Baseline erstellt, sobald der Projektstatus „Aktuell“ wird. Wenn diese Einstellung nicht aktiviert ist, müssen Sie Baselines manuell erstellen.

  Weitere Informationen zum Konfigurieren der Projektvoreinstellungen und zum Einrichten der automatischen Basiserstellung finden Sie unter [Konfigurieren von systemweiten Projektvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

  >[!CAUTION]
  >
  >Durch Aktivierung dieser Einstellung wird automatisch eine Baseline für ein Projekt erstellt, sobald der Status eines Projekts in „Aktuell“ geändert wird. Die erste erstellte Baseline ist die Standardbasislinie. Alle anderen Baselines müssen während der Laufzeit des Projekts manuell erstellt werden .

* **Manuell**: Sie können bei Bedarf neue Baselines für das Projekt erstellen, wenn das Projekt fortgesetzt wird. Sie können dann Baselines vergleichen, um den Fortschritt des Projekts im Zeitverlauf zu sehen.

So erstellen Sie eine Grundlinie:

1. Gehe zu einem Projekt.
1. Klicken Sie im linken Bedienfeld auf **Baselines**.

   Oder

   Klicken Sie **Weitere anzeigen** und dann auf **Baselines**.

   ![Baselines-Abschnitt im Projekt](assets/baselines-section-on-project-with-header.png)

1. Klicken Sie auf **Neue Baseline.**
1. Geben Sie den Namen für die Baseline an.
1. (Optional) Wenn dies die erste Baseline ist, können Sie sie als Standard auswählen.
1. Klicken Sie auf **Speichern**.

   Standardmäßig werden die folgenden Informationen zur von Ihnen erstellten Baseline angezeigt:

   * Name der Baseline
   * Geplantes Eingabedatum
   * Geplantes Startdatum des Projekts zum Zeitpunkt der Erstellung der Baseline
   * Voraussichtliches Startdatum des Projekts zum Zeitpunkt der Erstellung der Baseline
   * Tatsächliche Dauer des Projekts, als die Baseline erstellt wurde
   * % Abgeschlossen des Projekts, als die Baseline erstellt wurde
   * Standardmäßiger Indikator für Baseline, der anzeigt, ob eine Baseline die standardmäßige Baseline des Projekts ist

     >[!TIP]
     >
     >Es ist nicht möglich, Informationen von zwei Baselines gleichzeitig in derselben Ansicht oder in demselben Bericht anzuzeigen. Sie können nur Informationen von einer bestimmten Baseline und der Standard-Baseline im selben Bericht anzeigen. Sie können die Baseline, die Sie als Standard-Baseline betrachten, jederzeit während der Laufzeit des Projekts ändern.

1. (Optional) Klicken Sie auf die **Ansicht**, erstellen Sie dann eine neue Ansicht oder bearbeiten Sie die aktuelle Ansicht, um Felder zur Ansicht hinzuzufügen und zusätzliche Informationen zwischen Basislinien zu vergleichen. Weitere Informationen finden Sie unter [Erstellen oder Bearbeiten von Ansichten in Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

## Erstellen eines Baseline- oder eines Baseline-Aufgabenberichts

Um Baseline-Informationen anzuzeigen, können Sie auch einen Baseline- oder Baseline-Aufgabenbericht erstellen. Auf diese Weise können Sie eine beliebige Anzahl von Feldern zu den Baselines oder Baseline-Aufgaben anzeigen, um sie in einer Ansicht zu vergleichen.

>[!TIP]
>
>Sie müssen eine Baseline erstellen, bevor Sie einen Baseline- oder Baseline-Aufgabenbericht erstellen können.

Informationen zum Erstellen eines Berichts finden Sie unter [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Es wird empfohlen, dem Baseline- oder Baseline-Aufgabenbericht eine Gruppierung „Projektname“ hinzuzufügen, um die Lesbarkeit zu vereinfachen.

Informationen zum Erstellen einer Gruppierung finden Sie unter [Gruppierungen in Adobe Workfront erstellen](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md).
