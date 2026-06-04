---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Übersicht über den Projektaktualisierungstyp
description: Der Aktualisierungstyp eines Projekts gibt an, wie Adobe Workfront die Zeitleiste eines Projekts berechnet. Änderungen am Projektplan können zu Triggern in der Zeitleiste des Projekts führen. Die Zeitleiste des Projekts muss automatisch oder manuell neu berechnet werden, um sicherzustellen, dass es mit diesen Änderungen auf dem neuesten Stand ist.
author: Alina
feature: Work Management
exl-id: a6394961-2ac8-4b95-aa1b-dba8108c612f
TQID: https://experienceleague.adobe.com/bLY-ljw7HxR2kXRpi9jzMkSKbGSKhDrvzogvK5-wZ90
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 520
ht-degree: 0%

---

# Überblick über den Projektaktualisierungstyp

Der Aktualisierungstyp eines Projekts gibt an, wie Adobe Workfront die Zeitleiste eines Projekts berechnet. Änderungen am Projektplan können zu Triggern in der Zeitleiste des Projekts führen. Die Zeitleiste des Projekts muss automatisch oder manuell neu berechnet werden, um sicherzustellen, dass es mit diesen Änderungen auf dem neuesten Stand ist.

Informationen zur Neuberechnung der Projekt-Zeitleiste finden Sie unter [Neuberechnen von Projekt-Zeitleisten](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

## Projektaktualisierungstypen

Es gibt vier Aktualisierungstypen für ein Projekt, je nachdem, wann Workfront die Zeitleiste des Projekts neu berechnen soll. Wählen Sie einen Aktualisierungstyp aus der folgenden Liste aus.

Informationen zum Aktualisieren des Aktualisierungstyps des Projekts finden Sie unter [Auswahl des Aktualisierungstyps für das Projekt](../../../manage-work/projects/manage-projects/select-project-update-type.md).

>[!IMPORTANT]
>
>Wenn der Zeitplan eines Projekts länger als 15 Jahre ist, berechnet Workfront den Zeitplan nicht automatisch oder bei einer Änderung. Der Aktualisierungstyp eines Projekts, das länger als 15 Jahre dauert, ist immer „Manuell“.

* **Automatisch und Bei Änderung** Dies ist die Standardeinstellung. Die Zeitleiste des Projekts wird jedes Mal aktualisiert, wenn eine Änderung im Projekt oder in einem anderen Projekt auftritt, von dem die Zeitleiste abhängig ist. Die Zeitleiste des Projekts wird ebenfalls jede Nacht aktualisiert.\
  Dies ist die empfohlene Einstellung, da sie sicherstellt, dass die Zeitleiste des Projekts immer auf dem neuesten Stand ist.

  Wenn Sie eine Aufgabe oder das Projekt aktualisieren und eine Neuberechnung der Zeitleiste durchführen, werden alle verfügbaren Daten sofort angezeigt, sodass Sie weiterarbeiten können. Bei Projekten mit mehr als 100 Aufgaben werden Datumsangaben, für die längere Berechnungen erforderlich sind, abgeblendet.

  ![Datumsangaben bei Inline-Bearbeitung abgeblendet](assets/dates-dimmed-when-insline-editing-350x146.png)

  Dies bedeutet, dass die Neuberechnung noch nicht abgeschlossen ist und sich die Daten ändern können.

* **Nur Änderung** Die Zeitleiste des Projekts wird jedes Mal aktualisiert, wenn eine Änderung im Projekt oder in einem anderen Projekt erfolgt, von dem die Zeitleiste abhängig ist. Geplante Aktualisierungen werden nicht durchgeführt.\
  Sie sollten diese Option auswählen, wenn Sie sich Sorgen über die Systemleistung machen und wenn Änderungen selten im Projekt oder in anderen Projekten auftreten, von denen die Zeitleiste abhängig ist.

* **Nur automatisch** Die Zeitleiste des Projekts wird jede Nacht aktualisiert. Sie wird nicht sofort nach den Änderungen aktualisiert.\
  Sie sollten diese Option auswählen, wenn Sie sich Sorgen über die Systemleistung machen und wenn im Projekt oder in anderen Projekten, von denen die Timeline abhängig ist, täglich viele Änderungen auftreten.

  >[!NOTE]
  >
  >Ein Projekt wird nicht jede Nacht automatisch neu berechnet, wenn es sich im Status „Planung“ befindet. Er wird nur bei Änderung neu berechnet.

* **Nur manuell:** Die Projekt-Zeitleiste wird nur aktualisiert, wenn Sie die Option **Zeitleisten neu berechnen** auswählen, wie im Abschnitt „Manuelle Neuberechnung“ im Artikel [Neuberechnen von Projekt-Zeitleisten](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md) beschrieben.\
  Sie können diese Option auswählen, wenn Sie mehrere Änderungen am Projekt gleichzeitig vornehmen und die Neuberechnung der Zeitleiste nach allen Änderungen (und nicht nach jeder einzelnen Änderung) durchgeführt werden soll.
