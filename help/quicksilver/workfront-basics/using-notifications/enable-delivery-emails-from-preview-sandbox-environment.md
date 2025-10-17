---
navigation-topic: notifications
title: E-Mail-Versand über die Sandbox-Vorschau-Umgebung aktivieren
description: Wenn Sie E-Mail-Benachrichtigungen von der Sandbox-Vorschau-Umgebung erhalten möchten, müssen Sie diese Funktion in Ihren Benutzereinstellungen aktivieren, während Sie bei der Vorschau angemeldet sind.
author: Courtney, Becky
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: 64b8a835a57be8995c82a0ab15c40f46170c7067
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 1%

---

# E-Mail-Versand über die Sandbox-Vorschau-Umgebung aktivieren

[!UICONTROL Adobe Workfront] Deaktiviert die gesamte E-Mail-Kommunikation in der Vorschau- und der benutzerdefinierten Sandbox-Aktualisierungsumgebung. Weitere Informationen zur Sandbox-Vorschau-Umgebung finden Sie unter [Die Sandbox-Vorschau-Umgebung von Adobe Workfront](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). Informationen zur benutzerdefinierten Sandbox-Aktualisierungsumgebung finden Sie unter [Die benutzerdefinierte Sandbox-Aktualisierungsumgebung von Adobe Workfront](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Wenn Sie die folgenden E-Mail-Benachrichtigungen von der Sandbox-Vorschau-Umgebung erhalten möchten, müssen Sie diese Funktion in Ihren Benutzereinstellungen aktivieren, während Sie bei der Vorschau angemeldet sind:

* Durch Ereignisbenachrichtigungen ausgelöste E-Mail-Benachrichtigungen
* Erinnerungsbenachrichtigungen
* Automatische, verspätete oder frühzeitige Erinnerungsbenachrichtigungen
* E-Mail-Einladungen

Sie können dies für sich selbst oder für einen beliebigen Benutzer tun, auf den Sie Zugriff zum Bearbeiten haben. Weitere Informationen zum Zugriff, der zum Bearbeiten von Benutzern benötigt wird, finden Sie unter [Gewähren des Zugriffs für Benutzer](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>Berichtsversand und Push-Benachrichtigungen in der Mobile App sind für die Sandbox-Vorschau-Umgebung immer deaktiviert. Weder Sie noch der [!DNL Workfront]-Administrator können die Berichtsbereitstellung oder Push-Benachrichtigungen für die Mobile App aktivieren, wenn Sie auf die Sandbox-Vorschau-Umgebung zugreifen.
>
>Informationen zu Berichtssendungen finden Sie unter [Übersicht über die Berichtsbereitstellung](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] Lizenz</strong></td> 
   <td> 
   <p>Mitwirkender oder höher zum Ändern der eigenen Einstellung</p> <p>Standard, um die Einstellung für andere Benutzer zu bearbeiten</p> 
   Oder
   <p> Fordern Sie oder höher an, Ihre eigene Einstellung zu ändern</p> <p>Bearbeiten der Einstellung für andere Benutzer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen der Zugriffsebene</strong></td> 
   <td> <p>Sie müssen eine der folgenden Möglichkeiten haben:</p> 
    <ul> 
     <li> <p>Zugriffsebene des [!UICONTROL Systemadministrators].</p> </li> 
     <li> <p>In Ihrer Zugriffsebene muss [!UICONTROL Bearbeiten] für die Einstellung [!UICONTROL Benutzer] ausgewählt sein. Und für die Einstellung [!UICONTROL Users] müssen unter [!UICONTROL Feinabstimmung der Einstellungen] <img src="assets/gear-icon-in-access-levels.png"> die Option [!UICONTROL Create] und mindestens eine der beiden [!UICONTROL User Admin]-Optionen aktiviert sein. </li> 
     <li>Wenn Sie die Option [!UICONTROL Benutzeradmin (Gruppenbenutzer)] verwenden, müssen Sie Gruppenadministrator einer Gruppe sein, in der der Benutzer Mitglied ist.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>


Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aktivieren des Versands von E-Mails aus der Sandbox-Vorschau-Umgebung

1. Melden Sie sich bei Ihrer Sandbox-Vorschau-Umgebung an.
1. Klicken Sie auf Ihr Profilbild in der oberen rechten Ecke von [!DNL Adobe Workfront]. Klicken Sie anschließend auf das Menü **[!UICONTROL Mehr]** und wählen Sie **[!UICONTROL Bearbeiten]** aus.

   Oder

   Suchen Sie nach einem Benutzer in [!DNL Workfront] und klicken Sie auf seinen Namen. Klicken Sie anschließend auf das Menü **[!UICONTROL Mehr]** und wählen Sie **[!UICONTROL Bearbeiten]** aus.

   Oder

   Für mehrere Benutzer: Klicken Sie auf **[!UICONTROL Hauptmenü]** Symbol ![Hauptmenüsymbol](assets/main-menu-icon.png) in der rechten oberen Ecke von Workfront und dann auf **[!UICONTROL Benutzer]** ![Benutzersymbol](assets/users-icon-in-main-menu.png).  Wählen Sie dann mehrere Benutzer aus und klicken Sie auf **[!UICONTROL Bearbeiten]**.

1. Klicken Sie auf **[!UICONTROL Voreinstellungen]**.
1. Wählen **[!UICONTROL E-Mails von dieser Testumgebung empfangen]** aus.

   >[!NOTE]
   >
   >Diese Option ist nicht verfügbar, wenn Sie sich in einer Produktionsumgebung befinden.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.
