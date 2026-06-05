---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Anzeigen der tatsächlichen Stunden
description: Die Stunden, die Sie bei Ihren Arbeitselementen in Adobe Workfront anmelden, werden als Tatsächliche Stunden betrachtet. Tatsächliche Stunden stellen die tatsächliche Zeit dar, die zum Abschließen einer Aufgabe, eines Problems oder eines Projekts benötigt wurde.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/iOGP-byuQ0X7Sd-DhKYw7aHJe3Q8n2blSj-rrlnfK9k
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: d1573eb8-a2e8-4a06-9526-9c3410bf4914id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 5606ecce47d871bfaaa7d0c7e305651e6eb9c15b
workflow-type: tm+mt
source-wordcount: 1377
ht-degree: 3%

---

# Anzeigen der tatsächlichen Stunden

<!-- Audited: 5/2025 -->

Die Stunden, die Sie bei Ihren Arbeitselementen in Adobe Workfront anmelden, werden als Tatsächliche Stunden betrachtet.

Tatsächliche Stunden stellen die tatsächliche Zeit dar, die zum Abschließen einer Aufgabe, eines Problems oder eines Projekts benötigt wurde.

Es wird empfohlen, Stunden in Arbeitselementen zu protokollieren, bei denen es sich um Aufgaben und Probleme handelt. Als Workfront-Admin können Sie jedoch Benutzenden erlauben, Zeit in Projekten auch in Abhängigkeit von den Workflows Ihres Unternehmens zu protokollieren.

Weitere Informationen dazu, wie Sie Ihr System so einrichten, dass Benutzer Zeit in Projekten protokollieren können, finden Sie unter [Konfigurieren von Arbeitszeittabellen und Stundenvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Standard<p>
   <p>Work oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben, Projekte oder Probleme anzeigen oder erhöhen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Erweitern von Berechtigungen für eine Aufgabe, ein Projekt oder ein Problem</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
 Old:
 
 <table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   <p>New: Standard<p>
   <p>Or</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to Tasks, Projects, or Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a task, a project, or an issue</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Tatsächliche Stunden im Vergleich zu veralteten tatsächlichen Stunden

Je nachdem, aus welchem Bereich von Workfront Sie auf die tatsächlichen Stunden zugreifen, können diese auf eine der folgenden protokollierten Stunden verweisen:

* In Projekt-, Aufgaben- und Problemberichten und -listen:

   * **Tatsächliche Stunden**: Stunden, die zwischen Mai 2021 und heute für Projekte, Aufgaben oder Probleme protokolliert wurden. Sie werden in Stunden in der Workfront-Datenbank gespeichert und ihr Wertefeld wird `actualWorkRequiredDouble`.
   * **Legacy Actual Hours**: Stunden, die für Projekte, Aufgaben oder Probleme jederzeit zwischen einem Datum vor Mai 2021 und dem heutigen Tag protokolliert werden. Sie werden als Minuten in der Workfront-Datenbank gespeichert und ihr Wertefeld wird `actualWorkRequired`.

     Die aktuell protokollierten Stunden aktualisieren sowohl die tatsächlichen als auch die veralteten tatsächlichen Stunden.

     >[!IMPORTANT]
     >
     >Die Ist-Kosten des Projekts berechnen mithilfe von Legacy-Ist-Stunden.

* Im Bereich Projekt-, Aufgaben- oder Problemdetails können tatsächliche Stunden in den folgenden Feldern angezeigt werden:

   * **Tatsächliche Stunden**: Auf der Registerkarte „Details“ werden diese Stunden für Projekte, Aufgaben oder Probleme zwischen Mai 2021 und heute protokolliert. Sie werden in Stunden in der Workfront-Datenbank gespeichert und ihr Wertefeld wird `actualWorkRequiredDouble`.
   * **Tatsächliche Stunden**: In einem Projekt, einer Aufgabe oder einem benutzerdefinierten Formular für ein Problem, wenn der Zugriff über ein benutzerdefiniertes Feld erfolgt, das auf das native Feld für den nativen Feldverweis verweist. Hierbei handelt es sich um Stunden, die für Projekte, Aufgaben oder Probleme zwischen einem beliebigen Datum vor Mai 2021 und heute protokolliert werden. Sie werden in Stunden in der Workfront-Datenbank gespeichert und ihr Wertefeld wird `actualWorkRequiredDouble`.

     Die aktuell protokollierten Stunden aktualisieren sowohl die tatsächlichen als auch die veralteten tatsächlichen Stunden.

>[!NOTE]
>
>Es wird dringend empfohlen, das Feld „Tatsächliche Stunden“ zu verwenden, wenn dies möglich ist, da im Feld „Frühere Tatsächliche Stunden“ ungenaue Stunden angezeigt werden können, da Inkremente gerundet werden, wenn Stunden in Minuten gespeichert werden. Außerdem werden die veralteten tatsächlichen Stunden in den Diagrammen in Berichten nicht korrekt angezeigt.
> 
>Alle benutzerdefinierten Formeln, die veraltete „Tatsächliche Stunden“ verwenden, wurden auf „Tatsächliche Stunden“ migriert. Legacy-Tatsächliche Stunden können nicht mehr in Berechnungen und Formeln verwendet werden.

## Tatsächliche Stunden für Aufgaben und Probleme im Vergleich zu tatsächlichen Stunden für Projekte

Die tatsächlichen Stunden für Aufgaben und Probleme stellen die Anzahl der Stunden dar, die direkt für die Aufgaben und Probleme protokolliert werden.

Tatsächliche Stunden von untergeordneten Aufgaben werden auf die tatsächlichen Stunden der übergeordneten Aufgabe hochgerechnet. Die folgende Formel gilt für die tatsächlichen Stunden für eine übergeordnete Aufgabe:

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

Die Ist-Stunden für Projekte stellen die Summe der tatsächlichen Stunden aus allen Aufgaben des Projekts (einschließlich der Stunden, die direkt in übergeordneten Aufgaben protokolliert werden), allen Problemen des Projekts und den tatsächlichen Stunden dar, die im Projekt selbst protokolliert werden.

Die folgende Formel gilt für die tatsächlichen Stunden eines Projekts:

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## Tatsächliche Stunden suchen

Für Aufgaben, Projekte und Probleme ist es identisch, den Wert für Tatsächliche Stunden für ein Element zu finden.

### Tatsächliche Stunden im Abschnitt „Details“ {#actual-hours-in-the-details-section}

Die Suche nach tatsächlichen Stunden im Abschnitt „Details“ ist für Projekte, Aufgaben und Probleme identisch.

So suchen Sie tatsächliche Stunden in Aufgabendetails:

1. Wechseln Sie zu einer Aufgabe, für die Sie die tatsächlichen Stunden überprüfen möchten.
1. Klicken Sie im linken Bedienfeld auf **Aufgabendetails**. Der Abschnitt **Übersicht** wird angezeigt.
1. Suchen Sie den Wert **Tatsächliche Stunden** im Abschnitt **Arbeitszeit**. Dies ist die Gesamtzahl der für diese Aufgabe protokollierten Stunden.
1. (Optional und bedingt) Wenn der Verweis auf das native Feld „Tatsächliche Stunden“ zu einem Projekt, einer Aufgabe oder einem benutzerdefinierten Formular für ein Problem hinzugefügt wurde, wechseln Sie zum benutzerdefinierten Formular und suchen Sie im benutzerdefinierten Feld nach den tatsächlichen Stunden. Dies ist die Gesamtzahl der für das Objekt protokollierten Stunden.

### Tatsächliche Stunden im Abschnitt „Stunden“ {#actual-hours-in-the-hours-section}

Die tatsächliche Stundenanzahl im Abschnitt Stunden ist für Projekte, Aufgaben und Probleme identisch.

So suchen Sie die tatsächlichen Stunden im Abschnitt Stunden einer Aufgabe:

1. Wechseln Sie zu einer Aufgabe, für die Sie die tatsächlichen Stunden überprüfen möchten.

1. Klicken Sie im linken Bedienfeld auf **Stunden**. Eine Liste der für die Aufgabe protokollierten Stundeneinträge wird angezeigt, wobei in der Spalte **Stunden** die Gesamtzahl der tatsächlichen Stunden für die Aufgabe angezeigt wird.

1. Stellen Sie sicher **dass die** Standard“ und die **Projekt** Gruppierung auf diese Liste angewendet werden.
1. Die tatsächlichen Stunden für die Aufgabe werden in der Gruppierungszeile für die Spalte „Tatsächliche **&quot;**.

### Tatsächliche Stunden und veraltete tatsächliche Stunden in Berichten

Beim Erstellen von Aufgaben, Problemen oder Projektberichten können Sie die Ist-Stunden und die Legacy-Ist-Stunden für jede Aufgabe, jedes Problem oder jedes Projekt im Bericht anzeigen.

Informationen zur Differenz zwischen tatsächlichen Stunden und veralteten tatsächlichen Stunden finden Sie im Abschnitt [Tatsächliche Stunden vs. veraltete tatsächliche Stunden](#actual-hours-vs-legacy-actual-hours) in diesem Artikel.

>[!NOTE]
>
>Es wird dringend empfohlen, in allen Berichten das Feld Tatsächliche Stunden zu verwenden. Alte Ist-Stunden werden in Diagrammen in Berichten nicht korrekt angezeigt.
> 
>Beachten Sie beim Ersetzen des Felds, dass in „Frühere Tatsächliche Stunden“ Werte in Minuten gespeichert werden, während in „Tatsächliche Stunden“ Werte in Stunden mit Dezimalgenauigkeit gespeichert werden.

So zeigen Sie die tatsächlichen Stunden und die veralteten tatsächlichen Stunden in einem Aufgabenbericht an:

{{step1-to-reports}}

1. Klicken Sie auf der **Berichte** auf **Neuer Bericht** und wählen Sie dann **Aufgabe** als Objekt aus.
1. Klicken Sie unten rechts auf der Seite auf **Spalte hinzufügen**.
1. Beginnen Sie in **Dropdown-Feld****In dieser Spalte anzeigen** mit der Eingabe von „Tatsächliche Stunden“ und wählen Sie dann das Feld aus, wenn es in der Liste angezeigt wird.
1. Wiederholen Sie den obigen Schritt, um das Feld **Alte tatsächliche Stunden** zum Bericht hinzuzufügen.

1. Klicken Sie unten links auf der Seite auf **Speichern + Schließen** um den Bericht zu speichern.

1. Geben **im Dialogfeld „Diesen Bericht zum Speichern benennen** einen neuen Berichtsnamen ein und klicken Sie dann auf **Anwenden**.
1. Wiederholen Sie dieselben Schritte für einen Projekt- oder Problembericht.

### Tatsächliche Stunden in Ressourcen-Management-Tools {#actual-hours-in-resource-management-tools}

Wenn Sie den Fortschritt der Arbeit sehen möchten, die Ihre Benutzerinnen und Benutzer an ihren zugewiesenen Aufgaben und Problemen ausführen, können Sie sie in den folgenden Tools für das Ressourcenmanagement anzeigen:

* Der Nutzungsbericht.

  Weitere Informationen finden Sie [Übersicht über den Bericht zur Ressourcenauslastung](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* Der Ressourcenplaner.

  Weitere Informationen finden Sie unter [Verfügbare, geplante und tatsächliche Stunden oder FTE im Ressourcenplaner anzeigen, wenn Sie die Benutzeransicht verwenden](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).


### Tatsächliche Stunden in der Workfront-API

<!--this section was added as a result to this issue: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/6810910e0001b932e0948336208e76f2/overview-->

Die meisten Workfront-Felder, in denen Stunden gespeichert werden, werden in Minuten in der Workfront-Datenbank gespeichert. Beispielsweise wird der Name des Felds „Geplante Stunden“ für eine Aufgabe in der Workfront-Datenbank `workRequired` und in Minuten gespeichert.

Beim Zugriff auf diese Felder in API-Aufrufen muss die Konvertierung von Minuten in Stunden berücksichtigt werden.<!-- or in calculated custom fields or columns.-->

Die tatsächlichen Stunden, die für Projekte, Aufgaben oder Probleme protokolliert werden, werden derzeit als Minuten in der Workfront-Datenbank gespeichert und ihr Wertefeld wird `actualWorkRequired`.

Seit Oktober 2025 werden mit der API-Version 21 die tatsächlichen Stunden in den folgenden Feldern und Einheiten in der Datenbank gespeichert:

<!--above used to be this: With the following version of the Workfront API scheduled to release later in 2025, Actual Hours are stored in the following fields and units in the database: -->

* **Tatsächliche Stunden**: Stunden, die für ein Projekt, Aufgaben oder Probleme nach Mai 2021 protokolliert wurden. Sie werden in Stunden in der Workfront-Datenbank gespeichert und ihr Wertefeld wird `actualWorkRequiredDouble`.
* **Legacy Actual Hours**: Stunden, die für Projekte, Aufgaben oder Probleme jederzeit protokolliert werden, auch vor Mai 2021. Sie werden als Minuten in der Workfront-Datenbank gespeichert und ihr Wertefeld wird `actualWorkRequired`.

>[!NOTE]
>
>Alle benutzerdefinierten Formeln, die veraltete „Tatsächliche Stunden“ verwenden, wurden auf „Tatsächliche Stunden“ migriert. Legacy-Stunden oder -`actualWorkRequired` können nicht mehr in Berechnungen und Formeln verwendet werden.

Informationen zu API-Versionen finden Sie unter [API-Versionierung und Support-Zeitplan](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>Die Ist-Kosten des Projekts berechnen mithilfe von Legacy-Ist-Stunden.

Informationen zur Verwendung der tatsächlichen Stunden in berechneten Spalten oder Feldern finden Sie unter [Häufig gestellte Fragen zum Bericht](/help/quicksilver/reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

## Zeit erfassen

Sie können Zeit für Aufgaben, Probleme und Projekte auf verschiedene Weise protokollieren.

Weitere Informationen finden Sie unter [Zeit erfassen](../../../timesheets/create-and-manage-timesheets/log-time.md).
