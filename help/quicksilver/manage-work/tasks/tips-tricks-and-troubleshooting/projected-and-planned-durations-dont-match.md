---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-tasks
title: Voraussichtliche Dauer stimmt nicht mit geplanter Dauer überein
description: 'In diesem Artikel wird die Fehlerbehebung in Adobe Workfront beschrieben, wenn möglicherweise die folgende Meldung angezeigt wird: ''Die voraussichtliche Dauer einer Aufgabe/eines Problems ist auf 0 gestiegen und entspricht nicht der geplanten Dauer.'''
author: Alina
feature: Work Management
exl-id: ef135d44-3138-457d-b54a-3f1102ce3116
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 1%

---

# Projizierte Dauer stimmt nicht mit geplanter Dauer überein

## Problem

Sie erhalten die folgende Fehlermeldung: „Die projizierte Dauer einer Aufgabe/eines Problems ist auf 0 gestiegen und stimmt nicht mit der geplanten Dauer überein.“

## Ursache

Dies liegt daran, dass das voraussichtliche Startdatum mit dem voraussichtlichen Abschlussdatum übereinstimmt.

## Lösung

Es gibt viele Faktoren, die dazu führen können, dass das voraussichtliche Start- und Abschlussdatum übereinstimmen. Dieses Problem hängt weitgehend mit der Zeitzuweisung für die betreffende Aufgabe oder das betreffende Problem zusammen.

In den meisten Fällen sollte die Zuordnung je nach Dauertyp und Aufgabenbeschränkung für die Aufgabe das voraussichtliche Abschlussdatum viel weiter als erwartet ausdehnen. In einigen Fällen jedoch, die auf der Art und Weise basieren, wie der Dauertyp und die Aufgabenbeschränkung konfiguriert sind, ist es möglich, dass dies stattdessen null ist.

Hier finden Sie die besten Informationen, die Sie in diesen Fällen mit Links zu den zugehörigen unterstützenden Artikeln überprüfen können:

* Voraussichtliches Abschlussdatum: [Übersicht über das voraussichtliche Abschlussdatum für Projekte, Aufgaben und Probleme](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)
* Aufgabenbeschränkung: [Übersicht über Aufgabenbeschränkung](../../../manage-work/tasks/task-constraints/task-constraint-overview.md)
* Dauertyp: [Übersicht über Aufgabendauer und Dauertyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)

Wenn das voraussichtliche Abschlussdatum, die Aufgabenbeschränkung oder der Dauertyp erwartungsgemäß funktionieren, wenden Sie sich an den Support, um eine eingehendere Fehlerbehebung zu erhalten.
