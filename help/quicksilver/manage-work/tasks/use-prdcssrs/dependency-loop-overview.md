---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Übersicht über die Aufgabenabhängigkeitsschleife
description: Beim Hinzufügen von Vorgängerbeziehungen zu Aufgaben können Abhängigkeitsschleifen auftreten. Informationen zu Vorgängern finden Sie unter Übersicht über Aufgabenvorgänger.
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Übersicht über die Aufgabenabhängigkeitsschleife

Beim Hinzufügen von Vorgängerbeziehungen zu Aufgaben können Abhängigkeitsschleifen auftreten. Informationen zu Vorgängern finden Sie unter [Übersicht über Aufgabenvorgänger](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Übersicht über Abhängigkeitsschleifen

Abhängigkeitsschleifen entstehen, wenn zwei oder mehr Aufgaben voneinander abhängig sind. Adobe Workfront erlaubt es Ihnen nicht, eine Vorgängerbeziehung zwischen Aufgaben zu erstellen, wenn dadurch eine Abhängigkeitsschleife erzeugt wird.

**Beispiel:** Aufgabe 2 ist ein Vorgänger von Aufgabe 1, was bedeutet, dass Sie Aufgabe 2 abschließen müssen, bevor Sie mit der Arbeit an Aufgabe 1 beginnen können.

Wenn Sie versuchen, Aufgabe 1 zu einem Vorgänger von Aufgabe 2 zu machen, erhalten Sie einen Abhängigkeitsschleifenfehler, da Sie Aufgabe 1 erst starten können, nachdem Aufgabe 2 abgeschlossen wurde. Aufgabe 2 kann jedoch erst gestartet werden, wenn Aufgabe 1 abgeschlossen ist.

![Fehlermeldung für Abhängigkeitsschleife](assets/dependency-loop-error-message-350x209.png)

![Abhängigkeitsschleife in Aufgabenliste](assets/dependency-loop-in-task-list-nwe-350x97.png)

## Überlegungen zu Abhängigkeitsschleifen

* Abhängigkeitsschleifen können mehr als zwei Aufgaben umfassen. Manchmal sind beliebig viele übergeordnete Elemente der Aufgaben, die Sie mit einer Vorgängerbeziehung verbinden, diejenigen, die die Abhängigkeitsschleife erzeugen.
* Eine Abhängigkeitsschleife kann auch auftreten, wenn Sie versuchen, ein übergeordnetes Element zum Vorgänger eines untergeordneten Elements zu machen.
* Im Falle einer Abhängigkeitsschleife können Sie die Aufgaben oder das Projekt nicht speichern. Um die Abhängigkeitsschleife zu beheben, müssen Sie die Vorgängerbeziehung zwischen den in der Fehlermeldung aufgelisteten Aufgaben neu bewerten und die Konflikte entfernen, bevor Sie die Aufgaben oder das Projekt speichern können.


