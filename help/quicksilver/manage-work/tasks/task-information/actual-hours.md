---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Tatsächliche Stunden anzeigen
description: Die Stunden, die Sie bei Ihren Arbeitselementen in Adobe Workfront anmelden, werden als Tatsächliche Stunden betrachtet. Tatsächliche Stunden stellen die tatsächliche Zeit dar, die zum Abschließen einer Aufgabe, eines Problems oder eines Projekts benötigt wurde.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '1276'
ht-degree: 1%

---

# Tatsächliche Stunden anzeigen

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

<!--Old:
 
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
</table>-->

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
>Es wird empfohlen, das Feld „Tatsächliche Stunden“ zu verwenden, wenn dies möglich ist, da im Feld „Frühere Tatsächliche Stunden“ ungenaue Stunden angezeigt werden können, da Inkremente gerundet werden, wenn Stunden in Minuten gespeichert werden.

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

* Der Nutzungsbericht.\
  Weitere Informationen finden Sie [Übersicht über den Bericht zur Ressourcenauslastung](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* Der Ressourcenplaner.

  Weitere Informationen finden Sie unter [Verfügbare, geplante und tatsächliche Stunden oder FTE im Ressourcenplaner anzeigen, wenn Sie die Benutzeransicht verwenden](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).


### Tatsächliche Stunden in der Workfront-API

<!--this section was added as a result to this issue: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/6810910e0001b932e0948336208e76f2/overview-->

Die meisten Workfront-Felder, in denen Stunden gespeichert werden, werden in Minuten in der Workfront-Datenbank gespeichert. Beispielsweise wird der Name des Felds „Geplante Stunden“ für eine Aufgabe in der Workfront-Datenbank `workRequired` und in Minuten gespeichert.

Beim Zugriff auf diese Felder in API-Aufrufen oder in berechneten benutzerdefinierten Feldern oder Spalten muss die Konvertierung von Minuten in Stunden berücksichtigt werden.

Die tatsächlichen Stunden, die für Projekte, Aufgaben oder Probleme protokolliert werden, werden derzeit als Minuten in der Workfront-Datenbank gespeichert und ihr Wertefeld wird `actualWorkRequired`.

Da die folgende Version der Workfront-API voraussichtlich im Laufe des Jahres 2025 veröffentlicht wird, werden die tatsächlichen Stunden in den folgenden Feldern und Einheiten in der Datenbank gespeichert:

* **Tatsächliche Stunden**: Stunden, die für ein Projekt, Aufgaben oder Probleme nach Mai 2021 protokolliert wurden. Sie werden in Stunden in der Workfront-Datenbank gespeichert und ihr Wertefeld wird `actualWorkRequiredDouble`.
* **Legacy Actual Hours**: Stunden, die für Projekte, Aufgaben oder Probleme jederzeit protokolliert werden, auch vor Mai 2021. Sie werden als Minuten in der Workfront-Datenbank gespeichert und ihr Wertefeld wird `actualWorkRequired`.

Informationen zu API-Versionen finden Sie unter [API-Versionierung und Support-Zeitplan](/help/quicksilver/wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>Die Ist-Kosten des Projekts berechnen mithilfe von Legacy-Ist-Stunden.

Informationen zur Verwendung der tatsächlichen Stunden in berechneten Spalten oder Feldern finden Sie unter [Häufig gestellte Fragen zum Bericht](/help/quicksilver/reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

## Zeit erfassen

Sie können Zeit für Aufgaben, Probleme und Projekte auf verschiedene Weise protokollieren.

Weitere Informationen finden Sie unter [Zeit erfassen](../../../timesheets/create-and-manage-timesheets/log-time.md).
