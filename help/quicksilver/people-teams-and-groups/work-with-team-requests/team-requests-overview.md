---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Teamanfragen - Übersicht
description: Teamanfragen finden Sie im Bereich Teams im Hauptmenü.
author: Lisa
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
source-git-commit: dfd5c7423b65e6065ab9c2094578443b81189abd
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Übersicht über Teamanfragen

## Grundlegendes zu Teamanfragen

Teamanfragen finden Sie im Bereich [!UICONTROL Teams] im [!UICONTROL Hauptmenü]. Klicken Sie auf das [!UICONTROL Team-Anfragen]-Symbol ![Anfragesymbol](assets/request-icon.png) im linken Bedienfeld, um die Team-Anfragen anzuzeigen.

>[!NOTE]
>
>Agile-Teams haben keine Teamanfragen.

Die [!UICONTROL Team-Anfragen] zeigt die Anforderungen an, die für das Team, das derzeit in der Dropdown-Liste ausgewählt ist, auf Zuweisung warten. Die Zahl in Klammern gibt an, wie viele Elemente bereit zur Bearbeitung sind.

Eine Teamanfrage stellt ein ausstehendes Arbeitselement dar, das keinem bestimmten Benutzer zugewiesen ist. Stattdessen wird es einem Team zugewiesen und jedes Mitglied dieses Teams kann sich freiwillig dazu bereit erklären, die Verantwortung für das Element zu übernehmen. Wenn sich ein(e) Benutzende(r) bereit erklärt, an einer Teamanfrage zu arbeiten, akzeptiert er/sie die Arbeitsaufgabe als seine/ihre eigene. Die Aufgabe wird dem einzelnen Benutzer zusätzlich zum Team zugewiesen.

>[!NOTE]
>
>Eine Teamanfrage sollte nicht für die Zuweisung kollaborativer Aufgaben verwendet werden. Wenn Sie mehrere Benutzer zuweisen müssen, um an einer Aufgabe zusammenzuarbeiten, tun Sie dies über [!UICONTROL Erweiterte Zuweisungen] und nicht über Teamanfragen. Weitere Informationen finden Sie unter [Erstellen erweiterter Zuweisungen](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

## Grundlegendes zu [!UICONTROL Startbereit] und [!UICONTROL Alle] Optionen

Oben im Abschnitt „Team-Anfragen“ gibt es zwei Optionen: [!UICONTROL Bereit zum Start] und [!UICONTROL Alle].

Die [!UICONTROL Bereit zum Start]-Option zeigt nur Aufgaben und Probleme an, die alle folgenden Kriterien erfüllen:

* Alle Vorgänger haben die Bedingungen für ihre Vorgänger-Abhängigkeitstypen erfüllt.\
  Wenn der Typ der Vorgängerbeziehung beispielsweise [!UICONTROL Ende-Anfang] lautet (Vorgängeraufgabe muss abgeschlossen sein, bevor die abhängige Aufgabe beginnen kann), muss der Vorgänger als [!UICONTROL Abgeschlossen] markiert sein. (Weitere Informationen zu Vorgängerabhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).)

* Der angemeldete Benutzer ist die Person, die diesen Aufgaben und Problemen (bei Arbeitsanfragen) zugewiesen ist, oder das ausgewählte Team wird diesen Aufgaben und Problemen (bei Teamanfragen) zugewiesen.
* Der Projektstatus hat den Status &quot;[!UICONTROL &quot; ].
* Das [!UICONTROL Voraussichtliches Startdatum] oder [!UICONTROL Geplantes Startdatum] wurde überschritten oder soll innerhalb von zwei Wochen ab dem heutigen Datum beginnen (oder es wurde kein [!UICONTROL Voraussichtliches Startdatum] oder [!UICONTROL Geplantes Startdatum] definiert).
* Das [!UICONTROL Übergabedatum] ist bereits abgelaufen oder wird innerhalb von zwei Wochen ab dem aktuellen Datum liegen.

>[!NOTE]
>
>Wenn die Aufgabe die ersten drei Kriterien erfüllt und innerhalb von zwei Wochen nach dem aktuellen Datum ein Übergabedatum hat, wird sie als [!UICONTROL Bereit zum Start] angezeigt, auch wenn die geplanten/geplanten Termine länger als zwei Wochen zurückliegen. Wenn die Aufgabe kein Übergabedatum hat, müssen die geplanten/geplanten Termine innerhalb von zwei Wochen nach dem aktuellen Datum liegen.

Die [!UICONTROL Alle]-Option zeigt alle Aufgaben und Probleme in aktuellen Projekten an, die dem angemeldeten Benutzer zugewiesen sind, oder alle Aufgaben oder Probleme, die dem Team zugewiesen sind.
