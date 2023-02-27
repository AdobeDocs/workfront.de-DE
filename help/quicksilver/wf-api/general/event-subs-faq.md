---
content-type: api;faq
navigation-topic: general-api
title: Häufig gestellte Fragen - Ereignisabos
description: Häufig gestellte Fragen - Ereignisabos
author: Becky
feature: Workfront API
exl-id: a6120939-5d76-4f46-a304-125de6b22502
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '937'
ht-degree: 0%

---

# Häufig gestellte Fragen - Ereignisabos

<!--
{{highlighted-preview}}
-->

Im Folgenden finden Sie häufig gestellte Fragen zu Ereignisanmeldungen:

## Was ist ein Abonnement?

Ein Abonnement ist ein Datensatz, der verwendet wird, um Adobe Workfront-Ereignisse mit dem HTTP-Endpunkt eines Kunden abzugleichen und bereitzustellen. Diese Ressource besteht aus vier Hauptattributen:

* customer_id
* obj_code
* obj_id
* url

Ein Abonnement kann auch andere Attribute aufweisen, z. B. seine eigene eindeutige ID und das Datum seiner Erstellung. Die oben aufgeführten Attribute werden jedoch hauptsächlich verwendet, um Ereignisse zuzuordnen und sie an Kunden zu senden.

## Kann ich basierend auf bestimmten Kriterien in einer Ereignis-Payload auswählen, welche Ereignisse an einen Endpunkt gesendet werden?

Ereignisabonnementfilter bieten eine Möglichkeit, Ereignisunterschriften nach bestimmten Kriterien zu sortieren. Es wird empfohlen, Filter auf Ereignis-Abonnements anzuwenden, da dadurch die Anzahl der Nachrichten, die ein Endpunkt verbrauchen muss, erheblich reduziert werden kann. Weitere Informationen finden Sie unter [Filter für Ereignisabschlüsse](../../wf-api/general/event-subs-api.md#event).

## Warum gibt die API einen 409-Konflikt-Antwort-Code zurück?

Wenn Sie versuchen, ein Ereignisabonnement zu erstellen und einen Antwort-Code zu erhalten: 409 Konflikt, ist das Abonnement, das Sie zu erstellen versucht haben, ein Duplikat. In Workfront ist die Erstellung doppelter Abonnements nicht zulässig.

## Was soll ich tun, wenn meine Nachrichten nicht an meinen Endpunkt gesendet werden?

Suchen Sie nach den folgenden Szenarien und verwenden Sie die empfohlene Lösung:

* Stellen Sie sicher, dass Ihr Abonnement-Endpunkt, der durch die Variable **url** field - gibt einen HTTP-Antwort-Code (2.XX) zurück. Ist dies nicht der Fall, wenden Sie sich an den Workfront-Support oder lesen Sie [Versandanforderungen für Ereignisabschlüsse](../../wf-api/general/setup-event-sub-endpoint.md).

* Die Ereignisbereitstellungsanforderung kann einen Timeout aufweisen, bevor sie abgeschlossen wird. Stellen Sie sicher, dass Ihr Endpunkt innerhalb von 5 Sekunden konsistent reagiert. Dies ist die standardmäßige Zeitüberschreitung, die für die HTTP-Anforderung festgelegt wurde, um eine Ereignisabonnementmeldung bereitzustellen. Wenn Ihr Endpunkt nicht innerhalb von 5 Sekunden antwortet, wenden Sie sich an den Workfront-Support oder lesen Sie [Versandanforderungen für Ereignisabschlüsse](../../wf-api/general/setup-event-sub-endpoint.md).
* Die Ereignisse generieren möglicherweise nicht die Art, wie Sie denken. Stellen Sie sicher, dass Sie keine Annahmen darüber machen, wie oder wann Ereignisse ausgelöst werden sollen und was tun. Sie können beispielsweise davon ausgehen, dass das Aktualisieren eines Dokuments für eine Aufgabe ein Ereignis zur Aufgabenaktualisierung generiert, stattdessen jedoch ein Ereignis zum Erstellen oder Aktualisieren von Dokumenten generiert.
* Ihr Abonnement wird möglicherweise nicht wie erwartet konfiguriert. Sie können Ereignisabonnements in verschiedenen Umgebungen erstellen und erwarten, dass diese wie ihre anderen Workfront-Daten übertragen. Ereignisabonnementdaten sind jedoch nicht so konfiguriert, dass sie kopiert oder in andere Umgebungen weitergeleitet werden. Stellen Sie sicher, dass Sie API-Anfragen an die richtige Umgebung senden und dass die Abonnements in dieser Umgebung wie erwartet konfiguriert sind.
* Die Payload wurde nicht empfangen, da die erforderliche Workfront-IP-Adresse nicht zur Zulassungsliste Ihrer Firewall hinzugefügt wurde. Ereignisabonnemensereignisse werden nur von wenigen IP-Adressen gesendet. Stellen Sie sicher, dass das Zielnetzwerk über alle IP-Ausnahmen verfügt, die für den Empfang von Payloads von Workfront-Ereignisanmeldungen erforderlich sind.

## Warum dauert es übermäßig lange, bis meine Nachrichten meinen Endpunkt erreichen?

Einige der folgenden Szenarien können verantwortlich sein:

* Ein großer Vorgang, wie eine Massenaktualisierung, im System kann dazu führen, dass eine große Menge von Nachrichten gleichzeitig in die Warteschlange gestellt wird, was einige Zeit in Anspruch nehmen kann.
* Lange Berechnungen oder Timeline-Berechnungen für große Projekte können zu einer Verzögerung bei der Veröffentlichung von Nachrichten für Event-Abonnements führen, die verwendet werden sollen.
* Das Abonnement wurde möglicherweise deaktiviert.

   * Wenn nach einer Übergangsphase von 100 Nachrichten eine bestimmte URL - die mit einem oder mehreren Abonnements verknüpft sein könnte - mehr als 70 % der Zeit fehlschlägt oder die URL nach 2000 aufeinander folgenden Versuchen nicht gesendet werden kann, werden alle Nachrichten, die mit Abonnements derselben URL übereinstimmen, nicht für den Versand versucht. Stattdessen werden diese Nachrichten für einen erneuten Versuch sofort in die Warteschlange gestellt.

      Alle 10 Minuten, nachdem eine URL deaktiviert wurde, versuchen wir, die nächste Nachricht zur Verarbeitung zu senden. Wenn diese Nachricht erfolgreich ist, aktivieren wir diese URL und anschließend alle entsprechenden Abonnements erneut. Wenn diese Nachricht nicht gesendet werden kann, wird der 10-minütige Timer zurückgesetzt und es wird erneut versucht, nachdem er abläuft.

      Dieses Verhalten kann als inkonsistenter oder verzögerter Versand wahrgenommen werden, es folgt jedoch einfach unseren Richtlinien für den Umgang mit Ereignisabonnement-Nachrichten.

   * Eine Ereignis-Abonnement-URL wird deaktiviert, wenn eine der folgenden Bedingungen erfüllt ist:

      * Die Anmelde-URL konnte 7 Tage lang nicht bereitgestellt werden und hat in den letzten 72 Stunden mindestens 2000 aufeinander folgende Versandversuche fehlgeschlagen.
      * Die Abonnement-URL konnte 50.000 aufeinander folgende Versuche nicht durchführen.

## Was soll ich tun, wenn ich beim Versuch, die Ereignisabonnement-API aufzurufen, den Status 500 erhalte?

Wenden Sie sich an den Workfront-Support. Informationen zum Kontakt mit dem Support finden Sie unter [Support kontaktieren](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).

## Welche verschiedenen Authentifizierungstypen kann ich mit Workfront-Ereignisabonnements verwenden?

Sie können jede Authentifizierung verwenden, die ein Trägertoken verwendet. Die **authToken** -Feld eines Abonnements ist eine Zeichenfolge, die ein OAuth2-Träger-Token darstellt, das zur Authentifizierung mit der URL verwendet wird, die in der **url** -Feld. Theoretisch kann dieser Token-Wert alles sein, solange der Ziel-Endpunkt weiß, wie er seine Kodierung handhabt, d. h. **UTF-8**.

## Wie lange sollte es dauern, bis ich meine Ereignis-Payload von Workfront-Ereignisanmeldungen erhalte?

Im Allgemeinen erhalten Sie in weniger als 5 Sekunden nach der Protokollierung der Datenänderung Versandanfragen für Ereignisabonnement-Ereignisse. Im Durchschnitt werden Webhook-Benachrichtigungen in weniger als 1 Sekunde nach der Datenänderung empfangen. Der Dienst kann jedoch Nachrichten in so großen Mengen erhalten, dass es auch länger dauern kann.

## Zusätzliche Ressourcen

* **API-Dokumentation**: [Ereignisabonnement-API](../../wf-api/general/event-subs-api.md)

* **Best Practices**: [Best Practices für Ereignisabonnements](../../wf-api/general/event-sub-best-practice.md)

* **Felder, die die Payloads der Trigger-Ereignisanmeldung enthalten**: [Ressourcen für Ereignisabonnements](../../wf-api/api/event-sub-resource-fields.md)

* **Neuversuche bei Ereignisabonnements**: [Wiederholungen von Ereignisabonnements](../../wf-api/api/event-sub-retries.md)

* **Konfigurieren der Firewall für Workfront**: [Konfigurieren der Zulassungsliste Ihrer Firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)
