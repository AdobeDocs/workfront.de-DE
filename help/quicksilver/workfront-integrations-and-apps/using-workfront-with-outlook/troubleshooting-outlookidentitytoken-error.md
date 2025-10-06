---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 'Fehlerbehebung: OutlookIdentityToken-Fehler bei Verwendung von Workfront für Outlook'
description: Wenn bei der Verwendung von Workfront für Outlook ein OutlookIdentityToken-Fehler auftritt, müssen ältere Microsoft 365-Token für Ihr Unternehmen aktiviert werden.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4a911760-e3fe-4e77-b7aa-b08f9ea59d6a
source-git-commit: 793c8c940c8cb7ac53169edf21ddf28af2554120
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 43%

---

# Fehlerbehebung: OutlookIdentityToken-Fehler bei Verwendung von Workfront für Outlook

>[!IMPORTANT]
>
>[Microsoft hat die Unterstützung für veraltete Exchange Online-Token](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens) deaktiviert, die vom Workfront Outlook-Add-in zur Authentifizierung verwendet wurden. Diese Änderung durch Microsoft wurde schrittweise eingeführt und ist zum 1. Oktober 2025 abgeschlossen.
>
>**Da Microsoft diese Token deaktiviert hat, funktioniert die Integration von Workfront für Microsoft Outlook nicht mehr.**

Bei Verwendung von Workfront für Outlook wird möglicherweise der folgende Fehler angezeigt:

```
Unexpected error
Unable to get the outlookIdentityToken
```

Um diesen Fehler zu beheben, müssen Sie Microsoft 365-Legacytoken für Ihr Unternehmen aktivieren. Da dies in Microsoft 365 erfolgen muss, kann Workfront diese Token nicht für Ihr Unternehmen aktivieren.

Anweisungen zum Aktivieren von Microsoft 365-Legacytoken finden Sie unter [Aktivieren oder Deaktivieren von Legacytoken](https://learn.microsoft.com/de-de/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) in der Dokumentation zu Microsoft.

Weitere Informationen zu Legacytoken finden Sie unter [Kann ich Exchange Online Legacytoken wieder aktivieren?](https://learn.microsoft.com/de-de/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) in der Dokumentation zu Microsoft.
