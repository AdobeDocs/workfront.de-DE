---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: Übersicht über Aufgabenabhängigkeitstypen
description: Abhängigkeitstypen beziehen sich auf die Vorgängerbeziehungen zwischen Aufgaben. Sie definieren, wann die abhängige Aufgabe basierend auf dem Anfang oder Ende ihrer Vorgängerin beginnen oder beenden kann.
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
source-git-commit: 91d757513792604677d6285baafa795629b4506d
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Übersicht über Aufgabenabhängigkeitstypen

<!-- Audited: 12/2023 -->

Abhängigkeitstypen beziehen sich auf die Vorgängerbeziehungen zwischen Aufgaben. Sie definieren, wann die abhängige Aufgabe basierend auf dem Anfang oder Ende ihrer Vorgängerin beginnen oder beenden kann.

>[!IMPORTANT]
>
>Adobe Workfront schränkt die abhängigen Aufgaben nicht vom Starten oder Beenden basierend auf den Abhängigkeitstypen ein, es sei denn, die Vorgängerbeziehungen werden erzwungen. Informationen zum Erzwingen von Vorgängern finden Sie unter [Erzwingen von Vorgängern](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

Sie müssen den Abhängigkeitstyp einer Vorgängerbeziehung angeben, wenn Sie diese Beziehung zwischen Ihren Aufgaben herstellen.

Weitere Informationen zu Vorgängern finden Sie unter [Übersicht über Aufgabenvorgänger](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Im Folgenden finden Sie die Workfront-Abhängigkeitstypen:

* **Beenden-Start (fs)**: Die Vorgängeraufgabe muss beendet sein, bevor die abhängige Aufgabe beginnen kann. Dies ist der Standardabhängigkeitstyp, der verwendet wird, wenn kein anderer Abhängigkeitstyp angegeben ist.
* **Beenden-Beenden (ff)**: Die Vorgängeraufgabe muss beendet sein, bevor die abhängige Aufgabe beendet werden kann.
* **Start-Start (ss)**: Die Vorgängeraufgabe muss beginnen, bevor die abhängige Aufgabe gestartet werden kann. Die abhängige Aufgabe kann erst gestartet werden, wenn mindestens der Vorgänger gestartet wurde.
* **Start-Ende (sf)**: Die Vorgängeraufgabe muss beginnen, bevor die abhängige Aufgabe abgeschlossen werden kann. Sie können die abhängige Aufgabe starten, bevor der Vorgänger beginnt, aber Sie können sie nicht abschließen, es sei denn, der Vorgänger hat begonnen.
* **Geplanter Start (sd)**: Hiermit wird eine Aufgabe als „Beenden-Start“ geplant, aber der tatsächliche Erzwingungstyp ist „Beenden-Beenden“. Wenn Sie diese Option verwenden, wird die abhängige Aufgabe so geplant, dass sie nach Abschluss der Vorgängeraufgabe beginnt. Die Durchsetzung sorgt jedoch dafür, dass die abhängige Aufgabe jederzeit beginnen, aber erst abgeschlossen werden kann, wenn die Vorgängeraufgabe abgeschlossen ist.

>[!NOTE]
>
>Die Abkürzungen für die Abhängigkeitstypen werden in Aufgabenlisten zum Definieren von Vorgängerbeziehungen verwendet. Weitere Informationen finden Sie unter [Beispiele für Vorgängerwerte in einer Aufgabenliste](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md#examples-of-predecessor-values-in-a-task-list) in [Übersicht über Aufgabenvorgänger](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md).

