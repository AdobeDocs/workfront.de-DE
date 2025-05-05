---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Vorbereiten des Onboardings Ihres Unternehmens in der Adobe Admin Console
description: Da Adobe Workfront ein Adobe-Produkt ist, können Sie über die Adobe Admin Console darauf zugreifen. Auf diese Weise können Sie Workfront zusammen mit anderen Adobe-Konten und Produkten für Ihre Benutzerinnen und Benutzer an einem zentralen Ort verwalten.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: eb68357ed4fd8f323707aa4a54a0f946253bf4e0
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# Vorbereiten der Integration Ihres Unternehmens in die Adobe Admin Console

<!-- Audited: 12/2023 -->

Da Adobe Workfront ein Adobe-Produkt ist, können Sie über die Adobe Admin Console darauf zugreifen. Auf diese Weise können Sie Workfront zusammen mit anderen Adobe-Konten und Produkten für Ihre Benutzerinnen und Benutzer an einem zentralen Ort verwalten.

Alle Workfront-Kunden werden schließlich in die Adobe Admin Console verschoben. Nachdem Ihr Unternehmen zur Adobe Admin Console gewechselt ist, wird die Workfront-Authentifizierung von der Konsole verwaltet. Die Vorbereitung und Durchführung dieses Schritts früher legt den Grundstein für ein effizientes Arbeitsmanagement und positioniert Ihr Unternehmen für schnellere Innovationen in der Zukunft

Einen Überblick über Adobe Admin Console finden Sie unter Übersicht über die [Admin Console ](https://helpx.adobe.com/de/enterprise/using/admin-console.html).

## Migrations-Checkliste

Um sicherzustellen, dass Ihr Unternehmen zur Adobe Admin Console migrieren kann, müssen Sie die folgenden Schritte ausführen.

1. Identifizieren Sie die gewünschte Adobe Admin Console, der Sie Workfront hinzufügen möchten.

   * Wenn Ihr Unternehmen über keine bestehende Adobe Admin Console verfügt oder Sie keine bestehende Adobe Admin Console verwenden möchten, kann Ihnen der Workfront-Support bei der Erstellung einer neuen helfen.

   * Wenn Sie mehrere Adobe-Admin Consolen haben und sich nicht sicher sind, welche am besten zum Hinzufügen von Workfront geeignet ist, wenden Sie sich an den Workfront-Support.

1. Bestätigen Sie mit dem Workfront-Support, dass Sie eine bestehende Adobe Admin Console verwenden oder eine neue erstellen lassen möchten.

1. Einrichten der Identitätsverwaltung auf der Adobe Admin Console.

   >[!IMPORTANT]
   >
   >Bereiten Sie sich darauf vor, mit dem Workfront-Support und Ihrem IT-Team über Authentifizierungseinstellungen wie Single Sign-on (SSO) oder Nicht-SSO zu sprechen.

   Anweisungen finden Sie im Abschnitt Identity Management des [Bereitstellungshandbuchs für Adobe Admin Console](https://helpx.adobe.com/de/enterprise/using/deployment-planning.html).

1. (Bedingt) Wenn Sie Single Sign-on verwenden, verbinden Sie die neue Adobe Admin Console mit Ihrem bestehenden SSO-Anbieter.

   Weitere Informationen und Anweisungen finden Sie unter [Einrichten von Identitäten](https://helpx.adobe.com/de/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >Wenn Ihr Unternehmen kein Single Sign-on verwendet, erhalten alle Benutzenden, die zur Adobe Admin Console migriert wurden, eine E-Mail, in der sie ihr -Konto und -Passwort erstellen.

1. Sicherstellen, dass Benutzer-E-Mail-Adressen für die Migration bereit sind:

   1. Entfernen Sie doppelte E-Mails aus Workfront.

      Anweisungen finden Sie unter [Aktualisieren von E-Mail-Adressen vorhandener Benutzender in Ihrer Workfront](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md#update-email-addresses-of-existing-users-in-your-workfront-instance) in [Verhindern von Benutzerduplikaten](/help/quicksilver/administration-and-setup/manage-workfront/security/prevent-duplicate-users.md).

      Wenn in Ihrer Organisation doppelte E-Mail-Adressen vorhanden sind, wird der durch die E-Mail-Adresse mit der neuesten `lastLoginDate` dargestellte Benutzer in die Adobe Admin Console-Organisation verschoben. Alle anderen Benutzer mit dieser E-Mail-Adresse werden deaktiviert.

      >[!NOTE]
      >
      >Da jeweils nur ein Benutzer mit einer bestimmten E-Mail-Adresse aktiv sein kann, müssen Sie, wenn Sie einen anderen Benutzer mit derselben E-Mail-Adresse wie einen derzeit aktiven Benutzer aktivieren müssen, zunächst den derzeit aktiven Benutzer deaktivieren, bevor Sie den deaktivierten Benutzer aktivieren.

   1. (Bedingt) Wenn Sie benutzerdefinierte API-Integrationen verwenden, vergewissern Sie sich, dass diese Benutzer über eine gültige E-Mail-Adresse verfügen, auf die sie zugreifen können.

   1. (Optional) Es wird empfohlen, Benutzer zu deaktivieren, die keinen Zugriff mehr auf Workfront benötigen, sodass sie nicht zur Adobe Admin Console hinzugefügt werden.

   >[!IMPORTANT]
   >
   >Diese Aktionen in Bezug auf Benutzer-E-Mails müssen abgeschlossen sein, bevor Ihr Unternehmen zum Adobe Admin Console wechselt.

1. (Optional) Aktualisieren Sie alle benutzerdefinierten Integrationen für die Verwendung von OAuth2.

   Anweisungen zum Einrichten von OAuth2-Integrationen finden Sie unter [Erstellen von OAuth2-Programmen für Workfront-Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   >[!NOTE]
   >
   >Dieser Schritt ist optional, wird aber dringend empfohlen, da andere Formen der API-Authentifizierung und -Autorisierung in Zukunft nicht mehr unterstützt werden.

Nachdem Ihre Adobe Admin Console mit Workfront konfiguriert wurde, können Sie sie zum Erstellen Ihrer Workfront-Systemadministratoren verwenden.

Weitere Informationen finden Sie unter [Verwalten von Benutzern in der Adobe Admin Console](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

Eine Liste weiterer Aktionen, die sich je nachdem, ob Ihr Unternehmen Adobe Admin Console eingeführt hat, unterscheiden, finden Sie unter [Plattformbasierte Administrationsunterschiede (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
