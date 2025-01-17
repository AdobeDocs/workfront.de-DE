---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: Szenario,Leistung
navigation-topic: get-started-with-workfront-fusion-2-0
title: Leitplanken für die Leistung von Adobe Workfront Fusion
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: cdf46eb1-46ba-4707-9063-b76899195a2c
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 1%

---

# Leitplanken für [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben.
>
>Die Informationen in diesem Artikel finden Sie jetzt im Artikel:
>
>* [Limits bei der Leistung von Adobe Workfront Fusion](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/scenarios/fusion-performance-guardrails.html)
>
>Bitte aktualisieren Sie alle Lesezeichen.
>
>Dieser Artikel wird nicht mehr aktualisiert und in naher Zukunft entfernt.

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] benötigt zusätzlich zu einer [!DNL Adobe Workfront license] eine [!DNL Adobe Workfront Fusion].

Die Arbeitsautomatisierung erfordert eine schnelle Verarbeitung, sodass [!DNL Adobe Workfront Fusion] für hohe Leistung entwickelt wurde. Da langwierige Szenarien die Geschwindigkeit Ihrer Arbeit verlangsamen können, haben wir [!DNL Workfront Fusion] mit leistungserhaltenden Leitplanken entwickelt, die die Ausführungszeit, die Datengröße und andere Szenario-Parameter beschränken. [!DNL Workfront Fusion] Designer sollten sich dieser Leitplanken bewusst sein und sie in ihre Entwurfsverfahren integrieren.

## Browser

* Workfront Fusion unterstützt nur Chrome-basierte Browser.

## Szenarios

* Das standardmäßige Ausführungstimeout für das Szenario beträgt **40 Minuten**. Wenn die Ausführung diese Zeitüberschreitung erreicht, unterbricht [!DNL Workfront Fusion] je nach Szenario die Ausführung des Szenarios nach dem nächsten Zyklus oder Vorgang. Dadurch wird das Szenario kurz nach Erreichen der 40-Minuten-Grenze beendet
* Die maximale Größe einer Szenario-Blueprint beträgt **5 MB**, wir empfehlen jedoch, die Szenario-Größe unter **3 MB** zu belassen.

  Mobile-App-Module, die Daten mit einer großen Anzahl von Feldern erstellen oder aktualisieren, können zu sehr großen Blueprints führen.

   * Achten Sie bei Verwendung der [!DNL Workfront]-App darauf, nur die Felder auszuwählen, die für Ihre Anwendungsfälle zum Erstellen oder Aktualisieren erforderlich sind.
   * Verwenden Sie bei der Verwendung anderer Programme benutzerdefinierte API-Module, um mit jedem Datensatztyp zu interagieren, der über eine große Anzahl von Feldern verfügt.

* Es gibt zwar keine Begrenzung für die Anzahl der Module in einem Szenario, aber Szenarien mit mehr als 150 Modulen beeinträchtigen die Leistung Ihres [!DNL Workfront Fusion]. Aus diesem Grund empfehlen wir nicht, Szenarien mit mehr als 150 Modulen zu erstellen.

## Vorgänge

* Das standardmäßige Zeitlimit für Vorgänge beträgt in der Regel **40 Sekunden**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## Dateien

* Die Gesamtverarbeitungskapazität von Fusion beträgt **1 GB**. Das Limit basiert auf den Gesamtspeicherkosten. Jeder Arbeitsgang trägt zu diesen Kosten bei. Wenn eine einzelne Datei mit 400 MB heruntergeladen und hochgeladen wird, würden die Gesamtkosten für die Dateikapazität 800 MB betragen.
* Unternehmen, die den Workfront Ultimate-Plan verwenden, haben Zugriff auf eine Dateiverarbeitung, die über 1 GB hinausgeht. Die Fusion-Plattform kann einzelne Dateien mit bis zu 15 GB für eine einzelne Aktion (z. B. das Hochladen einer Datei) unterstützen, es gibt jedoch andere Faktoren, die die Datenübertragung beeinflussen. Die Dateigrößenbeschränkung einer einzelnen Aktion hängt davon ab, mit welchem Web-Service sich Fusion verbindet. Die Datenübertragung ist die Gesamtverarbeitung für eine einzelne Ausführung. Dies bedeutet, dass mehrere Aktionen in einer einzigen Ausführung zur gesamten Datenübertragung beitragen. Fusion verarbeitet Dateien, bis die Ausführungsgrenze von 40 Minuten erreicht ist.

  Weitere Informationen finden Sie unter [Arbeiten mit großen Dateien in Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/get-started/fusion-large-files.md).


## Speicherauslastung des Servers

* Die Speichernutzung des Servers für eine einzelne Ausführung ist auf **1 GB** beschränkt.

  Viele Faktoren, wie z. B. große Dateien oder komplexe Module, können die Speichernutzung des Servers auf eine Weise beeinflussen, die schwer vorherzusagen oder zu steuern ist. Aus diesem Grund kann Ihre Szenarioausführung das 1 GB-Speicherlimit überschreiten, auch wenn das Szenario allen anderen Leistungs-Schutzmechanismen folgt. Wenn Sie die Speicherbegrenzung überschreiten, schlägt die Ausführung fehl.

## Webhooks

* Die standardmäßige Maximalgröße einer Payload beträgt **5 MB**.
* Webhooks sind auf **100 Anfragen pro Sekunde beschränkt**. Wenn dieses Limit erreicht ist, sendet Workfront Fusion den Status 429 ([!UICONTROL Zu viele Anfragen]).
* [!DNL Workfront Fusion] speichert Webhook-Payloads 30 Tage lang. Der Zugriff auf eine Webhook-Payload mehr als 30 Tage nach dem Empfang führt zu dem Fehler &quot;[!UICONTROL Fehler beim Lesen der Datei aus dem Speicher.]&quot;
* Webhooks werden automatisch deaktiviert, wenn einer der folgenden Punkte zutrifft:

   * Der Webhook wurde seit mehr als 5 Tagen mit keinem Szenario verbunden
   * Der Webhook wird nur in inaktiven Szenarien verwendet, die seit mehr als 30 Tagen inaktiv sind.

* Deaktivierte Webhooks werden automatisch gelöscht und von der Registrierung entfernt, wenn sie mit keinem Szenario verbunden sind und sich seit mehr als 30 Tagen im Status Deaktiviert befinden.

## Ausführungsverlauf

* Die Ausführungsverlaufsprotokolle sind auf eine Größe von **100 MB)**. Wenn der Ausführungsverlauf diese Größe überschreitet, werden nur die ersten 100 MB angezeigt.
* Wenn ein Szenario mehrere gleichzeitige Ausführungen hat. Nur 5 Ausführungen werden im Bereich Ausführungen auf der Seite mit den Szenario-Details angezeigt. Dies gilt auch, wenn mehr als 5 Ausführungen laufen.

## Unvollständige Ausführungen

* Unvollständige Ausführungen sind auf eine Gesamtgröße von **500 MB** beschränkt. Wenn das Limit von 500 MB erreicht wird, werden keine unvollständigen Ausführungen mehr gespeichert.

## Weitere Zustellversuche

* Wenn bei Verwendung des Break-Moduls und Angabe der Wiederholungsanweisung ein Szenario innerhalb eines Zeitrahmens von 2 Minuten 10-mal nacheinander fehlschlägt, wird das Szenario automatisch deaktiviert.

