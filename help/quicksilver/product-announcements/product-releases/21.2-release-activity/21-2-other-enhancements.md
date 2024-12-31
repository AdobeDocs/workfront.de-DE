---
content-type: release-notes
keywords: Hinweise,vierteljährlich,Aktualisierung,Freigabe
navigation-topic: 2021-2-release-activity
title: 21.2 Weitere Verbesserungen
description: Auf dieser Seite werden alle anderen Verbesserungen beschrieben, die mit Version 21.2 an der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Woche vom 10. Mai 2021 in der Produktionsumgebung verfügbar gemacht. Eine Liste aller mit Version 21.2 verfügbaren Änderungen finden Sie in der Übersicht über die Version 21.2.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f136c08b-63c0-4e1e-a048-09eb84a0ed54
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '610'
ht-degree: 0%

---

# 21.2 Weitere Verbesserungen

Auf dieser Seite werden alle anderen Verbesserungen beschrieben, die mit Version 21.2 an der Vorschau-Umgebung vorgenommen wurden. Diese Verbesserungen werden in der Woche vom 10. Mai 2021 in der Produktionsumgebung verfügbar gemacht. Eine Liste aller mit Version 21.2 verfügbaren Änderungen finden Sie unter Übersicht über Version [21.2](../../../product-announcements/product-releases/21.2-release-activity/21-2-release-overview.md).

## Wir sind jetzt offiziell Adobe Workfront

Workfront wurde in Adobe Workfront umbenannt.

Die wichtigsten Bereiche innerhalb der Adobe Workfront-Anwendung und unserer kundenorientierten Websites wurden aktualisiert. Andere Bereiche werden in Kürze aktualisiert.

**Aktualisierte Bereiche**

* Anmeldebildschirm, obere Navigation, Proofing
* Benutzeroberfläche für Layout-Vorlagen, Hauptmenü, benutzerdefinierter Forms-Export (nur in der neuen Adobe Workfront-Version verfügbar)
* Mobile App von Workfront (iOS und Android)

Bald aktualisierte Bereiche

* Proofing-Apps für Desktop und Mobilgeräte
* PDF-Exporte für Listen und Berichte
* Favicon-Symbol auf der Browser-Registerkarte

**Später aktualisierte Bereiche**

* E-Mail-Benachrichtigungen

## Auf die Zulassungsliste setzen Validierung von E-Mails

>[!NOTE]
>
>Nur in der neuen Adobe Workfront-Version verfügbar.

Wenn Sie die E-Mail-Zulassungsliste verwenden, werden jetzt neue und aktualisierte Benutzer-E-Mail-Adressen anhand der -Zulassungsliste validiert. Wenn Sie einen neuen Benutzer hinzufügen oder einen vorhandenen Benutzer bearbeiten und eine E-Mail-Domain eingeben, die sich nicht auf der -Zulassungsliste befindet, werden Sie über eine Meldung darauf hingewiesen, dass der Benutzer keine E-Mail-Nachrichten erhält. Sie können das Benutzerprofil zwar weiterhin speichern, sollten die Domain jedoch zur -Zulassungsliste hinzufügen, damit die Benutzerin bzw. der Benutzer E-Mails erhält.

Weitere Informationen finden Sie [Bearbeiten des Benutzerprofils](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Neues Erscheinungsbild für Objektkopfzeilen

>[!NOTE]
>
>Diese Funktion wurde am 10. März 2020 in der Produktionsumgebung veröffentlicht.
>
>Diese Funktion ist nur in der neuen Adobe Workfront-Version verfügbar.

Um die Informationshierarchie weiter zu stärken und Benutzenden zu helfen, klarer zu verstehen, auf welcher Seite sie sich befinden, verfügt jetzt jede Objektkopfzeile über:

* Bunte, modernere Symbole für jeden Objekttyp
* Der Objekttyp, der über dem Objektnamen aufgeführt ist
* Aktualisierter Schriftstil und Textgröße
* Weitere kleinere Stiländerungen

Zuvor gab es kein Symbol und rechts neben dem Objekttitel erschien ein Badge mit dem Objektnamen.

Die Seitenkopfzeilen von Bereichen in der neuen Workfront-Version - wie erweiterte Analyse, Ressourcenverwaltung und andere - haben ebenfalls dieses aktualisierte Erscheinungsbild.

Weitere Informationen zu den neuen Objektkopfzeilen in der neuen Workfront-Version finden Sie unter [Neue Objektkopfzeilen](../../../workfront-basics/the-new-workfront-experience/new-object-headers.md).

![](assets/product-announcement-object-header-350x179.png)

## Aktualisierungen der Antworten bei der Objektstatussuche

Workfront speichert Objektstatus jetzt auf neue Weise.

Diese Änderungen wirken sich nicht auf die Art und Weise aus, wie Statussuchanfragen gestellt werden. API-Anfragen, die eine Objektstatussuche enthalten, geben jedoch eine unvollständige Liste der Gruppenstatus zurück.

Weitere Informationen finden Sie unter [Änderungen der Core-API: Statussuchantworten](../../../wf-api/api/api-changes-search.md) .

## Payloads von Ereignisabonnements wurden aktualisiert, sodass sie alle Felder enthalten, die auf ID enden

Alle Payloads von Ereignisabonnements enthalten jetzt jedes Feld, das auf „ID“ endet.

Beachten Sie, dass jedes Objekt über einen eigenen eindeutigen Satz verknüpfter Felder verfügt, der einen eindeutigen Satz verknüpfter Felder enthält, die auf eine ID enden. Das bedeutet, dass zwar jede Payload alle zugehörigen Felder dieses Objekts enthält, die auf ID enden, jedes Objekt jedoch einen anderen Satz von Feldern hat, die auf ID enden.

## Blueprints-Beta jetzt in der Vorschau verfügbar

>[!NOTE]
>
>Diese Funktion wird in der Produktionsumgebung erst ab Version 21.3 im weiteren Verlauf dieses Jahres allgemein verfügbar sein. Nur in der neuen Adobe Workfront-Version verfügbar.

Blueprints bieten grundlegende Bausteine, mit denen Sie ein Work-Management-System erstellen können, das mit Ihnen wächst. Systemadministratoren können den Blueprint-Katalog durchsuchen und einsatzbereite Projektvorlagen installieren.

Weitere Informationen finden Sie unter [Blueprints](../../../administration-and-setup/blueprints/blueprints.md).
