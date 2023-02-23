---
content-type: api
navigation-topic: api-navigation-topic
title: Aktualisieren von Integrationen, die die standardmäßige API-Versionierung verwenden
description: Aktualisieren von Integrationen, die die standardmäßige API-Versionierung verwenden
author: John
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 889084f9a3740b40c84c658f9b0c17270b0a37d7
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# Aktualisieren von Integrationen, die die standardmäßige API-Versionierung verwenden

<!-- This article is going to need a complete revamp or to be removed-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau-Sandbox-Umgebung verfügbar.</span>

Wir veröffentlichen alle zwei Jahre neue Versionen der Adobe Workfront-API. Jede Version wird drei Jahre nach ihrer Veröffentlichung unterstützt, wobei ein zusätzliches Jahr veraltet ist und die Version zwar verfügbar, aber nicht unterstützt wird.

Integrationen, die keine Version der API im URI angeben, werden automatisch an &quot;Standard&quot;weitergeleitet. Wenn Ihr API-Aufruf eine bestimmte Version der API verwenden soll, müssen Sie diese Version in Ihren Workfront-API-Anfragen angeben.

>[!NOTE]
>
>Wenn Ihr Unternehmen derzeit die Standard-API verwendet, hat Ihr Workfront-Administrator eine Mitteilung zum Ankündigungszentrum mit weiteren Anweisungen zur Standard-API erhalten.


<!--
Integrations that do not specify a version of the API in the URI are automatically routed to Default, which has been deprecated. In order for your Workfront integrations to be valid, you must specify a supported API version in your Workfront API requests.
-->

Informationen zum Festlegen einer Version in Ihren API-Anfragen finden Sie unter [API-Version in Ihren Integrationen angeben](../../wf-api/api/specify-api-version-integrations.md).

## Überlegungen zur Verwendung der Standard-API

Beachten Sie beim Arbeiten mit der Workfront-Standard-API Folgendes:

* Nach Version 23.2 wird die Standardversion der API auf die neueste Version festgelegt. Für jeden API-Aufruf ohne die angegebene Version wird die Standardversion verwendet. Jedes Mal, wenn Workfront eine neue API-Version veröffentlicht, wird die Standardversion auf die neueste Version aktualisiert. **Daher sollten nach Veröffentlichung einer neuen Version der Workfront-API alle API-Aufrufe, die die Standardversion verwenden, überprüft werden, um sicherzustellen, dass die Funktionalität weiterhin unterstützt wird.**.
* Wenn Ihr Unternehmen derzeit die veraltete Standard-API verwendet, hat Ihr Workfront-Administrator eine Mitteilung zum Ankündigungszentrum mit weiteren Anweisungen zur Standard-API erhalten.
* <span class="preview">Die Standard-API in der Vorschau-Umgebung ist derzeit auf die neueste Version eingestellt. Die Standard-API in der Produktionsumgebung wird auf die neueste Version nach Version 23.2 festgelegt.</span>

Die neueste Version der API finden Sie unter [API-Versionierung und Support-Zeitplan](../../wf-api/api/api-version-support-schedule.md).

<!--

## Deprecating Default

In an effort to improve the Workfront API, we are in the process of removing older API versions that have exceeded our support window of three years. One of these versions is Version 2, to which Default is mapped. This version was released in 2010, and much of the logic supported in the Attask/Workfront application at that time either no longer exists or has substantially changed.

We deprecated Default in July 2017, and we will no longer designate a specific version of the API to be the default version. Instead, all Workfront API requests must specify a specific API version.

>[!IMPORTANT]
>
> By July 1, 2018 all of your Workfront integrations that use Default must be updated to call a specific supported API version. After that date, all of your Workfront API requests used by integrations that do not specify a version will fail.

To learn about the Workfront deprecation cadence, see [API versioning and support schedule](../../wf-api/api/api-version-support-schedule.md).

-->

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

