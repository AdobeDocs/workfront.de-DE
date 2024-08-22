---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Fehlermeldung: XML Digital Signature konnte nicht validiert werden"
description: Sie können keine erfolgreiche Verbindung zu ADFS herstellen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 1%

---

# Fehlermeldung: Digitale XML-Signatur konnte nicht validiert werden

## Problem

Sie können keine erfolgreiche Verbindung zu ADFS herstellen.

![error_message.png](assets/error-message.png)

>[!NOTE]
>
>Wenn Sie eine erfolgreiche Testverbindung herstellen und weiterhin Probleme auftreten, kann es bei Ihnen zu falschen Zuordnungen von Attributen oder zu Problemen mit Verknüpfungs-IDs kommen. Wenden Sie sich bei Fragen an den Support.

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

## Ursache 1: Das Zertifikat ist falsch

### Lösung

Rufen Sie das Signaturzertifikat manuell vom ADFS-Server ab:

1. Klicken Sie in [!DNL Windows] auf **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0-Verwaltung]**.\
   Das Dialogfeld ADFS 2.0-Verwaltung wird angezeigt.

1. Wählen Sie im linken Bereich die Option **[!UICONTROL Vertrauensbeziehung]** > **[!UICONTROL Vertrauenswürdige Parteivertrauer]** aus.

1. Klicken Sie mit der rechten Maustaste auf **[!UICONTROL Vertrauenswürdigkeit der Partei]** und wählen Sie **[!UICONTROL Eigenschaften]** aus.

1. Klicken Sie auf die Registerkarte **[!UICONTROL Signatur]**.
1. Klicken Sie auf den Namen des Signaturzertifikats und dann auf **[!UICONTROL Anzeigen]**.
1. Klicken Sie auf In **[!UICONTROL Datei]**... kopieren und wählen Sie **[!UICONTROL Weiter]** aus.

1. Wählen Sie **[!UICONTROL Base-64-kodiertes x.509 (CER)]** und klicken Sie auf **[!UICONTROL Next]**.

1. Geben Sie den Dateinamen an und klicken Sie auf **[!UICONTROL Weiter]**.
1. Klicken Sie auf **[!UICONTROL Beenden]**.
1. Navigieren Sie in [!DNL Adobe Workfront] zu **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Single Sign-On (SSO)]** und laden Sie das Signaturzertifikat manuell hoch.

## Ursache 2: Das Zertifikat wird mit DSA signiert, wenn [!DNL Workfront] eine RSA-Signatur erwartet

### Lösung

Erstellen Sie das Zertifikat neu und verwenden Sie die RSA-Signatur anstelle der DSA.

## Ursache 3: XML-Daten sind falsch

### Lösung

Exportieren und importieren Sie die XML-Metadaten erneut aus dem ADFS-Verwaltungssystem.

## Ursache 4: Die Anfrage konnte aufgrund eines Fehlers auf der SAML-Seite nicht ausgeführt werden

### Lösung

Wenden Sie sich an Ihren SAML-Provider.
