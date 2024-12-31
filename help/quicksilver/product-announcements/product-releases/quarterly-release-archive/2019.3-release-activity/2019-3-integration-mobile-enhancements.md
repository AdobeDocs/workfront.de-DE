---
product-previous: mobile
content-type: release-notes
navigation-topic: 2019-3-release-activity
title: 2019.3 Verbesserungen bei der Integration und Mobilgeräten
description: Auf dieser Seite werden alle Integrationsänderungen und Verbesserungen an Mobilgeräten beschrieben, die mit der Version 2019.3 vorgenommen wurden. Es wurde in der Woche vom 19. August 2019 in der Produktionsumgebung zur Verfügung gestellt.
author: Luke
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: 15e03405-63ff-48ea-b873-cf44f1f46282
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# 2019.3 Verbesserungen bei der Integration und Mobilgeräten

Auf dieser Seite werden alle Integrationsänderungen und Verbesserungen an Mobilgeräten beschrieben, die mit der Version 2019.3 vorgenommen wurden. Es wurde in der Woche vom 19. August 2019 in der Produktionsumgebung zur Verfügung gestellt.

Eine Liste aller in 2019.3 vorgenommenen Änderungen finden Sie unter [Übersicht über die Versionsaktivität 2019.3](../../../../product-announcements/product-releases/quarterly-release-archive/2019.3-release-activity/2019-3-release-activity-overview.md).

## Unterstützung freigegebener Elemente in der MS OneDrive-Integration

Jetzt können Sie Ihre freigegebenen OneDrive-Dateien und -Ordner mit Workfront-Objekten verknüpfen. Umgekehrt können Sie Dateien in Workfront in freigegebene Ordner in OneDrive hochladen.

Weitere Informationen finden Sie in den Abschnitten [Verknüpfen eines externen Dokuments mit Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents), [Verknüpfen von einem oder mehreren externen Ordnern](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-a-folder) und [Aktualisieren und Verknüpfen eines Dokuments aus Workfront mit einem externen Cloud-Anbieter](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#sending-documents) im Artikel [Verknüpfen von Dokumenten aus externen Anwendungen](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Weitere Informationen finden Sie im Abschnitt [Verknüpfen eines externen Dokuments mit Workfront](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) im Artikel [Verknüpfen von Dokumenten aus externen Anwendungen](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Für alle Workfront-Anmeldungen erforderliche Domain-Spezifikation

Bei allen Workfront-Anmeldungen muss der Benutzer jetzt die Domain angeben, wenn diese nicht bereits in der Workfront-URL angegeben ist. Wenn Sie diese Informationen benötigen, wird Ihre Workfront-Instanz sicherer. Wenn Ihre Workfront-Implementierung mehrere Instanzen hat, können Sie mit dieser Verbesserung außerdem denselben Benutzer zu jeder Instanz von Workfront innerhalb Ihrer Implementierung hinzufügen.

Diese Änderung kann sich sowohl auf Benutzeranmeldungen als auch auf API-Integrationen auswirken:

* **Benutzeranmeldungen**

  Wenn Ihre Unternehmens-Domain nicht in der Workfront-URL enthalten ist, wird jetzt auf dem Anmeldebildschirm neben den Feldern Benutzername und Kennwort ein neues Feld Domain angezeigt.

  Für die meisten Kunden ist keine Änderung erforderlich, da die Domain-Informationen bereits in der Workfront-URL enthalten sind. Beispiel: &quot;*domain*.my.workfront.com.“

* **API-Integrationen**

  Wenn Sie API-Code an eine Adresse senden, die Ihren Domain-Namen nicht enthält, funktioniert dieser API-Code nicht mehr.

Weitere Informationen finden Sie unter [Bei Adobe Workfront anmelden](../../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/log-in-to-workfront.md).

## Konvertieren von Aufgaben und Problemen in Projekte mithilfe der Mobile App in iOS

Sie können jetzt einzelne Aufgaben und Probleme in der Mobile App von Workfront in iOS in Projekte konvertieren.

## Melden Sie sich mit Fingerabdruck oder Gesicht-ID bei der Mobile App an

Je nach Gerät können Sie sich mit der Fingerabdruck- oder Gesichtstechnologie bei der Mobile App von Workfront anmelden. Wenn Sie sich bei der App anmelden, werden Sie gefragt, ob Sie sich mit der von Ihrem Telefon unterstützten Authentifizierungsmethode anmelden möchten.

Weitere Informationen zur Verwaltung dieser Funktion finden Sie unter [Adobe Workfront für iOS](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-ios.md) oder [Adobe Workfront für Android](../../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/workfront-for-android.md).

## Neue Einstellung zum automatischen Abmelden von Benutzern auf Mobilgeräten

Um die Sicherheit der Mobile App von Workfront für Sie und Ihr Unternehmen zu erhöhen, werden Benutzer nach 15 Tagen Inaktivität automatisch abgemeldet. Workfront-Administratoren können dieses Zeitlimit in der Web-Anwendung unter „Setup“ > „System“ > „Voreinstellungen“ anpassen.

Weitere Informationen finden Sie unter [Systemsicherheitseinstellungen konfigurieren](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Mobile App erfordert beim Anmelden die Domäne .

Zur Verbesserung der Sicherheit erfordert die Workfront Mobile App jetzt die Angabe Ihrer Domain, wenn Sie sich nicht mit Single Sign-On-Anmeldeinformationen anmelden.

>[!NOTE]
>
>Verfügbarkeit von iOS: 12. Juni 2019
>
>Produktionsverfügbarkeit: 17. Juni 2019

## Löschen von Objekten mit der Mobile App in iOS

>[!NOTE]
>
>Diese Funktion wurde in den App Stores für iOS in der Woche vom 19. August 2019 zur Verfügung gestellt.

Sie können jetzt Objekte wie Aufgaben, Probleme und Arbeitszeittabellen in der iOS Mobile App löschen. Sie müssen über die richtigen Berechtigungen für das Objekt verfügen, um es löschen zu können.

## Filtern nach eingestellten Projekten in der Mobile App

>[!NOTE]
>
>Diese Funktion wird in den App-Stores sowohl für iOS als auch für Android in der Woche vom 19. August 2019 verfügbar sein.

Wir haben auf der Registerkarte „Projekte“ in der Mobile App die Option „Inaktive Projekte“ als Filter hinzugefügt.

## Zurücksetzen des Kennworts mithilfe der Mobile App

Sie können die Workfront Mobile App verwenden, um Ihr Kennwort zurückzusetzen, wenn Sie es vergessen haben. Tippen Sie auf Kennwort vergessen? und folgen Sie den Anweisungen auf dem Bildschirm. Sie können Ihr SSO-Passwort in der Mobile App nicht zurücksetzen.

## Neues Erscheinungsbild für Mobilgeräte

Wir haben die folgenden Verbesserungen des Erscheinungsbilds hinzugefügt, um Ihr Erlebnis mit der Workfront Mobile App zu verbessern.

* Folgender Eintrag wurde aus der oberen Leiste auf der Seite „Details“ in hervorgehobene Bereiche auf dem Bildschirm verschoben:

   * Das Pluszeichen befindet sich jetzt in der linken unteren Ecke des Bildschirms
   * Das Häkchen, um mit der Arbeit an einem Element zu beginnen, ist jetzt eine Schaltfläche Bearbeiten in der oberen Mitte des Bildschirms

* Sie können jetzt angehängte benutzerdefinierte Formulare anzeigen, indem Sie unten auf der Detailseite auf Mehr anzeigen tippen.
* Das Erscheinungsbild der Seiten zum Senden von Aufgaben, Problemen und Anfragen wurde geändert.

