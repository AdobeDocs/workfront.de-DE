---
content-type: release-notes
navigation-topic: product-releases-archive
title: Versionsaktivität von Beta 2 2017.2
description: Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschau-Umgebung mit Beta 2 Version 2017.2 verfügbar sind. Die Funktion auf dieser Seite wurde am 24. Mai 2017 in der Vorschau-Umgebung verfügbar gemacht. Sie wird zwischen Ende Juli und Anfang August 2017 in der Produktionsumgebung verfügbar gemacht.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0aa8d61e-cf8c-46a7-b093-a0dbc90d37fd
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# Versionsaktivität von Beta 2 2017.2

Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschau-Umgebung mit Beta 2 Version 2017.2 verfügbar sind. Die Funktion auf dieser Seite wurde am 24. Mai 2017 in der Vorschau-Umgebung verfügbar gemacht. Sie wird zwischen Ende Juli und Anfang August 2017 in der Produktionsumgebung verfügbar gemacht.

>[!IMPORTANT]
>
>Die auf dieser Seite beschriebene Funktion kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller in 2017.2 vorgenommenen Änderungen finden Sie unter [Übersicht über die Versionsaktivität 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

Die Beta-Version 2017.2 enthält Verbesserungen sowohl für Workfront-Administratoren als auch für andere Benutzer:

**Für Administratoren:**

* [API-Verbesserung: Ereignisabonnements](#api-enhancement-event-subscriptions)

**Für alle Benutzer:**

* [Projekte abonnieren](#subscribe-to-projects)
* [Abo von Elementen aus E-Mail beenden](#unsubscribe-from-items-from-email)
* [Konfigurieren Sie, wie Meilensteine im Gantt-Diagramm angezeigt werden](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [Ressourcenpool-Vorlagen](#resource-pools-templates)
* [Anzeigen von Versionen von Korrekturabzugsdokumenten in Workfront](#view-versions-of-proofed-documents-within-workfront)
* [Neues Anfordererobjekt im Bericht zu Korrekturabzugsgenehmigungen](#new-requester-object-in-proof-approval-report)

## API-Verbesserung: Ereignisabonnements {#api-enhancement-event-subscriptions}

Wenn eine Aktion auf einem Workfront-Objekt stattfindet, das von Ereignisabonnements unterstützt wird, können Sie jetzt Workfront so konfigurieren, dass eine Antwort an Ihren gewünschten Endpunkt gesendet wird. Dies bedeutet, dass Ihre Integrationen in Echtzeit mit der Workfront-API interagieren können.

Weitere Informationen finden Sie unter [Ereignisabonnement-API](../../../../wf-api/general/event-subs-api.md). 

## Projekte abonnieren {#subscribe-to-projects}

Sie können jetzt neue Kommentare zu Projekten abonnieren, zu denen Sie nicht Mitglied des Projektteams sind. Vor dieser Version konnten Sie nur Kommentare zu Problemen und Aufgaben abonnieren.

Weitere Informationen zum Abonnieren von Elementen finden Sie unter [Abonnieren von Elementen in Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Abo von Elementen aus E-Mail stornieren {#unsubscribe-from-items-from-email}

Sie können sich über den „Unsubscribe“-Link in der Abonnement-E-Mail von Elementen abmelden. Zuvor konnten Sie das Abonnement für ein Element nur über die Workfront-Benutzeroberfläche kündigen.

Weitere Informationen zum Abmelden von Abonnement-E-Mails finden Sie im Abschnitt „Abmelden von E-Mail-Benachrichtigungen“ in [Adobe Workfront-Benachrichtigungen](../../../../workfront-basics/using-notifications/wf-notifications.md) 

## Konfigurieren der Anzeige von Meilensteinen im Gantt-Diagramm {#configure-how-milestones-are-displayed-on-the-gantt-chart}

***KORREKTUR &#x200B;**: Diese Funktion befindet sich derzeit nicht in der Sandbox-Vorschau-Umgebung. Die Veröffentlichung ist für einen späteren Zeitpunkt im Juni 2017 geplant.*

Es gibt jetzt zwei Optionen zum Anzeigen von Meilensteininformationen in einem Gantt-Diagramm. Sie können einen oder beide der folgenden Meilensteinindikatoren konfigurieren:

* Meilenstein-Diamanten (Symbol)

  Dieses Symbol wird im Gantt-Diagramm nach jeder Aufgabe angezeigt, die mit einem Meilenstein verbunden ist.

* Meilenstein-Linien

  Nach jeder Aufgabe, die mit dem Meilenstein verbunden ist, wird eine Linie für alle Aufgaben im Gantt-Diagramm angezeigt.

Vor dieser Änderung gab es nur eine Option, um die Anzeige von Meilensteinen in einem Gantt-Diagramm zu ermöglichen, die als „Meilensteine“ bezeichnet wird. Diese Option aktiviert sowohl das Meilenstein-Diamantsymbol als auch die Meilensteinlinie. Diese Indikatoren konnten nicht getrennt werden. Die beiden Optionen sind jetzt für alle Gantt-Diagramme verfügbar, einschließlich aller Projektlisten und Berichte. 

Weitere Informationen zum Konfigurieren der Anzeige von Informationen im Gantt-Diagramm finden Sie unter [Konfigurieren der Anzeige von Informationen im Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Vorlagen für Ressourcenpools {#resource-pools-templates}

Sie können jetzt Ressourcenpools für Vorlagen angeben. Vor dieser Version konnten Sie Ressourcenpools nur mit Benutzern und Projekten verknüpfen.

Weitere Informationen zu Ressourcenpools finden Sie unter [Ressourcenpools - Übersicht](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## Anzeigen von Versionen von Korrekturabzugsdokumenten in Workfront {#view-versions-of-proofed-documents-within-workfront}

Sie können jetzt Korrekturabzüge aus allen Versionen eines Korrekturabzugs in der Benutzeroberfläche von Workfront anzeigen. 

Vor dieser Änderung konnten Sie nur die neueste Version des Korrekturabzugs anzeigen.

Benutzende ohne Proofing-Lizenz können:

* Öffnen eines Korrekturabzugs für eine frühere Version eines Korrekturabzugs

Benutzende mit Proofing-Lizenz haben folgende Möglichkeiten:

* Öffnen eines Korrekturabzugs für eine frühere Version eines Korrekturabzugs
* Anzeigen der Details eines Korrekturabzugs für eine frühere Version eines geprüften Dokuments

Weitere Informationen finden Sie unter [Dokumentversionen verwalten](../../../../documents/managing-documents/manage-document-versions.md) in [Dokumentversionen verwalten](../../../../documents/managing-documents/manage-document-versions.md).

## Neues Anfordererobjekt im Bericht zu Korrekturabzugsgenehmigungen {#new-requester-object-in-proof-approval-report}

Beim Erstellen eines Berichts zur Korrekturabzugsgenehmigung gibt es jetzt ein neues Anfordererobjekt. Mit diesem Objekt können Sie Berichte zu Informationen über den Benutzer erstellen, der die Genehmigung des Korrekturabzugs angefordert hat. 

Das neue Anfordererobjekt im Bericht zu Korrekturabzugsgenehmigungen enthält alle Felder, die in anderen Objektberichten mit dem vorhandenen Benutzerobjekt verfügbar sind.

>[!NOTE]
>
> Diese Informationen sind im Bericht erst ab dem Zeitpunkt verfügbar, zu dem diese Funktion in die jeweilige Vorschau- oder Produktionsumgebung eingeführt wurde. Informationen in Berichten zum Objekt des Anforderers vor dem Zeitpunkt, zu dem diese Funktion eingeführt wurde, sind nicht verfügbar.

Sie greifen auf das Anfordererobjekt zu, wenn Sie einen Bericht zu Korrekturabzugsgenehmigungen erstellen, wie in [Erstellen eines benutzerdefinierten Berichts](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) beschrieben.

Weitere Informationen zum Objektbericht für Korrekturabzugsgenehmigungen finden Sie im Abschnitt [Objekte in Adobe Workfront verstehen](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) in [Objekte in Adobe Workfront verstehen](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
