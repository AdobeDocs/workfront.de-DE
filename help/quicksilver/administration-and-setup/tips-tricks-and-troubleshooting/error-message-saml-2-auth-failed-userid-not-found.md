---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''Fehlermeldung: SAML 2.0 Authentifizierung fehlgeschlagen: Benutzerkennung nicht gefunden"'
description: Wenn Sie SAML 2.0 verwenden, bedeutet der Fehler "SAML 2.0 Authentication Failed-User Identifier Not Found", dass eine UID oder NAME ID nicht von den ADFS-Anforderungsregeln übergeben wird. In ADFS muss der "Relying Party Trust"über eine Anforderungsregel verfügen, die entweder eine UID oder einen NAME-ID-Wert übergibt. Wenn Sie eine [!DNL Workfront] Verbindung testen sollte, sollte dies bei Erfolg angezeigt werden.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 1%

---

# Fehlermeldung: SAML 2.0 Authentifizierung fehlgeschlagen: Benutzerkennung nicht gefunden

## Problem

Bei Verwendung von SAML 2.0 erhalte ich diesen Fehler: &quot;SAML 2.0 Authentifizierung fehlgeschlagen: Benutzer-ID nicht gefunden.&quot;

## Ursache

Dies geschieht bei einem **UID** oder **NAME-ID** wird nicht von der **ADFS-Anforderungsregeln**.

In ADFS **Vertrauen von Parteien** eine **Anforderungsregel** , die entweder eine **UID** oder **NAME-ID** -Wert. Wenn Sie eine **[!DNL Workfront]Verbindung testen**, sollte dies bei Erfolg angezeigt werden.

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

1. Beim Bearbeiten der **[!UICONTROL ADFS INFO]** in der **[!UICONTROL Vertrauen in Partei]** > Objekt auswählen >**[!UICONTROL Anforderungsregeln bearbeiten]**.

1. Die **[!UICONTROL LDAP-Attribut]** (linke Spalte) sollte **[!UICONTROL E-Mail-Adressen]** (oder eine beliebige eindeutige Kennung).

1. Die **[!UICONTROL Ausgehender Anforderungstyp]** (rechte Spalte) sollte **[!UICONTROL Name: ID]**.

   >[!NOTE]
   >
   >Es muss nicht über die LDAP-Attribut-E-Mail-Adressen verfügen. Jede eindeutige Kennung, die den Benutzer identifiziert, kann verwendet werden, muss jedoch an [!DNL Adobe Workfront] als **NAME-ID**.
