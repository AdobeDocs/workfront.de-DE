---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 'Fehlerbehebung: OutlookIdentityToken-Fehler bei Verwendung von Workfront für Outlook'
description: Wenn bei der Verwendung von Workfront für Outlook ein OutlookIdentityToken-Fehler auftritt, müssen ältere Microsoft 365-Token für Ihr Unternehmen aktiviert werden.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4a911760-e3fe-4e77-b7aa-b08f9ea59d6a
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 31%

---

# Fehlerbehebung: OutlookIdentityToken-Fehler bei Verwendung von Workfront für Outlook

>[!IMPORTANT]
>
>[Microsoft deaktiviert die Unterstützung für veraltete Exchange Online-Token](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), die derzeit vom Workfront Outlook-Add-in zur Authentifizierung verwendet werden. Diese Änderung durch Microsoft hat bereits Auswirkungen auf Kunden und wird bis Oktober 2025 schrittweise eingeführt.
>
>* **Nachdem Microsoft diese Token vollständig deaktiviert hat, funktioniert die Integration von Workfront für Microsoft Outlook nicht mehr.**
>
>Im Rahmen dieser Änderung hat Microsoft die Entscheidung getroffen, die Art und Weise zu ändern, wie Token wieder aktiviert werden. Nach dem **30. Juni** können Administratoren Token nicht mehr selbst erneut aktivieren - nur der Microsoft-Support kann Ausnahmen gewähren. **Am 1. Oktober 2025 werden alte Token für alle Mandanten deaktiviert. Ausnahmen werden nicht gewährt.**


Bei Verwendung von Workfront für Outlook wird möglicherweise der folgende Fehler angezeigt:

```
Unexpected error
Unable to get the outlookIdentityToken
```

Um diesen Fehler zu beheben, müssen Sie Microsoft 365-Legacytoken für Ihr Unternehmen aktivieren. Da dies in Microsoft 365 erfolgen muss, kann Workfront diese Token nicht für Ihr Unternehmen aktivieren.

Anweisungen zum Aktivieren von Microsoft 365-Legacytoken finden Sie unter [Aktivieren oder Deaktivieren von Legacytoken](https://learn.microsoft.com/de-de/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) in der Dokumentation zu Microsoft.

Weitere Informationen zu Legacytoken finden Sie unter [Kann ich Exchange Online Legacytoken wieder aktivieren?](https://learn.microsoft.com/de-de/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) in der Dokumentation zu Microsoft.
