---
content-type: api
navigation-topic: general-api
title: Best Practices für Ereignisabonnements
description: Best Practices für Ereignisabonnements
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# Best Practices für Ereignisabonnements

Adobe Workfront-Ereignisabonnementmeldungen werden automatisch von Workfront gesendet, nachdem Sie Ihren Dienst korrekt konfiguriert und ein Ereignisabonnement erstellt haben, um diese Nachrichtenbereitstellungen Trigger. Weitere Informationen zum ordnungsgemäßen Einrichten von Ereignisanmeldungen finden Sie unter [Versandanforderungen für Ereignisabschlüsse](../../wf-api/general/setup-event-sub-endpoint.md).


Im Folgenden finden Sie einige Best Practices, mit denen Sie Ereignisabos effektiv erstellen können.

## Alle erforderlichen Anforderungstextfelder bereitstellen

Stellen Sie sicher, dass die API alle erforderlichen Anfrageinhalt-Felder erhält. Informationen zu allen erforderlichen Anforderungsattributen finden Sie unter [Ereignisabonnement-API](../../wf-api/general/event-subs-api.md).

## Vermeiden Sie das Einschließen von zusätzlichen Textkörperfeldern

Schließen Sie keine zusätzlichen Textkörperfelder in die Anfrage ein, da dies dazu führt, dass die API kein Abonnement erstellt.

## Führen Sie Tests innerhalb der Übergangsphase durch

Versuchen Sie, alle Abonnementtests innerhalb der Übergangsphase von 100 Nachrichten durchzuführen. Weitere Informationen zu dieser Übergangsphase finden Sie unter [Häufig gestellte Fragen - Ereignisabos](../../wf-api/general/event-subs-faq.md).

## Erfüllen Sie die Standardanforderungen an die Bereitstellung von Ereignisanmeldungsnachrichten

Stellen Sie sicher, dass Ihr Abonnement-Endpunkt den standardmäßigen Bedingungen für die Bereitstellung von Ereignisabonnementnachrichten entspricht. Weitere Informationen zu diesen Anforderungen finden Sie unter [Versandanforderungen für Ereignisabschlüsse](../../wf-api/general/setup-event-sub-endpoint.md).

## IP-Adressen der Zulassungslisten nach globaler Region

Um Payloads von Ereignisabonnenten über Ihre Firewall zu erhalten, müssen Sie die IP-Adressen zur Zulassungsliste hinzufügen. Weitere Informationen finden Sie unter [Ereignisabonnement-API](../../wf-api/general/event-subs-api.md).

## über die richtige Zugriffsebene und einen API-Schlüssel verfügen

Um ein Ereignisabonnement zu erstellen, abzufragen oder zu löschen, benötigt Ihr Workfront-Benutzer:

* Eine Zugriffsebene von **Systemadministrator**
Weitere Informationen finden Sie unter [Gewähren eines vollen Administratorzugriffs](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) oder [Benutzern administrativen Zugriff auf bestimmte Bereiche gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Ein API-Schlüssel

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more, see .</p>
  -->
