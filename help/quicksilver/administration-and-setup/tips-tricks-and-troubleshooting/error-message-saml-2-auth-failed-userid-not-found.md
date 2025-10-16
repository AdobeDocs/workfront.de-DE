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
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 2%

---

# Fehlermeldung: SAML 2.0-Authentifizierung fehlgeschlagen: Benutzerkennung nicht gefunden

## Problem

Ich erhalte diese Fehlermeldung bei Verwendung von SAML 2.0: „SAML 2.0-Authentifizierung fehlgeschlagen: Benutzer-ID nicht gefunden.“

## Ursache

Dies geschieht, wenn eine **UID** oder **NAME ID** nicht von den **ADFS-Anspruchsregeln** übergeben wird.

In ADFS muss **Vertrauensstellung der vertrauenden Seite** über eine **Anforderungsregel** verfügen, die entweder einen **UID**- oder einen **NAME ID**-Wert übergibt. Wenn Sie eine **[!DNL Workfront]Testverbindung ausführen** sollte diese bei Erfolg angezeigt werden.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationen der Zugriffsebene</td> 
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lösung

1. Beim Bearbeiten der **[!UICONTROL ADFS-]**&quot; im Fenster **[!UICONTROL Vertrauensstellungen der vertrauenden Seite]** > Objekt auswählen **[!UICONTROL Anspruchsregeln bearbeiten]**.

1. Das **[!UICONTROL LDAP-Attribut]** (linke Spalte) sollte **[!UICONTROL E-Mail-Adressen]** (oder eine eindeutige Kennung) enthalten.

1. Der **[!UICONTROL Typ des ausgehenden Anspruchs]** (rechte Spalte) sollte **[!UICONTROL Name ID]** lauten.

   >[!NOTE]
   >
   >Es muss nicht über die LDAP-Attribut E-Mail-Adressen verfügen. Es können alle eindeutigen Kennungen verwendet werden, die den Benutzer identifizieren. Sie müssen jedoch als [!DNL Adobe Workfront] ID an **übergeben**.
