---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Tatsächliche Stunden anzeigen
description: Die Stunden, die Sie bei Ihren Arbeitselementen in Adobe Workfront anmelden, werden als Tatsächliche Stunden betrachtet.
author: Alina
feature: Work Management
exl-id: c4b0e431-1765-416d-89f5-6ac663ac1d4f
source-git-commit: d68189272bd3f78de2d57b8393b44b698fa5db13
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 0%

---

# Tatsächliche Stunden anzeigen

<!-- Audited: 5/2025 -->

Die Stunden, die Sie bei Ihren Arbeitselementen in Adobe Workfront anmelden, werden als Tatsächliche Stunden betrachtet.

Tatsächliche Stunden stellen die tatsächliche Zeit dar, die zum Abschließen einer Aufgabe, eines Problems oder eines Projekts benötigt wurde.

Es wird empfohlen, Stunden in Arbeitselementen zu protokollieren, bei denen es sich um Aufgaben und Probleme handelt. Als Workfront-Admin können Sie jedoch Benutzenden erlauben, Zeit in Projekten auch in Abhängigkeit von den Workflows Ihres Unternehmens zu protokollieren.

Weitere Informationen dazu, wie Sie Ihr System so einrichten, dass Benutzer Zeit in Projekten protokollieren können, finden Sie unter [Konfigurieren von Arbeitszeittabellen und Stundenvoreinstellungen](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

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
   <p>Neu: Standard<p>
   <p>Oder</p>
   <p>Aktuell: Arbeit oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Aufgaben, Projekte oder Probleme anzeigen oder erhöhen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen oder Erweitern von Berechtigungen für eine Aufgabe, ein Projekt oder ein Problem</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

### Tatsächliche Stunden im Abschnitt „Stunden“ {#actual-hours-in-the-hours-section}

Die tatsächliche Stundenanzahl im Abschnitt Stunden ist für Projekte, Aufgaben und Probleme identisch.

So suchen Sie die tatsächlichen Stunden im Abschnitt Stunden :

1. Wechseln Sie zu einer Aufgabe, für die Sie die tatsächlichen Stunden überprüfen möchten.

1. Klicken Sie im linken Bedienfeld auf **Stunden**. Eine Liste der für die Aufgabe protokollierten Stundeneinträge wird angezeigt, wobei in der Spalte **Stunden** die Gesamtzahl der tatsächlichen Stunden für die Aufgabe angezeigt wird.

1. Stellen Sie sicher **dass die** Standard“ und die **Projekt** Gruppierung auf diese Liste angewendet werden.

### Tatsächliche Stunden in Berichten {#actual-hours-in-reports}

Beim Erstellen von Aufgaben, Problemen oder Projektberichten können Sie den tatsächlichen Stundenwert für jede Aufgabe, jedes Problem oder jedes Projekt im Bericht anzeigen.

So zeigen Sie die tatsächlichen Stunden in einem Aufgabenbericht an:

{{step1-to-reports}}

1. Klicken Sie auf der **Berichte** auf **Neuer Bericht** und wählen Sie dann **Aufgabe** als Objekt aus.
1. Klicken Sie unten rechts auf der Seite auf **Spalte hinzufügen**.
1. Beginnen Sie im angezeigten **In dieser Spalte anzeigen** mit der Eingabe von &quot;**Stunden“** wählen Sie dann das Feld aus, wenn es in der Liste angezeigt wird.

1. Klicken Sie unten links auf der Seite auf **Speichern + Schließen** um den Bericht zu speichern.

1. Geben **im Dialogfeld „Diesen Bericht zum Speichern benennen** einen neuen Berichtsnamen ein und klicken Sie dann auf **Anwenden**.

### Tatsächliche Stunden in Ressourcen-Management-Tools {#actual-hours-in-resource-management-tools}

Wenn Sie den Fortschritt der Arbeit sehen möchten, die Ihre Benutzerinnen und Benutzer an ihren zugewiesenen Aufgaben und Problemen ausführen, können Sie sie in den folgenden Tools für das Ressourcenmanagement anzeigen:

* Der Nutzungsbericht.\
  Weitere Informationen finden Sie [Übersicht über den Bericht zur Ressourcenauslastung](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* Der Ressourcenplaner.

  Weitere Informationen finden Sie unter [Verfügbare, geplante und tatsächliche Stunden oder FTE im Ressourcenplaner anzeigen, wenn Sie die Benutzeransicht verwenden](../../../resource-mgmt/resource-planning/view-hours-fte-user-view-resource-planner.md).


### Tatsächliche Stunden in der Workfront <!--database and the--> API-<!--, and custom data-->

<!--this section was added as a result to this issue: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/6810910e0001b932e0948336208e76f2/overview-->

Die meisten Workfront-Felder, in denen Stunden gespeichert werden, werden in Minuten in der Workfront-Datenbank gespeichert. Beispielsweise wird der Name des Felds „Geplante Stunden“ für eine Aufgabe in der Workfront-Datenbank `workRequired` und in Minuten gespeichert.

Beim Zugriff auf diese Felder in API-Aufrufen oder in berechneten benutzerdefinierten Feldern oder Spalten muss die Konvertierung von Minuten in Stunden berücksichtigt werden.

Je nachdem, wie Sie auf die tatsächlichen Stunden zugreifen, können diese in den folgenden Feldern und Einheiten in der Datenbank gespeichert werden:

* In der API: Der `valuefield` für die tatsächlichen Stunden ist `actualWorkRequiredDouble`, der in Stunden gespeichert wird.
* In der Workfront-Benutzeroberfläche (berechnetes benutzerdefiniertes Feld und Spalten): Die `valuefield` für die Ist-Stunden wird in Minuten `actualWorkRequired`.

<!--Change the above with this when we fix this for the Workfront UI: 

You must use the following valuefield name for Actual Hours in API calls or calculated custom fields or columns in Workfront: `actualWorkRequiredDouble`. -->

Informationen zur Verwendung der tatsächlichen Stunden in berechneten Spalten oder Feldern finden Sie unter [Häufig gestellte Fragen zum Bericht](/help/quicksilver/reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

## Zeit erfassen

Sie können Zeit für Aufgaben, Probleme und Projekte auf verschiedene Weise protokollieren.

Weitere Informationen finden Sie unter [Zeit erfassen](../../../timesheets/create-and-manage-timesheets/log-time.md).
