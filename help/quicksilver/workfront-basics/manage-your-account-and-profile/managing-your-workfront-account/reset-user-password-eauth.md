---
product-area: user-management
navigation-topic: manage-your-workfront-account
title: Zurücksetzen des Passworts einer Person mit erweiterter Authentifizierung
description: Wenn die erweiterte Authentifizierung (eAuth) für Ihre Umgebung aktiviert  [!DNL Workfront] , kann ein  [!DNL Workfront]  die Anmeldedaten für einen anderen Benutzer nicht zurücksetzen. Dies unterscheidet sich von  [!DNL Workfront]  ohne eAuth oder den Umgebungen, für die Single Sign-On (SSO) aktiviert ist.
author: Courtney
feature: Get Started with Workfront
hide: true
exl-id: 72f955e9-75ff-4ff7-b434-7a2b2d5ee0e8
TQID: https://experienceleague.adobe.com/DCTbiQAsLjKIEN4qNvPrCUDLO3eRnYhT1LYGKgwpf-Q
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 197
ht-degree: 16%

---

# Zurücksetzen des Passworts einer Person mit erweiterter Authentifizierung

<!--This article has been hidden by request-->

Wenn die erweiterte Authentifizierung (eAuth) für Ihre [!DNL Workfront]-Umgebung aktiviert ist, kann ein [!DNL Workfront]-Administrator die Anmeldedaten für einen anderen Benutzer nicht zurücksetzen. Dies unterscheidet sich von [!DNL Workfront] Umgebungen ohne eAuth oder den Umgebungen, für die Single Sign-On (SSO) aktiviert ist.

## Zugriffsanforderungen

Sie benötigen die folgenden Zugriffsrechte, um die Schritte in diesem Artikel auszuführen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Plan*</strong></td> 
   <td> <p> Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Lizenz*</strong></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen der Zugriffsebene*</strong></td> 
   <td> <p>Systemadministrator </p> </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

## Zurücksetzen des Passworts eines Benutzers in einer für eAuth aktivierten Umgebung

{{step-1-to-users}}

1. Wählen Sie **[!UICONTROL Benutzer]** aus, für den das Kennwort zurückgesetzt werden muss.
   ![Benutzer auswählen](assets/100520classicnweselectuser-350x105.png)

1. Klicken Sie auf die **[!UICONTROL Mehr]-Schaltfläche** die angezeigt wird, nachdem Sie die gewünschte **[!UICONTROL Benutzer]** ausgewählt haben, und wählen Sie die Option **[!UICONTROL E-Mail zu vergessenem Kennwort senden]** aus dem Dropdown-Menü aus.

   ![E-Mail zu vergessenem Kennwort senden](assets/100520classicnwesendemail-350x134.png)

Nach Auswahl der Option **[!UICONTROL E-Mail zu vergessenem Kennwort senden]** wird eine E-Mail an den ausgewählten Benutzer gesendet, die Anweisungen zum Ändern seines eigenen Kennworts enthält.

![E-Mail zurücksetzen](assets/pwresetemail-resized-350x461.png)
