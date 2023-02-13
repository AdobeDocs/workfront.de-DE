---
filename: prep-for-admin-console
user-type: administrator
content-type: reference
product-area: system-administration;workfront-integrations
navigation-topic: adobe-admin-console
title: Vorbereitung zur Integration Ihres Unternehmens in die Adobe Admin Console
description: Da Adobe Workfront ein Produkt der Adobe ist, können Sie über die Adobe Admin Console darauf zugreifen. Auf diese Weise können Sie Workfront gemeinsam mit anderen Benutzerkonten und -produkten für Adoben zentral verwalten.
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: d9b5e4a1-069e-48be-80d0-84f4bf8aea8b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Vorbereitung zur Integration Ihres Unternehmens in die Adobe Admin Console

Da Adobe Workfront ein Produkt der Adobe ist, können Sie über die Adobe Admin Console darauf zugreifen. Auf diese Weise können Sie Workfront gemeinsam mit anderen Benutzerkonten und -produkten für Adoben zentral verwalten.

Alle Workfront-Kunden werden schließlich in die Adobe Admin Console verschoben. Nachdem Ihr Unternehmen zur Adobe Admin Console wechselt, wird die Workfront-Authentifizierung von der Adobe Admin Console verwaltet. Die Vorbereitung und Durchführung dieses Schritts erfolgt frühzeitiger, damit Sie die Grundlagen für Effizienz im Arbeitsmanagement legen und Ihr Unternehmen für schnellere Innovationen in der Zukunft positionieren können

Einen Überblick über die Adobe Admin Console finden Sie unter [Übersicht über Admin Consolen](https://helpx.adobe.com/de/enterprise/using/admin-console.html).

## Checkliste für die Migration

Um sicherzustellen, dass Ihr Unternehmen zur Adobe Admin Console migrieren kann, müssen Sie die folgenden Schritte ausführen

1. Identifizieren Sie die gewünschte Adobe Admin Console, der Sie Workfront hinzufügen möchten.

   * Wenn Ihr Unternehmen nicht über eine vorhandene Adobe Admin Console verfügt oder Sie keine vorhandene Adobe Admin Console verwenden möchten, kann Ihnen der Workfront-Support bei der Erstellung einer neuen helfen.

   * Wenn Sie mehrere Adobe-Admin Consolen haben und nicht sicher sind, welche am besten geeignet ist, Adobe Workfront hinzuzufügen, wenden Sie sich an den Workfront-Support.

1. Vergewissern Sie sich beim Workfront-Support, dass Sie eine vorhandene Adobe Admin Console verwenden oder eine neue erstellen möchten.

1. Richten Sie die Identitätsverwaltung in der Adobe Admin Console ein.

   >[!IMPORTANT]
   >
   >Bereiten Sie sich darauf vor, mit dem Workfront-Support und Ihrem IT-Team über Authentifizierungseinstellungen wie Single Sign-on (SSO) oder Nicht-SSO zu sprechen.

   Anweisungen finden Sie im Abschnitt Identity Management des Bereitstellungshandbuchs für die Adobe Admin Console (https://helpx.adobe.com/enterprise/using/deployment-planning.html).

1. (Bedingt) Wenn Sie Single Sign-on verwenden, verbinden Sie die neue Adobe Admin Console mit Ihrem bestehenden SSO-Provider.

   Weitere Informationen und Anweisungen finden Sie unter [Identität einrichten](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

   >[!NOTE]
   >
   >Wenn Ihr Unternehmen Single Sign-on nicht verwendet, erhalten alle Benutzer, die in die Adobe Admin Console migriert wurden, eine E-Mail, um ihr Konto und ihr Kennwort zu erstellen.

1. Stellen Sie sicher, dass die E-Mail-Adressen der Benutzer für die Migration bereit sind:

   1. Entfernen doppelter E-Mails aus Workfront

      Anweisungen finden Sie unter E-Mail-Adressen vorhandener Benutzer in Ihrer Workfront-Instanz aktualisieren im Abschnitt Vermeiden von doppelten Benutzern.

      Wenn Ihre Organisation doppelte E-Mail-Adressen hat, wird der Benutzer durch die E-Mail-Adresse mit der neuesten `lastLoginDate` wird in die Adobe Admin Console-Organisation verschoben. Alle anderen Benutzer mit dieser E-Mail-Adresse werden deaktiviert.

      >[!NOTE]
      >
      >Da immer nur ein Benutzer mit einer bestimmten E-Mail-Adresse aktiv sein kann, müssen Sie zunächst den derzeit aktiven Benutzer deaktivieren, bevor Sie den deaktivierten Benutzer aktivieren, wenn Sie einen anderen Benutzer mit derselben E-Mail-Adresse wie einen derzeit aktiven Benutzer aktivieren müssen.

   2. (Bedingt) Wenn Sie benutzerdefinierte API-Integrationen verwenden, überprüfen Sie, ob diese Benutzer über eine gültige E-Mail-Adresse verfügen, auf die sie zugreifen können.

   3. (Optional) Es wird empfohlen, alle Benutzer zu deaktivieren, die keinen Zugriff mehr auf Workfront benötigen, damit sie nicht zur Adobe Admin Console hinzugefügt werden.
   >[!IMPORTANT]
   >
   >Diese Aktionen bezüglich Benutzer-E-Mails müssen abgeschlossen sein, bevor Ihr Unternehmen mit dem Umstieg auf Adobe Admin Console beginnt.

1. (Optional) Aktualisieren Sie alle benutzerdefinierten Integrationen, um OAuth2 zu verwenden.

   Anweisungen zum Einrichten von OAuth2-Integrationen finden Sie unter [OAuth2-Anwendungen für Workfront-Integrationen erstellen](../../administration-and-setup/configure-integrations/create-oauth-application.md).

   Das Erstellen von OAuth2-Integrationen ist nur im neuen Workfront-Erlebnis verfügbar.

   >[!NOTE]
   >
   >Dieser Schritt ist optional, wird jedoch dringend empfohlen, da andere Formen der API-Authentifizierung und -Autorisierung in Zukunft nicht mehr unterstützt werden.

Nachdem Ihr Adobe Admin Console mit Workfront konfiguriert wurde, können Sie ihn zur Verwaltung Ihrer Benutzer verwenden.

Weitere Informationen finden Sie unter [Benutzer in Adobe Admin Console verwalten](../../administration-and-setup/add-users/create-and-manage-users/admin-console.md).

Eine Liste weiterer Aktionen, die je nachdem, ob Ihr Unternehmen in die Adobe Admin Console integriert wurde, unterschiedlich sind, finden Sie unter [Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
