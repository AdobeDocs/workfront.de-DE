---
content-type: api;faq
navigation-topic: general-api
title: Häufig gestellte Fragen - Ereignisabonnements
description: Häufig gestellte Fragen - Ereignisabonnements
author: Becky
feature: Workfront API
role: Developer
exl-id: a6120939-5d76-4f46-a304-125de6b22502
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 0%

---

# Häufig gestellte Fragen - Ereignisabonnements

<!--
{{highlighted-preview}}
-->

Häufig gestellte Fragen zu Ereignisabonnements:

## Was ist ein Abonnement?

Ein Abonnement ist ein Datensatz, der zum Abgleichen und Bereitstellen von Adobe Workfront-Ereignissen an den HTTP-Endpunkt eines Kunden verwendet wird. Diese Ressource besteht aus vier primären Attributen:

* customer_id
* obj_code
* obj_id
* URL

Ein Abonnement kann auch andere Attribute aufweisen, z. B. seine eigene eindeutige ID und das Datum, an dem es erstellt wurde. Die oben aufgeführten Attribute werden jedoch hauptsächlich verwendet, um Ereignisse abzugleichen und sie Kunden bereitzustellen.

## Kann ich basierend auf bestimmten Kriterien in der Ereignis-Payload auswählen, welche Ereignisse an einen Endpunkt gesendet werden?

Ereignisabonnementfilter sind eine Möglichkeit, Ereignisuntergruppen nach angegebenen Kriterien zu sortieren. Es wird empfohlen, Filter auf Ereignisabonnements anzuwenden, da dadurch die Anzahl der Nachrichten, die ein Endpunkt verarbeiten muss, erheblich reduziert werden kann. Weitere Informationen finden Sie [Ereignisabonnement-Filter](../../wf-api/general/event-subs-api.md#event).

## Warum gibt die API einen 409-Konflikt-Antwort-Code zurück?

Wenn Sie versuchen, ein Ereignisabonnement zu erstellen und einen Antwort-Code: 409-Konflikt erhalten, ist das zu erstellende Abonnement ein Duplikat. Workfront lässt die Erstellung doppelter Abonnements nicht zu.

## Was sollte ich tun, wenn meine Nachrichten nicht an meinen Endpunkt gesendet werden?

Suchen Sie nach den folgenden Szenarien und verwenden Sie die empfohlene Lösung:

* Stellen Sie sicher, dass Ihr Abonnement-Endpunkt - definiert durch das Feld **url** - einen 2XX-HTTP-Antwort-Code zurückgibt. Ist dies nicht der Fall, wenden Sie sich an den Workfront-Support oder lesen Sie [Versandanforderungen für Ereignisabonnements](../../wf-api/general/setup-event-sub-endpoint.md).

* Die Zeit für die Anfrage zum Ereignisversand könnte überschritten sein, bevor sie abgeschlossen ist. Stellen Sie sicher, dass Ihr Endpunkt innerhalb von 5 Sekunden konsistent reagiert. Dies ist der standardmäßige Timeout-Wert für die HTTP-Anfrage zum Versand einer Ereignisabonnementnachricht. Wenn Ihr Endpunkt nicht innerhalb von 5 Sekunden reagiert, wenden Sie sich an den Workfront-Support oder lesen Sie [Versandanforderungen für Ereignisabonnements](../../wf-api/general/setup-event-sub-endpoint.md).
* Die Ereignisse haben möglicherweise nicht Ihre eigene Denkweise. Stellen Sie sicher, dass Sie keine Annahmen darüber treffen, wie oder wann Ereignisse ausgelöst werden sollten und wann. Wenn Sie beispielsweise glauben, dass durch die Aktualisierung eines Dokuments in einer Aufgabe ein Aufgabenaktualisierungsereignis, sondern stattdessen ein Dokumenterstellungsereignis oder ein Dokumentaktualisierungsereignis generiert wird.
* Ihr Abonnement ist möglicherweise nicht wie erwartet konfiguriert. Sie können Ereignisabonnements in verschiedenen Umgebungen erstellen und erwarten, dass sie wie andere Workfront-Daten übertragen werden. Ereignisabonnementdaten sind jedoch nicht so konfiguriert, dass sie in andere Umgebungen kopiert oder weitergeleitet werden. Stellen Sie sicher, dass Sie API-Anfragen an die richtige Umgebung senden und dass die Abonnements in dieser Umgebung erwartungsgemäß konfiguriert sind.
* Die Payload wurde nicht empfangen, da die erforderliche Workfront-IP-Adresse nicht zur -Zulassungsliste in Ihrer Firewall hinzugefügt wurde. Ereignisabonnement-Ereignisse werden nur von wenigen IP-Adressen gesendet. Stellen Sie sicher, dass das Zielnetzwerk über alle IP-Ausnahmen verfügt, die zum Empfang von Payloads von Workfront-Ereignisabonnements erforderlich sind.

## Warum dauert es zu lange, bis meine Nachrichten meinen Endpunkt erreichen?

Einige der folgenden Szenarien könnten dafür verantwortlich sein:

* Ein großer Vorgang - z. B. eine Massenaktualisierung - im System kann dazu führen, dass eine große Anzahl von Nachrichten gleichzeitig in die Warteschlange gestellt wird, was einige Zeit in Anspruch nehmen kann.
* Langwierige Berechnungen oder Zeitleistenberechnungen bei großen Projekten können zu einer Verzögerung bei der Veröffentlichung von Nachrichten an die zu nutzenden Ereignisabonnements führen.
* Das Abonnement wurde möglicherweise deaktiviert.

   * Wenn nach einer Übergangsphase von 100 Nachrichten eine bestimmte URL, die mit einem oder mehreren Abonnements verknüpft sein kann, in mehr als 70 % der Fälle fehlschlägt oder wenn die URL nach 2000 aufeinander folgenden Versuchen nicht zugestellt werden kann, werden alle Nachrichten, die mit Abonnements mit derselben URL übereinstimmen, nicht zum Versand versucht. Stattdessen werden diese Nachrichten sofort für einen erneuten Versuch in die Warteschlange gestellt.

     Alle 10 Minuten, nachdem eine URL deaktiviert wurde, versuchen wir, die nächste Nachricht zu versenden, die zur Verarbeitung durch kommt. Wenn diese Nachricht erfolgreich ist, aktivieren wir diese URL und anschließend alle passenden Abonnements erneut. Wenn diese Nachricht nicht gesendet werden kann, wird der 10-Minuten-Timer zurückgesetzt und wir versuchen es erneut, nachdem er abgelaufen ist.

     Dieses Verhalten kann als inkonsistenter oder verzögerter Versand wahrgenommen werden, es folgt jedoch einfach unseren Richtlinien für den Umgang mit Nachrichten vom Typ Ereignisabonnement.

   * Eine Ereignisabonnement-URL wird hart deaktiviert, wenn eine der folgenden Bedingungen erfüllt ist:

      * Die Abonnement-URL konnte 7 Tage lang nicht bereitgestellt werden und in den letzten 72 Stunden sind mindestens 2000 aufeinander folgende Zustellversuche fehlgeschlagen.
      * Die Abonnement-URL konnte keine 50.000 aufeinander folgenden Versuche bereitstellen.

## Was sollte ich tun, wenn ich beim Versuch, die Ereignis-Abonnement-API aufzurufen, den Status „500-Antwort“ erhalte?

Wenden Sie sich an den Workfront-Support. Informationen zum Kontaktieren des Supports finden Sie unter [Kundensupport kontaktieren](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## Welche verschiedenen Authentifizierungstypen kann ich mit Workfront-Ereignisabonnements verwenden?

Sie können eine beliebige Authentifizierung verwenden, die ein Bearer-Token verwendet. Das Feld **authToken** eines Abonnements ist eine Zeichenfolge, die ein OAuth2-Bearer-Token darstellt, das zur Authentifizierung mit der im Feld **url** angegebenen URL verwendet. Theoretisch könnte dieser Token-Wert alles sein, solange der Ziel-Endpunkt weiß, wie seine Kodierung verarbeitet wird, nämlich **utf-8**.

## Wie lange sollte es dauern, bis ich meine Ereignis-Payload von Workfront-Ereignisabonnements erhalte?

Im Allgemeinen kann davon ausgegangen werden, dass Versandanfragen für Ereignisabonnement-Ereignisse in weniger als 5 Sekunden nach der protokollierten Datenänderung empfangen werden. Im Durchschnitt werden Webhook-Benachrichtigungen in weniger als 1 Sekunde ab dem Zeitpunkt der Datenänderung empfangen. Der Service kann jedoch Nachrichten in einer derart großen Menge empfangen, dass er möglicherweise auch länger dauert.

## Zusätzliche Ressourcen

* **API-Dokumentation**: [Ereignisabonnement-API](../../wf-api/general/event-subs-api.md)

* **Best Practices**: [Best Practices für Ereignisabonnements](../../wf-api/general/event-sub-best-practice.md)

* **Felder, die Trigger-Ereignisabonnement-Payloads enthalten**: [Ressourcenfelder für Ereignisabonnements](../../wf-api/api/event-sub-resource-fields.md)

* **Wiederholungen von Ereignisabonnements**: [Wiederholungen von Ereignisabonnements](../../wf-api/api/event-sub-retries.md)

* **Firewall für Workfront konfigurieren**: [Die Firewall-Zulassungsliste konfigurieren](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)
