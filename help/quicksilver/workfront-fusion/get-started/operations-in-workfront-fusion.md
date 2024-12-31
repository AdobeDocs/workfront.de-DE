---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Betrieb in Adobe Workfront Fusion
description: Ein Vorgang in Adobe Workfront Fusion ist eine Aufgabe, die von einem Modul ausgeführt wird. Zu Tracking-Zwecken ist jede erfolgreiche Aktion, die von einem Modul ausgeführt wird, ein Vorgang.
author: Becky
feature: Workfront Fusion
exl-id: 34268fb6-e485-42be-b751-3ee79bbf5797
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Vorgänge in [!DNL Adobe Workfront Fusion]

Ein Vorgang in [!DNL Adobe Workfront Fusion] ist eine Aufgabe, die von einem Modul ausgeführt wird. Zu Tracking-Zwecken ist jede erfolgreiche Aktion, die von einem Modul ausgeführt wird, ein Vorgang.

## Überlegungen beim Zählen der Anzahl der Vorgänge

* Im Allgemeinen wird jede erfolgreiche Ausführung von Aktionsschritten als Vorgang betrachtet.

* Das erste Modul in einem Szenario wird nur einmal ausgeführt und immer als ein Vorgang gezählt, auch wenn kein Bundle zurückgegeben wird.

* Wie oft die übrigen Module ausgeführt werden, hängt von der Anzahl der Bundles ab, die sie verarbeiten müssen.  Ein Durchgang eines Moduls für ein Bundle ist ein Vorgang. Eine Ausnahme bildet das Aggregator-Modul, das als ein Vorgang pro Satz von Bundles gezählt wird, die verarbeitet werden.

* Vorgänge werden bei der [!UICONTROL Finalisierung] einer Szenarioausführung gezählt.

* Folgende Vorgänge werden **nicht** gezählt:

   * Alle Filterschritte.

   * Jede Aktion, die einen Fehler verursacht oder angehalten wird.

   * Alle Routen, die nicht ausgeführt werden, weil die Regeln der Route nicht eingehalten wurden, z. B. Ausweich- oder deaktivierte Routen.

   * Jede Aktion, die nicht ausgeführt wird, entweder weil ein Filter keine Daten durchlässt oder weil das Szenario aufgrund eines Fehlers angehalten wurde.

## Limits für Operationen

In Ihrem Unternehmen gibt es möglicherweise ein monatliches Betriebslimit. Dies basiert auf dem [!DNL Workfront], den Ihr Unternehmen erworben hat. Der [!UICONTROL Ultimate]-[!DNL Workfront] bietet unbegrenzte Operationen.

Wenn Ihr Unternehmen ein monatliches Limit hat, werden Sie benachrichtigt, wenn Sie sich dem Limit nähern. Wenn Sie das Limit überschreiten, wenden [!DNL Workfront] sich an Ihr Unternehmen, um sicherzustellen, dass Ihr Plan Ihren Anforderungen entspricht.

## Anzahl der in den letzten 30 Tagen durchgeführten Vorgänge anzeigen

Sie können ein Diagramm sehen, das die Anzahl der ausgeführten Vorgänge anzeigt. Diese Diagramme sind an den folgenden Speicherorten verfügbar:

* **Organisations-Dashboard**: Von der gesamten Organisation verwendete Vorgänge
* **Team-Dashboard**: Vorgänge, die von Szenarien verwendet werden, die diesem Team gehören (nur [!DNL Adobe Experience Cloud])
* **Seite mit Szenario**: Von diesem Szenario verwendete Vorgänge (nur [!DNL Adobe Experience Cloud])
