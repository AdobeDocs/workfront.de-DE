---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Fehlermeldung: SAML 2.0 Fehler: Primärer StatusCode'
description: Es kann keine erfolgreiche Verbindung zu ADFS hergestellt werden.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1ec18638-97b8-4307-9cea-05b28395eaee
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 2%

---

# Fehlermeldung: SAML 2.0 Fehler: Primär StatusCode

## Problem

Es kann keine erfolgreiche Verbindung zu ADFS hergestellt werden.

![SAML_2.0_error_Primär_status_code.png](assets/saml-2.0-error-primary-status-code.png)

>[!NOTE]
>
>Wenn Sie eine erfolgreiche Testverbindung herstellen und weiterhin Probleme auftreten, kann es sein, dass falsche Attributzuordnungen oder Probleme mit den Federation IDs vorliegen. Wenden Sie sich bei Fragen an den Support.

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

## Ursache 1: Der sichere Hash-Algorithmus ist auf SHA-256 festgelegt.

### Lösung

1. Klicken Sie unter Windows auf **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0-]**.\
   Das Dialogfeld ADFS 2.0-Verwaltung wird angezeigt.

1. Wählen **[!UICONTROL Vertrauensbeziehung]** > **[!UICONTROL Vertrauensstellungen der vertrauenden]** im linken Bereich aus.

1. Klicken Sie mit der rechten Maustaste auf die Vertrauensstellung der vertrauenden Seite in Bezug auf [!DNL Adobe Workfront] und wählen Sie dann **[!UICONTROL Eigenschaften]** aus.
1. Klicken Sie auf die **[!UICONTROL Erweitert]** und wählen Sie dann **[!UICONTROL SHA-1]** aus dem Dropdown **[!UICONTROL Menü Sicherer Hash-Algorithmus]** aus.
   ![SHA-1](assets/1-350x287.png)

## Ursache 2: Das ADFS-Signaturzertifikat läuft bald ab und wurde durch ein neues Zertifikat mit sich überschneidenden Datumsangaben ersetzt

### Lösung

Auf der Seite [!DNL Workfront] SSO-Setup wird das Gültigkeitsdatum des Zertifikats aufgeführt. Wenn das Zertifikat bald abläuft, müssen Sie das neue Signaturzertifikat manuell vom ADFS-Server abrufen:

1. Klicken Sie unter Windows auf **[!UICONTROL Start]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0-]**.\
   Das Dialogfeld ADFS 2.0-Verwaltung wird angezeigt.

1. Wählen **[!UICONTROL Vertrauensbeziehung]** > **[!UICONTROL Vertrauensstellungen der vertrauenden]** im linken Bereich aus.

1. Klicken Sie mit der rechten Maustaste auf die Vertrauensstellung der vertrauenden Seite in Bezug auf [!DNL Workfront] und wählen Sie **[!UICONTROL Eigenschaften]**.
1. Klicken Sie auf die Registerkarte **[!UICONTROL Signatur]**.
1. Klicken Sie auf den Namen des Signaturzertifikats und anschließend auf **[!UICONTROL Anzeigen]**.
1. Klicken Sie auf In **[!UICONTROL Datei]**… kopieren und wählen Sie **[!UICONTROL Weiter]**.

1. Wählen Sie **[!UICONTROL Base-64-kodiert x.509 (CER)]** aus und klicken Sie auf **[!UICONTROL Weiter]**.

1. Geben Sie den Dateinamen an und klicken Sie auf **[!UICONTROL Weiter]**.
1. Klicken Sie auf **[!UICONTROL Beenden]**.
1. Navigieren Sie in [!DNL Workfront] zu **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Single Sign-On (SSO)]** und laden Sie das Signaturzertifikat manuell hoch.

## Ursache 3: Die Zertifikatsperrprüfung schlägt fehl

Die Lösung hängt von der verwendeten ADFS-Version [!DNL Microsoft]. Lesen Sie die Dokumentation von [!DNL Microsoft], um die entsprechenden Befehle für Ihre Version zu erhalten.
