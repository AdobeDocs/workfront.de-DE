---
content-type: release-notes
keywords: notes,vierteljährlich,update,release
navigation-topic: 2021-2-release-activity
title: 21.2 Weitere Verbesserungen
description: Auf dieser Seite werden alle sonstigen Verbesserungen beschrieben, die mit Version 21.2 der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung ab der Woche vom 10. Mai 2021 verfügbar sein. Eine Liste aller in Version 21.2 verfügbaren Änderungen finden Sie in der Versionshinweise 21.2 .
author: Luke
feature: Product Announcements
exl-id: f136c08b-63c0-4e1e-a048-09eb84a0ed54
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '604'
ht-degree: 0%

---

# 21.2 Weitere Verbesserungen

Auf dieser Seite werden alle sonstigen Verbesserungen beschrieben, die mit Version 21.2 der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Produktionsumgebung ab der Woche vom 10. Mai 2021 verfügbar sein. Eine Liste aller in Version 21.2 verfügbaren Änderungen finden Sie unter [21.2 Versionsübersicht](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Wir sind jetzt offiziell in Adobe Workfront

Workfront wurde in Adobe Workfront umbenannt.

Die wichtigsten Bereiche innerhalb der Adobe Workfront-Anwendung und unserer kundenorientierten Websites werden jetzt aktualisiert. Andere Bereiche werden in Kürze aktualisiert.

**Aktualisierte Bereiche**

* Anmeldebildschirm, obere Navigation, Testversand
* Benutzeroberfläche für Layoutvorlagen, Hauptmenü, benutzerdefinierter Forms-Export (nur im neuen Adobe Workfront-Erlebnis verfügbar)
* Workfront Mobile App (iOS und Android)

Gebiete, die bald aktualisiert werden

* Testen von Apps für Desktop und Mobilgeräte
* PDF-Exporte für Listen und Berichte
* Symbol &quot;Favicon&quot;auf der Registerkarte &quot;Browser&quot;

**Bereiche, die später aktualisiert werden**

* E-Mail-Benachrichtigungen

## Validierung von E-Mail-Zulassungslisten

>[!NOTE]
>
>Nur im neuen Adobe Workfront-Erlebnis verfügbar.

Wenn Sie die E-Mail-Zulassungsliste verwenden, werden neue und aktualisierte Benutzer-E-Mail-Adressen jetzt anhand der Zulassungsliste validiert. Wenn Sie einen neuen Benutzer hinzufügen oder einen vorhandenen Benutzer bearbeiten und eine E-Mail-Domäne eingeben, die nicht auf der Zulassungsliste vorhanden ist, werden Sie in einer Nachricht darüber informiert, dass der Benutzer keine E-Mail-Nachrichten erhält. Sie können das Benutzerprofil weiterhin speichern, aber Sie sollten die Domäne zur Zulassungsliste hinzufügen, damit der Benutzer E-Mails erhält.

Weitere Informationen finden Sie unter [Benutzerprofil bearbeiten](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Neues Erscheinungsbild für Objektüberschriften

>[!NOTE]
>
>Diese Funktion wurde am 10. März 2020 in der Produktionsumgebung veröffentlicht.
>
>Diese Funktion ist nur im neuen Adobe Workfront-Erlebnis verfügbar.

Um die Informationshierarchie weiter zu stärken und den Benutzern ein besseres Verständnis darüber zu ermöglichen, auf welcher Seite sie sich befinden, hat jeder Objektheader jetzt Folgendes:

* Farbvolle, modernere Symbole für jeden Objekttyp
* Der Objekttyp, der über dem Objektnamen aufgeführt ist
* Aktualisierter Schriftstil und Textgröße
* Sonstige geringfügige Stiländerungen

Zuvor gab es kein Symbol und ein Abzeichen mit dem Objektnamen wurde rechts neben dem Objektnamen angezeigt.

Auch die Seitenkopfzeilen von Bereichen im neuen Workfront-Erlebnis, wie erweiterte Analysen, Ressourcenverwaltung und andere, haben dieses aktualisierte Erscheinungsbild.

Weitere Informationen zu den neuen Objektheadern im neuen Workfront-Erlebnis finden Sie unter [Neue Objektüberschriften](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

![](assets/product-announcement-object-header-350x179.png)

## Aktualisierungen der Antworten auf die Objektstatus-Suche

Workfront speichert nun Objektstatus auf neue Weise.

Diese Änderungen wirken sich nicht darauf aus, wie Statussuchanfragen ausgeführt werden. API-Anfragen mit einer Objektstatussuche geben jedoch eine unvollständige Liste der Gruppenstatus zurück.

Weitere Informationen finden Sie unter [Core-API-Änderungen: Statussuchantworten](../../../wf-api/api/api-changes-search.md) .

## Payloads für Ereignisabonnements aktualisiert, um alle Felder einzuschließen, die auf ID enden

Alle Payloads für Ereignisabonnements enthalten jetzt alle Felder, die auf &quot;ID&quot;enden.

Es ist wichtig zu beachten, dass jedes Objekt über einen eigenen eindeutigen Satz verknüpfter Felder verfügt, der einen eindeutigen Satz verknüpfter Felder enthält, die in ID enden. Das bedeutet, dass jede Payload zwar alle zugehörigen Felder dieses Objekts enthält, die in ID enden, aber jedes Objekt einen anderen Satz von Feldern hat, die in ID enden.

## Blueprint-Beta ist jetzt in der Vorschau verfügbar

>[!NOTE]
>
>Diese Funktion ist in der Produktionsumgebung erst ab Version 21.3 verfügbar, also später in diesem Jahr. Nur im neuen Adobe Workfront-Erlebnis verfügbar.

Blueprints bietet grundlegende Bausteine, mit denen Sie ein Arbeitsverwaltungssystem erstellen können, das mit Ihnen wächst. Systemadministratoren können den Blueprints-Katalog durchsuchen und gebrauchsfertige Projektvorlagen installieren.

Weitere Informationen finden Sie unter [Blueprints](../../../administration-and-setup/blueprints/blueprints.md).
