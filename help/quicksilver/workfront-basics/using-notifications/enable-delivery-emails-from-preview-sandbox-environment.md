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
ht-degree: 1%

---

# Aktivieren des Versands von E-Mails aus der Vorschau-Sandbox-Umgebung

[!UICONTROL Adobe Workfront] deaktiviert die gesamte E-Mail-Kommunikation aus der Vorschau- und der benutzerdefinierten Aktualisierungs-Sandbox-Umgebung. Informationen zur Vorschau-Sandbox-Umgebung finden Sie unter [Die Adobe Workfront-Vorschau-Sandbox-Umgebung](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md). Weitere Informationen zur Sandbox-Umgebung für benutzerdefinierte Aktualisierung finden Sie unter [Die Sandbox-Umgebung für benutzerdefinierte Adobe Workfront-Aktualisierung](../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md).

Wenn Sie die folgenden E-Mail-Benachrichtigungen von der Sandbox-Vorschau-Umgebung erhalten möchten, müssen Sie diese Funktion in Ihren Benutzereinstellungen aktivieren, während Sie in der Vorschau angemeldet sind:

* Durch Ereignisbenachrichtigungen ausgelöste E-Mail-Benachrichtigungen
* Erinnerungsbenachrichtigungen
* Automatische Verspätungs- oder Frühwarnbenachrichtigungen
* Einladungen per E-Mail

Sie können dies für sich selbst oder für jeden Benutzer tun, auf den Sie Zugriff haben. Weitere Informationen zum Zugriff, der zum Bearbeiten von Benutzern erforderlich ist, finden Sie unter [Gewähren des Zugriffs für Benutzer](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).

>[!NOTE]
>
>Berichtversand und Push-Benachrichtigungen in der Mobile App sind in der Sandbox-Umgebung &quot;Vorschau&quot;immer deaktiviert. Weder Sie noch der Administrator [!DNL Workfront] können die Berichtübermittlung oder Push-Benachrichtigungen für die mobile App aktivieren, wenn Sie auf die Umgebung &quot;Sandbox-Vorschau&quot;zugreifen.
>
>Informationen zu Berichtbereitstellungen finden Sie unter [Übersicht über die Berichtbereitstellung](../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

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
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Anfrage] oder höher zum Ändern Ihrer eigenen Einstellung</p> <p>[!UICONTROL Plan] zum Bearbeiten der Einstellung für andere Benutzer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationen auf Zugriffsebene*</strong></td> 
   <td> <p>Sie müssen über eine der folgenden Möglichkeiten verfügen:</p> 
    <ul> 
     <li> <p>Die Zugriffsstufe des [!UICONTROL Systemadministrators].</p> <p> Weitere Informationen zu dieser Zugriffsebene finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollen Administratorzugriffs für einen Benutzer</a>. </p> </li> 
     <li> <p>In Ihrer Zugriffsebene muss [!UICONTROL Bearbeiten] für die Einstellung [!UICONTROL Benutzer] ausgewählt sein. Außerdem müssen für die Einstellung [!UICONTROL Benutzer] unter [!UICONTROL Feinabstimmung Ihrer Einstellungen] <img src="assets/gear-icon-in-access-levels.png"> die Option [!UICONTROL Erstellen] und mindestens eine der beiden Optionen [!UICONTROL Benutzeradministrator] aktiviert sein. </p> <p>Wenn Sie die Option [!UICONTROL Benutzeradministrator (Gruppenbenutzer)] verwenden, müssen Sie Gruppenadministrator einer Gruppe sein, der der Benutzer angehört.</p> <p> <img src="assets/access-req-users-350x101.png" style="width: 350;height: 101;"> </p> <p>Weitere Informationen zur Einstellung [!UICONTROL Benutzer] für Zugriffsebene finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Gewähren des Zugriffs für Benutzer</a>.</p> </li> 
    </ul> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren [!DNL Workfront] -Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein [!DNL Workfront] -Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Aktivieren des Versands von E-Mails aus der Vorschau-Sandbox-Umgebung

1. Melden Sie sich bei Ihrer Vorschau-Sandbox-Umgebung an.
1. Klicken Sie auf Ihr Profilbild in der oberen rechten Ecke von [!DNL Adobe Workfront]. Klicken Sie dann auf das Menü **[!UICONTROL Mehr]** und wählen Sie **[!UICONTROL Bearbeiten]** aus.

   Oder

   Suchen Sie in [!DNL Workfront] nach einem Benutzer und klicken Sie auf seinen Namen. Klicken Sie dann auf das Menü **[!UICONTROL Mehr]** und wählen Sie **[!UICONTROL Bearbeiten]** aus.

   Oder

   Für mehrere Benutzer: Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in Workfront und dann auf **[!UICONTROL Benutzer]** ![](assets/users-icon-in-main-menu.png).  ![](assets/main-menu-icon.png)  Wählen Sie dann mehrere Benutzer aus und klicken Sie auf **[!UICONTROL Bearbeiten]**.

1. Klicken Sie auf **[!UICONTROL Voreinstellungen]**.
1. Wählen Sie **[!UICONTROL E-Mails aus dieser Testumgebung empfangen]** aus.

   >[!NOTE]
   >
   >Diese Option ist nicht verfügbar, wenn Sie sich in einer Produktionsumgebung befinden.

1. Klicken Sie auf **[!UICONTROL Änderungen speichern]**.
