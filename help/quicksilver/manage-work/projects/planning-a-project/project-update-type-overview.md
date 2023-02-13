---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Übersicht über den Projektaktualisierungstyp
description: Der Aktualisierungstyp eines Projekts gibt an, wie Adobe Workfront die Timeline eines Projekts berechnet. Änderungen am Projektplan können zu Triggern in der Zeitleiste des Projekts führen. Der Zeitrahmen des Projekts muss automatisch oder manuell neu berechnet werden, um sicherzustellen, dass er mit diesen Änderungen auf dem neuesten Stand ist.
author: Alina
feature: Work Management
exl-id: a6394961-2ac8-4b95-aa1b-dba8108c612f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Übersicht über den Projektaktualisierungstyp

Der Aktualisierungstyp eines Projekts gibt an, wie Adobe Workfront die Timeline eines Projekts berechnet. Änderungen am Projektplan können zu Triggern in der Zeitleiste des Projekts führen. Der Zeitrahmen des Projekts muss automatisch oder manuell neu berechnet werden, um sicherzustellen, dass er mit diesen Änderungen auf dem neuesten Stand ist.

Informationen zur Neuberechnung der Projekt-Timeline finden Sie unter [Projektzeitpläne neu berechnen](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

## Projektaktualisierungstypen

Es gibt vier Aktualisierungstypen für ein Projekt, je nachdem, wann Workfront die Projekt-Timeline neu berechnen soll. Wählen Sie in der folgenden Liste einen Aktualisierungstyp aus.

Informationen zum Aktualisieren des Aktualisierungstyps des Projekts finden Sie unter [Wählen Sie den Projektaktualisierungstyp aus](../../../manage-work/projects/manage-projects/select-project-update-type.md).

>[!IMPORTANT]
>
>Wenn die Timeline eines Projekts länger als 15 Jahre ist, berechnet Workfront die Timeline nicht automatisch oder bei Änderung. Der Aktualisierungstyp eines Projekts, das länger als 15 Jahre dauert, ist immer Manuell.

* **Automatisch und Bei Änderung:** Dies ist die Standardeinstellung. Die Projekt-Timeline wird jedes Mal aktualisiert, wenn eine Änderung im Projekt oder in einem anderen Projekt erfolgt, von dem die Timeline abhängig ist. Die Projekt-Timeline wird auch jede Nacht aktualisiert. \
   Dies ist die empfohlene Einstellung, da sie sicherstellt, dass die Projekt-Timeline immer auf dem neuesten Stand ist.

   Wenn Sie eine Aufgabe oder das Projekt aktualisieren und eine Timeline-Neuberechnung Trigger haben, werden alle verfügbaren Daten sofort angezeigt, sodass Sie mit der Arbeit fortfahren können. Bei Projekten mit mehr als 100 Aufgaben werden Daten, die längere Berechnungen erfordern, abgeblendet dargestellt.

   ![](assets/dates-dimmed-when-insline-editing-350x146.png)

   Dies bedeutet, dass die Neuberechnung noch nicht abgeschlossen ist und sich die Daten ändern können.

* **Nur ändern:** Die Projekt-Timeline wird jedes Mal aktualisiert, wenn eine Änderung im Projekt oder in einem anderen Projekt erfolgt, von dem die Timeline abhängig ist. Geplante Aktualisierungen treten nicht auf.\
   Sie können diese Option auswählen, wenn Sie Bedenken hinsichtlich der Systemleistung haben und nur selten Änderungen am Projekt oder an anderen Projekten auftreten, von denen die Timeline abhängig ist.

* **Nur Automatisch:** Die Projektzeitleiste wird jede Nacht aktualisiert. sie wird nicht sofort aktualisiert, nachdem Änderungen vorgenommen wurden.\
   Sie können diese Option auswählen, wenn Sie Bedenken hinsichtlich der Systemleistung haben und wenn täglich im Projekt oder in anderen Projekten, von denen die Timeline abhängig ist, viele Änderungen auftreten.

   >[!NOTE]
   >
   >Ein Projekt berechnet nicht automatisch jede Nacht neu, wenn es sich im Planungsstatus befindet. Es wird nur bei Veränderung neu berechnet.

* **Nur manuell:** Die Projekt-Timeline wird nur aktualisiert, wenn Sie die Option zum **Zeitleisten neu berechnen**, wie im Abschnitt &quot;Manuelle Neuberechnung&quot;im Artikel beschrieben [Projektzeitpläne neu berechnen](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
   Sie können diese Option auswählen, wenn Sie gleichzeitig viele Änderungen am Projekt vornehmen und möchten, dass die Timeline-Neuberechnung erfolgt, nachdem alle Änderungen vorgenommen wurden (und nicht nach jeder einzelnen Änderung).
