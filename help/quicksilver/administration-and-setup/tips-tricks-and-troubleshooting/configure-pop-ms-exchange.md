---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: POP in Microsoft Exchange konfigurieren
description: Ein POP-E-Mail [!DNL Microsoft Exchange] Konto in ist deaktiviert.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 1%

---

# POP in [!DNL Microsoft Exchange] konfigurieren

## Problem

Ein POP-E-Mail-Konto in [!DNL Microsoft Exchange] ist deaktiviert.

## Lösung

Bevor Sie Zeit mit der Fehlerbehebung des Problems verbringen, stellen Sie sicher, dass das POP-Konto des Benutzers ordnungsgemäß konfiguriert ist. Wenn weiterhin Probleme auftreten, nachdem Sie bestätigt haben, dass das POP-Konto korrekt konfiguriert ist, wenden Sie sich an den [!DNL Microsoft]-Support oder einen seiner Partner, um weitere Hilfe zu erhalten.

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

## POP in [!DNL Microsoft Exchange] konfigurieren

>[!NOTE]
>
>Die folgenden Schritte können als allgemeine Anleitung für die Konfiguration von POP in [!DNL Microsoft Exchange] für ein [!DNL Workfront] verwendet werden. Die Schritte können je nach Exchange-Version oder den von Microsoft vorgenommenen Code-Änderungen erheblich abweichen.

1. Starten und Aktivieren des POP3-Dienstes auf dem Exchange 2010-Server.

   >[!NOTE]
   >
   >Standardmäßig wird der POP3-Dienst nicht gestartet.

   1. Starten Sie den Server-Manager von [!DNL Microsoft].
   1. Navigieren Sie zu **[!UICONTROL Server-]** > **[!UICONTROL Konfiguration]** > **[!UICONTROL Windows-Firewall mit erweiterter Sicherheit]** > **[!UICONTROL Dienste]**.

   1. Klicken Sie mit der rechten Maustaste **[!DNL Microsoft Exchange]POP3** und klicken Sie dann auf **[!UICONTROL Eigenschaften]**.

   1. (Bedingt) Um sicherzustellen, dass der POP-Dienst automatisch gestartet wird, legen Sie auf der Registerkarte **[!UICONTROL Allgemein]** den **[!UICONTROL Startup]**-Typ auf [!UICONTROL Automatisch] fest.

1. POP3 für den Server konfigurieren.

   1. Starten Sie die [!DNL Microsoft Exchange] Management-Konsole.
   1. Navigieren Sie zu [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Server-Konfiguration]** > **[!UICONTROL Client-Zugriff]**.

   1. Wählen Sie **[!UICONTROL POP3]**.

      POP3 befindet sich auf der Liste unter den Registerkarten [!UICONTROL POP3] und [!UICONTROL IMAP4].

   1. Klicken Sie auf der rechten Seite unter **[!UICONTROL Aktionen]** auf **[!UICONTROL POP3]** und wählen Sie dann **[!UICONTROL Eigenschaften]**.

   1. Klicken Sie auf **[!UICONTROL POP3-Eigenschaften]** und öffnen Sie dann die Registerkarte **[!UICONTROL Bindung]**.

      Alle für den POP3-Server konfigurierten verfügbaren IP-Adressen und Portnummern werden angezeigt. Das obere Feld zeigt die unverschlüsselte und das untere Feld die IP-Adresse und die Ports für SSL/TLS-Verbindungen.

   1. Klicken Sie auf **[!UICONTROL POP3-Eigenschaften]** und öffnen Sie dann die Registerkarte **[!UICONTROL Authentifizierung]**.

   1. **[!UICONTROL Sicher auswählen]** anmelden.

      Eine TLS-Verbindung ist erforderlich, damit sich der Client beim Server authentifizieren kann.

1. Aktivieren oder Zulassen, dass Benutzer eine Verbindung zu POP herstellen.

   1. Starten Sie die [!DNL Microsoft Exchange] Management-Konsole.
   1. Navigieren Sie zu [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Empfängerkonfiguration]** > **[!UICONTROL Mailbox]**.

      Eine Liste mit Postfächern oder Benutzern wird angezeigt.

   1. Markieren Sie die E-Mail, die in [!DNL Workfront] verwendet wird.
   1. Wählen Sie auf der rechten Seite unter **[!UICONTROL Aktionen]** die Option **[!UICONTROL Eigenschaften]** aus und öffnen Sie dann die Registerkarte **[!UICONTROL Mailbox-Funktionen]**.

   1. (Bedingt) Wenn POP3 deaktiviert ist, klicken Sie auf **[!UICONTROL POP3]** und anschließend auf **[!UICONTROL Aktivieren]**.

      Eine Liste mit Postfächern oder Benutzern wird angezeigt.

1. Konfigurieren von Empfangs-Connectoren.

   1. Starten Sie [!DNL Microsoft Exchange] Verwaltungskonsole.
   1. Navigieren Sie zu [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Server-Konfiguration]** > **[!UICONTROL Hub-Transport]**.

      Eine Liste der Empfangs-Connectoren wird angezeigt.

   1. Bestätigen Sie, dass der *-Connector* Client *EX01* aktiviert ist.

      wobei *Client* *EX01* der Name Ihres Exchange-Servers ist.

   1. Wählen *Client EX01* und klicken Sie dann rechts unter **[!UICONTROL Aktionen]** auf **[!UICONTROL Eigenschaften]**.

   1. Öffnen Sie die **[!UICONTROL Authentifizierung]** und stellen Sie sicher, **[!UICONTROL Transport Layer Security (TLS)]** aktiviert ist.

      >[!NOTE]
      >
      >Um die Standardauthentifizierung zu erhalten, müssen Sie möglicherweise TLS und die integrierte Windows-Authentifizierung starten.
