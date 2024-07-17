---
content-type: reference
navigation-topic: announcements
title: TLS 1.2 in Adobe Workfront erforderlich
description: Um eine optimale Sicherheit zu gewährleisten, erfordert Adobe Workfront, dass alle Browserverbindungen und API-Integrationen, die auf TLS 1.0 oder früher basieren, auf TLS 1.2 aktualisiert werden. In der Vorschau-Umgebung ist TLS 1.0 bereits deaktiviert.
author: Luke
feature: Product Announcements
exl-id: 153668ae-0647-47fd-9153-ce45cd8c54ee
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# TLS 1.2 in Adobe Workfront erforderlich

Um eine optimale Sicherheit zu gewährleisten, erfordert Adobe Workfront, dass alle Browserverbindungen und API-Integrationen, die auf TLS 1.0 oder früher basieren, auf TLS 1.2 aktualisiert werden. In der Vorschau-Umgebung ist TLS 1.0 bereits deaktiviert.

Workfront hat den Support für TLS 1.0 im März 2018 offiziell eingestellt. Alle Integrationen mit TLS 1.0 funktionieren ab 9. Januar 2019 nicht mehr.  TLS 1.1 wird im 4. Quartal 2019 deaktiviert.

In den folgenden Abschnitten finden Sie weitere Details zu diesen wichtigen Meilensteinen sowie dazu, wie Sie sich auf diese Aktualisierung in Ihrem Unternehmen vorbereiten können:

## Workfront beendet die offizielle Unterstützung für TLS 1.0 (5. März 2018)

Workfront hat die offizielle Unterstützung für TLS 1.0 im März 2018 eingestellt.

Browserverbindungen und API-Integrationen, die TLS 1.0 nutzen, funktionieren weiterhin, Workfront löst jedoch keine Probleme in der Workfront-Anwendung, die mit TLS 1.0 in Verbindung stehen.

## Workfront-Integrationen mit TLS 1.0 deaktiviert (9. Januar 2019)

Ab dem 9. Januar 2019 müssen alle Workfront-Browserverbindungen und API-Integrationen, die TLS 1.0 nutzen, auf TLS 1.1 oder höher aktualisiert werden. Browserverbindungen und API-Integrationen, die weiterhin TLS 1.0 nutzen (eingehende oder ausgehende Verbindungen), können nach dieser Zeit nicht mehr mit der Workfront-Anwendung kommunizieren. 

## TLS 1.1 wird im 4. Quartal 2019 deaktiviert

In der Produktionsumgebung wurde TLS 1.1 am 21. Oktober 2019 deaktiviert. Danach funktionieren alle Integrationen mit TLS 1.1 nicht mehr.

Diese Änderung wird am 7. August in der Vorschau- und Sandbox-Umgebung wirksam, um Organisationen bei der Vorbereitung auf die Abschaltung zu unterstützen.

## Vorbereiten der TLS-Aktualisierung

* [Beim Zugriff auf Workfront über den Browser](#when-accessing-workfront-via-the-browser)
* [Bei der Verbindung zu Workfront über die API](#when-connecting-to-workfront-via-the-api)

### Beim Zugriff auf Workfront über den Browser {#when-accessing-workfront-via-the-browser}

Stellen Sie sicher, dass Benutzer in Ihrem Unternehmen über einen unterstützten Browser auf Workfront zugreifen. (Informationen zu unterstützten Browsern finden Sie unter [Browseranforderungen für Adobe Workfront](../../../workfront-basics/workfront-browser-requirements.md).)

Alle von Workfront unterstützten Browser sind mit TLS 1.2 kompatibel.

### Bei der Verbindung zu Workfront über die API {#when-connecting-to-workfront-via-the-api}

Wenn Sie Anwendungen von Drittanbietern über die API (entweder in- oder ausgehend) in Workfront integrieren, stellen Sie sicher, dass TLS 1.2 (und die TLS 1.2-Verschlüsselungsprotokolle) in Ihren Integrationen aktiviert ist.
