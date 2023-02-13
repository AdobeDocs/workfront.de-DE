---
content-type: api
navigation-topic: api-navigation-topic
title: API-Version in Ihren Integrationen angeben
description: API-Version in Ihren Integrationen angeben
author: John
feature: Workfront API
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# API-Version in Ihren Integrationen angeben

Alle Adobe Workfront-URIs müssen nach dem &quot;attask/api&quot;-Teil des URI auf eine bestimmte Version der API verweisen. Im folgenden Beispiel wird Version 7.0 aufgerufen:
`attask/api/v7.0/<objectName>/<objectId>` Stellen Sie sicher, dass alle Integrationen die derzeit unterstützten Workfront-APIs aufrufen.

## Veröffentlichungs- und Veraltungszeitplan für Workfront-APIs

Neue Versionen der API werden alle sechs bis acht Monate auf halbjährlicher Basis veröffentlicht. Jede Version wird drei Jahre nach ihrem Veröffentlichungsdatum unterstützt, wobei ein zusätzliches Jahr veraltet ist und die Version zwar verfügbar, aber nicht unterstützt wird.

Weitere Informationen zum Veröffentlichungsintervall und zur Einstellung der Verwendung von Workfront-APIs finden Sie unter [API-Versionierung und Support-Zeitplan](../../wf-api/api/api-version-support-schedule.md).

Workfront hat die Standardversion der API seit Juli 2017 eingestellt. Das bedeutet, dass Workfront eine bestimmte Version der API nicht mehr als Standardversion bezeichnet. Alle zukünftigen API-URIs müssen eine Version der API angeben, um gültig zu sein.

>[!IMPORTANT]
>
> Alle Integrationen, die die Standard-API-Version verwenden, müssen bis zum 1. Juli 2018 aktualisiert werden, um eine bestimmte unterstützte API-Version aufzurufen.

## Bestimmen der verwendeten API-Version

Sie können die Version der verwendeten API ermitteln, indem Sie den URI einer an die Workfront-API gesendeten HTTP-Anfrage überprüfen. Das folgende Beispiel zeigt einen Workfront-Anfrage-URI, der Version 7 der API angibt:

`https://<domainname>.my.workfront.com/attask/api/v7.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

Wenn ein URI keine Version angibt, verwendet er die Standardversion der API, wie im folgenden Beispiel gezeigt:

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> Integrationen, die keine Version der API im URI angeben, werden automatisch an die Standardversion der API weitergeleitet und funktionieren nach dem 1. Juli 2018 nicht mehr.

## Aktualisieren von Integrationen zur Verwendung unterstützter API-Versionen

Beim Erstellen oder Verwalten von Workfront-Integrationen sollten Sie eine Methode zur dynamischen Aktualisierung der API-Version und anderer Eigenschaften einschließen, die geändert werden können (z. B. Ihren API-Schlüssel).

Um die Aktualisierung von Integrationen effizienter zu gestalten, sollten Sie die folgenden Vorschläge für die Aufzeichnung von Integrationswerten berücksichtigen:

* Store-Werte, die künftigen Änderungen in einer Eigenschaftendatei unterliegen, die Sie aktualisieren
* Erstellen eines Webdiensts zur Verwaltung von Eigenschaften in Echtzeit
* Store-Eigenschaftswerte in einem Datenspeicher, den Ihre Anwendung lesen kann

Durch die Konzeption Ihrer Workfront-Integrationen mit diesem Ziel wird die Notwendigkeit umfangreicher Entwicklungsarbeiten entlastet, wenn sich diese Werte unweigerlich ändern.
