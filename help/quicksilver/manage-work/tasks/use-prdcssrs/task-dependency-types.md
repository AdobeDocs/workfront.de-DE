---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: Übersicht über Aufgabenabhängigkeitstypen
description: Abhängigkeitstypen beziehen sich auf die Vorgängerbeziehungen zwischen Aufgaben. Sie definieren, wann die abhängige Aufgabe basierend auf dem Anfang oder Ende ihrer Vorgängerin beginnen oder beenden kann.
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
TQID: https://experienceleague.adobe.com/AioKERGt0FLv1eBE5-evwa2d35fItwknWI-ZouBECSo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 322
ht-degree: 1%

---

# Überblick über Typen von Aufgabenabhängigkeiten

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

