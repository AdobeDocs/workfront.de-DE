---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Tatsächliche Stunden anzeigen
description: Die Stunden, die Sie bei Ihren Arbeitselementen in Adobe Workfront anmelden, werden als Tatsächliche Stunden betrachtet.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Tatsächliche Stunden anzeigen

Die Stunden, die Sie bei Ihren Arbeitselementen in Adobe Workfront anmelden, werden als Tatsächliche Stunden betrachtet.

Tatsächliche Stunden stellen die tatsächliche Zeit dar, die zum Abschließen einer Aufgabe, eines Problems oder eines Projekts benötigt wurde.

Es wird empfohlen, Stunden in Arbeitselementen zu protokollieren, bei denen es sich um Aufgaben und Probleme handelt.

Als Workfront-Administrator können Sie Benutzenden jedoch erlauben, auch Zeit in Projekten zu protokollieren, je nachdem, welche Workflows in Ihrer Organisation vorhanden sind.

Weitere Informationen dazu, wie Sie Ihr System so einrichten, dass Benutzer Zeit in Projekten protokollieren können, finden Sie unter [Konfigurieren von Arbeitszeittabellen und Stundenvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben, Projekte oder Probleme anzeigen oder erhöhen</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Erweitern von Berechtigungen für eine Aufgabe, ein Projekt oder ein Problem</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Tatsächliche Stunden für Aufgaben und Probleme im Vergleich zu tatsächlichen Stunden für Projekte

Die tatsächlichen Stunden für Aufgaben und Probleme stellen die Anzahl der Stunden dar, die direkt für die Aufgaben und Probleme protokolliert werden.

>[!NOTE]
>
>Tatsächliche Stunden von untergeordneten Aufgaben werden auf die tatsächlichen Stunden der übergeordneten Aufgabe hochgerechnet. Die folgende Formel gilt für die tatsächlichen Stunden für eine übergeordnete Aufgabe:

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

Die Ist-Stunden für Projekte stellen die Summe der tatsächlichen Stunden aus allen Aufgaben im Projekt dar (einschließlich der Stunden, die direkt in übergeordneten Aufgaben protokolliert werden), allen Problemen im Projekt sowie den tatsächlichen Stunden, die im Projekt selbst protokolliert werden.

Die folgende Formel gilt für die tatsächlichen Stunden eines Projekts:

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## Tatsächliche Stunden suchen

Für Aufgaben, Projekte und Probleme ist es identisch, den Wert für Tatsächliche Stunden für ein Element zu finden.

Die Informationen zu den tatsächlichen Stunden für Aufgaben finden Sie an den folgenden Speicherorten:

* [Tatsächliche Stunden im Abschnitt „Details“](#actual-hours-in-the-details-section)
* [Tatsächliche Stunden im Abschnitt „Stunden“](#actual-hours-in-the-hours-section)
* [Tatsächliche Stunden in Berichten](#actual-hours-in-reports)
* [Tatsächliche Stunden in Ressourcen-Management-Tools](#actual-hours-in-resource-management-tools)

### Tatsächliche Stunden im Abschnitt „Details“ {#actual-hours-in-the-details-section}

Die Suche nach tatsächlichen Stunden im Abschnitt „Details“ ist für Projekte, Aufgaben und Probleme identisch.

So suchen Sie tatsächliche Stunden in Aufgabendetails:

1. Wechseln Sie zu einer Aufgabe, für die Sie die tatsächlichen Stunden überprüfen möchten.
1. Klicken Sie **linken** auf „Aufgabendetails“.
1. Klicken Sie **Übersicht** und beachten Sie den Wert **Tatsächliche Stunden**.

   Dies ist die Gesamtzahl der für diese Aufgabe protokollierten Stunden.

### Tatsächliche Stunden im Abschnitt „Stunden“ {#actual-hours-in-the-hours-section}

Die tatsächliche Stundenanzahl im Abschnitt Stunden ist für Projekte, Aufgaben und Probleme identisch.

So suchen Sie die tatsächlichen Stunden im Abschnitt Stunden :

1. Wechseln Sie zu einer Aufgabe, für die Sie die tatsächlichen Stunden überprüfen möchten.
1. Klicken Sie **linken** auf „Stunden“.

   Abhängig von Ihrer Konfiguration kann der Abschnitt „Stunden“ unter &quot;**anzeigen“ aufgeführt**.

   Zeigt eine Liste der Stundeneinträge an, die bei der Aufgabe protokolliert sind.

1. Stellen Sie sicher **dass die** Standard“ und die **Projekt** Gruppierung auf diese Liste angewendet werden.

   Die Zahl, die in der Gruppierungszeile für die Spalte **Stunden** angezeigt wird, ist die Gesamtanzahl der tatsächlichen Stunden für die Aufgabe.

### Tatsächliche Stunden in Berichten {#actual-hours-in-reports}

Beim Erstellen von Aufgaben, Problemen oder Projektberichten können Sie den tatsächlichen Stundenwert für jede Aufgabe, jedes Problem oder jedes Projekt im Bericht anzeigen.

Das Hinzufügen der Spalte Tatsächliche Stunden zu einer Aufgabenansicht ähnelt dem Erstellen einer Ansicht in einem Bericht.

So zeigen Sie die tatsächlichen Stunden in einem Aufgabenbericht an:

1. Klicken Sie auf **Hauptmenü** Symbol ![](assets/main-menu-icon.png) in der oberen rechten Ecke von Workfront und dann auf **Berichte**.
1. Klicken Sie **Neuer Bericht** und wählen Sie dann **Aufgabe** als Objekt aus.

1. Klicken Sie **Spalte hinzufügen** und beginnen Sie mit der Eingabe **Tatsächliche Stunden**, wenn das **In dieser Spalte anzeigen** Dropdown-Feld angezeigt wird. Wählen Sie das Feld aus, wenn es in der Liste angezeigt wird.

1. Klicken Sie **Speichern + Schließen**, um den Bericht zu speichern.

   In der Spalte Tatsächliche Stunden wird die Anzahl der Stunden angezeigt, die für jede Aufgabe protokolliert wurden.

### Tatsächliche Stunden in Ressourcen-Management-Tools {#actual-hours-in-resource-management-tools}

Wenn Sie den Fortschritt der Arbeit sehen möchten, die Ihre Benutzerinnen und Benutzer an ihren zugewiesenen Aufgaben und Problemen ausführen, können Sie sie in den folgenden Tools für das Ressourcenmanagement anzeigen:

* Auslastungsbericht\
  Informationen zum Auslastungsbericht finden Sie unter [Übersicht über den Ressourcenauslastungsbericht](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* Ressourcenplaner.

  Informationen zum Anzeigen der tatsächlichen Stunden im Ressourcenplaner finden Sie unter [Verfügbare, geplante und tatsächliche Stunden oder FTE im Ressourcenplaner anzeigen, wenn Sie die Benutzeransicht verwenden](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).

## Zeit erfassen

Sie können Zeit für Aufgaben, Probleme und Projekte auf verschiedene Weise protokollieren.

Weitere Informationen zur Zeitprotokollierung in Workfront finden Sie unter [Zeit protokollieren](../../../timesheets/create-and-manage-timesheets/log-time.md).
