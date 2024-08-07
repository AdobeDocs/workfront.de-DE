---
content-type: release-notes
navigation-topic: product-releases-archive
title: Beta 2-Release-Aktivität 2017.2
description: Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschauumgebung mit Beta 2 Version 2017.2 verfügbar sind. Die Funktionalität auf dieser Seite wurde am 24. Mai 2017 in der Vorschau-Umgebung bereitgestellt. Es wird von Ende Juli bis Anfang August 2017 in der Produktionsumgebung zur Verfügung gestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0aa8d61e-cf8c-46a7-b093-a0dbc90d37fd
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 0%

---

# Beta 2-Release-Aktivität 2017.2

Auf dieser Seite werden alle Änderungen beschrieben, die in der Vorschauumgebung mit Beta 2 Version 2017.2 verfügbar sind. Die Funktionalität auf dieser Seite wurde am 24. Mai 2017 in der Vorschau-Umgebung bereitgestellt. Es wird von Ende Juli bis Anfang August 2017 in der Produktionsumgebung zur Verfügung gestellt.

>[!IMPORTANT]
>
>Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen, die in Version 2017.2 vorgenommen wurden, finden Sie unter [Übersicht über die Release-Aktivität 2017.2](../../../../product-announcements/product-releases/quarterly-release-archive/2017.2-release-activity/2017-2-release-activity-overview.md).

Die Beta 2-Version 2017.2 enthält Verbesserungen für Workfront-Administratoren und andere Benutzer:

**Für Administratoren:**

* [API-Verbesserung: Ereignisanmeldungen](#api-enhancement-event-subscriptions)

**Für alle Benutzer:**

* [Projekte abonnieren](#subscribe-to-projects)
* [Abmeldung von Elementen von E-Mail](#unsubscribe-from-items-from-email)
* [Konfigurieren der Anzeige von Meilensteinen auf dem Gantt-Diagramm](#configure-how-milestones-are-displayed-on-the-gantt-chart)
* [Ressourcen-Pools-Vorlagen](#resource-pools-templates)
* [Anzeigen von Versionen von Testdokumenten in Workfront](#view-versions-of-proofed-documents-within-workfront)
* [Neues Anforderungsobjekt im Bericht zur Bestätigung der Genehmigung](#new-requester-object-in-proof-approval-report)

## API-Verbesserung: Ereignisanmeldungen {#api-enhancement-event-subscriptions}

Wenn eine Aktion auf einem Workfront-Objekt erfolgt, das von Ereignisabonnements unterstützt wird, können Sie Workfront jetzt so konfigurieren, dass eine Antwort an den gewünschten Endpunkt gesendet wird. Dadurch können Ihre Integrationen in Echtzeit mit der Workfront-API interagieren.

Weitere Informationen finden Sie unter [Ereignis-Abonnement-API](../../../../wf-api/general/event-subs-api.md). 

## Abonnieren von Projekten {#subscribe-to-projects}

Sie können jetzt neue Kommentare zu Projekten abonnieren, für die Sie nicht Teil des Projektteams sind. Vor dieser Version konnten Sie nur Kommentare zu Problemen und Aufgaben abonnieren.

Weitere Informationen zum Abonnieren von Elementen finden Sie unter [Artikel in Adobe Workfront abonnieren](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Abmeldung von Elementen von E-Mail {#unsubscribe-from-items-from-email}

Über den Link &quot;Abmeldung&quot; in der Abmelde-E-Mail können Sie sich von Artikeln abmelden. Zuvor war es nur möglich, sich von einem Element in der Workfront-Benutzeroberfläche abzumelden.

Weitere Informationen zum Abmelden von Abonnement-E-Mails finden Sie im Abschnitt &quot;Abmeldung von E-Mail-Benachrichtigung&quot; in [Adobe Workfront-Benachrichtigungen](../../../../workfront-basics/using-notifications/wf-notifications.md) 

## Konfigurieren der Anzeige von Meilensteinen im Gantt-Diagramm {#configure-how-milestones-are-displayed-on-the-gantt-chart}

***KORREKTUR **: Diese Funktion befindet sich derzeit nicht in der Sandbox-Vorschau-Umgebung. Sie soll zu einem späteren Zeitpunkt im Juni 2017 veröffentlicht werden.*

Es gibt jetzt zwei Optionen zum Anzeigen von Meilensteininformationen in einem Gantt-Diagramm. Sie können eine oder beide der folgenden Meilensteinindikatoren konfigurieren:

* Milestone Diamonds (Symbol)

  Dieses Symbol wird im Gantt-Diagramm nach jeder Aufgabe angezeigt, die mit einem Meilenstein verknüpft ist.

* Meilenstein-Linien

  Nach jeder Aufgabe, die mit dem Meilenstein verknüpft ist, wird für alle Aufgaben im Gantt-Diagramm eine Zeile angezeigt.

Vor dieser Änderung gab es nur eine Option, mit der Meilensteine in einem Gantt-Diagramm angezeigt werden konnten, die als &quot;Meilensteine&quot;bezeichnet wurde. Mit dieser Option wurden sowohl das Meilensteindiamantensymbol als auch die Meilensteinlinie aktiviert. Diese Indikatoren konnten nicht getrennt werden. Die beiden Optionen sind jetzt in allen Gantt-Diagrammen verfügbar, einschließlich aller Projektlisten und Berichte. 

Weitere Informationen zum Konfigurieren der Anzeige von Informationen im Gantt-Diagramm finden Sie unter [Konfigurieren der Anzeige von Informationen im Gantt-Diagramm](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md).

## Ressourcen-Pools-Vorlagen {#resource-pools-templates}

Sie können nun Ressourcen-Pools für Vorlagen angeben. Vor dieser Version konnten Sie Resource Pools nur mit Benutzern und Projekten verknüpfen.

Weitere Informationen zu Ressourcen-Pools finden Sie unter [Überblick über Ressourcenpools](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## Anzeigen von Versionen von Testdokumenten in Workfront {#view-versions-of-proofed-documents-within-workfront}

Sie können jetzt auf der Workfront-Benutzeroberfläche Testsendungen aus allen Versionen eines Testdokuments anzeigen. 

Vor dieser Änderung konnten Sie nur die neueste Version des getesteten Dokuments anzeigen.

Benutzer ohne Testlizenz können:

* Testversand für eine frühere Version eines Testdokuments öffnen

Benutzer mit einer Testlizenz können Folgendes tun:

* Testversand für eine frühere Version eines Testdokuments öffnen
* Testversand-Details einer früheren Version eines Testdokuments anzeigen

Weitere Informationen finden Sie unter [Dokumentversionen verwalten](../../../../documents/managing-documents/manage-document-versions.md) in [Dokumentversionen verwalten](../../../../documents/managing-documents/manage-document-versions.md).

## Neues Anforderungsobjekt im Bericht zur Bestätigung der Genehmigung {#new-requester-object-in-proof-approval-report}

Beim Erstellen eines Berichts zur Bestätigung des Testversands gibt es jetzt ein neues Anforderungsobjekt. Mit diesem Objekt können Sie Berichte zu Informationen über den Benutzer erstellen, der die Testversandvalidierung beantragt hat. 

Das neue Anfordererobjekt im Bericht zur Bestätigung enthält alle Felder, die mit dem vorhandenen User -Objekt in anderen Objektberichten verfügbar sind.

>[!NOTE]
>
> Diese Informationen sind im Bericht nur ab dem Zeitpunkt verfügbar, zu dem diese Funktion erstmals in der jeweiligen Vorschau- oder Produktionsumgebung eingeführt wurde. Informationen in Berichten zum Anforderungsobjekt, die vor der Einführung dieser Funktion erstellt wurden, sind nicht verfügbar.

Sie greifen beim Erstellen eines Berichts zur Bestätigung des Testversands auf das Anfordererobjekt zu, wie in [Benutzerdefinierten Bericht erstellen](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md) beschrieben.

Weitere Informationen zum Objektbericht für Testsendungen finden Sie im Abschnitt [Objekte in Adobe Workfront verstehen](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) in [Objekte in Adobe Workfront verstehen](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).
