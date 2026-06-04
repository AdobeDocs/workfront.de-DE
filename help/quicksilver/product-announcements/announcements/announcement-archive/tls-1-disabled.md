---
content-type: reference
navigation-topic: announcements
title: In Adobe Workfront ist TLS 1.2 erforderlich
description: Um optimale Sicherheit zu bieten, verlangt Adobe Workfront ein Upgrade aller Browser-Verbindungen und API-Integrationen, die auf TLS 1.0 oder früher angewiesen sind, auf TLS 1.2. In der Vorschau-Umgebung ist TLS 1.0 bereits deaktiviert.
author: Luke
feature: Product Announcements
exl-id: 153668ae-0647-47fd-9153-ce45cd8c54ee
TQID: https://experienceleague.adobe.com/23UVEvZitUFvhkTkgOnubLK76Lzl8QKiyz-R4svWcc8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 380
ht-degree: 4%

---

# In Adobe Workfront ist TLS 1.2 erforderlich

Um optimale Sicherheit zu bieten, verlangt Adobe Workfront ein Upgrade aller Browser-Verbindungen und API-Integrationen, die auf TLS 1.0 oder früher angewiesen sind, auf TLS 1.2. In der Vorschau-Umgebung ist TLS 1.0 bereits deaktiviert.

Workfront hat die Unterstützung für TLS 1.0 im März 2018 offiziell eingestellt. Alle Integrationen, die TLS 1.0 nutzen, funktionieren seit dem 9. Januar 2019 nicht mehr.  TLS 1.1 wird im 4. Quartal 2019 deaktiviert.

In den folgenden Abschnitten finden Sie weitere Details zu diesen wichtigen Meilensteinen sowie dazu, wie Sie sich auf dieses Upgrade in Ihrer Organisation vorbereiten können:

## Workfront beendet die offizielle Unterstützung für TLS 1.0 (5. März 2018)

Workfront beendete im März 2018 die offizielle Unterstützung für TLS 1.0.

Browser-Verbindungen und API-Integrationen, die TLS 1.0 nutzen, sind weiterhin funktionsfähig, aber Workfront löst keine Probleme in der Workfront-Anwendung, die mit TLS 1.0 in Verbindung stehen.

## Workfront-Integrationen mit TLS 1.0 deaktiviert (9. Januar 2019)

Am 9. Januar 2019 müssen alle Workfront-Browser-Verbindungen und API-Integrationen, die TLS 1.0 nutzen, auf die Verwendung von TLS 1.1 oder höher aktualisiert werden. Browser-Verbindungen und API-Integrationen, die weiterhin TLS 1.0 (eingehende oder ausgehende Verbindungen) nutzen, können nach dieser Zeit nicht mehr mit der Workfront-Anwendung kommunizieren. 

## TLS 1.1 wird im 4. Quartal 2019 deaktiviert

In der Produktionsumgebung wurde TLS 1.1 am 21. Oktober 2019 deaktiviert. Nach dieser Zeit funktionieren alle Integrationen, die TLS 1.1 verwenden, nicht mehr.

Diese Änderung tritt am 7. August in den Vorschau- und Sandbox-Umgebungen in Kraft, um Organisationen bei der Vorbereitung auf das Abschalten zu unterstützen.

## Vorbereiten der TLS-Aktualisierung

* [Beim Zugriff auf Workfront über den Browser](#when-accessing-workfront-via-the-browser)
* [Beim Herstellen einer Verbindung zu Workfront über die API](#when-connecting-to-workfront-via-the-api)

### Beim Zugriff auf Workfront über den Browser {#when-accessing-workfront-via-the-browser}

Stellen Sie sicher, dass Benutzende in Ihrem Unternehmen über einen unterstützten Browser auf Workfront zugreifen. (Informationen zu unterstützten Browsern finden Sie unter [Adobe Workfront-Browser-Anforderungen](../../../workfront-basics/workfront-browser-requirements.md).)

Alle von Workfront unterstützten Browser sind mit TLS 1.2 kompatibel.

### Beim Herstellen einer Verbindung zu Workfront über die API {#when-connecting-to-workfront-via-the-api}

Wenn Sie Anwendungen von Drittanbietern über die API (eingehend oder ausgehend) in Workfront integrieren, stellen Sie sicher, dass TLS 1.2 (und die TLS 1.2-Verschlüsselungsprotokolle) in Ihren Integrationen aktiviert sind.
