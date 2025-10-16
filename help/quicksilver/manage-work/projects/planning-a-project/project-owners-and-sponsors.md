---
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: Übersicht über Projektbesitzer und Sponsoren
description: Sie können einen Projektbesitzer und einen Projektsponsor für ein Projekt bestimmen.
author: Alina
feature: Work Management
exl-id: e3e8be3f-105f-4702-8c93-ae8092f5d5d3
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# Übersicht über Projektbesitzer und Sponsoren

<!-- Audited: 1/2024 -->

Sie können einen Projektbesitzer und einen Projektsponsor für ein Projekt bestimmen.

Der Projektbesitzer ist die Person, die für den termin- und budgetgerechten Abschluss des Projekts verantwortlich ist.

Der Projektsponsor ist ein wichtiger Stakeholder für das Projekt, der Ressourcen in das Projekt investiert hat. Der Abschluss des Projekts kommt in der Regel dem Projektsponsor zugute.

Informationen zum Aktualisieren des Projektbesitzers oder Sponsors für ein Projekt finden Sie unter [Aktualisieren von Projektbesitzern und Sponsoren](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md).

## Projektbesitzer

Sie können den Manager eines Projekts bestimmen, indem Sie einen Projektbesitzer für ein Projekt oder eine Vorlage angeben.

Sie können für ein Projekt nur einen Projektbesitzer definieren.

Das Feld Projektbesitzer ermöglicht Folgendes:

* Sie können nur einen Benutzer als Projektbesitzer festlegen.
* Sie können Projektbesitzer als genehmigende Stunden für das Projekt festlegen.
* Sie können den Projektbesitzer beim Definieren von Projekt-, Aufgaben- oder Problemgenehmigungsprozessen als generische genehmigende Person bestimmen. Weitere Informationen zu Genehmigungen finden Sie unter [Genehmigungsprozess bearbeiten](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

  >[!IMPORTANT]
  >
  >Wenn Sie dem Projektbesitzer eine Genehmigung zuweisen und niemand als Eigentümer eines Projekts bestimmt wird, wird die Genehmigung dem Workfront-Hauptadministrator neu zugewiesen, wie im Abschnitt „Kundeninformationen“ im Bereich „Setup“ angegeben. Weitere Informationen finden Sie [Konfigurieren der grundlegenden Informationen für Ihr System](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
  >


* Sie können bestimmte Benachrichtigungen aktivieren, die nur an den Projektbesitzer gesendet werden.

  Weitere Informationen zu E-Mail-Benachrichtigungen finden Sie im Abschnitt [Konfigurieren von Ereignisbenachrichtigungen für alle Personen im &#x200B;](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify)) im Artikel [Konfigurieren von Ereignisbenachrichtigungen für alle Personen im System](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* Sie können das Feld Projektbesitzer in einem Bericht oder einer Liste anzeigen.

  Sie können das Feld Projektbesitzer auch in einer Ansicht, Gruppierung oder Eingabeaufforderung anzeigen.

  Sie können beispielsweise den folgenden Textmodusausdruck in einen Filter kopieren, um Projekte anzuzeigen, die dem angemeldeten Benutzer gehören:

  ```
  ownerID=$$USER.ID
  ```

Weitere Informationen zum Erstellen von Berichten finden Sie im Artikel [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Owner of a project</h2>
<p>(NOTE: drafted and moved to its own article)</p>
<ol>
<li value="1">Go to the project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project Details area, then click <strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Owner</strong> field.</p> <p>Only active users can be specified as Project Owners.</p> </li>
<li value="5"> Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Projektsponsoren

Sie können jeden Benutzer im System als Projektsponsor bestimmen. Der Projektsponsor ist in der Regel ein Manager, eine Führungskraft oder ein Stakeholder, der wissen muss, was mit dem Projekt geschieht.

Beachten Sie beim Zuweisen eines Projektsponsors Folgendes:

* Der Projektsponsor erhält keinen zusätzlichen Zugriff auf das Projekt, wird aber zu den E-Mail-Benachrichtigungen des Projekts hinzugefügt. Weitere Informationen zu Benachrichtigungen finden Sie im Artikel [Konfigurieren von Ereignisbenachrichtigungen für alle Personen im System](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* Sie können nur einen Projektsponsor bestimmen.
* Sie können den Projektsponsor als generische genehmigende Person bestimmen, wenn Sie Genehmigungsprozesse für Projekte, Aufgaben oder Probleme definieren. Weitere Informationen zu Genehmigungen finden Sie unter [Genehmigungsprozess bearbeiten](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

  >[!IMPORTANT]
  >
  >Wenn Sie dem Projektsponsor eine Genehmigung zuweisen und niemand als Sponsor eines Projekts angegeben ist, wird die Genehmigung dem Projektbesitzer erneut zugewiesen. Wenn niemand als Eigentümer des Projekts festgelegt ist, wird die Genehmigung dem Workfront-Administrator zugewiesen.

* Sie können das Feld Projektsponsor in einem Bericht oder einer Liste anzeigen.

  Sie können das Feld Projektsponsor auch in einer Ansicht, Gruppierung oder Eingabeaufforderung anzeigen.

  Sie können beispielsweise den folgenden Textmodusausdruck in einen Filter kopieren, um Projekte anzuzeigen, die vom angemeldeten Benutzer gesponsert werden:

  ```
  sponsorID=$$USER.ID
  ```



  Weitere Informationen zum Erstellen von Berichten finden Sie im Artikel [Erstellen eines benutzerdefinierten Berichts](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Sponsor of a project </h2>
<p>(NOTE: drafted and moved to its own article) </p>
<ol>
<li value="1">Go to the Project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project Details area, then click <strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Sponsor</strong> field.</p> <p>Only active users can be specified as Project Sponsors.</p> </li>
<li value="5"> Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->
