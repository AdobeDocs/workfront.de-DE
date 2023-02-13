---
navigation-topic: notifications
title: Aktivieren des Versands von E-Mails aus der Vorschau-Sandbox-Umgebung
description: Wenn Sie E-Mail-Benachrichtigungen von der Vorschau-Sandbox-Umgebung erhalten möchten, müssen Sie diese Funktion in Ihren Benutzereinstellungen aktivieren, während Sie bei der Vorschau angemeldet sind.
author: Lisa
feature: Get Started with Workfront
exl-id: e5c7e387-d08d-42f6-a9e6-f44e514ef902
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '517'
ht-degree: 0%

---

# Aktivieren des Versands von E-Mails aus der Vorschau-Sandbox-Umgebung

[!UICONTROL Adobe Workfront] Deaktiviert die gesamte E-Mail-Kommunikation sowohl in der Vorschau- als auch in der benutzerdefinierten Aktualisierungs-Sandbox-Umgebung. Informationen zur Vorschau-Sandbox-Umgebung finden Sie unter [Die Adobe Workfront-Vorschau-Sandbox-Umgebung](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). Informationen zur Umgebung der benutzerdefinierten Aktualisierungs-Sandbox finden Sie unter [Die benutzerdefinierte Adobe Workfront-Aktualisierungs-Sandbox-Umgebung](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Wenn Sie die folgenden E-Mail-Benachrichtigungen von der Sandbox-Vorschau-Umgebung erhalten möchten, müssen Sie diese Funktion in Ihren Benutzereinstellungen aktivieren, während Sie in der Vorschau angemeldet sind:

* Durch Ereignisbenachrichtigungen ausgelöste E-Mail-Benachrichtigungen
* Erinnerungsbenachrichtigungen
* Automatische Verspätungs- oder Frühwarnbenachrichtigungen
* Einladungen per E-Mail

Sie können dies für sich selbst oder für jeden Benutzer tun, auf den Sie Zugriff haben. Weitere Informationen über den für die Bearbeitung von Benutzern benötigten Zugriff finden Sie unter [Benutzern Zugriff gewähren](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>Berichtversand und Push-Benachrichtigungen in der Mobile App sind in der Sandbox-Umgebung &quot;Vorschau&quot;immer deaktiviert. Weder du noch der [!DNL Workfront] -Administrator kann die Berichtbereitstellung oder Push-Benachrichtigungen für die mobile App aktivieren, wenn Sie auf die Sandbox-Vorschau-Umgebung zugreifen.
>
>Informationen zu Berichtbereitstellungen finden Sie unter [Berichtversand - Übersicht](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Anfrage] oder höher zum Ändern Ihrer eigenen Einstellung</p> <p>[!UICONTROL Plan] zum Bearbeiten der Einstellung für andere Benutzer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Sie müssen über eine der folgenden Möglichkeiten verfügen:</p> 
    <ul> 
     <li> <p>Die Zugriffsstufe des [!UICONTROL Systemadministrators].</p> <p> Weitere Informationen zu dieser Zugriffsebene finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>. </p> </li> 
     <li> <p>In Ihrer Zugriffsebene muss [!UICONTROL Bearbeiten] für die Einstellung [!UICONTROL Benutzer] ausgewählt sein. Und für die Einstellung [!UICONTROL Benutzer] unter [!UICONTROL Feinabstimmung Ihrer Einstellungen] <img src="assets/gear-icon-in-access-levels.png"> , müssen die Option [!UICONTROL Erstellen] und mindestens eine der beiden [!UICONTROL User Admin]-Optionen aktiviert sein. </p> <p>Wenn Sie die Option [!UICONTROL Benutzeradministrator (Gruppenbenutzer)] verwenden, müssen Sie Gruppenadministrator einer Gruppe sein, der der Benutzer angehört.</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>Informationen zur Einstellung [!UICONTROL Benutzer] für die Zugriffsebene finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Benutzern Zugriff gewähren</a>.</p> </li> 
    </ul> <p>Hinweis: Wenn Sie noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] Administrator , wenn sie zusätzliche Einschränkungen für Ihre Zugriffsebene festlegen. Für Informationen zur [!DNL Workfront] Administrator kann Ihre Zugriffsebene ändern, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Aktivieren des Versands von E-Mails aus der Vorschau-Sandbox-Umgebung

1. Melden Sie sich bei Ihrer Vorschau-Sandbox-Umgebung an.
1. Klicken Sie auf Ihr Profilbild in der oberen rechten Ecke von [!DNL Adobe Workfront]. Klicken Sie dann auf die **[!UICONTROL Mehr]** Menü und wählen Sie **[!UICONTROL Bearbeiten]**.

   Oder

   Suchen Sie nach einem Benutzer in [!DNL Workfront] und klicken Sie auf ihren Namen. Klicken Sie dann auf die **[!UICONTROL Mehr]** Menü und wählen Sie **[!UICONTROL Bearbeiten]**.

   Oder

   Für mehrere Benutzer: Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Workfront auf **[!UICONTROL Benutzer]** ![](assets/users-icon-in-main-menu.png).  Wählen Sie dann mehrere Benutzer aus und klicken Sie auf **[!UICONTROL Bearbeiten]**.

1. Klicken **[!UICONTROL Voreinstellungen]**.
1. Auswählen **[!UICONTROL Empfangen von E-Mails aus dieser Testumgebung]**.

   >[!NOTE]
   >
   >Diese Option ist nicht verfügbar, wenn Sie sich in einer Produktionsumgebung befinden.

1. Klicken **[!UICONTROL Änderungen speichern]**.
