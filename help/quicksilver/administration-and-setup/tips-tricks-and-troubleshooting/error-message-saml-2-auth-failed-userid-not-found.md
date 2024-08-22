---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Fehlermeldung: SAML 2.0 Authentifizierung fehlgeschlagen: Benutzer-ID nicht gefunden"
description: Wenn Sie SAML 2.0 verwenden, bedeutet der Fehler "SAML 2.0 Authentication Failed-User Identifier Not Found", dass eine UID- oder NAME-ID nicht von den ADFS-Anforderungsregeln übergeben wird.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Fehlermeldung: SAML 2.0-Authentifizierung fehlgeschlagen: Benutzer-ID nicht gefunden

## Problem

Ich erhalte diesen Fehler bei Verwendung von SAML 2.0: &quot;SAML 2.0 Authentication Failed: User Identifier Not Found&quot;.

## Ursache

Dies geschieht, wenn eine **UID** oder **NAME ID** nicht von den **ADFS-Anforderungsregeln** übergeben wird.

In ADFS muss der **Vertrauenswürdige Partei-Trust** über eine **Schadensregel** verfügen, die entweder einen **UID**- oder einen **NAME-ID**-Wert übergibt. Wenn Sie eine **[!DNL Workfront]Testverbindung** ausführen, sollte dies bei Erfolg angezeigt werden.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan</td> 
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>
   <p>Neu: Standard</p>
   <p>oder</p>
   <p>Aktuell: Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td>Sie müssen ein [!DNL Workfront] -Administrator sein. </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lösung

1. Beim Bearbeiten von **[!UICONTROL ADFS INFO]** im Ordner **[!UICONTROL Vertrauende Parteivertrauer]** > Objekt auswählen >**[!UICONTROL Anforderungsregeln bearbeiten]**.

1. Das **[!UICONTROL LDAP-Attribut]** (linke Spalte) sollte über **[!UICONTROL E-Mail-Adressen]** (oder eine beliebige eindeutige Kennung) verfügen.

1. Der **[!UICONTROL ausgehende Anforderungstyp]** (rechte Spalte) sollte **[!UICONTROL Name ID]** sein.

   >[!NOTE]
   >
   >Es muss nicht über die LDAP-Attribut-E-Mail-Adressen verfügen. Jede eindeutige Kennung, die den Benutzer identifiziert, kann verwendet werden, muss jedoch als **NAME ID** an [!DNL Adobe Workfront] übergeben werden.
