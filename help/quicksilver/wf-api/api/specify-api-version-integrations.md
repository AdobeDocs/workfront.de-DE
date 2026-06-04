---
content-type: api
navigation-topic: api-navigation-topic
title: Angeben einer API-Version in Integrationen
description: Angeben einer API-Version in Integrationen
author: Becky
feature: Workfront API
role: Developer
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
TQID: https://experienceleague.adobe.com/GWA77t-kaVNG7tfSsg5Fe5kLtR3Ibo0YbW7Gp7wBQ0U
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 438
ht-degree: 3%

---

# API-Version in Ihren Integrationen angeben

Alle Adobe Workfront-URIs sollten auf eine bestimmte Version der API nach dem Teil „attask/api“ des URI verweisen. Im folgenden Beispiel wird Version 15.0 aufgerufen:

`attask/api/v15.0/<objectName>/<objectId>`

Stellen Sie sicher, dass alle Ihre Integrationen derzeit unterstützte Workfront-APIs aufrufen.

## Zeitplan für Veröffentlichung und Einstellung von Workfront-APIs

Neue Versionen der API werden regelmäßig veröffentlicht, in der Regel zweimal jährlich. Jede Version wird drei Jahre nach dem Veröffentlichungsdatum unterstützt, wobei ein weiteres Jahr als veraltet gilt, in dem die Version verfügbar ist, aber nicht unterstützt wird.

Weitere Informationen zum Veröffentlichungsintervall und zur Planung der Einstellung von Workfront-APIs finden Sie unter [API-Versionierung und Support-Zeitplan](../../wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>* Die Standardversion der API ist auf die neueste Version festgelegt. Für jeden API-Aufruf ohne die angegebene Version wird die Standardversion verwendet. Jedes Mal, wenn Workfront eine neue Version der API veröffentlicht, wird die Standardversion auf die neueste Version aktualisiert. **Daher sollten nach der Veröffentlichung einer neuen Version der Workfront-API alle API-Aufrufe, die die Standardversion verwenden, überprüft werden, um sicherzustellen, dass die Funktion weiterhin unterstützt wird.**
>
>* Wenn Ihr Unternehmen derzeit die Standard-API verwendet, hat Ihr Workfront-Administrator eine Ankündigungscenter-Nachricht mit weiteren Anweisungen zur Standard-API erhalten.
>
>Die neueste Version der API finden Sie unter [API-Versionierung und Support-Zeitplan](../../wf-api/api/api-version-support-schedule.md).


## Bestimmen der verwendeten API-Version

Sie können die verwendete API-Version ermitteln, indem Sie den URI einer HTTP-Anfrage überprüfen, die an die Workfront-API gesendet wird. Das folgende Beispiel zeigt einen Workfront-Anfrage-URI, der Version 15 der API angibt:

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

Wenn ein URI keine Version angibt, verwendet er die Standardversion der API, wie im folgenden Beispiel gezeigt:

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> Integrationen, die im URI keine Version der API angeben, werden automatisch an die Standardversion der API weitergeleitet.

## Aktualisieren von Integrationen zur Verwendung unterstützter API-Versionen

Beim Erstellen oder Verwalten von Workfront-Integrationen sollten Sie eine Methode zum dynamischen Aktualisieren der API-Version und andere Eigenschaften, die sich ändern können (z. B. Ihren API-Schlüssel), einbeziehen.

Um die Aktualisierung von Integrationen effizienter zu gestalten, sollten Sie die folgenden Vorschläge für die Aufzeichnung von Integrationswerten berücksichtigen:

* Werte vorbehaltlich künftiger Änderungen in einer von Ihnen aktualisierten Eigenschaftendatei speichern
* Erstellen eines Web-Services zur Verwaltung von Eigenschaften in Echtzeit
* Speichern von Eigenschaftswerten in einem Datenspeicher, den Ihre Anwendung lesen kann

Wenn Sie Ihre Workfront-Integrationen unter diesem Gesichtspunkt entwerfen, müssen Sie keine umfangreichen Entwicklungsarbeiten durchführen, wenn sich diese Werte unweigerlich ändern.
