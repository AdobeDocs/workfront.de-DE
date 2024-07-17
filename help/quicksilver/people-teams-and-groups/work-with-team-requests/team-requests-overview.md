---
content-type: reference
product-area: user-management;agile-and-teams
navigation-topic: people-teams-and-groups
title: Übersicht über Teamanfragen
description: Team-Anfragen finden Sie im Bereich Teams im Hauptmenü.
author: Lisa
feature: People Teams and Groups
exl-id: c131c021-8bc0-4a48-a873-9ee0e189bcab
source-git-commit: 9693ac3792fec3eca6218a228f2067519ed433ac
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Übersicht über Teamanfragen

## Grundlegendes zu Teamanfragen

Team-Anforderungen finden Sie im Bereich [!UICONTROL Teams] im [!UICONTROL Hauptmenü]. Klicken Sie auf das Symbol [!UICONTROL Team Requests] ![Anforderungssymbol](assets/request-icon.png) im linken Bereich, um Team-Anforderungen anzuzeigen.

>[!NOTE]
>
>Agile Teams verfügen nicht über Teamanfragen.

Auf der Registerkarte [!UICONTROL Team-Anforderungen] werden die Anforderungen angezeigt, die auf die Zuweisung für das Team warten, das derzeit in der Dropdown-Liste ausgewählt ist. Die Zahl in Klammern gibt an, wie viele Elemente bearbeitet werden können.

Eine Teamanfrage stellt ein ausstehendes Arbeitselement dar, das keinem bestimmten Benutzer zugewiesen ist. Stattdessen wird sie einem Team zugewiesen und jedes Mitglied dieses Teams kann sich freiwillig zur Übernahme der Verantwortung für den Artikel begeben. Wenn ein Benutzer sich bereit erklärt, an einer Teamanfrage zu arbeiten, akzeptiert der Benutzer die Arbeitszuweisung als eigene. Die Aufgabe wird dem einzelnen Benutzer zusätzlich zum Team zugewiesen.

>[!NOTE]
>
>Eine Teamanfrage sollte nicht für partizipative Aufgabenzuweisungen verwendet werden. Wenn Sie mehrere Benutzer für die Zusammenarbeit an einer Aufgabe zuweisen müssen, führen Sie dies über [!UICONTROL Erweiterte Zuweisungen] und nicht über Team-Anforderungen durch. Weitere Informationen finden Sie unter [Erweiterte Zuweisungen erstellen](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

## Grundlegendes zu den Optionen [!UICONTROL Bereit zum Start] und [!UICONTROL Alle]

Oben im Abschnitt &quot;Team Requests&quot;gibt es zwei Optionen: [!UICONTROL Bereit zum Start] und [!UICONTROL Alle].

Die Option [!UICONTROL Bereit zum Start] zeigt nur Aufgaben und Probleme an, die alle folgenden Kriterien erfüllen:

* Alle Vorgänger haben die Bedingungen für ihre Vorgängerabhängigkeitstypen erfüllt.\
  Wenn beispielsweise der Typ der Vorgängerbeziehung [!UICONTROL Finish-Start] ist (Vorgängeraufgabe muss beendet sein, bevor die abhängige Aufgabe gestartet werden kann), muss der Vorgänger als [!UICONTROL Complete] markiert sein. (Weitere Informationen zu Vorgängerabhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).)

* Der angemeldete Benutzer ist die Person, die diesen Aufgaben und Problemen (für Arbeitsanfragen) zugewiesen ist oder dem ausgewählten Team diese Aufgaben und Probleme (für Teamanfragen) zugewiesen hat.
* Der Projektstatus hat den Status &quot;[!UICONTROL Aktuell]&quot;.
* Das [!UICONTROL vorgeschlagene Startdatum] oder das [!UICONTROL geplante Startdatum] sind vergangen oder sollen innerhalb von zwei Wochen ab dem heutigen Datum beginnen (oder es wurde kein [!UICONTROL prognostiziertes Startdatum] oder [!UICONTROL Geplantes Startdatum] definiert).
* Das [!UICONTROL Übergabedatum] ist bereits eingetreten oder tritt innerhalb von zwei Wochen ab dem aktuellen Datum ein.

>[!NOTE]
>
>Wenn die Aufgabe die ersten drei Kriterien erfüllt und innerhalb von zwei Wochen nach dem aktuellen Datum ein Übermittlungsdatum hat, wird sie als [!UICONTROL Bereit zum Start] angezeigt, selbst wenn die geplanten/geplanten Daten länger als zwei Wochen sind. Wenn die Aufgabe kein Übermittlungsdatum hat, müssen die geplanten/geplanten Daten innerhalb von zwei Wochen nach dem aktuellen Datum liegen.

Die Option [!UICONTROL Alle] enthält alle Aufgaben und Probleme in aktuellen Projekten, die dem angemeldeten Benutzer zugewiesen sind, sowie alle Aufgaben oder Probleme, die dem Team zugewiesen sind.
