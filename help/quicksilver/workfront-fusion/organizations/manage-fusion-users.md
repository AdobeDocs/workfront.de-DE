---
filename: manage-fusion-users
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Verwalten [!DNL Adobe Workfront Fusion] Benutzer in Ihrer Organisation
description: Verwalten [!DNL Adobe Workfront Fusion] Benutzer in Ihrer Organisation
author: Becky
feature: Workfront Fusion
exl-id: fbb858a6-1230-41b4-892a-4ffeb2711922
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '376'
ht-degree: 0%

---

# Verwalten [!DNL Adobe Workfront Fusion] Benutzer in Ihrer Organisation

[!DNL Adobe Workfront Fusion] Administratoren können Benutzerrollen in [!DNL Workfront Fusion].

<!--

>[!IMPORTANT]
>
>The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>For instructions on adding a user in the Adobe Admin Console:
>
>* See [Add a user to an organization in Adobe Workfront Fusion](../../workfront-fusion/organizations/add-user-to-an-organization.md#create)
>* See the section "Add users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html)
>* Contact your Adobe Admin Console Administrator.
>
>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront Fusion/Adobe Business Platform)](../../workfront-fusion/fusion-in-admin-console/fusion-adobe-admin-console.md).

-->

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

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
    <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz**</td> 
   <td> <p>Workfront Fusion für Arbeitsautomatisierung und -integration,</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> 
     <p>Sie müssen [!DNL Workfront Fusion] Administrator für Ihre Organisation.</p>
     <p>Sie müssen [!DNL Workfront Fusion] Administrator für Ihr Team.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Benutzerrollen anzeigen oder bearbeiten {#view}

[!DNL Adobe Workfront Fusion] -Administratoren können Benutzerrollen anzeigen und aktualisieren.

1. Während Sie als [!DNL Workfront Fusion] Administrator, wählen Sie **[!UICONTROL Benutzer]** in der linken Navigation.
1. Klicken **[!UICONTROL Details]** in der Zeile des Benutzers, den Sie anzeigen möchten.
1. (Optional) Um die Rolle des Benutzers zu aktualisieren, klicken Sie auf das Dropdown-Menü im **[!DNL Role]** in der Zeile der Organisation, in der Sie die Benutzerrolle ändern möchten, und wählen Sie dann die neue Rolle aus.

## Anzeigen oder Bearbeiten von Benutzerdetails {#view2}

[!DNL Adobe Workfront Fusion] -Administratoren können Benutzerdetails anzeigen und aktualisieren.

1. Während Sie als [!DNL Workfront Fusion] Administrator, wählen Sie **[!UICONTROL Benutzer]** in der linken Navigation.
1. Klicken **[!UICONTROL Details]** in der Zeile des Benutzers, den Sie anzeigen möchten.
1. (Optional) Um die Benutzerdetails zu aktualisieren, klicken Sie auf **[!UICONTROL Optionen]** in der oberen rechten Ecke des Bildschirms, und wählen Sie **[!UICONTROL Details ändern]**.

## Benutzer löschen {#delete}

[!DNL Adobe Workfront Fusion] -Administratoren können Benutzer löschen.

1. Während Sie als [!DNL Workfront Fusion] Administrator, wählen Sie [!UICONTROL Benutzer] in der linken Navigation.
1. Klicken **[!UICONTROL Details]** in der Zeile des Benutzers, den Sie anzeigen möchten.
1. (Optional) Um die Benutzerdetails zu aktualisieren, klicken Sie auf **[!UICONTROL Optionen]** in der oberen rechten Ecke des Bildschirms, und wählen Sie **[!UICONTROL Löschen]**.

### Überlegungen zum Löschen eines Benutzers in Workfront Fusion

* Wenn ein Benutzer gelöscht wird, werden die Verbindungen, Schlüssel und Webhooks des Benutzers entfernt. Alle Szenarien, die dem Benutzer gehören, werden an den Organisationseigentümer übertragen. Die Verbindungen in diesen Szenarien müssen aktualisiert werden, da die zum Benutzer gehörigen Verbindungen nicht mehr gültig sind.
* Wenn dem gelöschten Benutzer Anwendungen oder öffentliche Vorlagen gehören, werden die Anwendungen oder öffentlichen Vorlagen an den Organisationseigentümer übertragen. Wenn kein Organisationseigentümer vorhanden ist, werden die Anwendungen oder öffentlichen Vorlagen an einen anderen Benutzer übertragen.
