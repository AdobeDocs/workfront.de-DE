---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,Sicherheit,Zertifikat,Admin,Ausnahme,Konfigurieren,Metadaten
navigation-topic: security
title: Verlängern des Adobe Workfront SAML 2.0-Metadatenzertifikats
description: Die Adobe Workfront-Server verwenden das SAML 2.0-Protokoll für die Authentifizierung und Autorisierung. Nach der Aktualisierung bleibt das neue Zertifikat ein Jahr lang gültig. Wenn es Zeit ist, das Zertifikat auf Ihrem Identitätsanbieter zu verlängern, erhalten Sie in Workfront einen Warnhinweis, dass diese Änderung vorgenommen werden muss. Als Workfront-Administrator können Sie diese Änderung auf Systemebene verwalten.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 945fa710e98b094a37258d5c94f7b1a2eb056abb
workflow-type: tm+mt
source-wordcount: '713'
ht-degree: 0%

---

# Verlängern des Adobe Workfront SAML 2.0-Metadatenzertifikats

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren wurde entfernt, da es nur für Organisationen galt, die noch nicht in Adobe Admin Console integriert waren. Dieses Verfahren ist für Organisationen auf der Adobe Admin Console nicht erforderlich.
>
>Da nun alle Workfront-Organisationen in die Adobe Admin Console integriert wurden, wird dieser Artikel in naher Zukunft entfernt.

<!--DELETE ME MARCH 2026-->

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch keine Einführung in Admin Console erhalten haben. Wenn Ihre Organisation in die Adobe Admin Console integriert wurde, ist keine Aktion erforderlich.
>
>Eine Liste der Verfahren, die sich je nachdem, ob Ihr Unternehmen in die Adobe Admin Console integriert wurde, unterscheiden, finden Sie unter [Plattformbasierte Administrationsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Die Adobe Workfront-Server verwenden das SAML 2.0-Protokoll für die Authentifizierung und Autorisierung. Nach der Aktualisierung bleibt das neue Zertifikat ein Jahr lang gültig. Wenn es Zeit ist, das Zertifikat auf Ihrem Identitätsanbieter zu verlängern, erhalten Sie in Workfront einen Warnhinweis, dass diese Änderung vorgenommen werden muss. Als Workfront-Administrator können Sie diese Änderung auf Systemebene verwalten.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certificate before the specified date. Mismatched certificates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>Dies ist nicht verfügbar, wenn die Workfront-Instanz Ihres Unternehmens mit Adobe IMS aktiviert ist. Wenden Sie sich an Ihren Netzwerk- oder IT-Administrator, wenn Sie weitere Informationen benötigen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan</td> 
   <td>Beliebig</td> 
  </tr> 
 <tr> 
  <td role="rowheader">Adobe Workfront-Lizenz</td> 
  <td> <p>Neu: Standard </p>
 <p>oder</p> 
<p>Aktuell: Plan </p> 
</td> 
 </tr>   
 <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Sie müssen ein Workfront-Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Konfigurieren von SAML 2.0 in Workfront

So überprüfen Sie die Warnmeldung und bestätigen die Aktualisierung der SAML 2.0-Metadaten in Ihrem Identitätsanbieter:

{{step-1-to-setup}}

1. Klicken Sie auf **System** > **Single Sign-On**.

1. Wählen Sie **Dropdown** Menü „Typ“ die Option **SAML 2.0**.

1. Klicken Sie **SAML 2.0-Metadaten herunterladen**.

   Dadurch wird das erneuerte Workfront-Zertifikat für SAML 2.0 heruntergeladen, das die richtigen Metadaten für Ihren Server enthält.

1. Kopieren Sie in Ihrem Identitätsanbieter Ihre aktuelle Assertion Consumer Service (ACS)-URL (auch als Antwort-URL bezeichnet) an einen sicheren Ort.

   >[!CAUTION]
   >
   >Kopieren Sie in Schritt 6 Ihre aktuelle Assertion Consumer Service (ACS)-URL an einen sicheren Ort, bevor Sie die Workfront-Metadaten in Ihren Single Sign-On (SSO)-Provider hochladen. Diese URL, auch als Antwort-URL bezeichnet, befindet sich auf der Workfront-Konfigurationsseite Ihres SSO-Anbieters.
   >
   >
   >Wenn sich die ACS-URL nach dem Hochladen der Workfront-Metadaten ändert, bedeutet dies, dass die Metadaten möglicherweise eine falsche ACS-URL enthalten. Sie müssen sie wieder in die kopierte Version ändern, damit Ihre Single-Sign-On-Verbindung nicht unterbrochen wird. Ihr aktualisiertes Zertifikat ist auch danach korrekt.

1. Aktualisieren Sie auf Ihrem Identitätsanbieter-Server das neue Zertifikat, das Sie heruntergeladen haben.
1. (Bedingt) Wenn sich die Assertion Consumer Service (ACS)-URL oder Antwort-URL in Ihrem Identitätsanbieter geändert hat, ändern Sie sie wieder in die URL, die Sie in Schritt 5 kopiert haben.
1. Stellen Sie in Workfront auf der **Single Sign-On (SSO))**, dass die folgende Option ausgewählt ist: **Das neue Workfront-Zertifikat wurde bereits zum Identitätsanbieter hochgeladen**.

   >[!NOTE]
   >
   >* Diese Option ist nur sichtbar, wenn Folgendes zutrifft:
   >   * Ihre Organisation ist bereits für SAML 2.0 eingerichtet
   >   * Das aktuelle Zertifikat läuft ab
   >   * Das neue Zertifikat ist verfügbar
   >* Wenn dieses Feld ausgewählt ist, können sich Workfront-Administratoren mit ihren SSO-Anmeldeinformationen oder Workfront-Anmeldeinformationen bei Workfront anmelden.

1. Klicken Sie auf **Speichern**.

   Die Warnmeldung wird nicht mehr angezeigt, da Sie die Verlängerung des SAML 2.0-Zertifikats auf dem Server Ihres Identitätsanbieters bestätigt haben.

1. Klicken Sie **Verbindung testen**, um Ihre Konfiguration zu testen.

   Es sollte eine Meldung angezeigt werden, die bestätigt, dass die Verbindung erfolgreich hergestellt wurde.

Für weitere Informationen oder Unterstützung bei der manuellen Konfiguration von Metadaten wenden Sie sich bitte an unser Support-Team, wie unter [Kundensupport kontaktieren](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md) beschrieben.
