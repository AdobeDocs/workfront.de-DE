---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: 'Fehlerbehebung: OutlookIdentityToken-Fehler bei Verwendung von Workfront für Outlook'
description: Wenn bei der Verwendung von Workfront für Outlook ein OutlookIdentityToken-Fehler auftritt, müssen ältere Microsoft 365-Token für Ihr Unternehmen aktiviert werden.
author: Becky
feature: Workfront Integrations and Apps
source-git-commit: 77cc1acde87b2ada96117daa06e98ba38e64fa8a
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# Fehlerbehebung: OutlookIdentityToken-Fehler bei Verwendung von Workfront für Outlook

Bei Verwendung von Workfront für Outlook wird möglicherweise der folgende Fehler angezeigt:

```
Unexpected error
Unable to get the outlookIdentityToken
```

Um diesen Fehler zu beheben, müssen Sie ältere Microsoft 365-Token für Ihr Unternehmen aktivieren. Da dies in Microsoft 365 erfolgen muss, kann Workfront diese Token für Ihr Unternehmen nicht aktivieren.

Anweisungen zur Aktivierung veralteter Microsoft 365-Token finden Sie unter [Aktivieren oder Deaktivieren veralteter Exchange Online-Token](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/turn-exchange-tokens-on-off) in der Dokumentation zu Microsoft.

Weitere Informationen zu Legacy-Token finden Sie unter [Kann ich ältere Exchange Online-Token wieder aktivieren?](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens#can-i-turn-exchange-online-legacy-tokens-back-on) in der Dokumentation zu Microsoft.
