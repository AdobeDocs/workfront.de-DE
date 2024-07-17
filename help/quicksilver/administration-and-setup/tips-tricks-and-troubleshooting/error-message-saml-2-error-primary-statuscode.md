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
source-wordcount: '378'
ht-degree: 1%

---

# Fehlermeldung: SAML 2.0-Fehler: Primärer StatusCode

## Problem

Sie können keine erfolgreiche Verbindung zu ADFS herstellen.

![SAML_2.0_Error_Primär_status_code.png](assets/saml-2.0-error-primary-status-code.png)

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
   <td>Alle</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Sie müssen ein [!DNL Workfront] -Administrator sein. Weitere Informationen finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollen Administratorzugriffs für einen Benutzer</a>.</p> <p><b>HINWEIS</b>: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ursache 1: Der sichere Hash-Algorithmus ist auf SHA-256 eingestellt

### Lösung

1. Klicken Sie unter Windows auf &quot;**[!UICONTROL Start]**&quot;> &quot;**[!UICONTROL Administration]**&quot;> &quot;**[!UICONTROL ADFS 2.0-Verwaltung]**&quot;.\
   Das Dialogfeld ADFS 2.0-Verwaltung wird angezeigt.

1. Wählen Sie im linken Bereich die Option **[!UICONTROL Vertrauensbeziehung]** > **[!UICONTROL Vertrauenswürdige Parteivertrauer]** aus.

1. Klicken Sie mit der rechten Maustaste auf die Vertrauenswürdigkeit der vertrauenswürdigen Partei in Bezug auf [!DNL Adobe Workfront] und wählen Sie dann **[!UICONTROL Eigenschaften]** aus.
1. Klicken Sie auf die Registerkarte **[!UICONTROL Erweitert]** und wählen Sie dann **[!UICONTROL SHA-1]** aus dem Dropdownmenü **[!UICONTROL Sicherer Hash-Algorithmus]** aus.\
   ![](assets/1-350x287.png)

## Ursache 2: Das ADFS-Signaturzertifikat läuft bald ab und wurde durch ein neues Zertifikat mit überlappenden Daten ersetzt

### Lösung

Auf der Seite &quot;[!DNL Workfront] SSO-Setup&quot;wird das Ablaufdatum des Zertifikats aufgeführt. Wenn das Zertifikat bald abläuft, müssen Sie das neue Signaturzertifikat manuell vom ADFS-Server abrufen:

1. Klicken Sie unter Windows auf &quot;**[!UICONTROL Start]**&quot;> &quot;**[!UICONTROL Administration]**&quot;> &quot;**[!UICONTROL ADFS 2.0-Verwaltung]**&quot;.\
   Das Dialogfeld ADFS 2.0-Verwaltung wird angezeigt.

1. Wählen Sie im linken Bereich die Option **[!UICONTROL Vertrauensbeziehung]** > **[!UICONTROL Vertrauenswürdige Parteivertrauer]** aus.

1. Klicken Sie mit der rechten Maustaste auf die Vertrauenswürdigkeit der vertrauenswürdigen Partei in Bezug auf [!DNL Workfront] und wählen Sie **[!UICONTROL Eigenschaften]** aus.
1. Klicken Sie auf die Registerkarte **[!UICONTROL Signatur]**.
1. Klicken Sie auf den Namen des Signaturzertifikats und dann auf **[!UICONTROL Anzeigen]**.
1. Klicken Sie auf In **[!UICONTROL Datei]**... kopieren und wählen Sie **[!UICONTROL Weiter]** aus.

1. Wählen Sie **[!UICONTROL Base-64-kodiertes x.509 (CER)]** und klicken Sie auf **[!UICONTROL Next]**.

1. Geben Sie den Dateinamen an und klicken Sie auf **[!UICONTROL Weiter]**.
1. Klicken Sie auf **[!UICONTROL Beenden]**.
1. Navigieren Sie in [!DNL Workfront] zu **[!UICONTROL Setup]** > **[!UICONTROL System]** > **[!UICONTROL Single Sign-On (SSO)]** und laden Sie das Signaturzertifikat manuell hoch.

## Ursache 3: Fehler bei der Zertifikatsperrungsprüfung

Die Lösung dafür hängt von der Version von [!DNL Microsoft] ADFS ab, die Sie verwenden. Konsultieren Sie die Dokumentation von [!DNL Microsoft] , um die entsprechenden Befehle für Ihre Version zu erhalten.
