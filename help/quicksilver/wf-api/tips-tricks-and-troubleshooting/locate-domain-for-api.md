---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Domänenformat für Adobe Workfront-API-Aufrufe
description: Suchen Sie Ihre Domäne zur Verwendung in der Adobe Workfront-API.
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: c2ce6776ceebe3c1d3915e3791fc84eb0245ba4d
workflow-type: tm+mt
source-wordcount: '147'
ht-degree: 0%

---

# Domänenformat für Adobe Workfront-API-Aufrufe

Wenn Sie die Workfront-API aufrufen, verwenden Sie die Domäne Ihres Unternehmens im -Aufruf. Das Format dieser Domänen-URL unterscheidet sich je nachdem, ob Ihr Unternehmen in die Adobe Unified Shell integriert wurde.

Um herauszufinden, ob sich Ihr Unternehmen auf der Adobe Unified Shell befindet, überprüfen Sie die URL, die beim Anzeigen einer Workfront-Seite angezeigt wird.

| Workfront-URL beginnt mit: | URL für API-Aufrufe: |
|---|---|
| `<yourdomain>.my.workfront.com` | `<yourdomain>.my.workfront.com` |
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

So suchen Sie Ihre Domäne:

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) oben rechts in Adobe Workfront oder (falls verfügbar) auf das Symbol **[!UICONTROL Hauptmenü]** (6}Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) oben links und klicken Sie dann auf das Symbol **[!UICONTROL Setup]** ![Setup](/help/_includes/assets/gear-icon-setup.png).![
1. Wählen Sie **System** und dann **Kundeninformationen** aus.

   Ihre Domäne wird rechts auf dem Bildschirm angezeigt.

   ![Domäne](assets/domain.png)

