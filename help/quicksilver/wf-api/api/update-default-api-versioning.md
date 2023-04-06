---
content-type: api
navigation-topic: api-navigation-topic
title: Aktualisieren von Integrationen, die die standardmäßige API-Versionierung verwenden
description: Aktualisieren von Integrationen, die die standardmäßige API-Versionierung verwenden
author: Becky
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 2b9eacc9b2c8f499cdd1794a55879a56224051c8
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---

# Aktualisieren von Integrationen, die die standardmäßige API-Versionierung verwenden

Wir veröffentlichen alle zwei Jahre neue Versionen der Adobe Workfront-API. Jede Version wird drei Jahre nach ihrer Veröffentlichung unterstützt, wobei ein zusätzliches Jahr veraltet ist und die Version zwar verfügbar, aber nicht unterstützt wird.

Integrationen, die keine Version der API im URI angeben, werden automatisch an &quot;Standard&quot;weitergeleitet. Wenn Ihr API-Aufruf eine bestimmte Version der API verwenden soll, müssen Sie diese Version in Ihren Workfront-API-Anfragen angeben.

>[!NOTE]
>
>Wenn Ihr Unternehmen derzeit die Standard-API verwendet, hat Ihr Workfront-Administrator eine Mitteilung zum Ankündigungszentrum mit weiteren Anweisungen zur Standard-API erhalten.

Informationen zum Festlegen einer Version in Ihren API-Anfragen finden Sie unter [API-Version in Ihren Integrationen angeben](../../wf-api/api/specify-api-version-integrations.md).

## Überlegungen zur Verwendung der Standard-API

Beachten Sie beim Arbeiten mit der Workfront-Standard-API Folgendes:

* Die Standardversion der API ist die neueste Version. Für jeden API-Aufruf ohne die angegebene Version wird die Standardversion verwendet. Jedes Mal, wenn Workfront eine neue API-Version veröffentlicht, wird die Standardversion auf die neueste Version aktualisiert. **Daher sollten nach Veröffentlichung einer neuen Version der Workfront-API alle API-Aufrufe, die die Standardversion verwenden, überprüft werden, um sicherzustellen, dass die Funktionalität weiterhin unterstützt wird.**.
* Wenn Ihr Unternehmen derzeit die veraltete Standard-API verwendet, hat Ihr Workfront-Administrator eine Mitteilung zum Ankündigungszentrum mit weiteren Anweisungen zur Standard-API erhalten.

Die neueste Version der API finden Sie unter [API-Versionierung und Support-Zeitplan](../../wf-api/api/api-version-support-schedule.md).

## Aktualisieren Ihrer Integrationen auf unterstützte API-Versionen

Wenn in Ihren Workfront-API-Anfragen keine Version angegeben ist, wird &quot;Standard&quot;verwendet. Wir empfehlen Ihren API-Anfragen, eine unterstützte Version der API anzugeben, vorzugsweise die neueste unterstützte API.

Beispielsweise gibt die folgende Workfront-API-Anfrage keine API-Version an:

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

Wenn diese Anforderung ausgeführt wird, erhalten Sie eine Antwort mit JSON-kodiertem Text, der Daten aus Ihrer Workfront-Instanz angibt. Da in diesem URI keine API-Version angegeben ist, wird der Aufruf an &quot;Standard&quot;gesendet.

Um eine Standard-API-Anfrage in eine versionierte API-Anfrage umzuwandeln, rufen Sie einfach eine unterstützte API-Version auf. Beispielsweise fordert der folgende URI Version 15 an:

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

Beim Aktualisieren Ihrer Workfront API-Anfragen können Sie eine beliebige unterstützte Version unserer API angeben. Weitere Informationen zum Referenzieren einer bestimmten API finden Sie unter [API-Version in Ihren Integrationen angeben](../../wf-api/api/specify-api-version-integrations.md).

Um das maximale Support-Fenster sicherzustellen, sollten Sie die neueste Version aufrufen. Eine Liste der unterstützten APIs finden Sie in [API-Versionierung und Support-Zeitplan](../../wf-api/api/api-version-support-schedule.md).

## Verlauf der Standardversion der API

Die ursprüngliche Absicht der &quot;Standard-API&quot;bzw. &quot;Standard-API&quot;bestand darin, sie der neuesten Version der Workfront-API zuzuordnen. Dadurch können Kunden mit grundlegenden Integrationen mit dem Namen Default ihre API-Anfragen nie aktualisieren.

Im Jahr 2011 veröffentlichte Workfront Version 3.0 der API. Der Standardwert wurde automatisch in Version 3.0 verschoben, wodurch viele Kundenintegrationen beschädigt wurden, die zu komplex waren, um Version 3.0 zu verwenden, ohne aktualisiert zu werden. Daher setzte Workfront diese Änderung zurück und ließ die Standardversion bei Version 2 zurück.

Seit 2011 hat Workfront die API-Funktionalität deutlich verbessert. Aus diesem Grund werden ältere Versionen unserer API nicht mehr unterstützt. Im Jahr 2017 haben wir anstelle der Aktualisierung von Standard das Konzept einer Standardversion vollständig entfernt. Dadurch sollten unsere Kunden ermutigt werden, stabile Versionen unserer APIs zu verwenden und ihre Integrationen auf einem Zyklus von höchstens drei Jahren zu halten.

Workfront reaktiviert jetzt die Standard-API-Version. Die Standard-API wird auf die neueste Version der Workfront-API festgelegt und jedes Mal, wenn eine neue Version veröffentlicht wird, auf die neueste Version aktualisiert.

