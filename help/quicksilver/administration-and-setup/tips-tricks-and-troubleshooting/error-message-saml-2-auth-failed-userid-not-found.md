---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Fehlermeldung: SAML 2.0-Authentifizierung fehlgeschlagen: Benutzerkennung nicht gefunden'
description: Wenn Sie SAML 2.0 verwenden, bedeutet der Fehler „Fehlgeschlagene SAML 2.0-Authentifizierung - Benutzerkennung nicht gefunden“, dass eine UID- oder NAME-ID nicht aus den ADFS-Anspruchsregeln übergeben wird.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
TQID: https://experienceleague.adobe.com/YxLEE1OvD-Wo3FSd5ewXMfijsTaCjjCjzAx-EWWlBPE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 225
ht-degree: 13%

---

# Fehlermeldung: SAML 2.0-Authentifizierung fehlgeschlagen: Benutzerkennung nicht gefunden

## Problem

Ich erhalte diese Fehlermeldung bei Verwendung von SAML 2.0: „SAML 2.0-Authentifizierung fehlgeschlagen: Benutzer-ID nicht gefunden.“

## Ursache

Dies geschieht, wenn eine **UID** oder **NAME ID** nicht von den **ADFS-Anspruchsregeln** übergeben wird.

In ADFS muss **Vertrauensstellung der vertrauenden Seite** über eine **Anforderungsregel** verfügen, die entweder einen **UID**- oder einen **NAME ID**-Wert übergibt. Wenn Sie eine **[!DNL Workfront]Testverbindung ausführen** sollte diese bei Erfolg angezeigt werden.

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] Packstück</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] Lizenz</td> 
   <td><p>Standard</p>
       <p>Abo</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.

+++

## Lösung

1. Beim Bearbeiten der **[!UICONTROL ADFS-]**&quot; im Fenster **[!UICONTROL Vertrauensstellungen der vertrauenden Seite]** > Objekt auswählen **[!UICONTROL Anspruchsregeln bearbeiten]**.

1. Das **[!UICONTROL LDAP-Attribut]** (linke Spalte) sollte **[!UICONTROL E-Mail-Adressen]** (oder eine eindeutige Kennung) enthalten.

1. Der **[!UICONTROL Typ des ausgehenden Anspruchs]** (rechte Spalte) sollte **[!UICONTROL Name ID]** lauten.

   >[!NOTE]
   >
   >Es muss nicht über die LDAP-Attribut E-Mail-Adressen verfügen. Es können alle eindeutigen Kennungen verwendet werden, die den Benutzer identifizieren. Sie müssen jedoch als **ID an [!DNL Adobe Workfront] übergeben**.
