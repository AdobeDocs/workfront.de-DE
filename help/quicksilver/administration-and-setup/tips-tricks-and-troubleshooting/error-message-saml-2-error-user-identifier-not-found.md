---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Fehlermeldung: SAML 2.0 Fehler: Benutzerkennung nicht gefunden'
description: Es kann keine erfolgreiche Verbindung zu ADFS hergestellt werden.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '200'
ht-degree: 1%

---

# Fehlermeldung: SAML 2.0 Fehler: Benutzerkennung nicht gefunden

## Problem

Es kann keine erfolgreiche Verbindung zu ADFS hergestellt werden.

![identifier_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>Wenn Sie eine erfolgreiche Testverbindung herstellen und weiterhin Probleme auftreten, kann es sein, dass falsche Attributzuordnungen oder Probleme mit den Federation IDs vorliegen. Wenden Sie sich bei Fragen an den Support.

## Ursache:

Behauptungen auf dem ADFS-Server sind falsch.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td>
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lösung

Stellen Sie auf dem ADFS-Server sicher, dass ein Anspruch für die Namens-ID besteht:

1. Klicken Sie unter Windows auf **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0-]**.\
   Das Dialogfeld ADFS 2.0-Verwaltung wird angezeigt.

1. Wählen **[!UICONTROL Vertrauensbeziehung]** > **[!UICONTROL Vertrauensstellungen der vertrauenden]** im linken Bereich aus.

1. Klicken Sie mit der rechten Maustaste auf die Vertrauensstellung der vertrauenden Seite in Bezug auf Adobe Workfront und wählen Sie **[!UICONTROL Anspruchsregeln bearbeiten]**.
1. Überprüfen Sie, ob der Anspruch über **[!UICONTROL Typ des ausgehenden Anspruchs]** von **[!UICONTROL Name ID]** verfügt.

![1.png](assets/1-350x287.png)
