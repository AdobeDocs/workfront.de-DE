---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: scenario,performance
navigation-topic: get-started-with-workfront-fusion-2-0
title: Limits bei der Leistung von Adobe Workfront Fusion
description: Adobe Workfront Fusion erfordert zusätzlich zu einer Adobe Workfront-Lizenz eine Adobe Workfront Fusion-Lizenz.
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: 229fd48d604385a1bfcaba2fd34eb6f3bbdde7a7
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] Leistungsgarantien

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] erfordert [!DNL Adobe Workfront Fusion] zusätzlich zu einer [!DNL Adobe Workfront license].

Die Arbeitsautomatisierung erfordert eine schnelle Verarbeitung. [!DNL Adobe Workfront Fusion] ist für hohe Leistung ausgelegt. Da langwierige Szenarien das Tempo Ihrer Arbeit verlangsamen können, haben wir [!DNL Workfront Fusion] mit leistungserhaltenden Limits, die die Ausführungszeit, Datengröße und andere Szenario-Parameter begrenzen. [!DNL Workfront Fusion] -Designer sollten sich dieser Limits bewusst sein und sie in ihre Designpraktiken integrieren.

## Szenarios

* Der standardmäßige Ausführungstimeout des Szenarios lautet **40 Minuten**. Wenn die Ausführung diesen Timeout erreicht, [!DNL Workfront Fusion] unterbricht je nach Szenario die Ausführung des Szenarios nach dem nächsten Zyklus oder Vorgang. Dadurch wird das Szenario kurz nach Erreichen der 40-Minuten-Grenze angehalten
* Die maximale Größe eines Szenario-Blueprints beträgt **5 MB** Wir empfehlen jedoch, die Szenario-Größe unter **3 MB**.

   App-Module, die Daten mit einer großen Anzahl von Feldern erstellen oder aktualisieren, können zu sehr großen Blueprints führen.

   * Bei Verwendung von [!DNL Workfront] nur die Felder auswählen, die für Ihre Anwendungsfälle zum Erstellen oder Aktualisieren benötigt werden.
   * Verwenden Sie bei Verwendung anderer Apps benutzerdefinierte API-Module, um mit jedem Datensatztyp zu interagieren, der über eine große Anzahl von Feldern verfügt.

* Es gibt zwar keine Obergrenze für die Anzahl der Module in einem Szenario, Szenarien mit mehr als 150 Modulen wirken sich jedoch negativ auf die Leistung Ihrer [!DNL Workfront Fusion] System. Daher empfehlen wir nicht, Szenarien mit mehr als 150 Modulen zu erstellen.

## Vorgänge

* Die standardmäßige Zeitüberschreitung bei Vorgängen ist normalerweise **40 Sekunden**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## Dateien

* Die Gesamtverarbeitungskapazität der Fusion für Dateien beträgt **1 GB**. Die Begrenzung basiert auf den Gesamtspeicherkosten. Jeder Vorgang trägt zu diesen Kosten bei. Wenn eine einzelne Datei von 400 MB heruntergeladen und hochgeladen wird, belaufen sich die Gesamtkosten für die Dateikapazität auf 800 MB.

## Speichernutzung des Servers

* Die Speichernutzung des Servers für eine einzelne Ausführung ist auf **1 GB**.

   Viele Faktoren, wie große Dateien oder komplexe Module, können die Speichernutzung von Servern auf eine Weise beeinflussen, die schwer vorherzusagen oder zu steuern ist. Aus diesem Grund kann die Ausführung Ihres Szenarios die Speichergrenze von 1 GB überschreiten, selbst wenn das Szenario alle anderen Leistungsgarantien erfüllt. Wenn Sie die Speicherbegrenzung überschreiten, schlägt die Ausführung fehl.

## Webhooks

* Die standardmäßige Maximalgröße einer Payload beträgt **5 MB**.
* Webhooks sind auf **100 Anfragen pro Sekunde**. Wenn diese Grenze erreicht ist, sendet Workfront Fusion einen 429 ([!UICONTROL Zu viele Anforderungen]).
* [!DNL Workfront Fusion] speichert Webhook-Payloads für 30 Tage. Wenn Sie mehr als 30 Tage nach dem Erhalt auf eine Webhook-Payload zugreifen, tritt der Fehler auf &quot;[!UICONTROL Datei konnte nicht aus Speicher gelesen werden.]&quot;
* Webhooks werden automatisch deaktiviert, wenn eine der folgenden Aktionen zutrifft:

   * Der Webhook ist seit mehr als 5 Tagen mit keinem Szenario verbunden
   * Der Webhook wird nur in inaktiven Szenarien verwendet, die seit mehr als 30 Tagen inaktiv sind.

* Deaktivierte Webhooks werden automatisch gelöscht und abgemeldet, wenn sie mit keinem Szenario verbunden sind und seit über 30 Tagen den Status deaktiviert haben.
