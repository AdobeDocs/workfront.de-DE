---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Betrieb in Adobe Workfront Fusion
description: Ein Vorgang in Adobe Workfront Fusion ist eine Aufgabe, die von einem Modul ausgeführt wird. Zu Tracking-Zwecken ist jede von einem Modul ausgeführte erfolgreiche Aktion ein Vorgang.
author: Becky
feature: Workfront Fusion
source-git-commit: 8d82fd10a6742f13f62b5479fafa5b42e567700f
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Vorgänge in [!DNL Adobe Workfront Fusion]

Ein Vorgang in [!DNL Adobe Workfront Fusion] ist eine Aufgabe, die von einem Modul ausgeführt wird. Zu Tracking-Zwecken ist jede von einem Modul ausgeführte erfolgreiche Aktion ein Vorgang.

## Erwägungen beim Zählen der Anzahl der Vorgänge

* Im Allgemeinen gilt jede erfolgreiche Ausführung eines Aktionsschritts als Vorgang.

* Das erste Modul in einem Szenario wird nur einmal ausgeführt und immer als ein Vorgang gezählt, auch wenn es kein Bundle zurückgibt.

* Wie oft der Rest der Module ausgeführt wird, hängt von der Anzahl der Pakete ab, die verarbeitet werden müssen.  Eine Ausführung eines Moduls für ein Bundle ist ein Vorgang. Eine Ausnahme ist das Aggregatormodul, das pro verarbeiteten Bundle als ein Vorgang gezählt wird.

* Vorgänge werden auf der [!UICONTROL Fertigstellung] -Phase der Ausführung eines Szenarios.

* Die folgenden **not** als Vorgänge gezählt werden:

   * Alle Filterschritte.

   * Jede Aktion, die fehlerhaft oder angehalten wird.

   * Jede Route, die nicht ausgeführt wird, weil die Regeln der Route nicht eingehalten wurden, z. B. Fallback oder deaktivierte Routen.

   * Jede Aktion, die nicht ausgeführt wird, entweder weil ein Filter keine Daten zulässt oder weil das Szenario aufgrund eines Fehlers angehalten wurde.

## Betriebsbeschränkungen

Ihr Unternehmen hat möglicherweise eine monatliche Betriebsgrenze. Dies basiert auf der [!DNL Workfront] planen, dass Ihr Unternehmen einen Kauf tätigt. Die [!UICONTROL Ultimate] [!DNL Workfront] Plan bietet unbegrenzte Betriebsmöglichkeiten.

Wenn Ihr Unternehmen eine monatliche Beschränkung hat, werden Sie benachrichtigt, wenn Sie sich dem Grenzwert nähern. Wenn Sie die Grenze überschreiten, [!DNL Workfront] wird sich an Ihre Organisation wenden, um sicherzustellen, dass Ihr Plan Ihren Anforderungen entspricht.

## Anzahl der in den letzten 30 Tagen durchgeführten Vorgänge anzeigen

Sie können eine Grafik mit der Anzahl der durchgeführten Vorgänge sehen. Diese Diagramme sind an den folgenden Stellen verfügbar:

* **Organisations-Dashboard**: Von der gesamten Organisation verwendete Vorgänge
* **Team-Dashboard**: Vorgänge, die in Szenarien verwendet werden, die diesem Team gehören ([!DNL Adobe Experience Cloud] nur)
* **Seite mit Details zum Szenario**: Von diesem Szenario verwendete Vorgänge ([!DNL Adobe Experience Cloud] nur)

