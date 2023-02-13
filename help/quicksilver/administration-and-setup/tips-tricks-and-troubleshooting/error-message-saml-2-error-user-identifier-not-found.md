---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''Fehlermeldung: SAML 2.0-Fehler: Benutzerkennung nicht gefunden"'
description: Sie können keine erfolgreiche Verbindung zu ADFS herstellen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 1%

---

# Fehlermeldung: SAML 2.0-Fehler: Benutzerkennung nicht gefunden

## Problem

Sie können keine erfolgreiche Verbindung zu ADFS herstellen.

![identifier_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>Wenn Sie eine erfolgreiche Testverbindung herstellen und weiterhin Probleme auftreten, kann es bei Ihnen zu falschen Zuordnungen von Attributen oder zu Problemen mit Verknüpfungs-IDs kommen. Wenden Sie sich bei Fragen an den Support.

## Ursache:

Behauptungen auf dem ADFS-Server sind falsch

## Zugriffsanforderungen

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen [!DNL Workfront] Administrator. Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p> <p><b>NOTE</b>: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Lösung

Stellen Sie auf dem ADFS-Server sicher, dass ein Anspruch auf Namen-ID besteht:

1. Klicken Sie unter Windows auf **[!UICONTROL Starten]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0-Verwaltung]**.\
   Das Dialogfeld ADFS 2.0-Verwaltung wird angezeigt.

1. Auswählen **[!UICONTROL Vertrauensbeziehung]** > **[!UICONTROL Vertrauen in Partei]** im linken Bereich.

1. Klicken Sie mit der rechten Maustaste auf das Vertrauen der vertrauenswürdigen Partei in Bezug auf Adobe Workfront und wählen Sie **[!UICONTROL Anforderungsregeln bearbeiten]**.
1. Stellen Sie sicher, dass der Anspruch eine **[!UICONTROL Ausgehender Anforderungstyp]** von **[!UICONTROL Name: ID]**.

![1.png](assets/1-350x287.png)
