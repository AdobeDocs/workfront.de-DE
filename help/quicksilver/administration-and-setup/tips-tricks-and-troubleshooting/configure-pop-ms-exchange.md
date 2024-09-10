---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: POP in Microsoft Exchange konfigurieren
description: Ein POP-E-Mail-Konto in [!DNL Microsoft Exchange] ist deaktiviert.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# POP in [!DNL Microsoft Exchange] konfigurieren

## Problem

Ein POP-E-Mail-Konto in [!DNL Microsoft Exchange] ist deaktiviert.

## Lösung

Bevor Sie Zeit für die Problembehebung verbringen, stellen Sie sicher, dass das POP-Konto des Benutzers ordnungsgemäß konfiguriert ist. Wenn nach der Bestätigung, dass das POP-Konto korrekt konfiguriert ist, weiterhin Probleme auftreten, wenden Sie sich an den Support von [!DNL Microsoft] oder einen seiner Partner, um weitere Hilfe zu erhalten.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

## Zugriffsanforderungen

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
   <td>[!UICONTROL Systemadministrator]</td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## POP in [!DNL Microsoft Exchange] konfigurieren

>[!NOTE]
>
>Die folgenden Schritte können als allgemeine Anleitung zum Konfigurieren von POP in [!DNL Microsoft Exchange] für ein Produktions-[!DNL Workfront]-System verwendet werden. Die Schritte können je nach der Exchange-Version oder den von Microsoft vorgenommenen Codeänderungen erheblich voneinander abweichen.

1. Starten und aktivieren Sie den POP3-Dienst auf dem Exchange 2010-Server.

   >[!NOTE]
   >
   >Standardmäßig wird der POP3-Dienst nicht gestartet.

   1. Starten Sie den Server-Manager von [!DNL Microsoft].
   1. Navigieren Sie zu: **[!UICONTROL Server-Manager]** > **[!UICONTROL Konfiguration]** >**[!UICONTROL Windows-Firewall mit erweiterter Sicherheit]** > **[!UICONTROL Dienste]**.

   1. Klicken Sie mit der rechten Maustaste auf **[!DNL Microsoft Exchange]POP3** und klicken Sie dann auf **[!UICONTROL Eigenschaften]**.

   1. (Bedingt) Um sicherzustellen, dass der POP-Dienst automatisch startet, legen Sie auf der Registerkarte **[!UICONTROL Allgemein]** den Typ **[!UICONTROL Start]** auf [!UICONTROL Automatisch] fest.

1. Konfigurieren Sie POP3 für den Server.

   1. Starten Sie die Verwaltungskonsole [!DNL Microsoft Exchange] .
   1. Navigieren Sie zu: [!DNL Microsoft] **[!UICONTROL On-Premise-Austausch]** > **[!UICONTROL Server-Konfiguration]** > **[!UICONTROL Client-Zugriff]**.

   1. Wählen Sie **[!UICONTROL POP3]** aus.

      POP3 befindet sich auf der Liste unter den Registerkarten [!UICONTROL POP3] und [!UICONTROL IMAP4] .

   1. Wählen Sie rechts unter **[!UICONTROL Aktionen]** die Option **[!UICONTROL POP3]** und dann **[!UICONTROL Eigenschaften]** aus.

   1. Klicken Sie auf **[!UICONTROL POP3-Eigenschaften]** und öffnen Sie dann die Registerkarte **[!UICONTROL Bindung]**.

      Alle verfügbaren IP-Adressen und Portnummern, die für den POP3-Server konfiguriert sind, werden angezeigt. Das obere Feld zeigt das Feld Entschlüsselt an und das untere Feld zeigt die IP und Ports für SSL/TLS-Verbindungen an.

   1. Klicken Sie auf **[!UICONTROL POP3-Eigenschaften]** und öffnen Sie dann die Registerkarte **[!UICONTROL Authentifizierung]**.

   1. **[!UICONTROL Wählen Sie die Anmeldung &quot;Secure]**&quot;.

      Eine TLS-Verbindung ist erforderlich, damit der Client sich beim Server authentifizieren kann.

1. Aktivieren oder erlauben Sie Benutzern, eine Verbindung zum POP herzustellen.

   1. Starten Sie die Verwaltungskonsole [!DNL Microsoft Exchange] .
   1. Navigieren Sie zu: [!DNL Microsoft] **[!UICONTROL On-Premise-Austausch]** > **[!UICONTROL Empfängerkonfiguration]** > **[!UICONTROL Postfach]**.

      Eine Liste von Postfächern oder Benutzern wird angezeigt.

   1. Markieren Sie die in [!DNL Workfront] verwendete E-Mail.
   1. Wählen Sie rechts unter **[!UICONTROL Aktionen]** die Option **[!UICONTROL Eigenschaften]** aus und öffnen Sie dann die Registerkarte **[!UICONTROL Postfachfunktionen]** .

   1. (Bedingt) Wenn POP3 deaktiviert ist, klicken Sie auf **[!UICONTROL POP3]** und dann auf **[!UICONTROL Enable]**.

      Eine Liste von Postfächern oder Benutzern wird angezeigt.

1. Konfigurieren von Receiver-Connectoren.

   1. Starten Sie [!DNL Microsoft Exchange] Management Console.
   1. Navigieren Sie zu: [!DNL Microsoft] **[!UICONTROL On-Premise-Austausch]** > **[!UICONTROL Server-Konfiguration]** > **[!UICONTROL Hub-Transport]**.

      Eine Liste der Empfänger-Connectoren wird angezeigt.

   1. Vergewissern Sie sich, dass der Empfangs-Connector *Client* *EX01* aktiviert ist.

      Dabei ist *Client* *EX01* der Name Ihres Exchange-Servers.

   1. Wählen Sie *Client EX01* und dann rechts unter **[!UICONTROL Aktionen]** die Option **[!UICONTROL Eigenschaften]**.

   1. Öffnen Sie die Registerkarte **[!UICONTROL Authentifizierung]** und stellen Sie sicher, dass die Option **[!UICONTROL Transport Layer Security (TLS)]** aktiviert ist.

      >[!NOTE]
      >
      >Um über eine einfache Authentifizierung zu verfügen, müssen Sie möglicherweise TLS und die integrierte Windows-Authentifizierung starten.
