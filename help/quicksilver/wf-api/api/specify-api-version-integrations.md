---
content-type: api
navigation-topic: api-navigation-topic
title: API-Version in Ihren Integrationen angeben
description: API-Version in Ihren Integrationen angeben
author: John
feature: Workfront API
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 889084f9a3740b40c84c658f9b0c17270b0a37d7
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# API-Version in Ihren Integrationen angeben

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau-Sandbox-Umgebung verfügbar.</span>

Alle Adobe Workfront-URIs müssen nach dem &quot;attask/api&quot;-Teil des URI auf eine bestimmte Version der API verweisen. Im folgenden Beispiel wird Version 15.0 aufgerufen:

`attask/api/v15.0/<objectName>/<objectId>`

Stellen Sie sicher, dass alle Integrationen die derzeit unterstützten Workfront-APIs aufrufen.

## Veröffentlichungs- und Veraltungszeitplan für Workfront-APIs

Neue Versionen der API werden regelmäßig veröffentlicht, in der Regel zweimal jährlich. Jede Version wird drei Jahre nach ihrem Veröffentlichungsdatum unterstützt, wobei ein zusätzliches Jahr veraltet ist und die Version zwar verfügbar, aber nicht unterstützt wird.

Weitere Informationen zum Veröffentlichungsintervall und zur Einstellung der Verwendung von Workfront-APIs finden Sie unter [API-Versionierung und Support-Zeitplan](../../wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>* Nach Version 23.2 wird die Standardversion der API auf die neueste Version festgelegt. Für jeden API-Aufruf ohne die angegebene Version wird die Standardversion verwendet. Jedes Mal, wenn Workfront eine neue API-Version veröffentlicht, wird die Standardversion auf die neueste Version aktualisiert. Daher sollten nach der Veröffentlichung einer neuen Version der Workfront-API alle API-Aufrufe, die die Standardversion verwenden, überprüft werden, um sicherzustellen, dass die Funktionalität weiterhin unterstützt wird.
>
>* Wenn Ihr Unternehmen derzeit die Standard-API verwendet, hat Ihr Workfront-Administrator eine Mitteilung zum Ankündigungszentrum mit weiteren Anweisungen zur Standard-API erhalten.
>
>* <span class="preview">Die Standard-API in der Vorschau-Umgebung ist auf die neueste Version eingestellt. Die Standard-API in der Produktionsumgebung wird auf die neueste Version nach der Version 23.2 (April 2023) eingestellt</span>.
>
>Die neueste Version der API finden Sie unter [API-Versionierung und Support-Zeitplan](../../wf-api/api/api-version-support-schedule.md).


## Bestimmen der verwendeten API-Version

Sie können die Version der verwendeten API ermitteln, indem Sie den URI einer an die Workfront-API gesendeten HTTP-Anfrage überprüfen. Das folgende Beispiel zeigt einen Workfront-Anfrage-URI, der Version 15 der API angibt:

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

Wenn ein URI keine Version angibt, verwendet er die Standardversion der API, wie im folgenden Beispiel gezeigt:

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> Integrationen, die keine Version der API im URI angeben, werden automatisch zur Standardversion der API weitergeleitet.

## Aktualisieren von Integrationen zur Verwendung unterstützter API-Versionen

Beim Erstellen oder Verwalten von Workfront-Integrationen sollten Sie eine Methode zur dynamischen Aktualisierung der API-Version und anderer Eigenschaften einschließen, die geändert werden können (z. B. Ihren API-Schlüssel).

Um die Aktualisierung von Integrationen effizienter zu gestalten, sollten Sie die folgenden Vorschläge für die Aufzeichnung von Integrationswerten berücksichtigen:

* Store-Werte, die künftigen Änderungen in einer Eigenschaftendatei unterliegen, die Sie aktualisieren
* Erstellen eines Webdiensts zur Verwaltung von Eigenschaften in Echtzeit
* Store-Eigenschaftswerte in einem Datenspeicher, den Ihre Anwendung lesen kann

Durch die Konzeption Ihrer Workfront-Integrationen mit diesem Ziel wird die Notwendigkeit umfangreicher Entwicklungsarbeiten entlastet, wenn sich diese Werte unweigerlich ändern.
