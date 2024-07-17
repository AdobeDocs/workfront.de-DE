---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Anzeigen und Verwalten benutzerdefinierter OAuth2-Anwendungen
description: Als Adobe Workfront-Administrator können Sie die OAuth2-Anwendungen für Ihre Workfront-Instanz anzeigen und verwalten, die anderen Anwendungen den Zugriff auf Workfront ermöglichen.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: 6f041459caf040846ffdec5bc75e9d74c99e318b
workflow-type: tm+mt
source-wordcount: '720'
ht-degree: 0%

---

# Anzeigen und Verwalten benutzerdefinierter OAuth2-Anwendungen

Als [!DNL Adobe Workfront] -Administrator können Sie die OAuth2-Anwendungen für Ihre Instanz von [!DNL Workfront] anzeigen und verwalten, die anderen Anwendungen den Zugriff auf [!UICONTROL Workfront] ermöglichen.

>[!NOTE]
>
>* Im Kontext von OAuth2 bezieht sich &quot;Oauth2-Anwendung&quot;auf diese Art von Zugriffslink zwischen einer App und einem Server wie [!DNL Workfront]. Weitere Informationen finden Sie unter [Erstellen von OAuth2-Anwendungen für [!DNL Workfront] Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md) .
>* Sie können bis zu zehn OAuth2-Anwendungen gleichzeitig haben.

* Informationen zum Erstellen benutzerdefinierter OAuth2-Anwendungen finden Sie unter [Erstellen von OAuth2-Anwendungen für [!DNL Workfront] Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mit Benutzeranmeldeinformationen (Fluss des Autorisierungscodes) finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des Autorisierungscodeflusses](../../wf-api/api/oauth-app-code-token-flow.md).
* Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mithilfe der Serverauthentifizierung (JWT-Fluss) finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des JWT-Flusses](../../wf-api/api/oauth-app-jwt-flow.md).
* Anweisungen zum Konfigurieren und Verwenden der OAuth2-Anwendung mit PKCE finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mit PKCE Flow](../../wf-api/api/oauth-app-pkce-flow.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> Sie müssen ein [!DNL Workfront] -Administrator sein. </p>
    <p>Weitere Informationen zu [!DNL Workfront] -Administratoren finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren eines vollen Administratorzugriffs für einen Benutzer</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Sie müssen [!UICONTROL OAuth2]-Anwendungen für Ihr Unternehmen erstellen, bevor Sie sie anzeigen oder verwalten können.

Weitere Informationen finden Sie unter [Erstellen von OAuth2-Anwendungen für [!DNL Workfront] Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md) .

## Benutzerdefinierte OAuth2-Anwendungen verwalten

* [Anzeigen und Bearbeiten benutzerdefinierter OAuth2-Anwendungen](#view-and-edit-custom-oauth2-applications)
* [Löschen benutzerdefinierter OAuth2-Anwendungen](#delete-custom-oauth2-applications)

### Anzeigen und Bearbeiten benutzerdefinierter OAuth2-Anwendungen {#view-and-edit-custom-oauth2-applications}

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]** und wählen Sie dann **[!UICONTROL OAuth Applications]** aus.
1. Klicken Sie auf **[!UICONTROL App-Integration erstellen]**.
1. Bewegen Sie den Mauszeiger über die Anwendung und klicken Sie auf **[!UICONTROL Bearbeiten]** ![](assets/edit-icon.png) , wenn sie ganz rechts angezeigt wird.
1. (Optional) Bearbeiten Sie alle Details der Anwendung.

   Informationen zu Feldern, die sich auf OAuth2- und JWT-Apps beziehen, finden Sie unter [Erstellen von OAuth2-Anwendungen für [!DNL Workfront] Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### Löschen benutzerdefinierter OAuth2-Anwendungen {#delete-custom-oauth2-applications}

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]** und wählen Sie dann **[!UICONTROL OAuth Applications]** aus.
1. Klicken Sie auf ** **.
1. Bewegen Sie den Mauszeiger über die Anwendung und klicken Sie auf **[!UICONTROL Löschen]** ![](assets/delete.png) , wenn sie ganz rechts angezeigt wird.

## Verwalten von Client-Geheimnissen in OAuth2-Anwendungen

* [Client-Geheimnisdetails anzeigen](#view-client-secret-details)
* [Notizen für Client Secret hinzufügen oder bearbeiten](#add-or-edit-notes-for-client-secret)
* [Client-Geheimnis löschen](#delete-client-secret)

### Client-Geheimnisdetails anzeigen {#view-client-secret-details}

>[!IMPORTANT]
>
>Sie können das Client-Geheimnis nicht selbst anzeigen. Wenn Sie Ihr Client-Geheimnis verloren haben, müssen Sie es löschen und ein neues erstellen.
>
>* Informationen zum Löschen eines Client-Geheimnisses finden Sie unter [Client-Geheimnis löschen](#delete-client-secret) in diesem Artikel.
>* Informationen zum Erstellen eines neuen Client-Geheimnisses finden Sie unter [Erstellen einer OAuth2-Anwendung](../../administration-and-setup/configure-integrations/create-oauth-application.md#create) in [Erstellen von OAuth2-Anwendungen für [!DNL Workfront] Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>



1. Klicken Sie auf das Symbol *[!UICONTROL *Hauptmenü]** ![](assets/main-menu-icon.png) in der oberen rechten Ecke von [!DNL Adobe Workfront] und klicken Sie dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]** und wählen Sie dann **[!UICONTROL OAuth Applications]** aus.
1. Bewegen Sie den Mauszeiger über die Anwendung und klicken Sie auf das Symbol **[!UICONTROL Bearbeiten]** , wenn es ganz rechts angezeigt wird.
1. Details zum Client-Geheimnisbereich anzeigen:

   * Erstellungsdatum
   * Zuletzt verwendetes Datum
   * Notizen

     Informationen zum Hinzufügen von Notizen zu einem Client-Geheimnis finden Sie unter [Hinzufügen oder Bearbeiten von Notizen zum Client-Geheimnis](#add-or-edit-notes-for-client-secret).

### Notizen für Client Secret hinzufügen oder bearbeiten {#add-or-edit-notes-for-client-secret}

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]** und wählen Sie dann **[!UICONTROL OAuth Applications]** aus.
1. Klicken Sie auf **[!UICONTROL App-Integration erstellen]**.
1. Bewegen Sie den Mauszeiger über die Anwendung und klicken Sie auf das Symbol **[!UICONTROL Bearbeiten]** , wenn es ganz rechts angezeigt wird.
1. Suchen Sie nach dem Client-Geheimnis, für das Sie eine Notiz hinzufügen oder bearbeiten möchten.
1. Klicken Sie auf das Feld, das Details zum Client-Geheimnis enthält.

   Sie können jetzt Text für Anmerkungen hinzufügen oder vorhandenen Text für Anmerkungen bearbeiten.

   >[!NOTE]
   >
   >Der Text für Notizen ist maximal 64 Zeichen lang.

1. Klicken Sie auf das vorkonfigurierte Feld oder drücken Sie die **[!UICONTROL Eingabetaste]**, um den Text der Notiz zu speichern.

### Client-Geheimnis löschen {#delete-client-secret}

1. Klicken Sie auf das Symbol **[!UICONTROL Hauptmenü]** oben rechts in [!DNL Adobe Workfront] und dann auf **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).![](assets/main-menu-icon.png)

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]** und wählen Sie dann **[!UICONTROL OAuth Applications]** aus.
1. Klicken Sie auf **[!UICONTROL App-Integration erstellen]**.
1. Bewegen Sie den Mauszeiger über die Anwendung und klicken Sie auf das Symbol **[!UICONTROL Bearbeiten]** , wenn es ganz rechts angezeigt wird.
1. Suchen Sie nach dem Client-Geheimnis, das Sie löschen möchten.
1. Klicken Sie auf das Symbol **[!UICONTROL Löschen]** ![](assets/delete.png) neben dem Client-Geheimnis.
