---
content-type: api
navigation-topic: general-api
title: Versandanforderungen für Ereignisabschlüsse
description: Versandanforderungen für Ereignisabschlüsse
author: Becky
feature: Workfront API
role: Developer
exl-id: 1b621b35-6c8b-4f6a-bcba-ed6cbfe83a8c
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---


# Versandanforderungen für Ereignisabschlüsse

Ereignis-Abonnementnachrichten sind Benachrichtigungen, die so eingerichtet werden können, dass Benutzer benachrichtigt werden, wenn bestimmte Ereignisse auftreten. Weitere Informationen zu Abonnements für Ereignisse finden Sie unter [FAQs - Abonnements für Ereignisse](../../wf-api/general/event-subs-faq.md).

## Standards für die Bereitstellung von Ereignisabonnementnachrichten

Dienstendpunkte, die Adobe Workfront-Ereignisabonnementnachrichten verwenden, müssen die folgenden grundlegenden Anforderungen erfüllen, um sicherzustellen, dass Nachrichten richtig gesendet und empfangen werden:

* Der Dienstendpunkt muss HTTP-POST-Anfragen akzeptieren. Die HTTP-POST ist die Anfragemethode, die in allen Sendungen von Ereignis-Abonnementnachrichten, einschließlich Validierungsmeldungen, verwendet wird.

* Damit das System für den Ereignisabonnement-Versand bestätigen kann, dass die Nachricht erfolgreich empfangen wurde, muss der Endpunkt für alle eingehenden Nachrichten einen HTTP-Status von 200 Ebenen (z. B. 200 OK oder 202) zurückgeben.

* Wenn kein Status von 200 Ebenen zurückgegeben wird, geht das Abonnementsystem des Ereignisses davon aus, dass die Nachricht nicht erfolgreich zugestellt wurde, und beginnt mit der Anwendung der entsprechenden Wiederholungsrichtlinie. Weitere Informationen zur Workfront-Wiederholungsrichtlinie finden Sie unter [Wiederholungen von Ereignisabonnements](../../wf-api/api/event-sub-retries.md).

* In Verbindung mit der Rückgabe des Status von 200 Ebenen als Antwortstatus muss die HTTP-Antwort innerhalb von fünf Sekunden nach dem Start des Versandversuchs empfangen werden. Diese Einschränkung stellt sicher, dass Geschäftsprozesse oder Infrastrukturbeschränkungen von Verbrauchern den Versand anderer Nachrichten nicht verzögern.

* Wenn ein langwieriger Geschäftsprozess Trigger von einer Ereignisabonnementnachricht verarbeitet, empfiehlt Workfront  dass

   1. Der Endpunkt speichert die Nachrichteninformationen bei Erhalt und antwortet sofort mit einem Status von 200 Ebenen.
   1. Nachdem ein Endpunkt auf eine Versandanfrage zum Abonnement eines Ereignisses geantwortet hat, können die gespeicherten Nachrichten verarbeitet werden.
