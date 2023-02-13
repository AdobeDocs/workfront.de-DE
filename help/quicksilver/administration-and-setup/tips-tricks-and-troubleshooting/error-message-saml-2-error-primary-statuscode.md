---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Fehlermeldung: SAML 2.0-Fehler: Primärer StatusCode'
description: Sie können keine erfolgreiche Verbindung zu ADFS herstellen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1ec18638-97b8-4307-9cea-05b28395eaee
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 0%

---

# Fehlermeldung: SAML 2.0-Fehler: Primärer StatusCode

## Problem

Sie können keine erfolgreiche Verbindung zu ADFS herstellen.

![SAML_2.0_Error_Primär_Status_Code.png](assets/saml-2.0-error-primary-status-code.png)

>[!NOTE]
>
>Wenn Sie eine erfolgreiche Testverbindung herstellen und weiterhin Probleme auftreten, kann es bei Ihnen zu falschen Zuordnungen von Attributen oder zu Problemen mit Verknüpfungs-IDs kommen. Wenden Sie sich bei Fragen an den Support.

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

## Ursache 1: Der sichere Hash-Algorithmus ist auf SHA-256 eingestellt.

### Lösung

1. Klicken Sie unter Windows auf **[!UICONTROL Starten]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0-Verwaltung]**.\
   Das Dialogfeld ADFS 2.0-Verwaltung wird angezeigt.

1. Auswählen **[!UICONTROL Vertrauensbeziehung]** > **[!UICONTROL Vertrauen in Partei]** im linken Bereich.

1. Klicken Sie mit der rechten Maustaste auf das Vertrauen der vertrauenden Partei, das mit [!DNL Adobe Workfront], wählen Sie **[!UICONTROL Eigenschaften]**.
1. Klicken Sie auf **[!UICONTROL Erweitert]** Registerkarte und wählen Sie **[!UICONTROL SHA-1]** von **[!UICONTROL Sicherer Hashalgorithmus]** Dropdown-Menü.\
   ![](assets/1-350x287.png)

## Ursache 2: Das ADFS-Signaturzertifikat läuft bald ab und wurde durch ein neues Zertifikat mit überlappenden Daten ersetzt

### Lösung

Die [!DNL Workfront] Auf der SSO-Setup-Seite wird das Ablaufdatum des Zertifikats aufgeführt. Wenn das Zertifikat bald abläuft, müssen Sie das neue Signaturzertifikat manuell vom ADFS-Server abrufen:

1. Klicken Sie unter Windows auf **[!UICONTROL Starten]** > **[!UICONTROL Administration]** > **[!UICONTROL ADFS 2.0-Verwaltung]**.\
   Das Dialogfeld ADFS 2.0-Verwaltung wird angezeigt.

1. Auswählen **[!UICONTROL Vertrauensbeziehung]** > **[!UICONTROL Vertrauen in Partei]** im linken Bereich.

1. Klicken Sie mit der rechten Maustaste auf das Vertrauen der vertrauenden Partei, das mit [!DNL Workfront]und wählen Sie **[!UICONTROL Eigenschaften]**.
1. Klicken Sie auf **[!UICONTROL Unterschrift]** Registerkarte.
1. Klicken Sie auf den Namen des Signaturzertifikats und klicken Sie auf **[!UICONTROL Ansicht]**.
1. Klicken Sie auf Kopieren nach **[!UICONTROL Datei]**... und wählen Sie **[!UICONTROL Nächste]**.

1. Auswählen **[!UICONTROL Base-64-kodierte x.509 (CER)]** und klicken Sie auf **[!UICONTROL Nächste]**.

1. Geben Sie den Dateinamen an und klicken Sie auf **[!UICONTROL Nächste]**.
1. Klicken **[!UICONTROL Beenden]**.
1. In [!DNL Workfront], navigieren Sie zu **[!UICONTROL Einrichtung]** > **[!UICONTROL System]** > **[!UICONTROL Single Sign-On (SSO)]** und laden Sie das Signaturzertifikat manuell hoch.

## Ursache 3: Zertifikatsperrungsprüfung schlägt fehl

Die Lösung dafür hängt von der Version der [!DNL Microsoft] ADFS, die Sie verwenden. Besprechen [!DNL Microsoft]-Dokumentation, um die entsprechenden Befehle für Ihre Version zu erhalten.
