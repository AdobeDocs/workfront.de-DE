---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 Beta-Version
description: Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit der Beta-Endversion 2018.2 verfügbar waren. Die Funktion wurde am 20. Juni 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird im Juli 2018 im Produktionsumfeld zur Verfügung gestellt.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 36001571-bf8c-4fe8-a66b-09d3726f66d3
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# 2018.2 Beta-Version

Auf dieser Seite werden alle Änderungen beschrieben, die zuletzt in der Vorschau-Umgebung mit der Beta-Endversion 2018.2 verfügbar waren. Die Funktion wurde am 20. Juni 2018 in der Vorschau-Umgebung bereitgestellt. Sie wird im Juli 2018 im Produktionsumfeld zur Verfügung gestellt.

>[!IMPORTANT]
>
> Die auf dieser Seite beschriebene Funktionalität kann sich vor der Verfügbarkeit in der Produktionsumgebung ändern.

Eine Liste aller Änderungen, die 2018.2 vorgenommen wurden, finden Sie unter  [Übersicht über die Versionsaktivität 2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md).

Die folgenden neuen Funktionen werden zum Zeitpunkt der Produktionsversion 18.2 veröffentlicht:

* [Festlegen von E-Mail-Versanddiensten für Antworten auf Workfront-E-Mail-Benachrichtigungen](#specify-mail-delivery-services-for-replying-to-workfront-email-notifications)
* [Empfangen von E-Mail-Benachrichtigungen für Kommentare zu Dokumenten](#receive-email-notifications-for-comments-on-documents)
* [Vom System verfolgte Aktualisierungen enthalten kein Symbol mehr](#system-tracked-updates-no-longer-contain-an-icon)
* [Option zum Konvertieren eines Kommentars in eine Aufgabe wurde entfernt](#option-to-convert-a-comment-to-a-task-was-removed)
* [Workfront für Salesforce](#workfront-for-salesforce)
* [Workfront für Slack-Verbesserungen](#workfront-for-slack-improvements)
* [Mobile Verbesserungen](#mobile-improvements)

## Festlegen von E-Mail-Versanddiensten für Antworten auf Workfront-E-Mail-Benachrichtigungen {#specify-mail-delivery-services-for-replying-to-workfront-email-notifications}

Workfront-Administratoren haben jetzt bei der Konfiguration von Workfront die Möglichkeit, über E-Mail-Antworten Kommentare zu Objekten abzugeben. Workfront kann so konfiguriert werden, dass entweder der Standard-E-Mail-Dienst oder ein POP-E-Mail-Konto verwendet wird.

Vor dieser Aktualisierung mussten Workfront-Administratoren für jeden Benutzer ein POP-Konto einrichten. 

Informationen zum Konfigurieren eines POP-E-Mail-Kontos finden Sie unter .

Weitere Informationen zum Standard-E-Mail-Dienst finden Sie unter .

## Empfangen von E-Mail-Benachrichtigungen für Kommentare zu Dokumenten {#receive-email-notifications-for-comments-on-documents}

Sie erhalten jetzt eine E-Mail-Benachrichtigung, wenn jemand ein Dokument kommentiert, dessen Inhaber Sie sind. Diese Option ist standardmäßig aktiviert. Sie können die Benachrichtigungseinstellung &quot;In meinem Dokument wird ein Kommentar hinzugefügt&quot;verwenden, um die E-Mail-Benachrichtigungsoption zu deaktivieren.

Vor dieser Änderung haben Sie keine Benachrichtigungen erhalten, wenn jemand ein Dokument kommentiert hat, dessen Inhaber Sie sind. 

Weitere Informationen finden Sie unter [Ihre eigenen E-Mail-Benachrichtigungen ändern](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Bei der Veröffentlichung dieser Funktion erhielten Benutzer zusätzlich zu einer E-Mail-Benachrichtigung eine In-App-Benachrichtigung. Sie erhalten keine In-App-Benachrichtigung mehr, wenn jemand ein Dokument kommentiert, dessen Inhaber Sie sind. 

## Vom System verfolgte Aktualisierungen enthalten kein Symbol mehr {#system-tracked-updates-no-longer-contain-an-icon}

Jedes Mal, wenn das Workfront-System eine Aktualisierung im Bereich Updates für ein Objekt erstellt (z. B. in einem Projekt), enthält diese Aktualisierung kein entsprechendes Symbol mehr.

Vor dieser Änderung enthielt jedes Systemupdate auch ein Symbol, das die durchgeführte Aktualisierung darstellte.

Weitere Informationen zu Systemaktualisierungen finden Sie unter [Vom System getrackte Aktualisierungen](../../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## Option zum Konvertieren eines Kommentars in eine Aufgabe wurde entfernt {#option-to-convert-a-comment-to-a-task-was-removed}

Die Option zum Konvertieren eines Kommentars in eine Aufgabe wurde entfernt.

Zuvor konnten Sie einen Kommentar in eine Aufgabe konvertieren, während Sie sich im Bereich &quot;Updates&quot;eines Objekts befinden.

## Workfront für Salesforce {#workfront-for-salesforce}

Wir veröffentlichen eine neue vordefinierte Integration zwischen Salesforce und Workfront. Sie können Folgendes tun:

* Erstellen Sie automatisch neue Workfront-Projekte, wenn eine Salesforce-Gelegenheit eine bestimmte Phase erreicht, wenn ein neues Produkt zu einer Gelegenheit hinzugefügt wird oder wenn der Kontotyp aktualisiert wird.
* Erstellen Sie Workfront-Anforderungen aus einer Salesforce-Gelegenheit oder einem Salesforce-Konto.

Diese Integration steht allen Kunden mit einer Workfront Pro Edition oder höher zur Verfügung und ist kostenlos.

Weitere Informationen zu Workfront für Salesforce finden Sie unter  [Adobe Workfront für Salesforce](../../../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce.md).

## Workfront für Slack-Verbesserungen {#workfront-for-slack-improvements}

Sie können konfigurieren, dass Workfront-Benachrichtigungen in Ihrem Slack Workfront-Kanal empfangen werden.

Die folgenden Workfront-Benachrichtigungen können auch für die Bereitstellung auf Slack konfiguriert werden:

* Wenn jemand Sie in einem Kommentar oder einer Aktualisierung markiert.
* Wenn Sie einer neuen Aufgabe oder einem neuen Problem zugewiesen sind.
* Wenn Sie aufgefordert werden, einen Artikel zu genehmigen.

Vor dieser Verbesserung konnten Sie keine Workfront-Benachrichtigungen in Slack erhalten.

Weitere Informationen zu Workfront-Benachrichtigungen unter Slack finden Sie unter [Empfangen von Adobe Workfront-Benachrichtigungen in Slack](../../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Mobile Verbesserungen {#mobile-improvements}

Die folgenden neuen Funktionen werden zum Zeitpunkt der Produktionsversion 18.2 in den mobilen Stores veröffentlicht:

* Inline-Bearbeitung für Objektnamen 

  Sie können jetzt Felder wie den Namen eines Projekts, einer Aufgabe oder eines Problems in der App inline bearbeiten.

* Hochladen von Dokumenten 

  Sie können jetzt Dokumente in Objekte in der mobilen Workfront-App hochladen.

* Profilbild hochladen 

  Sie können jetzt ein Profilfoto in Ihre mobile iOS-App hochladen.

  Diese Funktion ist nur für die mobile iOS-App verfügbar.

Die folgenden Funktionen wurden bereits für die Android Beta-Version der mobilen Workfront-App veröffentlicht und stehen auch für die öffentlichen Android- und iOS-Apps zur Verfügung. Das Erlebnis für die iOS-Plattform unterscheidet sich von dem bereits veröffentlichten Android-Erlebnis:

* Neue untere Navigationsleiste für iOS 

* Neues Tutorial-Erlebnis für iOS 

Weitere Informationen zu diesen Funktionen sowie Videos zu diesen Funktionen finden Sie unter [Aktivität &quot;Beta 4&quot;(Version 2018.2)](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-beta-4-release-activity.md) und [Aktivität &quot;Beta-Version 5&quot;2018.2](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-beta-5-release-activity.md).
