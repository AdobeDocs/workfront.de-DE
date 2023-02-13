---
content-type: overview
product-area: projects;user-management
navigation-topic: plan-a-project
title: Übersicht über Projekteigentümer und Projektsponsoren
description: Sie können einen Projektverantwortlichen und einen Projektsponsor für ein Projekt bestimmen.
author: Alina
feature: Work Management
exl-id: e3e8be3f-105f-4702-8c93-ae8092f5d5d3
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# Übersicht über Projekteigentümer und Projektsponsoren

Sie können einen Projektverantwortlichen und einen Projektsponsor für ein Projekt bestimmen.

Der Projektinhaber ist die Person, die für den fristgerechten und budgetären Abschluss des Projekts verantwortlich ist.

Der Projektsponsor ist ein wichtiger Akteur des Projekts, der über Ressourcen verfügt, die in das Projekt investiert wurden. Der Abschluss des Projekts kommt in der Regel dem Projektsponsor zugute.

Informationen dazu, wie Sie den Projekteigentümer oder -sponsor für ein Projekt aktualisieren, finden Sie unter [Projekteigentümer und -sponsoren aktualisieren](../../../manage-work/projects/planning-a-project/update-project-owners-and-sponsors.md).

## Projekteigentümer

Sie können den Projektmanager bestimmen, indem Sie einen Projekteigentümer für ein Projekt oder eine Vorlage angeben.

Sie können für ein Projekt nur einen Projekteigentümer definieren.

Im Feld Projekteigentümer können folgende Elemente verwendet werden:

* Sie können nur einen Benutzer als Projekteigentümer festlegen.
* Sie können Projekteigentümer als Stundenvalidierer für das Projekt festlegen.
* Sie können den Projekteigentümer beim Definieren von Projekt-, Aufgaben- oder Problemgenehmigungsprozessen als generischen Genehmiger festlegen. Informationen zu Genehmigungen finden Sie unter [Validierungsprozess bearbeiten](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

   >[!IMPORTANT]
   >
   >Wenn Sie dem Projekteigentümer eine Genehmigung zuweisen und niemand als Projekteigentümer bestimmt wird, wird die Genehmigung dem Workfront-Hauptadministrator neu zugewiesen, wie im Abschnitt Kundeninformationen im Bereich Einrichtung angegeben. Weitere Informationen finden Sie unter [Grundlegende Informationen für Ihr System konfigurieren](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).


* Sie können bestimmte Benachrichtigungen aktivieren, die nur an den Projekteigentümer gesendet werden.

   Weitere Informationen zu E-Mail-Benachrichtigungen finden Sie im Abschnitt . [Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md#modify) im Artikel [Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* Sie können das Feld &quot;Projektinhaber&quot;in einem Bericht oder einer Liste anzeigen.

   Sie können das Feld &quot;Projekteigentümer&quot;auch in einer Ansicht, Gruppierung oder Eingabeaufforderung anzeigen.

   Sie können beispielsweise den folgenden Textmodusausdruck in einen Filter kopieren, um Projekte anzuzeigen, die dem angemeldeten Benutzer gehören: 

   ```
   ownerID=$$USER.ID
   ```

Weitere Informationen zum Erstellen von Berichten finden Sie im Artikel [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Owner of a project</h2>
<p>(NOTE:&nbsp;drafted and moved to its own article)</p>
<ol>
<li value="1">Go to the project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Owner</strong> field.</p> <p>Only active users can be specified as Project Owners.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Projektsponsoren

Sie können jeden Benutzer im System als Projektsponsor bestimmen. Der Projektsponsor ist in der Regel ein Manager, Führungskraft oder Interessenträger, der wissen muss, was mit dem Projekt geschieht.

Beachten Sie bei der Zuweisung eines Projekt-Sponsors Folgendes:

* Der Projektsponsor erhält keinen zusätzlichen Zugriff auf das Projekt, wird aber zu den E-Mail-Benachrichtigungen des Projekts hinzugefügt. Informationen zu Benachrichtigungen finden Sie im Artikel [Ereignisbenachrichtigungen für alle Benutzer im System konfigurieren](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

* Sie können nur einen Projektsponsor bestimmen.
* Sie können den Projektsponsor als generischen Genehmiger festlegen, wenn Sie Projekt-, Aufgaben- oder Problemgenehmigungsprozesse definieren. Informationen zu Genehmigungen finden Sie unter [Validierungsprozess bearbeiten](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/edit-an-approval-process.md).

   >[!IMPORTANT]
   >
   >Wenn Sie dem Projektsponsor eine Genehmigung zuweisen und niemand als Sponsor eines Projekts benannt ist, wird die Genehmigung dem Projekteigentümer neu zugewiesen. Wenn niemand als Eigentümer des Projekts benannt ist, wird die Genehmigung dem Workfront-Administrator zugewiesen.

* Sie können das Feld Projektsponsor in einem Bericht oder einer Liste anzeigen.

   Sie können auch das Feld Projektsponsor in einer Ansicht, Gruppierung oder Eingabeaufforderung anzeigen.

   Sie können beispielsweise den folgenden Textmodusausdruck in einen Filter kopieren, um Projekte anzuzeigen, die vom angemeldeten Benutzer gesponsert wurden:

   ```
   sponsorID=$$USER.ID
   ```

    

   Weitere Informationen zum Erstellen von Berichten finden Sie im Artikel [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Update the Project Sponsor of a project </h2>
<p>(NOTE: drafted and moved to its own article) </p>
<ol>
<li value="1">Go to the Project you want to update.</li>
<li value="2"> Click <strong>Project Details</strong> in the left panel. </li>
<li value="3"> Click&nbsp;the <strong>Edit</strong> icon <img src="assets/qs-edit-icon.png"> in the upper-right corner of the Project&nbsp;Details area, then click&nbsp;<strong>Overview</strong>.  </li>
<li value="4"> <p>Specify the name of a user for the <strong>Project Sponsor</strong> field.</p> <p>Only active users can be specified as Project Sponsors.</p> </li>
<li value="5"> Click&nbsp;<strong>Save Changes</strong>. </li>
</ol>
</div>
-->
