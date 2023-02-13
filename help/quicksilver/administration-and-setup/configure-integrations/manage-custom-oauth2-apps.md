---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Anzeigen und Verwalten benutzerdefinierter OAuth2-Anwendungen
description: Als Adobe Workfront-Administrator können Sie die OAuth2-Anwendungen für Ihre Workfront-Instanz anzeigen und verwalten, die anderen Anwendungen den Zugriff auf Workfront ermöglichen.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: f7e3182776e6b62103cd755b2fbd5057efc95394
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 1%

---

# Anzeigen und Verwalten benutzerdefinierter OAuth2-Anwendungen

Als [!DNL Adobe Workfront] Administrator können Sie die OAuth2-Anwendungen für Ihre Instanz von [!DNL Workfront], die anderen Anwendungen den Zugriff erlauben [!UICONTROL Workfront].

>[!NOTE]
>
>Im Kontext von OAuth2 bezieht sich &quot;Oauth2-Anwendung&quot;auf diese Art von Zugriffslink zwischen einer App und einem Server wie [!DNL Workfront]. Weitere Informationen finden Sie unter [Erstellen von OAuth2-Anwendungen für [!DNL Workfront] Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md)

* Informationen zum Erstellen benutzerdefinierter OAuth2-Anwendungen finden Sie unter [Erstellen von OAuth2-Anwendungen für [!DNL Workfront] Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mit Benutzeranmeldeinformationen (Autorisierungscode-Ablauf) finden Sie unter [Benutzerdefinierte OAuth 2-Anwendungen Ihres Unternehmens mithilfe des Autorisierungscode-Flusses konfigurieren und verwenden](../../wf-api/api/oauth-app-code-token-flow.md).
* Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mithilfe der Serverauthentifizierung (JWT-Fluss) finden Sie unter [Benutzerdefinierte OAuth 2-Anwendungen Ihres Unternehmens mithilfe des JWT-Flusses konfigurieren und verwenden](../../wf-api/api/oauth-app-jwt-flow.md).
* Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mit PKCE finden Sie unter [Benutzerdefinierte OAuth 2-Anwendungen Ihres Unternehmens mithilfe des PKCE-Flusses konfigurieren und verwenden](../../wf-api/api/oauth-app-pkce-flow.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> Sie müssen [!DNL Workfront] Administrator. </p>
    <p>Informationen über [!DNL Workfront] Administratoren, siehe <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

## Voraussetzungen

Sie müssen [!UICONTROL OAuth2] Anwendungen für Ihre Organisation erstellen, bevor Sie sie anzeigen oder verwalten können.

Weitere Informationen finden Sie unter [Erstellen von OAuth2-Anwendungen für [!DNL Workfront] Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Benutzerdefinierte OAuth2-Anwendungen verwalten

* [Anzeigen und Bearbeiten benutzerdefinierter OAuth2-Anwendungen](#view-and-edit-custom-oauth2-applications)
* [Löschen benutzerdefinierter OAuth2-Anwendungen](#delete-custom-oauth2-applications)

### Anzeigen und Bearbeiten benutzerdefinierter OAuth2-Anwendungen {#view-and-edit-custom-oauth2-applications}

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]**, wählen Sie **[!UICONTROL OAuth-Anwendungen]**.
1. Klicken **[!UICONTROL App-Integration erstellen]**.
1. Bewegen Sie den Mauszeiger über die Anwendung und klicken Sie auf **[!UICONTROL Bearbeiten]** ![](assets/edit-icon.png) wenn es ganz rechts erscheint.
1. (Optional) Bearbeiten Sie alle Details der Anwendung.

   Informationen zu Feldern für OAuth2- und JWT-Apps finden Sie unter [Erstellen von OAuth2-Anwendungen für [!DNL Workfront] Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### Löschen benutzerdefinierter OAuth2-Anwendungen {#delete-custom-oauth2-applications}

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]**, wählen Sie **[!UICONTROL OAuth-Anwendungen]**.
1. Klicken **  **.
1. Bewegen Sie den Mauszeiger über die Anwendung und klicken Sie auf **[!UICONTROL Löschen]** ![](assets/delete.png) wenn es ganz rechts erscheint.

## Verwalten von Client-Geheimnissen in OAuth2-Anwendungen

* [Client-Geheimnisdetails anzeigen](#view-client-secret-details)
* [Notizen für Client Secret hinzufügen oder bearbeiten](#add-or-edit-notes-for-client-secret)
* [Geheimen Client-Schlüssel löschen](#delete-client-secret)

### Client-Geheimnisdetails anzeigen {#view-client-secret-details}

>[!IMPORTANT]
>
>Sie können das Client-Geheimnis nicht selbst anzeigen. Wenn Sie Ihr Client-Geheimnis verloren haben, müssen Sie es löschen und ein neues erstellen.
>
>* Informationen zum Löschen eines Client-Geheimnisses finden Sie unter [Client-Geheimnis löschen](#delete-client-secret) in diesem Artikel.
>* Informationen zum Erstellen eines neuen Client-Geheimnisses finden Sie unter [Erstellen einer OAuth2-Anwendung](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) in [Erstellen von OAuth2-Anwendungen für [!DNL Workfront] Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>




1. Klicken Sie auf *[!UICONTROL *Hauptmenü]** Symbol ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]**, wählen Sie **[!UICONTROL OAuth-Anwendungen]**.
1. Bewegen Sie den Mauszeiger über die Anwendung und klicken Sie auf **[!UICONTROL Bearbeiten]** angezeigt, wenn es ganz rechts angezeigt wird.
1. Details zum Client-Geheimnisbereich anzeigen:

   * Erstellungsdatum
   * Zuletzt verwendetes Datum
   * Notizen

      Informationen zum Hinzufügen von Notizen zu einem Client-Geheimnis finden Sie unter [Notizen für Client Secret hinzufügen oder bearbeiten](#add-or-edit-notes-for-client-secret).

### Notizen für Client Secret hinzufügen oder bearbeiten {#add-or-edit-notes-for-client-secret}

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]**, wählen Sie **[!UICONTROL OAuth-Anwendungen]**.
1. Klicken **[!UICONTROL App-Integration erstellen]**.
1. Bewegen Sie den Mauszeiger über die Anwendung und klicken Sie auf **[!UICONTROL Bearbeiten]** angezeigt, wenn es ganz rechts angezeigt wird.
1. Suchen Sie nach dem Client-Geheimnis, für das Sie eine Notiz hinzufügen oder bearbeiten möchten.
1. Klicken Sie auf das Feld, das Details zum Client-Geheimnis enthält.

   Sie können jetzt Text für Anmerkungen hinzufügen oder vorhandenen Text für Anmerkungen bearbeiten.

   >[!NOTE]
   >
   >Der Text für Notizen ist maximal 64 Zeichen lang.

1. Klicken Sie auf &quot;Out of the box&quot;oder drücken Sie die **[!UICONTROL Eingabe]** , um den Text der Notiz zu speichern.

### Geheimen Client-Schlüssel löschen {#delete-client-secret}

1. Klicken Sie auf **[!UICONTROL Hauptmenü]** icon ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront]Klicken Sie auf **[!UICONTROL Einrichtung]** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]**, wählen Sie **[!UICONTROL OAuth-Anwendungen]**.
1. Klicken **[!UICONTROL App-Integration erstellen]**.
1. Bewegen Sie den Mauszeiger über die Anwendung und klicken Sie auf **[!UICONTROL Bearbeiten]** angezeigt, wenn es ganz rechts angezeigt wird.
1. Suchen Sie nach dem Client-Geheimnis, das Sie löschen möchten.
1. Klicken Sie auf **[!UICONTROL Löschen]** icon ![](assets/delete.png) neben dem Client-Geheimnis.
