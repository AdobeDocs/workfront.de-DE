---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Domänenformat für Adobe Workfront-API-Aufrufe
description: Suchen Sie Ihre Domäne zur Verwendung in der Adobe Workfront-API.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 8487f8d4b1651df268720806cfe07fa271a7b87d
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

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]** icon ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke auf **[!UICONTROL Einrichtung]** ![Einrichtungssymbol](/help/_includes/assets/gear-icon-setup.png).
1. Auswählen **System**, wählen Sie **Kundeninformationen**.

   Ihre Domäne wird rechts auf dem Bildschirm angezeigt.

   ![Domäne](assets/domain.png)