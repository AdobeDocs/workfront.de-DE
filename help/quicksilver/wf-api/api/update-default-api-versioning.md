---
content-type: api
navigation-topic: api-navigation-topic
title: Aktualisieren von Integrationen, die die Standard-API-Versionierung verwenden
description: Aktualisieren von Integrationen, die die Standard-API-Versionierung verwenden
author: Becky
feature: Workfront API
role: Developer
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
TQID: https://experienceleague.adobe.com/E8QRlaGlxvGtgM6Q-23W1trqkejL5Y8RDUzHJtBF1uc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 640
ht-degree: 3%

---

# Aktualisieren von Integrationen, die die Standard-API-Versionierung verwenden

Wir veröffentlichen alle zwei Jahre neue Versionen der Adobe Workfront-API. Jede Version wird drei Jahre nach ihrer Veröffentlichung unterstützt, wobei ein weiteres Jahr als veraltet gilt, in dem die Version verfügbar ist, aber nicht unterstützt wird.

Integrationen, die keine Version der API im URI angeben, werden automatisch auf den Standard weitergeleitet. Wenn Sie möchten, dass Ihr API-Aufruf eine bestimmte Version der API verwendet, müssen Sie diese Version in Ihren Workfront-API-Anfragen angeben.

>[!NOTE]
>
>Wenn Ihr Unternehmen derzeit die Standard-API verwendet, hat Ihr Workfront-Administrator eine Ankündigungscenter-Nachricht mit weiteren Anweisungen zur Standard-API erhalten.

Informationen zur Angabe einer Version in Ihren API-Anfragen finden Sie unter [Angeben einer API-Version in Ihren Integrationen](../../wf-api/api/specify-api-version-integrations.md).

## Überlegungen zur Verwendung der Standard-API

Beachten Sie beim Arbeiten mit der Workfront-Standard-API Folgendes:

* Die Standardversion der API ist die neueste Version. Für jeden API-Aufruf ohne die angegebene Version wird die Standardversion verwendet. Jedes Mal, wenn Workfront eine neue Version der API veröffentlicht, wird die Standardversion auf die neueste Version aktualisiert. **Daher sollten nach der Veröffentlichung einer neuen Version der Workfront-API alle API-Aufrufe, die die Standardversion verwenden, überprüft werden, um sicherzustellen, dass die Funktion weiterhin unterstützt wird**.
* Wenn Ihr Unternehmen derzeit die veraltete Standard-API verwendet, hat Ihr Workfront-Administrator eine Ankündigungscenter-Nachricht mit weiteren Anweisungen zur Standard-API erhalten.

Die neueste Version der API finden Sie unter [API-Versionierung und Support-Zeitplan](../../wf-api/api/api-version-support-schedule.md).

## Aktualisieren Ihrer Integrationen auf unterstützte API-Versionen

Wenn in den Workfront-API-Anfragen keine Version angegeben ist, wird die Standardversion verwendet. Es wird empfohlen, in API-Anfragen eine unterstützte Version der API anzugeben, vorzugsweise für die neueste unterstützte API.

Die folgende Workfront-API-Anfrage gibt beispielsweise keine API-Version an:

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

Wenn diese Anfrage erfolgt, erhalten Sie eine Antwort mit JSON-kodiertem Text, der Daten aus Ihrer Workfront-Instanz angibt. Da in diesem URI keine API-Version angegeben ist, wird der Aufruf an „Default“ (Standard) gesendet.

Um eine Standard-API-Anfrage in eine versionierte API-Anfrage umzuwandeln, rufen Sie einfach eine unterstützte API-Version auf. Beispielsweise fordert der folgende URI Version 15 an:

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

Beim Aktualisieren Ihrer Workfront-API-Anfragen können Sie eine beliebige unterstützte Version Ihrer API angeben. Weitere Informationen zum Referenzieren einer bestimmten API finden Sie unter [API-Version in Ihren Integrationen angeben](../../wf-api/api/specify-api-version-integrations.md).

Um das maximale Support-Fenster zu ermitteln, sollten Sie die neueste Version aufrufen. Eine Liste der unterstützten APIs finden Sie unter [API-Versionierung und Support-Zeitplan](../../wf-api/api/api-version-support-schedule.md).

## Verlauf der Standardversion der API

Die ursprüngliche Absicht der „Standard-API“, oder „Standard“, war es, sie der neuesten Version der Workfront-API zuzuordnen. Dies würde es Kunden mit grundlegenden Integrationen, die als Standard bezeichnet werden, ermöglichen, ihre API-Anfragen nie zu aktualisieren.

2011 veröffentlichte Workfront Version 3.0 der API. Die Standardeinstellung wurde automatisch auf Version 3.0 verschoben, was viele Kundenintegrationen beschädigte, die zu komplex waren, um Version 3.0 zu verwenden, ohne aktualisiert zu werden. Infolgedessen hat Workfront diese Änderung rückgängig gemacht und die Standardversion bei Version 2 belassen.

Seit 2011 hat Workfront die API-Funktionalität erheblich erweitert. Aus diesem Grund werden ältere Versionen unserer API nicht mehr unterstützt. Im Jahr 2017 haben wir das Konzept einer Standardversion vollständig entfernt, anstatt Default zu aktualisieren. Dies sollte unsere Kunden ermutigen, stabile Versionen unserer APIs zu verwenden und ihre Integrationen über einen Zyklus von höchstens drei Jahren zu pflegen.

Workfront stellt jetzt die Standard-API-Version wieder her. Die Standard-API ist auf die neueste Version der Workfront-API festgelegt und wird bei jeder Veröffentlichung einer neuen Version auf die neueste Version aktualisiert.

