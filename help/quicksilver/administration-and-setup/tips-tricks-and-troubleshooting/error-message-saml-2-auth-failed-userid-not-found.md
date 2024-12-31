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
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Fehlermeldung: SAML 2.0-Authentifizierung fehlgeschlagen: Benutzerkennung nicht gefunden

## Problem

Ich erhalte diese Fehlermeldung bei Verwendung von SAML 2.0: „SAML 2.0-Authentifizierung fehlgeschlagen: Benutzer-ID nicht gefunden.“

## Ursache

Dies geschieht, wenn eine **UID** oder **NAME ID** nicht von den **ADFS-Anspruchsregeln** übergeben wird.

In ADFS muss **Vertrauensstellung der vertrauenden Seite** über eine **Anforderungsregel** verfügen, die entweder einen **UID**- oder einen **NAME ID**-Wert übergibt. Wenn Sie eine **[!DNL Workfront]Testverbindung ausführen** sollte diese bei Erfolg angezeigt werden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

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

1. Beim Bearbeiten der **[!UICONTROL ADFS-]**&quot; im Fenster **[!UICONTROL Vertrauensstellungen der vertrauenden Seite]** > Objekt auswählen **[!UICONTROL Anspruchsregeln bearbeiten]**.

1. Das **[!UICONTROL LDAP-Attribut]** (linke Spalte) sollte **[!UICONTROL E-Mail-Adressen]** (oder eine eindeutige Kennung) enthalten.

1. Der **[!UICONTROL Typ des ausgehenden Anspruchs]** (rechte Spalte) sollte **[!UICONTROL Name ID]** lauten.

   >[!NOTE]
   >
   >Es muss nicht über die LDAP-Attribut E-Mail-Adressen verfügen. Es können alle eindeutigen Kennungen verwendet werden, die den Benutzer identifizieren. Sie müssen jedoch als **ID an [!DNL Adobe Workfront] übergeben**.
