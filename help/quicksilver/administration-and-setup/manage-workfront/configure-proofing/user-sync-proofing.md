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
TQID: 'https://experienceleague.adobe.com/oHi8YTmAgh3KY1xfh6psNCLr4Gng0iniB3LUqbBzcOw'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '333'
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
