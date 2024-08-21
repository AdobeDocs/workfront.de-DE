---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,security,certificate,Admin,Exemption,configure,metadata
navigation-topic: security
title: Adobe Workfront SAML 2.0-Metadatenzertifikat erneuern
description: Die Adobe Workfront-Server verwenden für Authentifizierung und Autorisierung das SAML 2.0-Protokoll. Nach der Aktualisierung bleibt das neue Zertifikat ein Jahr gültig. Wenn es an der Zeit ist, das Zertifikat in Ihrem Identitäts-Provider zu verlängern, erhalten Sie eine Warnung in Workfront, die Sie darauf hinweist, dass diese Änderung erforderlich ist. Als Workfront-Administrator können Sie diese Änderung auf Systemebene verwalten.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 206ea3ad1398849e26dea7fe77f6d7c027825b6f
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# Adobe Workfront SAML 2.0-Metadatenzertifikat erneuern

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die Admin Console integriert wurden. Wenn Ihr Unternehmen in der Adobe Admin Console integriert wurde, ist keine Aktion erforderlich.
>
>Eine Liste der Verfahren, die sich je nachdem, ob Ihr Unternehmen in die Adobe Admin Console integriert wurde, unterscheiden, finden Sie unter [Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Die Adobe Workfront-Server verwenden für Authentifizierung und Autorisierung das SAML 2.0-Protokoll. Nach der Aktualisierung bleibt das neue Zertifikat ein Jahr gültig. Wenn es an der Zeit ist, das Zertifikat in Ihrem Identitäts-Provider zu verlängern, erhalten Sie eine Warnung in Workfront, die Sie darauf hinweist, dass diese Änderung erforderlich ist. Als Workfront-Administrator können Sie diese Änderung auf Systemebene verwalten.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certificate before the specified date. Mismatched certificates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>Dies ist nicht verfügbar, wenn die Workfront-Instanz Ihres Unternehmens mit Adobe IMS aktiviert ist. Wenden Sie sich an Ihren Netzwerk- oder IT-Administrator, wenn Sie weitere Informationen benötigen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Alle</td> 
  </tr> 
 <tr> 
  <td role="rowheader">Adobe Workfront-Lizenz</td> 
  <td> <p>Neu: Standard </p>
 <p>oder</p> 
<p>Aktuell: Plan </p> 
</td> 
 </tr>   
 <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## SAML 2.0 in Workfront konfigurieren

So überprüfen Sie die Warnmeldung und bestätigen die Aktualisierung der SAML 2.0-Metadaten in Ihrem Identitäts-Provider:

{{step-1-to-setup}}

1. Klicken Sie auf **System** > **Single Sign-On**.

1. Wählen Sie im Dropdownmenü **Typ** die Option **SAML 2.0** aus.

1. Klicken Sie auf **SAML 2.0-Metadaten herunterladen**.

   Dadurch wird das erneuerte Workfront-Zertifikat für SAML 2.0 heruntergeladen, das die richtigen Metadaten für Ihren Server enthält.

1. Kopieren Sie in Ihrem Identitätsanbieter Ihre aktuelle ACS-URL (Assertion Consumer Service) (auch als Antwort-URL bezeichnet) an einen sicheren Ort.

   >[!CAUTION]
   >
   >Bevor Sie die Workfront-Metadaten in Schritt 6 in Ihren Single Sign-On (SSO)-Provider hochladen, kopieren Sie Ihre aktuelle ACS-URL (Assertion Consumer Service) an einen sicheren Ort. Diese URL, auch als Antwort-URL bezeichnet, befindet sich auf der Workfront-Konfigurationsseite Ihres SSO-Anbieters.
   >
   >
   >Wenn sich die ACS-URL nach dem Hochladen der Workfront-Metadaten ändert, bedeutet dies, dass die Metadaten möglicherweise eine falsche ACS-URL enthalten. Sie müssen sie wieder in die kopierte ändern, um die Single-Sign-On-Verbindung nicht zu unterbrechen. Ihr aktualisiertes Zertifikat ist nach diesem Vorgang weiterhin korrekt.

1. Aktualisieren Sie auf Ihrem Identitäts-Provider-Server das neue Zertifikat, das Sie heruntergeladen haben.
1. (Bedingt) Wenn sich die ACS-URL (Assertion Consumer Service) oder die Antwort-URL in Ihrem Identitäts-Provider geändert hat, ändern Sie sie zurück zu der URL, die Sie in Schritt 5 kopiert haben.
1. Stellen Sie in Workfront auf der Seite **Single Sign-on (SSO)** sicher, dass diese Option aktiviert ist: **Das neue Workfront-Zertifikat wurde bereits in den Identitätsanbieter hochgeladen**.

   >[!NOTE]
   >
   >* Diese Option ist nur sichtbar, wenn die folgenden Punkte zutreffen:
   >   * Ihr Unternehmen ist bereits für SAML 2.0 eingerichtet.
   >   * Das aktuelle Zertifikat läuft ab
   >   * Das neue Zertifikat ist verfügbar
   >* Wenn dieses Feld ausgewählt ist, können sich Workfront-Administratoren mit ihren SSO-Anmeldeinformationen oder Workfront-Anmeldeinformationen bei Workfront anmelden.

1. Klicken Sie auf **Speichern**.

   Die Warnmeldung wird nicht mehr angezeigt, da Sie die Verlängerung des SAML 2.0-Zertifikats auf dem Server Ihres Identitäts-Providers bestätigt haben.

1. Klicken Sie auf **Verbindung testen** , um Ihre Konfiguration zu testen.

   Es sollte eine Meldung angezeigt werden, die bestätigt, dass die Verbindung erfolgreich hergestellt wurde.

Wenden Sie sich für weitere Informationen oder Unterstützung bei der manuellen Konfiguration von Metadaten an unser Support-Team, wie unter [Support kontaktieren](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md) beschrieben.
