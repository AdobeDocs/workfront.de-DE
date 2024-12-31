---
content-type: release-notes
navigation-topic: product-releases-archive
title: Aktivität "Beta-Endversion 2018.2“
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit der Beta-Endversion 2018.2 verfügbar waren. Die Funktion wurde am 20. Juni 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird ab Juli 2018 in der Produktionsumgebung verfügbar sein.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 36001571-bf8c-4fe8-a66b-09d3726f66d3
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# Aktivität &quot;Beta-Endversion 2018.2“

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit der Beta-Endversion 2018.2 verfügbar waren. Die Funktion wurde am 20. Juni 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird ab Juli 2018 in der Produktionsumgebung verfügbar sein.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktion kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen in Version 2018.2 finden Sie unter  Übersicht über die Versionsaktivität [2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

Die folgenden neuen Funktionen werden zum Zeitpunkt der Veröffentlichung der Produktionsversion 18.2 veröffentlicht:

* [Angeben der E-Mail-Zustelldienste für die Antwort auf Workfront-E-Mail-Benachrichtigungen](#specify-mail-delivery-services-for-replying-to-workfront-email-notifications)
* [E-Mail-Benachrichtigungen für Kommentare zu Dokumenten erhalten](#receive-email-notifications-for-comments-on-documents)
* [System-getrackte Updates enthalten kein Symbol mehr](#system-tracked-updates-no-longer-contain-an-icon)
* [Option zum Konvertieren eines Kommentars in eine Aufgabe wurde entfernt](#option-to-convert-a-comment-to-a-task-was-removed)
* [Workfront für Salesforce](#workfront-for-salesforce)
* [Verbesserungen bei Workfront for Slack](#workfront-for-slack-improvements)
* [Verbesserungen für Mobilgeräte](#mobile-improvements)

## Angeben von E-Mail-Zustelldiensten für das Antworten auf E-Mail-Benachrichtigungen in Workfront {#specify-mail-delivery-services-for-replying-to-workfront-email-notifications}

Workfront-Administratoren haben jetzt beim Konfigurieren von Workfront die Wahl zwischen E-Mail-Versand-Services, damit Benutzer Objekte über E-Mail-Antworten kommentieren können. Workfront kann so konfiguriert werden, dass entweder der standardmäßige E-Mail-Service oder ein POP-E-Mail-Konto verwendet wird.

Vor diesem Update mussten Workfront-Administratoren für jeden Benutzer ein POP-Konto einrichten. 

Informationen zum Konfigurieren eines POP-E-Mail-Kontos finden Sie unter .

Weitere Informationen zum standardmäßigen E-Mail-Service finden Sie unter .

## E-Mail-Benachrichtigungen für Kommentare zu Dokumenten empfangen {#receive-email-notifications-for-comments-on-documents}

Sie erhalten jetzt eine E-Mail-Benachrichtigung, wenn jemand einen Kommentar zu einem Dokument in Ihrem Besitz abgibt. Diese Option ist standardmäßig aktiviert. Sie können die Benachrichtigungseinstellung „Ein Kommentar wird zu meinem Dokument hinzugefügt“ verwenden, um die Option „E-Mail-Benachrichtigung“ zu deaktivieren.

Vor dieser Änderung haben Sie keine Benachrichtigungen erhalten, wenn jemand ein Dokument kommentiert hat, dessen Inhaber Sie sind. 

Weitere Informationen finden Sie unter [Eigene E-Mail-Benachrichtigungen ändern](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Als diese Funktion ursprünglich veröffentlicht wurde, erhielten Benutzerinnen und Benutzer zusätzlich zu einer E-Mail-Benachrichtigung eine In-App-Benachrichtigung. Sie erhalten keine In-App-Benachrichtigung mehr, wenn jemand einen Kommentar zu einem Dokument in Ihrem Besitz abgibt. 

## Systemgesteuerte Updates enthalten kein Symbol mehr {#system-tracked-updates-no-longer-contain-an-icon}

Jedes Mal, wenn das Workfront-System ein Update im Bereich Updates für ein Objekt erstellt (z. B. innerhalb eines Projekts), enthält dieses Update kein entsprechendes Symbol mehr.

Vor dieser Änderung enthielt jede Systemaktualisierung auch ein Symbol für die vorgenommene Aktualisierung.

Weitere Informationen zu Systemaktualisierungen finden Sie unter [System-getrackte Aktualisierungen](../../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## Option zum Konvertieren eines Kommentars in eine Aufgabe wurde entfernt {#option-to-convert-a-comment-to-a-task-was-removed}

Die Option zum Konvertieren eines Kommentars in eine Aufgabe wurde entfernt.

Zuvor konnten Sie im Bereich Aktualisierungen eines Objekts einen Kommentar in eine Aufgabe konvertieren.

## Workfront für Salesforce {#workfront-for-salesforce}

Wir veröffentlichen eine neue vordefinierte Integration zwischen Salesforce und Workfront. Sie können Folgendes tun:

* Erstellen Sie automatisch neue Workfront-Projekte, wenn eine Opportunity in Salesforce eine bestimmte Phase erreicht, wenn ein neues Produkt zu einer Opportunity hinzugefügt wird oder wenn der Kontotyp aktualisiert wird.
* Erstellen Sie Workfront-Anfragen über eine Opportunity oder ein Konto in Salesforce.

Diese Integration steht allen Kundinnen und Kunden mit einer Workfront Pro Edition oder höher zur Verfügung und ist kostenlos.

Weitere Informationen zu Workfront für Salesforce finden Sie unter  [Adobe Workfront für Salesforce](../../../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce.md).

## Verbesserungen bei Workfront für Slack {#workfront-for-slack-improvements}

Sie können konfigurieren, dass Workfront-Benachrichtigungen in Ihrem Slack-Workfront-Kanal empfangen werden.

Die folgenden Workfront-Benachrichtigungen können auch so konfiguriert werden, dass sie in Slack gesendet werden:

* Wenn Sie jemand in einem Kommentar oder einer Aktualisierung taggt.
* Wenn Sie einer neuen Aufgabe oder einem neuen Problem zugewiesen werden.
* Wenn Sie aufgefordert werden, ein Element zu genehmigen.

Vor dieser Verbesserung konnten Sie keine Workfront-Benachrichtigungen auf Slack erhalten.

Weitere Informationen zu Workfront-Benachrichtigungen auf Slack finden Sie unter [Empfangen von Adobe Workfront-Benachrichtigungen auf Slack](../../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Verbesserungen für Mobilgeräte {#mobile-improvements}

Die folgenden neuen Funktionen werden zum Zeitpunkt der Veröffentlichung der Produktionsversion 18.2 in den mobilen Stores veröffentlicht:

* Inline-Bearbeitung für Objektnamen 

  Sie können jetzt Felder wie den Namen eines Projekts, einer Aufgabe oder eines Problems in der Mobile App inline bearbeiten.

* Dokumente hochladen 

  Sie können jetzt Dokumente in Objekte in der Workfront Mobile App hochladen.

* Hochladen eines Profilbilds 

  Sie können jetzt ein Profilfoto in Ihre iOS Mobile App hochladen.

  Diese Funktion ist nur für die Mobile App von iOS verfügbar.

Die folgenden Funktionen wurden bereits in der Android Beta-Version der Workfront-Mobile-App veröffentlicht und werden auch für die öffentliche Android und iOS-Mobile-Apps veröffentlicht. Das Erlebnis für die iOS-Plattform unterscheidet sich von dem bereits veröffentlichten Android-Erlebnis wie folgt:

* Neue Navigationsleiste unten für iOS 

* Neues Tutorial-Erlebnis für iOS 

Weitere Informationen zu diesen Funktionen und Videos, in denen diese Funktionen veranschaulicht werden, finden Sie unter [Versionsaktivität von Beta 4 ](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-beta-4-release-activity.md)2018.2 und [Versionsaktivität von Beta 5](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-beta-5-release-activity.md).
