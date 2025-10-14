---
user-type: administrator
content-type: reference;overview
product-area: system-administration;documents
navigation-topic: configure-proofing-functionality
title: Benutzersynchronisierung zwischen Adobe Workfront und Workfront Proof
description: Benutzerinformationen werden von Adobe Workfront mit Workfront Proof synchronisiert. Sie werden nicht von Workfront Proof mit Workfront synchronisiert. Aus diesem Grund müssen Sie diese Änderungen jedes Mal, wenn Sie Benutzende erstellen oder ändern, in Workfront vornehmen. Sie können in Workfront Proof keine Änderungen an Benutzenden vornehmen.
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

Benutzerinformationen werden von Adobe Workfront mit Workfront Proof synchronisiert. Sie werden nicht von Workfront Proof mit Workfront synchronisiert. Aus diesem Grund müssen Sie diese Änderungen jedes Mal, wenn Sie Benutzende erstellen oder ändern, in Workfront vornehmen. Sie können in Workfront Proof keine Änderungen an Benutzenden vornehmen.

Die folgenden Abschnitte enthalten Informationen zur Benutzersynchronisierung von Workfront mit Workfront Proof:

## Synchronisierte Informationen

Workfront synchronisiert die folgenden Benutzerinformationen mit Workfront Proof:

* Name (Vor- und Nachname des Benutzers)
* E-Mail-Adresse

## Wenn eine Synchronisierung erfolgt

Benutzerinformationen werden unter folgenden Umständen von Workfront mit Workfront Proof synchronisiert:

* Die Informationen eines Benutzers werden in Workfront aktualisiert
* Ein Benutzer wird in Workfront erstellt

Je nachdem, ob in Workfront Proof ein Benutzer mit derselben E-Mail-Adresse vorhanden ist, tritt einer der folgenden Schritte auf:

* **Wenn in Workfront Proof kein Benutzer mit einer entsprechenden E-Mail vorhanden ist und**

   * **Proofing ist für den Benutzer aktiviert:** Der Benutzer wird in Workfront Proof als Benutzer erstellt.
   * **Proofing ist für den Benutzer nicht aktiviert:** Der Benutzer wird in Workfront Proof als Kontakt erstellt.

* **Wenn in Workfront Proof eine Benutzerin oder ein Benutzer mit einer übereinstimmenden E-Mail vorhanden ist:** Proofing ist für diese Person in Workfront aktiviert (falls noch nicht aktiviert) und die Informationen werden zwischen den beiden Benutzerinnen bzw. Benutzern synchronisiert.

  Weitere Informationen finden Sie [Konfigurieren des Proofing-Zugriffs einer &#x200B;](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md) in [Konfigurieren des Proofing-Zugriffs einer Benutzerin oder eines Benutzers](../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md).

  >[!IMPORTANT]
  >
  >Wenn Benutzende mit einer entsprechenden E-Mail in ihrer eigenen oder einer anderen Proofing-Umgebung vorhanden sind, erstellt Workfront eine Alias-E-Mail-Adresse, indem die Konto-ID der Benutzenden als Suffix zu ihrer E-Mail hinzugefügt wird. Beispiel: *username+accountid@domain.com*. Benutzer erhalten weiterhin Korrekturabzugs-Benachrichtigungen, falls eine Alias-E-Mail erstellt wird.
