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
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: tm+mt
source-wordcount: '628'
ht-degree: 1%

---

# Benutzer über die [!DNL Adobe Admin Console] zu [!DNL Adobe Workfront Fusion] hinzufügen

>[!IMPORTANT]
>
>Die auf dieser Seite beschriebenen Verfahren gelten nur für Organisationen, die in den [!DNL Adobe Admin Console] integriert wurden.
>
>Wenn Ihr Unternehmen noch nicht in den [!DNL Adobe Admin Console] integriert wurde, finden Sie weitere Informationen unter [Hinzufügen eines Benutzers zu einer Organisation in  [!DNL Adobe Workfront Fusion]](../organizations/add-user-to-an-organization.md).
>
>Eine Liste der Verfahren, die sich je nachdem, ob Ihr Unternehmen in den [!DNL Adobe Admin Console] integriert wurde, unterscheiden, finden Sie unter [Plattformbasierte Verwaltungsunterschiede ([!DNL Adobe Workfront Fusion]/[!DNL Adobe Business Platform])](../fusion-in-admin-console/fusion-adobe-admin-console.md).

Sie können einen Benutzer zum [!DNL Adobe Admin Console] hinzufügen und ihn [!DNL Adobe Workfront Fusion] zuweisen oder einen vorhandenen Benutzer im [!DNL Adobe Admin Console] zu [!DNL Workfront Fusion] zuweisen.

Ein Video mit der Beschreibung von [!DNL Workfront Fusion] in der [!DNL Adobe Admin Console], einschließlich des Hinzufügens von Benutzern, finden Sie unter [[!DNL Fusion] in Adobe IMS](https://video.tv.adobe.com/v/3412464/){target=_blank}.

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] oder höher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!UICONTROL Select]- oder [!UICONTROL Prime] [!DNL Adobe Workfront]-Plan verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können. [!DNL Workfront Fusion] ist im [!UICONTROL Ultimate] [!DNL Workfront]-Plan enthalten.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] erwerben, um die in diesem Artikel beschriebenen Funktionen nutzen zu können.</p>
   </td> 
  </tr>
   <tr> 
   <td role="rowheader">[!DNL Adobe] Administratorberechtigungen</td> 
   <td>Sie müssen ein [!UICONTROL Produktkonfigurationsadministrator] von [!DNL Adobe] -Produkten für Ihr Unternehmen sein.</td> 
  </tr>
  </tbody> 
</table>

&#42;Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

&#42;&#42;Informationen zu [!DNL Adobe Workfront Fusion] Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md)



## Voraussetzungen

Bevor Sie die [!DNL Admin Console] für [!DNL Workfront] verwenden, sollten Sie eine E-Mail erhalten, in der Sie zur Konsole eingeladen werden.

1. Wenn Sie neu bei [!DNL Adobe] sind und eine E-Mail erhalten haben, in der Sie darüber informiert werden, dass Sie jetzt über Administratorrechte für die Verwaltung von [!DNL Adobe] Software und Services für Ihr Unternehmen verfügen, klicken Sie auf die Schaltfläche in der E-Mail, um ein [!DNL Adobe] -Konto zu erstellen, und öffnen Sie das [!DNL Admin Console].

   Oder

   Wenn Sie bereits über ein Adobe-Konto verfügen, gehen Sie zur Seite [[!DNL Adobe Admin Console] Seite](https://adminconsole.adobe.com/).


## Fügen Sie den [!DNL Adobe Admin Console] und [!DNL Workfront Fusion] einen neuen Benutzer hinzu.

1. Wählen Sie auf der Seite [[!DNL Adobe Admin Console] Seite](https://adminconsole.adobe.com/) die Registerkarte **[!UICONTROL Produkte]** in der oberen Navigationsleiste und dann die Kachel **[!DNL Workfront Fusion]** des Produkts aus.

   ![Fusion in Admin Console](assets/fusion-product-admin-console.png)

1. Wählen Sie in der angezeigten Liste die Organisation aus, der Sie einen Benutzer hinzufügen möchten.

   ![Fusion-Instanz in Admin Console](assets/fusion-instances-admin-console.png)

1. Klicken Sie in der angezeigten Liste mit der ausgewählten Registerkarte **[!UICONTROL Produktprofile]** auf den Namen des Links [!DNL Workfront Fusion] [!UICONTROL Produktprofil] .

   ![Workfront Fusion-Produktprofil](../../administration-and-setup/add-users/create-and-manage-users/assets/prod-profile-1.png)

   >[!IMPORTANT]
   >
   > Nehmen Sie keine Änderungen am [!UICONTROL Produktprofil] selbst vor.

1. Klicken Sie bei ausgewählter Registerkarte **[!UICONTROL Benutzer]** oberhalb der Liste auf **[!UICONTROL Benutzer hinzufügen]**.

1. Geben Sie in das Feld **[!UICONTROL Benutzer zu diesem Produktprofil hinzufügen]** die E-Mail-Adresse oder den Namen eines Benutzers ein, den Sie hinzufügen möchten, und wählen Sie dann den Benutzer in der angezeigten Liste aus.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Der Benutzer wird in [!DNL Workfront Fusion] erstellt.

   <!--
    >[!IMPORTANT]
    >
    > Do not make any changes to the Product Profile itself.
    -->

1. (Optional) Fahren Sie mit [Ändern der Zugriffsstufe eines Benutzers in [!DNL Workfront Fusion]](#change-a-users-access-level-in-workfront-fusion) fort.

## Ändern der Zugriffsstufe eines Benutzers in Workfront Fusion

### Benutzerrolle in Administrator ändern

Die Zuweisung einer Administratorrolle für einen Benutzer muss in der [!DNL Adobe Admin Console] erfolgen.

1. Wählen Sie auf der Seite [!DNL Workfront Fusion] [!UICONTROL Produktprofil] , auf der Sie den Benutzer hinzugefügt haben, die Registerkarte **[!UICONTROL Administratoren]** aus.

1. Klicken Sie auf **[!UICONTROL Admin hinzufügen]**.

1. Geben Sie im Feld **[!UICONTROL Produktprofiladministratoren hinzufügen]** die E-Mail-Adresse oder den Namen eines Benutzers ein, den Sie hinzufügen möchten, und wählen Sie dann den Benutzer in der angezeigten Liste aus.

1. Klicken Sie auf **[!UICONTROL Speichern]**.

   Dieser Benutzer ist jetzt Administrator in [!DNL Workfront Fusion].

### Ändern Sie die Benutzerrolle in [!UICONTROL Member], [!UICONTROL Accountant] oder [!UICONTROL App-Entwickler].

Die Rollen [!UICONTROL Member], [!UICONTROL Accountant] und [!UICONTROL App-Entwickler] werden innerhalb von [!DNL Workfront Fusion] verarbeitet.

Anweisungen finden Sie unter [Anzeigen oder Bearbeiten von Benutzerrollen](../organizations/manage-fusion-users.md#view-or-edit-user-roles) im Artikel [Verwalten [!DNL Adobe Workfront Fusion] Benutzer in Ihrer Organisation](../organizations/manage-fusion-users.md) .

## Zuweisen eines vorhandenen Benutzers im [!DNL Adobe Admin Console] zu [!DNL Workfront Fusion]

1. Beginnen Sie mit der Bearbeitung des Benutzers, wie im Abschnitt &quot;Benutzerdetails bearbeiten&quot;des Artikels [Benutzer einzeln verwalten](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) in der [!DNL Adobe Admin Console] -Dokumentation beschrieben.

1. Fügen Sie **[!DNL Adobe Workfront Fusion]** zu den dem Benutzer zugewiesenen Produkten hinzu.
