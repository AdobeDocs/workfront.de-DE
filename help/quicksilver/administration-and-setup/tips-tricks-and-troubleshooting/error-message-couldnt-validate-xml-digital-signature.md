---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Fehlermeldung: Digitale XML-Signatur konnte nicht validiert werden'
description: Es kann keine erfolgreiche Verbindung zu ADFS hergestellt werden.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d30a67dd-4f91-41cf-b1ba-fefadc4e396a
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 1%

---

# Fehlermeldung: Digitale XML-Signatur konnte nicht validiert werden

## Problem

Es kann keine erfolgreiche Verbindung zu ADFS hergestellt werden.

![error_message.png](assets/error-message.png)

>[!NOTE]
>
>Wenn Sie eine erfolgreiche Testverbindung herstellen und weiterhin Probleme auftreten, kann es sein, dass falsche Attributzuordnungen oder Probleme mit den Federation IDs vorliegen. Wenden Sie sich bei Fragen an den Support.

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

## Ursache 1: Das Zertifikat ist falsch

### Lösung

Manuelles Abrufen des Signaturzertifikats vom ADFS-Server:

1. Klicken Sie [!DNL Windows] auf **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0-Verwaltung]**.\
   Das Dialogfeld ADFS 2.0-Verwaltung wird angezeigt.

1. Wählen **[!UICONTROL Vertrauensbeziehung]** > **[!UICONTROL Vertrauensstellungen der vertrauenden]** im linken Bereich aus.

1. Klicken Sie mit der rechten Maustaste auf **[!UICONTROL Vertrauensstellung der vertrauenden Seite]** und wählen Sie **[!UICONTROL Eigenschaften]** aus.

1. Klicken Sie auf die Registerkarte **[!UICONTROL Signatur]**.
1. Klicken Sie auf den Namen des Signaturzertifikats und anschließend auf **[!UICONTROL Anzeigen]**.
1. Klicken Sie auf In **[!UICONTROL Datei]**… kopieren und wählen Sie **[!UICONTROL Weiter]**.

1. Wählen Sie **[!UICONTROL Base-64-kodiert x.509 (CER)]** aus und klicken Sie auf **[!UICONTROL Weiter]**.

1. Geben Sie den Dateinamen an und klicken Sie auf **[!UICONTROL Weiter]**.
1. Klicken Sie auf **[!UICONTROL Beenden]**.
1. Navigieren Sie in [!DNL Adobe Workfront] zu **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Single Sign-On (SSO)]** und laden Sie das Signaturzertifikat manuell hoch.

## Ursache 2: Das Zertifikat wird mit DSA signiert, wenn [!DNL Workfront] eine RSA-Signatur erwartet

### Lösung

Erstellen Sie das Zertifikat neu und verwenden Sie die RSA-Signatur anstelle des DSA.

## Ursache 3: XML-Daten sind falsch

### Lösung

Exportieren Sie die XML-Metadaten erneut und importieren Sie sie erneut aus dem ADFS-Verwaltungssystem.

## Ursache 4: Die Anfrage konnte aufgrund eines Fehlers auf der SAML-Seite nicht ausgeführt werden.

### Lösung

Kontaktieren Sie Ihren SAML-Anbieter.
