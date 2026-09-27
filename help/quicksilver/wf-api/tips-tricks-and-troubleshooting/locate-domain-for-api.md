---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Domain-Format für Adobe Workfront-API-Aufrufe
description: Suchen Sie Ihre Domain zur Verwendung in der Adobe Workfront-API
author: Becky
feature: Workfront API
role: Developer
exl-id: 8f5b78c9-b84f-4f56-b7cc-ba686fac2da1
TQID: 'https://experienceleague.adobe.com/jzwKwes6zxs0KwpjFyP4VL7k2oRVx6KGUP07EQHE-gY'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
    internal-label: APIs
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: 682536a8-4872-5ee6-a8a6-8012d713482c
    internal-label: Workfront API
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 29%
---
# Domain-Format für Adobe Workfront-API-Aufrufe

Wenn Sie einen API-Aufruf an die Workfront-API durchführen, verwenden Sie im Aufruf die Domain Ihres Unternehmens.

Die URL, die Sie für den API-Aufruf erstellen, hängt von der URL ab, mit der Sie eine Verbindung zu Workfront herstellen.

| Workfront-URL beginnt mit: | URL für API-Aufrufe: |
|---|---|
| `experience.adobe.com` | `<yourdomain>.my.workfront.adobe.com` |

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

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
   <p>Abo</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++


So suchen Sie Ihre Domain:

1. Klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon.png) in der oberen rechten Ecke von Adobe Workfront oder (falls verfügbar) klicken Sie auf das **[!UICONTROL Hauptmenü]**-Symbol ![Hauptmenü](/help/_includes/assets/main-menu-icon-left-nav.png) in der oberen linken Ecke und klicken Sie dann auf **** Setup![Setup-Symbol](/help/_includes/assets/gear-icon-setup.png).
1. Wählen Sie **System** und dann **Kundeninformationen** aus.

   Ihre Domain wird auf der rechten Seite des Bildschirms aufgeführt.

   ![Domain](assets/domain.png)

