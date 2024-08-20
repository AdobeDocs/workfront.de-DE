---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Benutzersynchronisierung zwischen Adobe Workfront und Workfront Proof
description: Benutzerinformationen werden von Adobe Workfront mit Workfront Proof synchronisiert, nicht aber von Workfront Proof mit Workfront. Daher müssen Sie diese Änderungen jedes Mal, wenn Sie Benutzer erstellen oder ändern, in Workfront vornehmen. In Workfront Proof können Sie keine Änderungen an Benutzern vornehmen.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 4c88a249-b156-45c9-a44c-32f906bfa8a2
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 0%

---

# Benutzersynchronisierung zwischen Adobe Workfront und Workfront Proof

Benutzerinformationen werden von Adobe Workfront mit Workfront Proof synchronisiert, nicht aber von Workfront Proof mit Workfront. Daher müssen Sie diese Änderungen jedes Mal, wenn Sie Benutzer erstellen oder ändern, in Workfront vornehmen. In Workfront Proof können Sie keine Änderungen an Benutzern vornehmen.

Die folgenden Abschnitte enthalten Informationen zur Benutzersynchronisierung von Workfront nach Workfront Proof:

## Synchronisierte Informationen

Workfront synchronisiert die folgenden Benutzerinformationen mit Workfront Proof:

* Name (der Vor- und Nachname des Benutzers)
* E-Mail-Adresse

## Bei Synchronisation

Benutzerinformationen werden unter folgenden Umständen von Workfront nach Workfront Proof synchronisiert:

* Benutzerinformationen werden in Workfront aktualisiert
* Ein Benutzer wird in Workfront erstellt

Je nachdem, ob ein Benutzer mit derselben E-Mail-Adresse in Workfront Proof vorhanden ist, geschieht eine der folgenden Aktionen:

* **Wenn kein Benutzer mit einer entsprechenden E-Mail in Workfront Proof und** vorhanden ist

   * **Der Testversand ist für den Benutzer aktiviert:** Der Benutzer wird in Workfront Proof als Benutzer erstellt.
   * **Der Testversand ist für den Benutzer nicht aktiviert:** Der Benutzer wird in Workfront Proof als Kontakt erstellt.

* **Wenn ein Benutzer mit einer übereinstimmenden E-Mail in Workfront Proof vorhanden ist:** Die Testfunktion ist für diesen Benutzer in Workfront aktiviert (sofern sie nicht bereits aktiviert war) und die Informationen werden zwischen den beiden Benutzern synchronisiert.

  Weitere Informationen finden Sie unter [Konfigurieren des Testzugriffs eines Benutzers auf einen Benutzer](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) in [Konfigurieren des Testversand-Zugriffs eines Benutzers](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

  >[!IMPORTANT]
  >
  >Wenn ein Benutzer mit einer entsprechenden E-Mail-Adresse in seiner eigenen oder in einer anderen Testumgebung vorhanden ist, erstellt Workfront eine Alias-E-Mail-Adresse, indem die Konto-ID des Benutzers als Suffix zu seiner E-Mail hinzugefügt wird. Beispiel: *username+accountid@domain.com*. Benutzer erhalten weiterhin Testversandbenachrichtigungen, falls eine Alias-E-Mail erstellt wird.
