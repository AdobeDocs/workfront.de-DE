---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Domain-Format für Adobe Workfront-API-Aufrufe
description: Suchen Sie Ihre Domain zur Verwendung in der Adobe Workfront-API
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
source-git-commit: b9547764abd4f1f61d93da6bc66d9e6776954f4d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 2%

---

# Domain-Format für Adobe Workfront-API-Aufrufe

Wenn Sie einen API-Aufruf an die Workfront-API durchführen, verwenden Sie im Aufruf die Domain Ihres Unternehmens. Das Format dieser Domain-URL unterscheidet sich, je nachdem, ob Ihr Unternehmen in die Adobe Unified Shell integriert wurde.

Um herauszufinden, ob sich Ihr Unternehmen auf der Adobe Unified Shell befindet, überprüfen Sie die URL, die angezeigt wird, wenn Sie eine Workfront-Seite aufrufen.

| Workfront-URL beginnt mit: | URL für API-Aufrufe: |
|---|---|
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


So suchen Sie Ihre Domain:

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **&#x200B;**&#x200B;Setup![Setup-Symbol](/help/_includes/assets/gear-icon-setup.png).
1. Wählen Sie **System** und dann **Kundeninformationen** aus.

   Ihre Domain wird auf der rechten Seite des Bildschirms aufgeführt.

   ![Domain](assets/domain.png)

