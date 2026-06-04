---
content-type: api
navigation-topic: general-api
title: Best Practices für Ereignisabonnements
description: Best Practices für Ereignisabonnements
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
TQID: https://experienceleague.adobe.com/uT7erlnJR5-h-KKGQiuztzZKBtwtEvWQ8U-EUgN4TG4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 356
ht-degree: 23%

---

# Best Practices für Ereignisabonnements

Nachrichten zu Ereignisabonnements von Adobe Workfront werden automatisch von Workfront gesendet, nachdem Sie Ihren Dienst korrekt konfiguriert und einen Trigger für Ereignisabonnements erstellt haben, um diese Nachrichtensendungen zu verwalten. Weitere Informationen zum ordnungsgemäßen Einrichten von Ereignisabonnements finden Sie unter [Versandanforderungen für Ereignisabonnements](../../wf-api/general/setup-event-sub-endpoint.md).


Nachfolgend finden Sie einige Best Practices, die Ihnen bei der effektiven Erstellung von Ereignisabonnements helfen.

## Alle erforderlichen Felder für den Anfragetext angeben

Stellen Sie sicher, dass alle erforderlichen Felder für den Anfragetext für die API bereitgestellt werden. Informationen zu allen erforderlichen Anforderungsattributen finden Sie unter [Ereignisabonnement-API](../../wf-api/general/event-subs-api.md).

## Vermeiden Sie das Einfügen von zusätzlichen Textfeldern

Fügen Sie in die Anfrage keine zusätzlichen Textfelder ein, da dies dazu führt, dass die API kein Abonnement erstellen kann.

## Vermeiden einer Überlastung von Ereignisabonnements

Der Ereignisabonnementdienst wurde entwickelt, um für alle Benutzenden eine zuverlässige Bereitstellung von Ereignissen zu gewährleisten. Damit dies sichergestellt wird, wurden Schutzmaßnahmen eingeführt, um eine übermäßige Ereignisproduktion durch eine einzelne Person zu verhindern, die potenziell die Service-Qualität für alle Benutzenden beeinträchtigen könnte. Daher kann es bei Benutzenden, die innerhalb eines kurzen Zeitraums zu viele Ereignisse mit hoher Rate produzieren, zu Sandboxing und zu Verzögerungen bei der Ereignisbereitstellung kommen.

## Vollständige Tests innerhalb der Übergangsphase

Versuchen Sie, alle Abonnementtests innerhalb der 100-Nachrichten-Übergangsphase durchzuführen. Weitere Informationen zu dieser Übergangsphase finden Sie unter [FAQs - Ereignisabonnements](../../wf-api/general/event-subs-faq.md).

## Erfüllen Sie die Standardanforderungen für den Nachrichtenversand im Ereignisabonnement

Stellen Sie sicher, dass Ihr Abonnement-Endpunkt den Versandanforderungen für Standard-Ereignisabonnements-Nachrichten entspricht. Weitere Informationen zu diesen Anforderungen finden Sie unter [Versandanforderungen für Ereignisabonnements](../../wf-api/general/setup-event-sub-endpoint.md).

## Zulassungsliste der IP-Adressen nach globaler Region

Um Payloads von Ereignisabonnements über Ihre Firewall zu erhalten, müssen Sie die IP-Adressen der Zulassungsliste nach globaler Region hinzufügen. Weitere Informationen finden Sie unter [Ereignisabonnement-API](../../wf-api/general/event-subs-api.md).

## Die richtige Zugriffsebene und Authentifizierung

Um ein Ereignisabonnement zu erstellen, abzufragen oder zu löschen, benötigt Ihr Workfront-Benutzer Folgendes:

* Eine Zugriffsebene von **Systemadministrator**
Weitere Informationen finden Sie unter [Gewähren des vollständigen administrativen Zugriffs für einen Benutzer](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) oder [Gewähren des administrativen Zugriffs für bestimmte Bereiche](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Wenn Ihr Unternehmen Adobe IMS (Identity Management-System) verwendet, schließen Sie ein IMS-Benutzer-Token ein, das in der `X-User-Token`-Kopfzeile übergeben wird.
