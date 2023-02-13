---
user-type: administrator
product-area: system-administration
keywords: SAML 2.0,security,certificate,Admin,Exemption,configure,metadata
navigation-topic: security
title: Adobe Workfront SAML 2.0-Metadatenzertifikat erneuern
description: Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die Admin Console integriert wurden. Wenn Ihr Unternehmen in der Adobe Admin Console integriert wurde, müssen Sie diese Aktion über die Adobe Admin Console durchführen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4b481215-36a1-4945-828a-1598502529d8
source-git-commit: 3f84f6b8d6cb36fdb23ff332c4078ac1da4a8745
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 0%

---

# Adobe Workfront SAML 2.0-Metadatenzertifikat erneuern

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die Admin Console integriert wurden. Wenn Ihr Unternehmen in der Adobe Admin Console integriert wurde, ist keine Aktion erforderlich.
>
>Eine Liste der Verfahren, die je nachdem, ob Ihr Unternehmen in die Adobe Admin Console integriert wurde, unterschiedlich sind, finden Sie unter [Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Die Adobe Workfront-Server verwenden für Authentifizierung und Autorisierung das SAML 2.0-Protokoll. Nach der Aktualisierung bleibt das neue Zertifikat ein Jahr gültig. Wenn es an der Zeit ist, das Zertifikat in Ihrem Identitäts-Provider zu verlängern, erhalten Sie eine Warnung in Workfront, die Sie darauf hinweist, dass diese Änderung vorgenommen werden muss. Als Workfront-Administrator können Sie diese Änderung auf Systemebene verwalten.

<!--Use this Important note box in the last few weeks before each update.

You must take action to update the metadata in your identity provider with the information from the renewed certiﬁcate before the speciﬁed date. Mismatched certiﬁcates can keep your users from logging in to Workfront after November 22, 2022.
 
-->

>[!NOTE]
>
>Dies ist nicht verfügbar, wenn die Workfront-Instanz Ihres Unternehmens mit Adobe IMS aktiviert ist. Weitere Informationen erhalten Sie von Ihrem Netzwerk- oder IT-Administrator.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen Workfront-Administrator sein.</p> <p><b>NOTE</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## SAML 2.0 in Workfront konfigurieren

So überprüfen Sie die Warnmeldung und bestätigen die Aktualisierung der SAML 2.0-Metadaten in Ihrem Identitäts-Provider:

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Einrichtung** ![](assets/gear-icon-settings.png).

1. Klicken **System** > **Single Sign-on**.

1. Im **Typ** Dropdown-Menü auswählen **SAML 2.0**.

1. Klicken **SAML 2.0-Metadaten herunterladen**.

   Dadurch wird das erneuerte Workfront-Zertifikat für SAML 2.0 heruntergeladen, das die richtigen Metadaten für Ihren Server enthält.

   >[!CAUTION]
   >
   >Kopieren Sie vor dem Hochladen der Workfront-Metadaten in Ihren Single Sign-On (SSO)-Provider in Schritt 5 Ihre aktuelle ACS-URL (Assertion Consumer Service) an einen sicheren Ort. Diese URL, auch als Antwort-URL bezeichnet, befindet sich auf der Workfront-Konfigurationsseite Ihres SSO-Anbieters.
   >
   >
   >Wenn sich die ACS-URL nach dem Hochladen der Workfront-Metadaten ändert, bedeutet dies, dass die Metadaten möglicherweise eine falsche ACS-URL enthalten. Sie müssen sie wieder in die kopierte ändern, um die Single-Sign-On-Verbindung nicht zu unterbrechen. Ihr aktualisiertes Zertifikat ist nach diesem Vorgang weiterhin korrekt.

1. Wechseln Sie zu Ihrem Identitäts-Provider-Server und aktualisieren Sie das neue Zertifikat, das Sie heruntergeladen haben.
1. In Workfront im **Single Sign-on (SSO)-Seite** müssen Sie sicherstellen, dass diese Option aktiviert ist: **Das neue Workfront-Zertifikat wurde bereits in den Identitätsanbieter hochgeladen**.

   Wenn dieses Feld ausgewählt ist, können sich Workfront-Administratoren mit ihren SSO-Anmeldeinformationen oder Workfront-Anmeldeinformationen bei Workfront anmelden.

1. Klicken Sie auf **Speichern**.

   Die Warnmeldung wird nicht mehr angezeigt, da Sie die Verlängerung des SAML 2.0-Zertifikats auf dem Server Ihres Identitäts-Providers bestätigt haben.

1. Klicken **Verbindung testen** , um Ihre Konfiguration zu testen.

   Es sollte eine Meldung angezeigt werden, die bestätigt, dass die Verbindung erfolgreich hergestellt wurde.

Wenden Sie sich für weitere Informationen oder Unterstützung bei der manuellen Konfiguration von Metadaten an unser Support-Team, wie hier beschrieben: [Support kontaktieren](../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
