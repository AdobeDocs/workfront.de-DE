---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: administrator-integrations
title: Anzeigen und Verwalten benutzerdefinierter OAuth2-Anwendungen
description: Als Adobe Workfront-Administrator können Sie die OAuth2-Programme für Ihre Workfront-Instanz anzeigen und verwalten, die anderen Programmen den Zugriff auf Workfront ermöglichen.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
author: Becky
exl-id: 158430e5-8857-4bd8-86a6-2ba106b1638c
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '669'
ht-degree: 0%

---

# Anzeigen und Verwalten benutzerdefinierter OAuth2-Anwendungen

Als [!DNL Adobe Workfront] können Sie die OAuth2-Programme für Ihre Instanz von [!DNL Workfront] anzeigen und verwalten, die anderen Programmen den Zugriff auf [!UICONTROL Workfront] ermöglichen.

>[!NOTE]
>
>* Im Kontext von OAuth2 bezieht sich „OAuth2-Anwendung“ auf diese Art von Zugriffs-Link zwischen einer Anwendung und einem Server wie [!DNL Workfront]. Weitere Informationen finden Sie unter [Erstellen von OAuth2-Anwendungen für  [!DNL Workfront] -Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md)
>* Sie können bis zu zehn OAuth2-Anwendungen gleichzeitig haben.

* Informationen zum Erstellen benutzerdefinierter OAuth2-Anwendungen finden Sie unter [Erstellen von OAuth2-Anwendungen für  [!DNL Workfront] -Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md)
* Anweisungen zur Konfiguration und Verwendung der OAuth2-Anwendung mit Benutzeranmeldeinformationen (Autorisierungs-Code-Fluss) finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe eines Autorisierungs-Code-Flusses](../../wf-api/api/oauth-app-code-token-flow.md).
* Anweisungen zur Konfiguration und Verwendung der OAuth2-Anwendung mithilfe der Server-Authentifizierung (JWT-Fluss) finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe des JWT-Flusses](../../wf-api/api/oauth-app-jwt-flow.md).
* Anweisungen zur Konfiguration und Verwendung der OAuth2-Anwendung mithilfe von PKCE finden Sie unter [Konfigurieren und Verwenden der benutzerdefinierten OAuth 2-Anwendungen Ihres Unternehmens mithilfe von PKCE-Fluss](../../wf-api/api/oauth-app-pkce-flow.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
   <td role="rowheader">[!DNL Adobe Workfront] Lizenz*</td> 
   <td> <p>[!UICONTROL Plan] oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> Sie müssen [!DNL Workfront] sein. </p>
    <p>Informationen zu [!DNL Workfront] finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Gewähren des vollständigen Administratorzugriffs für einen Benutzer</a>.</p>
     </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

## Voraussetzungen

Sie müssen [!UICONTROL OAuth2]-Programme für Ihr Unternehmen erstellen, bevor Sie sie anzeigen oder verwalten können.

Weitere Informationen finden Sie unter [Erstellen von OAuth2-Anwendungen für  [!DNL Workfront] -Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md)

## Verwalten benutzerdefinierter OAuth2-Anwendungen

* [Anzeigen und Bearbeiten benutzerdefinierter OAuth2-Anwendungen](#view-and-edit-custom-oauth2-applications)
* [Löschen benutzerdefinierter OAuth2-Anwendungen](#delete-custom-oauth2-applications)

### Anzeigen und Bearbeiten benutzerdefinierter OAuth2-Anwendungen {#view-and-edit-custom-oauth2-applications}

{{step-1-to-setup}}

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]** und wählen Sie dann **[!UICONTROL OAuth-Anwendungen]**.
1. Klicken Sie **[!UICONTROL App-Integration erstellen]**.
1. Bewegen Sie den Mauszeiger über die Anwendung und klicken Sie auf **[!UICONTROL Bearbeiten]** ![Bearbeiten-](assets/edit-icon.png), wenn sie ganz rechts angezeigt wird.
1. (Optional) Bearbeiten Sie alle Details der Anwendung.

   Felder, die sich auf OAuth2- und JWT-Apps beziehen, finden Sie unter [Erstellen von OAuth2-Programmen für  [!DNL Workfront] -Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md).

### Löschen benutzerdefinierter OAuth2-Anwendungen {#delete-custom-oauth2-applications}

{{step-1-to-setup}}

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]** und wählen Sie dann **[!UICONTROL OAuth-Anwendungen]**.
1. Bewegen Sie den Mauszeiger über die Anwendung und klicken Sie auf **[!UICONTROL Löschen]** ![Löschen](assets/delete.png), wenn sie ganz rechts angezeigt wird.

## Verwalten von Client-Geheimnissen in OAuth2-Anwendungen

* [Details zum Client-Geheimnis anzeigen](#view-client-secret-details)
* [Hinzufügen oder Bearbeiten von Hinweisen für Client-Geheimnis](#add-or-edit-notes-for-client-secret)
* [Geheimen Client-Schlüssel löschen](#delete-client-secret)

### Details zum Client-Geheimnis anzeigen {#view-client-secret-details}

>[!IMPORTANT]
>
>Das Client-Geheimnis selbst kann nicht angezeigt werden. Wenn Sie Ihr Client-Geheimnis verloren haben, müssen Sie es löschen und ein neues erstellen.
>
>* Informationen zum Löschen eines Client-Geheimnisses finden Sie unter [Löschen des Client-](#delete-client-secret)) in diesem Artikel.
>* Informationen zum Erstellen eines neuen Client-Geheimnisses finden Sie unter [Erstellen einer OAuth2](../../administration-and-setup/configure-integrations/create-oauth-application.md#create)Anwendung) in [Erstellen von OAuth2-Anwendungen für  [!DNL Workfront] -Integrationen](../../administration-and-setup/configure-integrations/create-oauth-application.md).
>

{{step-1-to-setup}}

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]** und wählen Sie dann **[!UICONTROL OAuth-Anwendungen]**.
1. Bewegen Sie den Mauszeiger über die Anwendung und klicken Sie auf **[!UICONTROL Bearbeiten]**-Symbol, wenn es ganz rechts angezeigt wird.
1. Details finden Sie im Bereich Client-Geheimnis :

   * Erstellungsdatum
   * Datum der letzten Verwendung
   * Notizen

     Informationen zum Hinzufügen von Hinweisen zu Client-Geheimnissen finden Sie unter [Hinzufügen oder Bearbeiten von Hinweisen zu Client-Geheimnissen](#add-or-edit-notes-for-client-secret).

### Hinzufügen oder Bearbeiten von Hinweisen für Client-Geheimnis {#add-or-edit-notes-for-client-secret}

{{step-1-to-setup}}

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]** und wählen Sie dann **[!UICONTROL OAuth-Anwendungen]**.
1. Klicken Sie **[!UICONTROL App-Integration erstellen]**.
1. Bewegen Sie den Mauszeiger über die Anwendung und klicken Sie auf **[!UICONTROL Bearbeiten]**-Symbol, wenn es ganz rechts angezeigt wird.
1. Suchen Sie das Client-Geheimnis, für das Sie eine Anmerkung hinzufügen oder bearbeiten möchten.
1. Klicken Sie auf das Feld, das Details zum Client-Geheimnis enthält.

   Sie können jetzt Notizentext hinzufügen oder vorhandenen Notizentext bearbeiten.

   >[!NOTE]
   >
   >Notizentext darf maximal 64 Zeichen enthalten.

1. Klicken Sie im Lieferumfang auf oder drücken Sie die **[!UICONTROL Eingabetaste]**, um den Notizentext zu speichern.

### Geheimen Client-Schlüssel löschen {#delete-client-secret}

{{step-1-to-setup}}

1. Klicken Sie im linken Navigationsbereich auf **[!UICONTROL System]** und wählen Sie dann **[!UICONTROL OAuth-Anwendungen]**.
1. Klicken Sie **[!UICONTROL App-Integration erstellen]**.
1. Bewegen Sie den Mauszeiger über die Anwendung und klicken Sie auf **[!UICONTROL Bearbeiten]**-Symbol, wenn es ganz rechts angezeigt wird.
1. Suchen Sie den zu löschenden geheimen Client-Schlüssel.
1. Klicken Sie auf das **[!UICONTROL Löschen]**-Symbol ![Löschen](assets/delete.png) neben dem Client-Geheimnis.
