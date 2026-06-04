---
content-type: api
navigation-topic: general-api
title: Versandanforderungen für Ereignisabonnements
description: Versandanforderungen für Ereignisabonnements
author: Becky
feature: Workfront API
role: Developer
exl-id: 1b621b35-6c8b-4f6a-bcba-ed6cbfe83a8c
TQID: https://experienceleague.adobe.com/rft0idTJddZkXvAcOymqXarAs1zTf77HttI6vuwCTlw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 275
ht-degree: 4%

---

# Versandanforderungen für Ereignisabonnements

Ereignisabonnementnachrichten sind Benachrichtigungen, die eingerichtet werden können, um Benutzende über bestimmte Ereignisse zu informieren. Weitere Informationen zu Ereignisabonnements finden Sie unter [FAQs - Ereignisabonnements](../../wf-api/general/event-subs-faq.md).

## Standards für den Versand von Nachrichten zu Ereignisabonnements

Service-Endpunkte, die Nachrichten zu Adobe Workfront-Ereignisabonnements verwenden, müssen die folgenden grundlegenden Anforderungen erfüllen, um sicherzustellen, dass Nachrichten ordnungsgemäß gesendet und empfangen werden:

* Der Service-Endpunkt muss HTTP-POST-Anfragen akzeptieren. HTTP-POST ist die Anfragemethode, die bei allen Sendungen von Ereignisabonnementnachrichten verwendet wird, einschließlich Validierungsnachrichten.

* Damit das Versandsystem des Ereignisabonnements den erfolgreichen Empfang der Nachricht bestätigen kann, muss der Endpunkt für alle eingehenden Nachrichten einen HTTP-Status von 200 Ebenen zurückgeben (z. B. 200 OK oder 202).

* Wenn kein Status mit 200 Ebenen zurückgegeben wird, geht das Ereignisabonnementsystem davon aus, dass die Nachricht nicht erfolgreich zugestellt wurde, und beginnt mit der Anwendung der entsprechenden Wiederholungsrichtlinie. Weitere Informationen zur Workfront-Wiederholungsrichtlinie finden Sie unter [Wiederholen von Ereignisabonnements](../../wf-api/api/event-sub-retries.md).

* In Verbindung mit der Rückgabe eines Status mit 200 Ebenen als Antwortstatus muss die HTTP-Antwort innerhalb von fünf Sekunden nach dem Start des Versandversuchs empfangen werden.Durch diese Einschränkung wird sichergestellt, dass Geschäftsprozesse oder Infrastrukturbeschränkungen von Privatkunden den Versand anderer Nachrichten bis zum Versand nicht verzögern.

* Wenn ein langwieriger Geschäftsprozess von einer Ereignisabonnementmeldung Trigger, empfiehlt Workfront Folgendes

   1. Der Endpunkt speichert die Nachrichteninformationen beim Empfang und antwortet sofort mit einem Status von 200 Ebenen.
   1. Nachdem ein Endpunkt auf eine Versandanforderung für ein Ereignisabonnement reagiert hat, können die gespeicherten Nachrichten verarbeitet werden.

* Nachrichten oder Objekte von Ereignisabonnements dürfen nicht größer als 1 MB sein.
