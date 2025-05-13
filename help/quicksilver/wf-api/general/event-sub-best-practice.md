---
content-type: api
navigation-topic: general-api
title: Best Practices für Ereignisabonnements
description: Best Practices für Ereignisabonnements
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 19e0b792bc49ede0504af479952fdbdf384dc73c
workflow-type: tm+mt
source-wordcount: '282'
ht-degree: 0%

---


# Best Practices für Ereignisabonnements

Nachrichten zu Ereignisabonnements von Adobe Workfront werden automatisch von Workfront gesendet, nachdem Sie Ihren Dienst korrekt konfiguriert und einen Trigger für Ereignisabonnements erstellt haben, um diese Nachrichtensendungen zu verwalten. Weitere Informationen zum ordnungsgemäßen Einrichten von Ereignisabonnements finden Sie unter [Versandanforderungen für Ereignisabonnements](../../wf-api/general/setup-event-sub-endpoint.md).


Nachfolgend finden Sie einige Best Practices, die Ihnen bei der effektiven Erstellung von Ereignisabonnements helfen.

## Alle erforderlichen Felder für den Anfragetext angeben

Stellen Sie sicher, dass alle erforderlichen Felder für den Anfragetext für die API bereitgestellt werden. Informationen zu allen erforderlichen Anforderungsattributen finden Sie unter [Ereignisabonnement-API](../../wf-api/general/event-subs-api.md).

## Vermeiden Sie das Einfügen von zusätzlichen Textfeldern

Fügen Sie in die Anfrage keine zusätzlichen Textfelder ein, da dies dazu führt, dass die API kein Abonnement erstellen kann.

## Vollständige Tests innerhalb der Übergangsphase

Versuchen Sie, alle Abonnementtests innerhalb der 100-Nachrichten-Übergangsphase durchzuführen. Weitere Informationen zu dieser Übergangsphase finden Sie unter [FAQs - Ereignisabonnements](../../wf-api/general/event-subs-faq.md).

## Erfüllen Sie die Standardanforderungen für den Nachrichtenversand im Ereignisabonnement

Stellen Sie sicher, dass Ihr Abonnement-Endpunkt den Versandanforderungen für Standard-Ereignisabonnements-Nachrichten entspricht. Weitere Informationen zu diesen Anforderungen finden Sie unter [Versandanforderungen für Ereignisabonnements](../../wf-api/general/setup-event-sub-endpoint.md).

## Zulassungsliste der IP-Adressen nach globaler Region

Um Payloads von Ereignisabonnements über Ihre Firewall zu erhalten, müssen Sie die IP-Adressen der Zulassungsliste nach globaler Region hinzufügen. Weitere Informationen finden Sie unter [Ereignisabonnement-API](../../wf-api/general/event-subs-api.md).

## Die richtige Zugriffsebene und Authentifizierung

Um ein Ereignisabonnement zu erstellen, abzufragen oder zu löschen, benötigt Ihr Workfront-Benutzer Folgendes:

* Zugriffsebene von **Systemadministrator**
Weitere Informationen finden Sie unter [Gewähren des vollständigen administrativen Zugriffs für einen Benutzer](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) oder [Gewähren des administrativen Zugriffs für bestimmte Bereiche](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Für die Verwendung der Ereignisabonnement-API ist eine `sessionID` Kopfzeile erforderlich

  Weitere Informationen finden Sie unter [Authentifizierung](api-basics.md#authentication) in [API-Grundlagen](api-basics.md).
