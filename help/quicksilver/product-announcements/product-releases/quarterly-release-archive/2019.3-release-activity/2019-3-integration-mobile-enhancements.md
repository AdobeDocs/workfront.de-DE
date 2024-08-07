---
product-previous: mobile
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: Verbesserungen der Integration und Mobile 2019.3
description: Auf dieser Seite werden alle Änderungen beschrieben, die mit Version 2019.3 vorgenommen wurden. Es wurde in der Produktionsumgebung in der Woche vom 19. August 2019 zur Verfügung gestellt.
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 15e03405-63ff-48ea-b873-cf44f1f46282
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Verbesserungen der Integration und Mobile 2019.3

Auf dieser Seite werden alle Änderungen beschrieben, die mit Version 2019.3 vorgenommen wurden. Es wurde in der Produktionsumgebung in der Woche vom 19. August 2019 zur Verfügung gestellt.

Eine Liste aller Änderungen, die in Version 2019.3 vorgenommen wurden, finden Sie unter [Übersicht über die Release-Aktivität 2019.3](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Unterstützung freigegebener Elemente in der MS OneDrive-Integration

Jetzt können Sie Ihre freigegebenen OneDrive-Dateien und -Ordner mit Workfront-Objekten verknüpfen. Umgekehrt können Sie Dateien in Workfront in freigegebene Ordner in OneDrive hochladen.

Weitere Informationen finden Sie in den Abschnitten [Verknüpfen eines externen Dokuments mit Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents), [Verknüpfen eines oder mehrerer externer Ordner](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-a-folder) und [Aktualisieren und Verknüpfen eines Dokuments von Workfront mit einem externen Cloud-Anbieter](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) im Artikel [Verknüpfen von Dokumenten aus externen Anwendungen](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Weitere Informationen finden Sie im Abschnitt &quot;[Verknüpfen eines externen Dokuments mit Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents)&quot;im Artikel &quot;[Verknüpfen von Dokumenten aus externen Anwendungen&quot;](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)&quot;.

## Domänenspezifikation für alle Workfront-Anmeldungen erforderlich

Bei allen Workfront-Anmeldungen muss der Benutzer jetzt die Domäne angeben, wenn die Domäne nicht bereits in der Workfront-URL angegeben ist. Wenn Sie diese Informationen benötigen, wird die Sicherheit Ihrer Workfront-Instanz erhöht. Wenn Ihre Implementierung von Workfront mehrere Instanzen aufweist, können Sie mit dieser Verbesserung außerdem denselben Benutzer zu jeder Instanz von Workfront in Ihrer Implementierung hinzufügen.

Diese Änderung kann sich sowohl auf Benutzeranmeldungen als auch auf API-Integrationen auswirken:

* **Benutzeranmeldungen**

  Wenn Ihre Unternehmensdomäne nicht in der Workfront-URL enthalten ist, wird jetzt auf dem Anmeldebildschirm neben den Feldern Benutzername und Kennwort ein neues Feld Domäne angezeigt.

  Für die meisten Kunden ist keine Änderung erforderlich, da die Domäneninformationen bereits in der Workfront-URL enthalten sind. Beispiel: &quot;*domain*.my.workfront.com&quot;.

* **API-Integrationen**

  Wenn ein API-Code an eine Adresse gesendet wird, die Ihren Domänennamen nicht enthält, funktioniert dieser API-Code nicht mehr.

Weitere Informationen finden Sie unter [Bei Adobe Workfront anmelden](../../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/log-in-to-workfront.md).

## Konvertieren von Aufgaben und Problemen in Projekte mit der mobilen App in iOS

Sie können jetzt einzelne Aufgaben und Probleme in der mobilen Workfront-App in iOS in Projekte konvertieren.

## Melden Sie sich mit der Fingerabdruck- oder Gesicht-ID bei der mobilen App an

Je nach Gerät können Sie sich mit der Fingerabdruck- oder Gesicht-ID-Technologie bei der mobilen Workfront-App anmelden. Wenn Sie sich bei der Mobile App anmelden, werden Sie gefragt, ob Sie sich mit der von Ihrem Telefon unterstützten Authentifizierungsmethode anmelden möchten.

Weitere Informationen zum Verwalten dieser Funktion finden Sie unter [Adobe Workfront für iOS](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md) oder [Adobe Workfront für Android](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md).

## Neue Einstellung für die automatische Abmeldung von Benutzern auf einem Mobilgerät

Damit die mobile Workfront-App für Sie und Ihr Unternehmen sicherer wird, werden Benutzer nach 15 Tagen Inaktivität automatisch abgemeldet. Workfront-Administratoren können diese Zeitbeschränkung in der Webanwendung unter Einrichtung > System > Voreinstellungen anpassen.

Weitere Informationen finden Sie unter [Systemsicherheitsvoreinstellungen konfigurieren](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Mobile App erfordert Domäne beim Anmelden

Zur Verbesserung der Sicherheit müssen Sie bei der Workfront Mobile App jetzt Ihre Domäne angeben, wenn Sie sich nicht mit Single-Sign-On-Anmeldedaten anmelden.

>[!NOTE]
>
>iOS-Verfügbarkeit: 12. Juni 2019
>
>Produktionsverfügbarkeit: 17. Juni 2019

## Löschen von Objekten mithilfe der Mobile App in iOS

>[!NOTE]
>
>Diese Funktion wurde am 19. August 2019 in den App Stores für iOS zur Verfügung gestellt.

Sie können jetzt Objekte wie Aufgaben, Probleme und Timesheets in der mobilen iOS-App löschen. Sie müssen über die richtigen Berechtigungen für das Objekt verfügen, um es zu löschen.

## Filtern nach &quot;Dead Projects&quot;in der Mobile App

>[!NOTE]
>
>Diese Funktion ist ab der 19. August 2019 in den App Stores für iOS und Android verfügbar.

&quot;Inaktive Projekte&quot;wurde auf der Registerkarte &quot;Projekte&quot;der Mobile App als Filteroption hinzugefügt.

## Zurücksetzen Ihres Kennworts mithilfe der Mobile App

Sie können die Workfront Mobile App verwenden, um Ihr Kennwort zurückzusetzen, wenn Sie es vergessen haben. Tippen Sie auf Kennwort vergessen? und folgen Sie den Anweisungen auf dem Bildschirm. Sie können Ihr SSO-Kennwort in der Mobile App nicht zurücksetzen.

## Neues Erscheinungsbild für Mobilgeräte

Wir haben die folgenden Verbesserungen hinsichtlich Aussehen und Verhalten hinzugefügt, um Ihr Erlebnis in der mobilen Workfront-App zu verbessern.

* Die folgenden Bereiche wurden aus der oberen Leiste der Detailseite in markantere Bereiche auf dem Bildschirm verschoben:

   * Das Pluszeichen befindet sich jetzt in der unteren linken Ecke des Bildschirms
   * Das Häkchen, mit dem ein Element bearbeitet werden soll, ist jetzt die Schaltfläche &quot;Work On It&quot;(Bearbeiten auf einem Element) in der oberen Mitte des Bildschirms.

* Sie können jetzt angehängte benutzerdefinierte Formulare anzeigen, indem Sie unten auf der Detailseite auf Mehr anzeigen tippen.
* Das Erscheinungsbild der Seiten, die Sie zum Senden von Aufgaben, Problemen und Anforderungen verwenden, wurde geändert.

