---
content-type: overview
product-area: projects
navigation-topic: manage-tasks
title: Überblick über das Projekt - Kritischer Pfad
description: Das Bestimmen des kritischen Pfads eines Projekts ist eine automatische Möglichkeit für Adobe Workfront, eine Reihe von Aufgaben in einem Projekt zu kennzeichnen, die sich auf die Timeline des Projekts auswirken können. Aufgaben, die sich auf die Timeline des Projekts auswirken können, werden als Aufgaben des kritischen Pfads gekennzeichnet.
author: Alina
feature: Work Management
exl-id: 9cbc84bf-d02b-4bb7-8d5d-922554d1262e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '771'
ht-degree: 0%

---

# Überblick über das Projekt - Kritischer Pfad

Das Bestimmen des kritischen Pfads eines Projekts ist eine automatische Möglichkeit für Adobe Workfront, eine Reihe von Aufgaben in einem Projekt zu kennzeichnen, die sich auf die Timeline des Projekts auswirken können. Aufgaben, die sich auf die Timeline des Projekts auswirken können, werden als Aufgaben des kritischen Pfads gekennzeichnet.

Die folgenden Funktionen können sich auf den kritischen Pfad eines Projekts auswirken:

* Die Arbeitsaufschlüsselungsstruktur des Projekts.

   Weitere Informationen zur Struktur der Arbeitsaufschlüsselung finden Sie unter [Bestimmen der Arbeitsaufschlüsselungsstruktur in einem Projekt](../../../manage-work/projects/planning-a-project/determine-project-work-breakdown-structure.md)

* Die Zeit (Dauer), die der Abschluss jeder Aufgabe benötigt.
* Die Abhängigkeiten zwischen den Aufgaben.

   Beachten Sie Folgendes:

   * Wenn eine Aufgabe auf dem Kritischen Pfad eine Vorgängerbeziehung hat, befinden sich ihre Vorgänger und Nachfolger auch auf dem kritischen Pfad, wenn sich die Datumsänderungen der Vorgänger oder Nachfolger direkt auf ihre abhängigen Personen auswirken.

      >[!TIP]
      >
      >Wenn sich das Datum des Nachfolgers einer Aufgabe nicht direkt auf das Datum ihrer abhängigen Aufgaben auswirkt und sich dies nicht auf die Daten des Projekts auswirkt, befindet sich die Nachfolgeaufgabe nicht auf dem kritischen Pfad.
      >
      >
      >![](assets/successor-not-on-critical-path-350x150.png)     >

   * Wenn eine Unteraufgabe als Aufgabe &quot;Kritischer Pfad&quot;identifiziert wird, wird die übergeordnete Aufgabe auch als Aufgabe &quot;Kritischer Pfad&quot;identifiziert, wenn das voraussichtliche Anfangsdatum und die voraussichtliche Uhrzeit der übergeordneten Aufgabe mit denen der Unteraufgabe übereinstimmen.

Unter Berücksichtigung dieser Funktionen berechnet das System den kritischen Pfad anhand des längsten Pfads zwischen der frühesten Aufgabe und der Aufgabe, die das Ende des Projekts bestimmt. Bei der Berechnung des kritischen Pfads wird berücksichtigt, wann die einzelnen Aufgaben zum frühesten und letzten Mal gestartet und beendet werden können, ohne das Projekt zu verlängern. Dieser Prozess bestimmt, welche Aufgaben &quot;kritisch&quot;sind (und zum längsten Pfad gehören) und welche Aufgaben über &quot;Gesamt-Float&quot;verfügen (kann verzögert werden, ohne das Projekt länger zu machen).

Jede Verzögerung in der Aktivität einer Aufgabe auf dem kritischen Pfad wirkt sich direkt auf das geplante Abschlussdatum des Projekts aus (es gibt keinen Float auf dem kritischen Pfad).

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
   <td> <p>Zugriff auf Aufgaben anzeigen oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für eine Aufgabe </p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Kritischen Pfad anzeigen

Sie können die Aufgaben, die zum kritischen Pfad gehören, in den folgenden Bereichen der Workfront-Anwendung anzeigen:

* [Kritischen Pfad im Gantt-Diagramm anzeigen](#view-the-critical-path-in-the-gantt-chart)
* [Kritischen Pfad in einer Aufgabenliste oder einem Bericht anzeigen](#view-the-critical-path-in-a-task-list-or-report)

### Kritischen Pfad im Gantt-Diagramm anzeigen {#view-the-critical-path-in-the-gantt-chart}

So zeigen Sie Aufgaben auf dem kritischen Pfad in der Gantt-Grafik an:

1. Wechseln Sie zu einem Projekt, für das Sie den kritischen Pfad anzeigen möchten.
1. Klicken **Aufgaben** im linken Bereich.
1. Klicken Sie auf **Gantt-Diagramm** in der oberen rechten Ecke der Aufgabenliste.

   ![gantt_chart_icon__1_.png](assets/gantt-chart-icon--1-.png)

1. Erweitern Sie die **Optionen** Menü und aktivieren Sie dann die **Kritischer Pfad** -Option.

   Die Aufgaben, die sich auf dem kritischen Pfad befinden, haben eine rote Linie über ihrer Zeitleiste im Gantt-Diagramm.

   ![crtitical_path_on_gantt__1_.png](assets/crtitical-path-on-gantt--1--350x137.png)

### Kritischen Pfad in einer Aufgabenliste oder einem Bericht anzeigen {#view-the-critical-path-in-a-task-list-or-report}

So zeigen Sie in einer Aufgabenliste an, welche Aufgaben sich auf dem kritischen Pfad befinden:

1. Wechseln Sie zu einem Projekt, für das Sie den kritischen Pfad anzeigen möchten.
1. Klicken **Aufgaben** im linken Bereich.
1. Aus dem **Ansicht** Dropdown-Menü auswählen **Status**.

   Die Aufgaben, die sich auf dem kritischen Pfad befinden, haben einen **Kritischer Pfad** -Markierung in **Flags** der Liste.

   Sie können dieselbe Ansicht auf einen Aufgabenbericht anwenden.

   Weitere Informationen zum Erstellen von Berichten finden Sie im Artikel [Benutzerdefinierten Bericht erstellen](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

   Oder

   Aus dem **Filter** Dropdown-Menü auswählen **Neuer Filter**.

1. Klicken **Filterregel hinzufügen** und Eingabe beginnen **Ist kritisch** im **Nur zeigen mir Aufgaben, in denen die ...** -Feld.

1. Wählen Sie sie aus, wenn sie in der Liste angezeigt wird.
1. Klicken **Filter speichern**.

   Die Liste sollte nur Aufgaben anzeigen, die sich auf dem kritischen Pfad befinden.
