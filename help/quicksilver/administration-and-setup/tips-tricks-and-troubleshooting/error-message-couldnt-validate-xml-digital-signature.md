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
TQID: https://experienceleague.adobe.com/lPAWprUiJA2ZJFUEdzXNTMTM1oXHEKNpc5VAadI-yqI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dcid: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 274
ht-degree: 12%

---

# Fehlermeldung: Digitale XML-Signatur konnte nicht validiert werden

## Problem

Es kann keine erfolgreiche Verbindung zu ADFS hergestellt werden.

![error_message.png](assets/error-message.png)

>[!NOTE]
>
>Wenn Sie eine erfolgreiche Testverbindung herstellen und weiterhin Probleme auftreten, kann es sein, dass falsche Attributzuordnungen oder Probleme mit den Federation IDs vorliegen. Wenden Sie sich bei Fragen an den Support.

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
