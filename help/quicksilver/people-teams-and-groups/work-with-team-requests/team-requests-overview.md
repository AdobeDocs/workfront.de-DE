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

## Team-Anforderungen verstehen

Team-Anforderungen finden Sie im Abschnitt [!UICONTROL Teams] -Gebiet [!UICONTROL Hauptmenü]. Klicken Sie auf [!UICONTROL Team-Anforderungen] icon ![Symbol &quot;Anforderung&quot;](assets/request-icon.png) im linken Bereich, um Team-Anforderungen anzuzeigen.

>[!NOTE]
>
>Agile Teams verfügen nicht über Teamanfragen.

Die [!UICONTROL Team-Anforderungen] zeigt die Anforderungen an, die auf die Zuweisung des Teams warten, das derzeit in der Dropdown-Liste ausgewählt ist. Die Zahl in Klammern gibt an, wie viele Elemente bearbeitet werden können.

Eine Teamanfrage stellt ein ausstehendes Arbeitselement dar, das keinem bestimmten Benutzer zugewiesen ist. Stattdessen wird sie einem Team zugewiesen und jedes Mitglied dieses Teams kann sich freiwillig zur Übernahme der Verantwortung für den Artikel begeben. Wenn ein Benutzer sich bereit erklärt, an einer Teamanfrage zu arbeiten, akzeptiert der Benutzer die Arbeitszuweisung als eigene. Die Aufgabe wird dem einzelnen Benutzer zusätzlich zum Team zugewiesen.

>[!NOTE]
>
>Eine Teamanfrage sollte nicht für partizipative Aufgabenzuweisungen verwendet werden. Wenn Sie mehrere Benutzer für die Zusammenarbeit an einer Aufgabe zuweisen müssen, führen Sie dies durch [!UICONTROL Erweiterte Zuweisungen] und nicht über Team-Anfragen. Weitere Informationen finden Sie unter [Erweiterte Zuweisungen erstellen](../../manage-work/tasks/assign-tasks/create-advanced-assignments.md).

## Die [!UICONTROL Bereit zum Start] und [!UICONTROL Alle] options

Oben im Abschnitt &quot;Team Requests&quot;gibt es zwei Optionen: [!UICONTROL Bereit zum Start] und [!UICONTROL Alle].

Die [!UICONTROL Bereit zum Start] zeigt nur Aufgaben und Probleme an, die alle folgenden Kriterien erfüllen:

* Alle Vorgänger haben die Bedingungen für ihre Vorgängerabhängigkeitstypen erfüllt.\
   Wenn beispielsweise der Typ der Vorgängerbeziehung [!UICONTROL Finish-Start] (Vorgängeraufgabe muss beendet sein, bevor die abhängige Aufgabe gestartet werden kann), muss der Vorgänger als [!UICONTROL Fertig]. (Weitere Informationen zu Vorgängerabhängigkeitstypen finden Sie unter [Übersicht über Aufgabenabhängigkeitstypen](../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

* Der angemeldete Benutzer ist die Person, die diesen Aufgaben und Problemen (für Arbeitsanfragen) zugewiesen ist oder dem ausgewählten Team diese Aufgaben und Probleme (für Teamanfragen) zugewiesen hat.
* Der Projektstatus hat den Status [!UICONTROL Aktuell].
* Die [!UICONTROL Projiziertes Startdatum] oder [!UICONTROL Geplantes Startdatum] ist vergangen oder soll innerhalb von zwei Wochen ab dem heutigen Datum beginnen (oder [!UICONTROL Projiziertes Startdatum] oder [!UICONTROL Geplantes Startdatum] wurde definiert).
* Die [!UICONTROL Übermittlungsdatum] ist bereits eingetreten oder tritt innerhalb von zwei Wochen nach dem aktuellen Datum ein.

>[!NOTE]
>
>Wenn die Aufgabe die ersten drei Kriterien erfüllt und innerhalb von zwei Wochen nach dem aktuellen Datum ein Übermittlungsdatum hat, wird sie als [!UICONTROL Bereit zum Start] auch wenn die geplanten/geplanten Daten länger als zwei Wochen dauern. Wenn die Aufgabe kein Übermittlungsdatum hat, müssen die geplanten/geplanten Daten innerhalb von zwei Wochen nach dem aktuellen Datum liegen.

Die [!UICONTROL Alle] zeigt alle Aufgaben und Probleme bei aktuellen Projekten an, die dem angemeldeten Benutzer zugewiesen sind, oder alle Aufgaben oder Probleme, die dem Team zugewiesen sind.
