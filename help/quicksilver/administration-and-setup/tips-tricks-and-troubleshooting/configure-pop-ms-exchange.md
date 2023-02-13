---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: POP in Microsoft Exchange konfigurieren
description: Ein POP-E-Mail-Konto in [!DNL Microsoft Exchange] deaktiviert ist.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# POP konfigurieren in [!DNL Microsoft Exchange]

## Problem

Ein POP-E-Mail-Konto in [!DNL Microsoft Exchange] deaktiviert ist.

## Lösung

Bevor Sie Zeit für die Problembehebung verbringen, stellen Sie sicher, dass das POP-Konto des Benutzers ordnungsgemäß konfiguriert ist. Wenn nach der Bestätigung, dass das POP-Konto korrekt konfiguriert ist, weiterhin Probleme auftreten, wenden Sie sich an [!DNL Microsoft] Unterstützung oder eines ihrer Partner für zusätzliche Hilfe.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

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

## POP konfigurieren in [!DNL Microsoft Exchange]

>[!NOTE]
>
>Die folgenden Schritte können als allgemeine Anleitung zum Konfigurieren von POP in [!DNL Microsoft Exchange] für eine Produktion [!DNL Workfront] System. Die Schritte können je nach der Exchange-Version oder den von Microsoft vorgenommenen Codeänderungen erheblich voneinander abweichen.

1. Starten und aktivieren Sie den POP3-Dienst auf dem Exchange 2010-Server.

   >[!NOTE]
   >
   >Standardmäßig wird der POP3-Dienst nicht gestartet.

   1. Starten [!DNL Microsoft]Server Manager.
   1. Navigieren Sie: **[!UICONTROL Server Manager]** > **[!UICONTROL Konfiguration]** >**[!UICONTROL Windows-Firewall mit erweiterter Sicherheit]** > **[!UICONTROL Dienste]**.

   1. Rechtsklick **[!DNL Microsoft Exchange]POP3** Klicken Sie auf **[!UICONTROL Eigenschaften]**.

   1. (Bedingt) Um sicherzustellen, dass der POP-Dienst automatisch gestartet wird, wird auf der **[!UICONTROL Allgemein]** Registerkarte, legen Sie die **[!UICONTROL Start]** type to [!UICONTROL Automatisch].

1. Konfigurieren Sie POP3 für den Server.

   1. Starten Sie die [!DNL Microsoft Exchange] Verwaltungskonsole.
   1. Navigieren Sie: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Serverkonfiguration]** > **[!UICONTROL Zugriff auf Client]**.

   1. Auswählen **[!UICONTROL POP3]**.

      POP3 befindet sich auf der Liste unter [!UICONTROL POP3] und [!UICONTROL IMAP4] Registerkarten.

   1. Auf der rechten Seite unter **[!UICONTROL Aktionen]** auswählen **[!UICONTROL POP3]**, wählen Sie **[!UICONTROL Eigenschaften]**.

   1. Klicken **[!UICONTROL POP3-Eigenschaften]**, und öffnen Sie dann die **[!UICONTROL Bindung]** Registerkarte.

      Alle für den POP3-Server konfigurierten IP-Adressen und Anschlussnummern werden angezeigt. Das obere Feld zeigt das Feld Entschlüsselt an und das untere Feld zeigt die IP und Ports für SSL/TLS-Verbindungen an.

   1. Klicken **[!UICONTROL POP3-Eigenschaften]**, und öffnen Sie dann die **[!UICONTROL Authentifizierung]** Registerkarte.

   1. **[!UICONTROL Sichern auswählen]** anmelden.

      Eine TLS-Verbindung ist erforderlich, damit der Client sich beim Server authentifizieren kann.

1. Aktivieren oder erlauben Sie Benutzern, eine Verbindung zum POP herzustellen.

   1. Starten Sie die [!DNL Microsoft Exchange] Verwaltungskonsole.
   1. Navigieren Sie: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Empfängerkonfiguration]** > **[!UICONTROL Postfach]**.

      Eine Liste von Postfächern oder Benutzern wird angezeigt.

   1. Markieren Sie die in verwendete E-Mail. [!DNL Workfront].
   1. Auf der rechten Seite unter **[!UICONTROL Aktionen]** auswählen **[!UICONTROL Eigenschaften]**, und öffnen Sie dann die **[!UICONTROL Funktionen des Postfachs]** Registerkarte.

   1. (Bedingt) Wenn POP3 deaktiviert ist, klicken Sie auf **[!UICONTROL POP3]** Klicken Sie auf **[!UICONTROL Aktivieren]**.

      Eine Liste von Postfächern oder Benutzern wird angezeigt.

1. Konfigurieren von Receiver-Connectoren.

   1. Starten [!DNL Microsoft Exchange] Verwaltungskonsole.
   1. Navigieren Sie: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Serverkonfiguration]** > **[!UICONTROL Hub-Transport]**.

      Eine Liste der Empfänger-Connectoren wird angezeigt.

   1. Empfänger-Connector bestätigen *Client* *EX01* aktiviert ist.

      Wo *Client* *EX01* ist der Name Ihres Exchange-Servers.

   1. Auswählen *Client EX01*, dann rechts unter **[!UICONTROL Aktionen]** auswählen **[!UICONTROL Eigenschaften]**.

   1. Öffnen Sie die **[!UICONTROL Authentifizierung]** und dann **[!UICONTROL Transport Layer Security (TLS)]** aktiviert ist.

      >[!NOTE]
      >
      >Um über eine einfache Authentifizierung zu verfügen, müssen Sie möglicherweise TLS und die integrierte Windows-Authentifizierung starten.
