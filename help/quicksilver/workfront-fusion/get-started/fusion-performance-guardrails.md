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
source-git-commit: 7c27dc98c4ce59d598be537a1f09c6eddf9bce42
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---

# [!DNL Adobe Workfront Fusion] Leistungsgarantien

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] erfordert zusätzlich zu einem [!DNL Adobe Workfront license] eine [!DNL Adobe Workfront Fusion] -Lizenz.

Die Arbeitsautomatisierung erfordert eine schnelle Verarbeitung, daher ist [!DNL Adobe Workfront Fusion] für hohe Leistung ausgelegt. Da langwierige Szenarien das Tempo Ihrer Arbeit verlangsamen können, haben wir [!DNL Workfront Fusion] mit leistungserhaltenden Limits entwickelt, die die Ausführungszeit, Datengröße und andere Szenario-Parameter begrenzen. [!DNL Workfront Fusion] -Designer sollten sich dieser Limits bewusst sein und sie in ihre Designpraktiken integrieren.

## Browser

* Workfront Fusion unterstützt nur Chrome-basierte Browser.

## Szenarios

* Der standardmäßige Ausführungstimeout des Szenarios ist **40 Minuten**. Wenn die Ausführung diesen Timeout erreicht, unterbricht [!DNL Workfront Fusion] die Ausführung des Szenarios nach dem nächsten Zyklus oder Vorgang, je nach Szenario. Dadurch wird das Szenario kurz nach Erreichen der 40-Minuten-Grenze angehalten
* Die maximale Größe eines Szenario-Blueprints beträgt **5 MB**, wir empfehlen jedoch, die Szenariogröße unter **3 MB** zu belassen.

  App-Module, die Daten mit einer großen Anzahl von Feldern erstellen oder aktualisieren, können zu sehr großen Blueprints führen.

   * Stellen Sie bei Verwendung der [!DNL Workfront] -App sicher, dass Sie nur die Felder auswählen, die für Ihre Anwendungsfälle zum Erstellen oder Aktualisieren erforderlich sind.
   * Verwenden Sie bei Verwendung anderer Apps benutzerdefinierte API-Module, um mit jedem Datensatztyp zu interagieren, der über eine große Anzahl von Feldern verfügt.

* Es gibt zwar keine Obergrenze für die Anzahl der Module in einem Szenario, Szenarien mit mehr als 150 Modulen wirken sich jedoch negativ auf die Leistung Ihres [!DNL Workfront Fusion]-Systems aus. Aus diesem Grund empfehlen wir nicht, Szenarien mit über 150 Modulen zu erstellen.

## Vorgänge

* Der Standardwert für das Zeitlimit für den Vorgang ist normalerweise **40 Sekunden**.

<!--
* The operation timeout for calls to Adobe Workfront is **120 seconds**.
-->

## Dateien

* Die Gesamtverarbeitungskapazität von Fusion für Dateien beträgt **1 GB**. Die Begrenzung basiert auf den Gesamtspeicherkosten. Jeder Vorgang trägt zu diesen Kosten bei. Wenn eine einzelne Datei von 400 MB heruntergeladen und hochgeladen wird, belaufen sich die Gesamtkosten für die Dateikapazität auf 800 MB.
* Organisationen mit Workfront Ultimate-Abo haben Zugriff auf eine Dateiverarbeitungssteigerung von mehr als 1 GB. Die Fusion-Plattform kann einzelne Dateien mit bis zu 15 GB für eine einzelne Aktion unterstützen (z. B. Upload-Datei). Es gibt jedoch andere Faktoren, die sich auf die Datenübertragung auswirken. Die Dateigrößenbeschränkung für einzelne Aktionen hängt vom Webdienst ab, mit dem Fusion eine Verbindung herstellt. Die Datenübertragung ist die Gesamtverarbeitung für eine einzelne Ausführung. Das bedeutet, dass mehrere Aktionen in einer Ausführung zur gesamten Datenübertragung beitragen. Fusion verarbeitet die Dateien, bis die Ausführungsgrenze von 40 Minuten erreicht ist.

  Weitere Informationen finden Sie unter [Arbeiten mit großen Dateien in Adobe Workfront Fusion](/help/quicksilver/workfront-fusion/get-started/fusion-large-files.md).


## Speichernutzung des Servers

* Die Speicherauslastung des Servers für eine einzelne Ausführung ist auf **1 GB** beschränkt.

  Viele Faktoren, wie große Dateien oder komplexe Module, können die Speichernutzung von Servern auf eine Weise beeinflussen, die schwer vorherzusagen oder zu steuern ist. Aus diesem Grund kann die Ausführung Ihres Szenarios die Speichergrenze von 1 GB überschreiten, selbst wenn das Szenario alle anderen Leistungsgarantien erfüllt. Wenn Sie die Speicherbegrenzung überschreiten, schlägt die Ausführung fehl.

## Webhooks

* Die standardmäßige Maximalgröße einer Payload beträgt **5 MB**.
* Webhooks sind auf **100 Anforderungen pro Sekunde** beschränkt. Wenn diese Grenze erreicht ist, sendet Workfront Fusion den Status 429 ([!UICONTROL Zu viele Anforderungen]).
* [!DNL Workfront Fusion] speichert Webhook-Payloads für 30 Tage. Wenn Sie mehr als 30 Tage nach dem Erhalt auf eine Webhook-Payload zugreifen, wird der Fehler &quot;[!UICONTROL Datei konnte nicht aus dem Speicher gelesen werden.]&quot; angezeigt.
* Webhooks werden automatisch deaktiviert, wenn eine der folgenden Aktionen zutrifft:

   * Der Webhook ist seit mehr als 5 Tagen mit keinem Szenario verbunden
   * Der Webhook wird nur in inaktiven Szenarien verwendet, die seit mehr als 30 Tagen inaktiv sind.

* Deaktivierte Webhooks werden automatisch gelöscht und abgemeldet, wenn sie mit keinem Szenario verbunden sind und seit über 30 Tagen den Status deaktiviert haben.

## Ausführungsverlauf

* Die Ausführungsverlauflogs sind auf eine Größe von **100 MB** beschränkt. Wenn der Ausführungsverlauf diese Größe überschreitet, werden nur die ersten 100 MB angezeigt.
* Wenn ein Szenario mehrere gleichzeitige Ausführungen hat. Nur fünf Ausführungen werden im Bereich &quot;Ausführungen&quot;der Seite mit den Szenariodetails angezeigt. Dies gilt auch dann, wenn mehr als fünf Ausführungen ausgeführt werden.

## Unvollständige Ausführungen

* Unvollständige Ausführungen sind auf eine Gesamtgröße von **500 MB** beschränkt. Bei Erreichen der Grenze von 500 MB werden keine unvollständigen Ausführungen mehr gespeichert.

## Weitere Zustellversuche

* Wenn Sie das Break-Modul verwenden und die Anweisung &quot;Retry&quot;angeben, wird das Szenario automatisch deaktiviert, wenn ein Szenario innerhalb eines Zeitraums von 2 Minuten nacheinander 10-mal fehlschlägt.

