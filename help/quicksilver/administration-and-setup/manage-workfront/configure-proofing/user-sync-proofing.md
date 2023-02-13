---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Benutzersynchronisierung zwischen Adobe Workfront und Workfront Testversand
description: Benutzerinformationen werden von Adobe Workfront mit Workfront Testing synchronisiert. Es wird nicht vom Workfront-Testversand zu Workfront synchronisiert. Daher müssen Sie diese Änderungen jedes Mal, wenn Sie Benutzer erstellen oder ändern, in Workfront vornehmen. In Workfront Testversand können Sie keine Änderungen an Benutzern vornehmen.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
source-git-commit: b310e36c9eb148db631e7a3552a35dcccc652d60
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Benutzersynchronisierung zwischen Adobe Workfront und Workfront Testversand

Benutzerinformationen werden von Adobe Workfront mit Workfront Testing synchronisiert. Es wird nicht vom Workfront-Testversand zu Workfront synchronisiert. Daher müssen Sie diese Änderungen jedes Mal, wenn Sie Benutzer erstellen oder ändern, in Workfront vornehmen. In Workfront Testversand können Sie keine Änderungen an Benutzern vornehmen.

In den folgenden Abschnitten finden Sie Informationen zur Benutzersynchronisierung von Workfront zu Workfront Testversand:

## Synchronisierte Informationen

Workfront synchronisiert die folgenden Benutzerinformationen mit Workfront Testing:

* Name (der Vor- und Nachname des Benutzers)
* E-Mail-Adresse

## Bei Synchronisation

Benutzerinformationen werden unter folgenden Umständen von Workfront mit Workfront Testing synchronisiert:

* Benutzerinformationen werden in Workfront aktualisiert
* Ein Benutzer wird in Workfront erstellt

Je nachdem, ob ein Benutzer mit derselben E-Mail-Adresse in Workfront Testing vorhanden ist, geschieht eine der folgenden Aktionen:

* **Wenn kein Benutzer mit der entsprechenden E-Mail in Workfront Testing vorhanden ist und**

   * **Der Testversand ist für den Benutzer aktiviert:** Der Benutzer wird als Benutzer in Workfront Testversand erstellt.
   * **Der Testversand ist für den Benutzer nicht aktiviert:** Der Benutzer wird als Kontakt in Workfront Testversand erstellt.

* **Wenn ein Benutzer mit einer entsprechenden E-Mail in Workfront Testing vorhanden ist:** Der Testversand ist für diesen Benutzer in Workfront aktiviert (sofern er noch nicht aktiviert war) und die Informationen werden zwischen den beiden Benutzern synchronisiert.

   Weitere Informationen finden Sie unter [Konfigurieren des Testversand-Zugriffs eines Benutzers](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) in [Konfigurieren des Testversand-Zugriffs eines Benutzers](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

   >[!IMPORTANT]
   >
   >Wenn ein Benutzer mit einer entsprechenden E-Mail-Adresse in seiner eigenen oder in einer anderen Testumgebung vorhanden ist, erstellt Workfront eine Alias-E-Mail-Adresse, indem die Konto-ID des Benutzers als Suffix zu seiner E-Mail hinzugefügt wird. Beispiel: *username+accountid@domain.com*. Benutzer erhalten weiterhin Testversandbenachrichtigungen, falls eine Alias-E-Mail erstellt wird.
