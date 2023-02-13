---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Tatsächliche Stunden anzeigen
description: Die Stunden, in denen Sie sich in Adobe Workfront bei Ihren Arbeitselementen anmelden, gelten als tatsächliche Stunden.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Tatsächliche Stunden anzeigen

Die Stunden, in denen Sie sich in Adobe Workfront bei Ihren Arbeitselementen anmelden, gelten als tatsächliche Stunden.

Die tatsächlichen Stunden stellen die tatsächliche Zeit dar, die Sie zum Abschließen einer Aufgabe, eines Problems oder eines Projekts benötigt haben.

Es wird empfohlen, Stunden für Arbeitselemente zu protokollieren, bei denen es sich um Aufgaben und Probleme handelt.

Als Workfront-Administrator können Sie Benutzern jedoch auch die Möglichkeit geben, sich in Projekten zu registrieren, je nachdem, welche Workflows in Ihrem Unternehmen ausgeführt werden.

Weitere Informationen zum Einrichten Ihres Systems, das Benutzern die Möglichkeit gibt, sich bei Projekten anzumelden, finden Sie unter [Zeitblatt- und Stundenvoreinstellungen konfigurieren](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

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
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Aufgaben, Projekte oder Probleme anzeigen oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für eine Aufgabe, ein Projekt oder ein Problem</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Tatsächliche Stunden für Aufgaben und Probleme im Vergleich zu tatsächlichen Zeiten für Projekte

Die tatsächlichen Stunden für Aufgaben und Probleme stellen die Anzahl der Stunden dar, die direkt bei den Aufgaben und Problemen protokolliert werden.

>[!NOTE]
>
>Die tatsächlichen Stunden von untergeordneten Aufgaben werden auf die tatsächlichen Stunden der übergeordneten Aufgabe übertragen. Die folgende Formel gilt für die tatsächlichen Stunden einer übergeordneten Aufgabe:

```
Parent Task Actual Hours = All Tasks Actual Hours + Parent Task Actual Hours
```

Die tatsächlichen Stunden für Projekte stellen die Gesamtanzahl der tatsächlichen Stunden aus allen Aufgaben im Projekt dar (einschließlich der Stunden, die direkt bei den übergeordneten Aufgaben protokolliert werden), alle Probleme im Projekt sowie die tatsächlichen Stunden, die im Projekt selbst protokolliert wurden.

Die folgende Formel gilt für die tatsächlichen Stunden eines Projekts:

```
Project Actual Hours = All Tasks Actual Hours + All Issues Actual Hours + All Project Actual Hours
```

## Tatsächliche Stunden suchen

Die Suche nach dem Wert für &quot;Tatsächliche Stunden&quot;für ein Element ist für Aufgaben, Projekte und Probleme identisch.

Informationen zu Aufgaben finden Sie in den folgenden Ordnern:

* [Tatsächliche Stunden im Detailabschnitt](#actual-hours-in-the-details-section)
* [Tatsächliche Stunden im Abschnitt Stunden](#actual-hours-in-the-hours-section)
* [Tatsächliche Stunden in Berichten](#actual-hours-in-reports)
* [Tatsächliche Stunden in Ressourcen-Management-Tools](#actual-hours-in-resource-management-tools)

### Tatsächliche Stunden im Detailabschnitt {#actual-hours-in-the-details-section}

Die Suche nach tatsächlichen Stunden im Bereich Details ist für Projekte, Aufgaben und Probleme identisch.

So suchen Sie tatsächliche Stunden in Aufgabendetails:

1. Gehen Sie zu einer Aufgabe, für die Sie die tatsächlichen Stunden überprüfen möchten.
1. Klicken **Aufgabendetails** im linken Bereich.
1. Klicken **Übersicht** und beachten Sie die **Tatsächliche Stunden** -Wert.

   Dies ist die Gesamtzahl der Stunden, die bei dieser Aufgabe protokolliert wurden.

### Tatsächliche Stunden im Abschnitt Stunden {#actual-hours-in-the-hours-section}

Die Suche nach tatsächlichen Stunden im Abschnitt Stunden ist für Projekte, Aufgaben und Probleme identisch.

So suchen Sie den Abschnitt &quot;Tatsächliche Stunden in Stunden&quot;:

1. Gehen Sie zu einer Aufgabe, für die Sie die tatsächlichen Stunden überprüfen möchten.
1. Klicken **Stunden** im linken Bereich.

   Abhängig von Ihrer Konfiguration kann der Abschnitt Stunden unter **Mehr anzeigen**.

   Dadurch wird eine Liste der für die Aufgabe protokollierten Stundeneinträge angezeigt.

1. Stellen Sie sicher, dass **Standard** und **Projekt** Gruppierung wird auf diese Liste angewendet.

   Die in der Gruppierungszeile für die **Stunden** gibt die Gesamtzahl der tatsächlichen Stunden für die Aufgabe an.

### Tatsächliche Stunden in Berichten {#actual-hours-in-reports}

Beim Erstellen von Aufgaben, Problemen oder Projektberichten können Sie den Wert für die tatsächlichen Stunden für jede Aufgabe, jedes Problem oder jedes Projekt im Bericht anzeigen.

Das Hinzufügen der Spalte &quot;Tatsächliche Stunden&quot;zu einer Aufgabenansicht ähnelt dem Erstellen einer Ansicht in einem Bericht.

So zeigen Sie die tatsächlichen Stunden in einem Aufgabenbericht an:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **Berichte**.
1. Klicken **Neuer Bericht**, wählen Sie **Aufgabe** als Objekt.

1. Klicken **Spalte hinzufügen** und beginnen Sie mit der Eingabe **Tatsächliche Stunden** wenn die **In dieser Spalte anzeigen** angezeigt. Wählen Sie das Feld aus, wenn es in der Liste angezeigt wird.

1. Klicken **Speichern und schließen** , um den Bericht zu speichern.

   In der Spalte &quot;Tatsächliche Stunden&quot;wird die Anzahl der Stunden angezeigt, die bei jeder Aufgabe protokolliert wurden.

### Tatsächliche Stunden in Ressourcen-Management-Tools {#actual-hours-in-resource-management-tools}

Wenn Sie den Fortschritt der Arbeit sehen möchten, die Ihre Benutzer an ihren zugewiesenen Aufgaben und Problemen durchführen, können Sie sie in den folgenden Tools für die Ressourcenverwaltung anzeigen:

* Nutzungsbericht\
   Informationen zum Nutzungsbericht finden Sie unter [Übersicht über den Bericht &quot;Ressourcenauslastung&quot;](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* Ressourcenplaner.

   Informationen zur Anzeige der tatsächlichen Stunden im Ressourcenplaner finden Sie unter [Anzeigen der verfügbaren, geplanten und tatsächlichen Stunden oder der FTE im Ressourcenplaner bei Verwendung der Benutzeransicht](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).

## Protokollzeit

Sie können die Zeit für Aufgaben, Probleme und Projekte auf verschiedene Arten protokollieren.

Weitere Informationen zur Protokollierungszeit in Workfront finden Sie unter [Protokollzeit](../../../timesheets/create-and-manage-timesheets/log-time.md).
