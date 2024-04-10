---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Szenario,Leistung
navigation-topic: get-started-with-workfront-fusion-2-0
title: Leitplanken für die Leistung von Adobe Workfront Fusion
description: Adobe Workfront Fusion erfordert zusätzlich zu einer Adobe Workfront-Lizenz eine Adobe Workfront Fusion-Lizenz.
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: 370743780e5be419eb6a8c432619e5d76acfbfce
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 1%

---

# [!DNL Adobe Workfront Fusion] Leitplanken für die Leistung

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] Erfordert eine [!DNL Adobe Workfront Fusion] Lizenz zusätzlich zu einer [!DNL Adobe Workfront license].

Die Arbeitsautomatisierung erfordert eine schnelle Verarbeitung. [!DNL Adobe Workfront Fusion] ist für hohe Leistung konzipiert. Da langwierige Szenarien das Arbeitstempo verlangsamen können, haben wir Folgendes entworfen [!DNL Workfront Fusion] mit leistungserhaltenden Leitplanken, die die Ausführungszeit, die Datengröße und andere Szenario-Parameter begrenzen. [!DNL Workfront Fusion] Designer sollten sich dieser Leitplanken bewusst sein und sie in ihre Design-Praktiken integrieren.

## Browser

Workfront Fusion unterstützt nur Chrome-basierte Browser.

## Szenarios

* Das standardmäßige Ausführungszeitlimit für das Szenario ist **40 Minuten**. Wenn die Ausführung diese Zeitüberschreitung erreicht, [!DNL Workfront Fusion] Unterbricht die Ausführung des Szenarios je nach Szenario nach dem nächsten Zyklus oder Vorgang. Dadurch wird das Szenario kurz nach Erreichen der 40-Minuten-Grenze beendet
* Die maximale Größe eines Szenario-Blueprints beträgt **5 MB** Es wird jedoch empfohlen, die Szenario-Größe unter zu halten **3 MB**.

  Mobile-App-Module, die Daten mit einer großen Anzahl von Feldern erstellen oder aktualisieren, können zu sehr großen Blueprints führen.

   * Bei Verwendung der [!DNL Workfront] -App verwenden, achten Sie darauf, nur die Felder auszuwählen, die für Ihre Anwendungsfälle zum Erstellen oder Aktualisieren von Daten benötigt werden.
   * Verwenden Sie bei der Verwendung anderer Programme benutzerdefinierte API-Module, um mit jedem Datensatztyp zu interagieren, der über eine große Anzahl von Feldern verfügt.

* Es gibt zwar keine Begrenzung für die Anzahl der Module in einem Szenario, aber Szenarien mit mehr als 150 Modulen beeinträchtigen die Leistung Ihrer [!DNL Workfront Fusion] System. Aus diesem Grund empfehlen wir nicht, Szenarien mit mehr als 150 Modulen zu erstellen.

## Vorgänge

* Das standardmäßige Zeitlimit für Vorgänge beträgt in der Regel **40 Sekunden**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## Dateien

* Die Gesamtverarbeitungskapazität von Fusion für Dateien beträgt **1 GB**. Das Limit basiert auf den Gesamtspeicherkosten. Jeder Arbeitsgang trägt zu diesen Kosten bei. Wenn eine einzelne Datei mit 400 MB heruntergeladen und hochgeladen wird, würden die Gesamtkosten für die Dateikapazität 800 MB betragen.

## Server-Speicherauslastung

* Die Speicherauslastung des Servers für eine einzelne Ausführung ist begrenzt auf **1 GB**.

  Viele Faktoren, wie z. B. große Dateien oder komplexe Module, können die Speichernutzung des Servers auf eine Weise beeinflussen, die schwer vorherzusagen oder zu kontrollieren ist. Aus diesem Grund kann die Ausführung des Szenarios die Speicherbegrenzung von 1 GB überschreiten, auch wenn das Szenario allen anderen Leistungs-Schutzmechanismen folgt. Wenn Sie die Speicherbegrenzung überschreiten, schlägt die Ausführung fehl.

## Webhooks

* Die standardmäßige maximale Größe einer Payload beträgt **5 MB**.
* Webhooks sind beschränkt auf **100 Anfragen pro Sekunde**. Wenn diese Grenze erreicht ist, sendet Workfront Fusion eine 429 ([!UICONTROL Zu viele Anfragen]Status ).
* [!DNL Workfront Fusion] speichert Webhook-Payloads 30 Tage lang. Der Zugriff auf eine Webhook-Payload mehr als 30 Tage nach dem Empfang führt zum Fehler &quot;[!UICONTROL Datei konnte nicht aus dem Speicher gelesen werden.]&quot;
* Webhooks werden automatisch deaktiviert, wenn einer der folgenden Punkte zutrifft:

   * Der Webhook wurde seit mehr als 5 Tagen mit keinem Szenario verbunden
   * Der Webhook wird nur in inaktiven Szenarien verwendet, die seit mehr als 30 Tagen inaktiv sind.

* Deaktivierte Webhooks werden automatisch gelöscht und die Registrierung aufgehoben, wenn sie mit keinem Szenario verbunden sind und sich seit mehr als 30 Tagen im Status Deaktiviert befinden.

## Ausführungsverlauf

* Ausführungsverlaufsprotokolle sind auf eine Größe von begrenzt. **100 MB**. Wenn der Ausführungsverlauf diese Größe überschreitet, werden nur die ersten 100 MB angezeigt.

## Weitere Zustellversuche

Wenn bei Verwendung des Break-Moduls und Angabe der Wiederholungsanweisung ein Szenario innerhalb eines Zeitrahmens von 2 Minuten 10-mal nacheinander fehlschlägt, wird das Szenario automatisch deaktiviert.
