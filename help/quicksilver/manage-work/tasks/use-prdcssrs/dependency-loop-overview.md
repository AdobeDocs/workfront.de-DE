---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Übersicht über die Aufgabenabhängigkeitsschleife
description: Beim Hinzufügen von Vorgängerbeziehungen zu Aufgaben können Abhängigkeitsschleifen auftreten. Informationen zu Vorgängern finden Sie unter Übersicht über Aufgabenvorgänger.
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
TQID: https://experienceleague.adobe.com/cQbPOUES-tmSgZTpXrft8lQby-ubPmI-TZ1PjdGURMc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 263
ht-degree: 1%

---

# Überblick über die Aufgabenabhängigkeitsschleife

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


