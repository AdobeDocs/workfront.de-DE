---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Benutzer über die Adobe Admin Console zu Adobe Workfront Fusion hinzufügen
description: Sie können einen Benutzer zur Adobe Admin Console hinzufügen und ihn Adobe Workfront Fusion zuweisen oder einen vorhandenen Benutzer in Adobe Admin Console Workfront Fusion zuweisen.
author: Becky
feature: Workfront Fusion
exl-id: c8924e00-1154-4cf8-84e8-472251b5fc28
hidefromtoc: true
source-git-commit: 6cd6b1433fb56b92872f0ad80bb1a700fc0854cc
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 1%

---

# Benutzer hinzufügen zu [!DNL Adobe Workfront Fusion] durch [!DNL Adobe Admin Console]

>[!IMPORTANT]
>
>Die auf dieser Seite beschriebenen Verfahren gelten nur für Organisationen, die in der [!DNL Adobe Admin Console].
>
>Wenn Ihr Unternehmen noch nicht in der [!DNL Adobe Admin Console], siehe [Einen Benutzer zu einer Organisation in hinzufügen [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md).
>
>Für eine Liste von Verfahren, die je nachdem, ob Ihr Unternehmen in die [!DNL Adobe Admin Console], siehe [Plattformbasierte Verwaltungsunterschiede ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md).

Sie können einen Benutzer zum [!DNL Adobe Admin Console] und weisen sie [!DNL Adobe Workfront Fusion]oder weisen Sie einen vorhandenen Benutzer in der [!DNL Adobe Admin Console] nach [!DNL Workfront Fusion].

Für ein Video mit einer Beschreibung [!DNL Workfront Fusion] im [!DNL Adobe Admin Console]Informationen zum Hinzufügen von Benutzern finden Sie unter [[!DNL Fusion] zu Adobe IMS](https://video.tv.adobe.com/v/3412464/){target=_blank}.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die in diesem Artikel enthaltene Funktionalität nutzen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>[!UICONTROL Workfront Fusion für Arbeitsautomatisierung und -integration] </p> <p>[!UICONTROL Workfront Fusion for Work Automation] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] Administratorrechte</td> 
   <td>Sie müssen ein [!UICONTROL Produktkonfigurationsadministrator] von sein. [!DNL Adobe] Produkte für Ihre Organisation.</td> 
  </tr>
  </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] Administrator.

&#42;&#42;Informationen über [!DNL Adobe Workfront Fusion] Lizenzen, siehe [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## Voraussetzungen

Vor der Verwendung von [!DNL Admin Console] für [!DNL Workfront]sollten Sie eine E-Mail erhalten, in der Sie zur Konsole eingeladen werden.

1. Wenn Sie neu bei [!DNL Adobe] und Sie erhalten eine E-Mail, in der Sie darüber informiert werden, dass Sie jetzt über Administratorrechte verfügen, um [!DNL Adobe] Software und Dienste für Ihr Unternehmen, klicken Sie auf die Schaltfläche in der E-Mail, um eine [!DNL Adobe] und öffnen Sie das [!DNL Admin Console].

   Oder

   Wenn Sie bereits über ein Adobe-Konto verfügen, wechseln Sie zum [[!DNL Adobe Admin Console] page](https://adminconsole.adobe.com/).


## Fügen Sie dem [!DNL Adobe Admin Console] und [!DNL Workfront Fusion]

1. Aus dem [[!DNL Adobe Admin Console] page](https://adminconsole.adobe.com/), wählen Sie die **[!UICONTROL Produkte]** in der oberen Navigationsleiste ein und wählen Sie dann die **[!DNL Workfront Fusion]** Produktkachel.

   ![Fusion in der Admin Console](assets/fusion-product-admin-console.png)

1. Wählen Sie in der angezeigten Liste die Organisation aus, der Sie einen Benutzer hinzufügen möchten.

   ![Fusionsinstanz in Admin Console](assets/fusion-instances-admin-console.png)

1. In der angezeigten Liste wird mit der **[!UICONTROL Produktprofile]** Registerkarte ausgewählt ist, klicken Sie auf den Namen der [!DNL Workfront Fusion] [!UICONTROL Produktprofil] Link.

   ![Workfront Fusion-Produktprofil](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > Nehmen Sie keine Änderungen an der [!UICONTROL Produktprofil] selbst.

1. Mit dem **[!UICONTROL Benutzer]** oberhalb der Liste ausgewählte Registerkarte, klicken Sie auf **[!UICONTROL Benutzer hinzufügen]**.

1. Im **[!UICONTROL Benutzer zu diesem Produktprofil hinzufügen]** Geben Sie die E-Mail-Adresse oder den Namen eines Benutzers ein, den Sie hinzufügen möchten, und wählen Sie dann den Benutzer in der angezeigten Liste aus.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Der Benutzer wird in [!DNL Workfront Fusion].

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. (Optional) Fahren Sie mit [Ändern der Zugriffsebene eines Benutzers in [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion)

## Ändern der Zugriffsstufe eines Benutzers in Workfront Fusion

### Benutzerrolle in Administrator ändern

Dem Benutzer muss eine Administratorrolle zugewiesen werden im [!DNL Adobe Admin Console].

1. Im [!DNL Workfront Fusion] [!UICONTROL Produktprofil] Seite, auf der Sie den Benutzer hinzugefügt haben, wählen Sie die **[!UICONTROL Administratoren]** Registerkarte.

1. Klicken **[!UICONTROL Admin hinzufügen]**.

1. Im **[!UICONTROL Produktprofiladministratoren hinzufügen]** Geben Sie die E-Mail-Adresse oder den Namen eines Benutzers ein, den Sie hinzufügen möchten, und wählen Sie dann den Benutzer in der angezeigten Liste aus.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Dieser Benutzer ist jetzt Administrator in [!DNL Workfront Fusion].

### Ändern Sie die Benutzerrolle in [!UICONTROL Mitglied], [!UICONTROL Buchhalter]oder [!UICONTROL App-Entwickler].

[!UICONTROL Mitglied], [!UICONTROL Buchhalter]und [!UICONTROL App-Entwickler] -Rollen werden in [!DNL Workfront Fusion].

Anweisungen finden Sie unter [Benutzerrollen anzeigen oder bearbeiten](../organizations/manage-fusion-users.md#view-or-edit-user-roles) im Artikel [Verwalten [!DNL Adobe Workfront Fusion] Benutzer in Ihrer Organisation](../organizations/manage-fusion-users.md)

## Zuweisen eines vorhandenen Benutzers im [!DNL Adobe Admin Console] nach [!DNL Workfront Fusion]

1. Beginnen Sie mit der Bearbeitung des Benutzers, wie im Abschnitt &quot;Benutzerdetails bearbeiten&quot;des Artikels beschrieben. [Benutzer einzeln verwalten](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) im [!DNL Adobe Admin Console] Dokumentation.

1. Hinzufügen **[!DNL Adobe Workfront Fusion]** zu den dem Benutzer zugewiesenen Produkten.
