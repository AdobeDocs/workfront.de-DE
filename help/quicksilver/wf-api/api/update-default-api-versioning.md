---
content-type: api
navigation-topic: api-navigation-topic
title: Aktualisieren von Integrationen, die die standardmäßige API-Versionierung verwenden
description: Aktualisieren von Integrationen, die die standardmäßige API-Versionierung verwenden
author: John
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 0%

---

# Aktualisieren von Integrationen, die die standardmäßige API-Versionierung verwenden

Wir veröffentlichen alle zwei Jahre neue Versionen der Adobe Workfront-API. Jede Version wird drei Jahre nach ihrer Veröffentlichung unterstützt, wobei ein zusätzliches Jahr veraltet ist und die Version zwar verfügbar, aber nicht unterstützt wird.

Integrationen, die keine Version der API im URI angeben, werden automatisch in &quot;Standard&quot;umgeleitet, was nicht mehr unterstützt wird. Damit Ihre Workfront-Integrationen gültig sind, müssen Sie in Ihren Workfront-API-Anfragen eine unterstützte API-Version angeben.

Informationen zum Festlegen einer Version in Ihren API-Anfragen finden Sie unter [API-Version in Ihren Integrationen angeben](../../wf-api/api/specify-api-version-integrations.md).

## Grundlegendes zur Standardversion der API

Die ursprüngliche Absicht der &quot;Standard-API&quot;bzw. &quot;Standard-API&quot;bestand darin, sie der neuesten Version der Workfront-API zuzuordnen. Dadurch können Kunden mit grundlegenden Integrationen mit dem Namen Default ihre API-Anfragen nie aktualisieren.

Im Jahr 2011 veröffentlichte Workfront Version 3.0 der API. Der Standardwert wurde automatisch in Version 3.0 verschoben, wodurch viele Kundenintegrationen beschädigt wurden, die zu komplex waren, um Version 3.0 zu verwenden, ohne aktualisiert zu werden. Daher setzte Workfront diese Änderung zurück und ließ die Standardversion bei Version 2 zurück.

Leider wurde dieses Thema nie erneut angesprochen. Da wir nun planen, die API-Funktionalität deutlich zu verbessern, sind wir gezwungen, ältere Versionen unserer API, einschließlich Default, abzulehnen. Statt Default zu aktualisieren, wodurch zweifellos mehr Integrationen beschädigt würden, entfernen wir das Konzept einer Standardversion vollständig. Dadurch sollen unsere Kunden ermutigt werden, stabile Versionen unserer APIs zu verwenden und ihre Integrationen auf einem Zyklus von höchstens drei Jahren zu halten.

## Veralteter Standard

Um die Workfront-API zu verbessern, entfernen wir derzeit ältere API-Versionen, die unser Supportzeitraum von drei Jahren überschritten haben. Eine dieser Versionen ist Version 2, der Standard zugeordnet ist. Diese Version wurde 2010 veröffentlicht und ein Großteil der Logik, die zu diesem Zeitpunkt in der Attask/Workfront-Anwendung unterstützt wurde, existiert nicht mehr oder hat sich wesentlich geändert.

Die Standardversion wurde im Juli 2017 eingestellt. Eine bestimmte Version der API wird nicht mehr als Standardversion festgelegt. Stattdessen müssen alle Workfront API-Anfragen eine bestimmte API-Version angeben.

>[!IMPORTANT]
>
> Bis zum 1. Juli 2018 müssen alle Workfront-Integrationen, die Standard verwenden, aktualisiert werden, um eine bestimmte unterstützte API-Version aufzurufen. Nach diesem Datum schlagen alle Ihre Workfront API-Anfragen fehl, die von Integrationen verwendet werden, die keine Version angeben.

Weitere Informationen zur Einstellung der Workfront finden Sie unter [API-Versionierung und Support-Zeitplan](../../wf-api/api/api-version-support-schedule.md).

## Aktualisieren Ihrer Integrationen auf unterstützte API-Versionen

Wenn in Ihren Workfront-API-Anfragen keine Version angegeben ist, wird &quot;Standard&quot;verwendet. Sie müssen Ihre API-Anfragen aktualisieren, um eine unterstützte Version der API anzugeben, vorzugsweise auf die neueste unterstützte API.

Beispielsweise gibt die folgende Workfront-API-Anfrage keine API-Version an:

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

Wenn diese Anforderung ausgeführt wird, erhalten Sie eine Antwort mit JSON-kodiertem Text, der Daten aus Ihrer Workfront-Instanz angibt. Da in diesem URI keine API-Version angegeben ist, wird der Aufruf an &quot;Standard&quot;gesendet.

Um eine Standard-API-Anfrage in eine versionierte API-Anfrage umzuwandeln, rufen Sie einfach eine unterstützte API-Version auf. Beispielsweise fordert der folgende URI Version 9 an:

`https://davidwhite.my.workfront.com/attask/api/`**v9.0**`/project/metadata`

Beim Aktualisieren Ihrer Workfront API-Anfragen können Sie eine beliebige unterstützte Version unserer API angeben. Weitere Informationen zum Referenzieren einer bestimmten API finden Sie unter [API-Version in Ihren Integrationen angeben](../../wf-api/api/specify-api-version-integrations.md).

Um das maximale Support-Fenster sicherzustellen, sollten Sie die neueste Version (Version 9) aufrufen. Eine Liste der unterstützten APIs finden Sie in [API-Versionierung und Support-Zeitplan](../../wf-api/api/api-version-support-schedule.md).

Sie müssen die Integrationen, die Sie mit Default haben, unbedingt aktualisieren. Wenn Sie derzeit über Integrationen verfügen, die keine Version angeben, erhalten Sie möglicherweise eine Benachrichtigung von Ihrem Workfront-Vertriebsmitarbeiter, Kundenerfolgsmanager oder Support-Mitarbeiter oder eine Mitteilung zum Anzeigen des Zentrums.

Stellen Sie so bald wie möglich sicher, dass Ihre Integrationen aktualisiert werden, um eine unterstützte Version unserer API aufzurufen.
