---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: Übersicht über Aufgabenabhängigkeitstypen
description: Abhängigkeitstypen beziehen sich auf die Vorgängerbeziehungen zwischen Aufgaben. Sie definieren, wann die abhängige Aufgabe basierend auf dem Start oder der Fertigstellung ihres Vorgängers starten oder beenden kann.
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
source-git-commit: 45c82f659d02dca69d2a2c390b084330773d4252
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Übersicht über Aufgabenabhängigkeitstypen

Abhängigkeitstypen beziehen sich auf die Vorgängerbeziehungen zwischen Aufgaben. Sie definieren, wann die abhängige Aufgabe basierend auf dem Start oder der Fertigstellung ihres Vorgängers starten oder beenden kann.

>[!IMPORTANT]
>
>Adobe Workfront schränkt die abhängigen Aufgaben nicht vom Starten oder Beenden basierend auf den Abhängigkeitstypen ein, es sei denn, die Vorgängerbeziehungen werden erzwungen. Informationen zur Durchsetzung von Vorgängern finden Sie unter [Durchsetzen von Vorgängern](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

Sie müssen den Abhängigkeitstyp einer Vorgängerbeziehung angeben, wenn Sie diese Beziehung zwischen Ihren Aufgaben herstellen.

Weitere Informationen zu Vorgängern finden Sie unter [Übersicht über die Vorgänger von Aufgaben](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Die folgenden Workfront-Abhängigkeitstypen sind verfügbar:

* **Finish-Start (fs)**: Die Vorgängeraufgabe muss beendet sein, bevor die abhängige Aufgabe gestartet werden kann. Dies ist der Standardabhängigkeitstyp, der verwendet wird, wenn kein anderer Abhängigkeitstyp angegeben ist.
* **Finish-Finish (ff)**: Die Vorgängeraufgabe muss beendet sein, bevor die abhängige Aufgabe beendet werden kann.
* **Start-Start (ss)**: Die Vorgängeraufgabe muss beginnen, bevor die abhängige Aufgabe gestartet werden kann. Sie können die abhängige Aufgabe nur starten, wenn der Vorgänger mindestens gestartet hat.
* **Start-Finish (sf)**: Die Vorgängeraufgabe muss beginnen, bevor die abhängige Aufgabe beendet werden kann. Sie können die abhängige Aufgabe starten, bevor der Vorgänger gestartet wird, aber erst beenden Sie sie, wenn der Vorgänger gestartet wurde.
* **Geplanter Start (sd)**: Hiermit wird eine Aufgabe als &quot;Finish-Start&quot;geplant, der tatsächliche Durchsetzungstyp ist jedoch &quot;Finish-Finish&quot;. Wenn Sie dies verwenden, wird geplant, dass die abhängige Aufgabe nach Abschluss der Vorgängeraufgabe beginnt. Die Durchsetzung macht es jedoch so, dass die abhängige Aufgabe jederzeit beginnen kann, aber nicht beendet werden kann, bis die Vorgängeraufgabe beendet ist.

>[!NOTE]
>
>Die Abkürzungen für die Abhängigkeitstypen werden in Aufgabenlisten verwendet, um Vorgängerbeziehungen zu definieren. Weitere Informationen finden Sie unter [Beispiele für Vorgängerwerte in einer Aufgabenliste](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md#examples-of-predecessor-values-in-a-task-list) in [Übersicht über die Vorgänger von Aufgaben](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md).

