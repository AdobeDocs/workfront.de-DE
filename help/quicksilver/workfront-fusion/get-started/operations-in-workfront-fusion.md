---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Betrieb in Adobe Workfront Fusion
description: Ein Vorgang in Adobe Workfront Fusion ist eine Aufgabe, die von einem Modul ausgeführt wird. Zu Tracking-Zwecken ist jede von einem Modul ausgeführte erfolgreiche Aktion ein Vorgang.
author: Becky
feature: Workfront Fusion
exl-id: 34268fb6-e485-42be-b751-3ee79bbf5797
source-git-commit: abb021a6857f8016d4f8b6bcf99fe818e47faea6
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Vorgänge in [!DNL Adobe Workfront Fusion]

Ein Vorgang in [!DNL Adobe Workfront Fusion] ist eine Aufgabe, die von einem Modul ausgeführt wird. Zu Tracking-Zwecken ist jede von einem Modul ausgeführte erfolgreiche Aktion ein Vorgang.

## Erwägungen beim Zählen der Anzahl der Vorgänge

* Im Allgemeinen gilt jede erfolgreiche Ausführung eines Aktionsschritts als Vorgang.

* Das erste Modul in einem Szenario wird nur einmal ausgeführt und immer als ein Vorgang gezählt, auch wenn es kein Bundle zurückgibt.

* Wie oft der Rest der Module ausgeführt wird, hängt von der Anzahl der Pakete ab, die verarbeitet werden müssen.  Eine Ausführung eines Moduls für ein Bundle ist ein Vorgang. Eine Ausnahme ist das Aggregatormodul, das pro verarbeiteten Bundle als ein Vorgang gezählt wird.

* Vorgänge werden in der Phase [!UICONTROL Fertigstellung] der Ausführung eines Szenarios gezählt.

* Die folgenden Vorgänge werden als **nicht** gezählt:

   * Alle Filterschritte.

   * Jede Aktion, die fehlerhaft oder angehalten wird.

   * Jede Route, die nicht ausgeführt wird, weil die Regeln der Route nicht eingehalten wurden, z. B. Fallback oder deaktivierte Routen.

   * Jede Aktion, die nicht ausgeführt wird, entweder weil ein Filter keine Daten zulässt oder weil das Szenario aufgrund eines Fehlers angehalten wurde.

## Betriebsbeschränkungen

Ihr Unternehmen hat möglicherweise eine monatliche Betriebsgrenze. Dies basiert auf dem [!DNL Workfront] -Plan, den Ihr Unternehmen erworben hat. Der Plan [!UICONTROL Ultimate] [!DNL Workfront] bietet unbegrenzte Operationen.

Wenn Ihr Unternehmen eine monatliche Beschränkung hat, werden Sie benachrichtigt, wenn Sie sich dem Grenzwert nähern. Wenn Sie das Limit überschreiten, kontaktiert [!DNL Workfront] Ihre Organisation, um sicherzustellen, dass Ihr Plan Ihren Anforderungen entspricht.

## Anzahl der in den letzten 30 Tagen durchgeführten Vorgänge anzeigen

Sie können eine Grafik mit der Anzahl der durchgeführten Vorgänge sehen. Diese Diagramme sind an den folgenden Orten verfügbar:

* **Organisations-Dashboard**: Vorgänge, die von der gesamten Organisation verwendet werden
* **Team-Dashboard**: Vorgänge, die von Szenarien verwendet werden, die diesem Team gehören ([!DNL Adobe Experience Cloud] nur)
* **Seite mit Details zum Szenario**: Von diesem Szenario verwendete Vorgänge ([!DNL Adobe Experience Cloud] nur)
