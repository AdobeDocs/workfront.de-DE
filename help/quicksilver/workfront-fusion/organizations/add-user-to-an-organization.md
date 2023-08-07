---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Hinzufügen eines Benutzers zu einer Organisation in Adobe Workfront Fusion
description: Sie können in Adobe Workfront Fusion Organisationen Benutzer hinzufügen.
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 2884f709ef9ea89f275ff88db41ddde725dbd781
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# Hinzufügen eines Benutzers zu einer Organisation in Adobe Workfront Fusion

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in die [!DNL Adobe Admin Console]. Wenn Ihr Unternehmen bei der [!DNL Adobe Admin Console], müssen Sie diese Aktion durch [!DNL Adobe Admin Console].
>
>Anweisungen zum Hinzufügen eines Benutzers im[!DNL  Adobe Admin Console]finden Sie im Abschnitt &quot;Benutzerdetails bearbeiten&quot;des Artikels [Benutzer einzeln verwalten](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) oder kontaktieren Sie Ihre [!UICONTROL Adobe Admin Console] Administrator.
>
>Eine Liste der Verfahren, die je nachdem, ob Ihr Unternehmen in die Adobe Admin Console integriert wurde, unterschiedlich sind, finden Sie unter [Plattformbasierte Verwaltungsunterschiede (Adobe Workfront Fusion/Adobe Business Platform)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

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
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz*</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: nein [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für Arbeitsautomatisierung und Integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über [!UICONTROL Select] oder [!UICONTROL Prime] verfügen [!DNL Adobe Workfront] Planung, Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden. [!DNL Workfront Fusion] ist in [!UICONTROL Ultimate] enthalten. [!DNL Workfront] Plan.</p>
   <p>Oder</p>
   <p>Alte Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] sowie [!DNL Adobe Workfront] , um die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
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

## Hinzufügen von Benutzern zu einer Organisation

<p>Das Verfahren zum Hinzufügen eines Benutzers zu Ihrer Fusion-Organisation hängt davon ab, ob Ihr Unternehmen in die Adobe Business Platform integriert wurde. </p>
<ul>
<li> <p><a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Hinzufügen eines Benutzers zu einer Organisation, die in die Adobe Business Platform integriert wurde</a> </p> </li>
<li> <p><a href="#add-a-user-to-an-organization-that-has-not-been-onboarded-to-the-adobe-business-console" class="MCXref xref">Benutzer zu einer Organisation hinzufügen, die nicht in der Adobe Business Console integriert wurde</a> </p> </li>
</ul>
<div>
<p><strong>Hinzufügen eines Benutzers zu einer Organisation, die in die Adobe Business Platform integriert wurde</strong></p>
<p>Wenn Ihr Unternehmen in die Adobe Business Platform integriert wurde, müssen Sie diese Aktion über die Adobe Admin Console durchführen.</p>
<p>Anweisungen zum Hinzufügen eines Benutzers in Adobe Admin Console:</p>
<ul>
<li> <p>Siehe <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">Erstellen von Benutzern in Workfront mit Adobe Admin Console</a></p> </li>
<li> <p>Siehe den Abschnitt "Benutzer hinzufügen"im Artikel <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Benutzer einzeln verwalten</a></p> </li>
<li> <p>Wenden Sie sich an Ihren Adobe Admin Console-Administrator.</p> </li>
</ul>
<p>Eine Liste der Verfahren, die je nachdem, ob Ihr Unternehmen in die Adobe Business Platform integriert wurde, unterschiedlich sind, finden Sie unter <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">Plattformbasierte Verwaltungsunterschiede (Adobe Workfront/Adobe Business Platform)</a>.</p>
</div>
<p><strong>Benutzer zu einer Organisation hinzufügen, die nicht in der Adobe Business Console integriert wurde</strong></p>

Um Benutzer zur Organisation hinzuzufügen, müssen Sie Administrator der Organisation sein, der Sie Benutzer hinzufügen möchten. Informationen zu Rollen finden Sie unter [Organisationsrollen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

So fügen Sie einen Benutzer zur Organisation hinzu:

1. Navigieren Sie zu **[!UICONTROL Organisationen]** im Menü und wählen Sie die Organisation aus, der Sie einen Benutzer hinzufügen möchten.
1. Öffnen Sie die **[!UICONTROL Benutzer]** in Ihrem Dashboard.
1. Klicks **[!UICONTROL Neuen Benutzer einladen]**, füllen Sie das Formular aus (E-Mail, Nachricht, Rolle) und senden Sie die Einladung durch Klicken auf **[!UICONTROL Senden]**.

>[!NOTE]
>
>   
><p>Wenn die Schaltfläche [!UICONTROL Neuen Benutzer einladen] nicht angezeigt wird, wurde Ihr Unternehmen in die [!DNL Adobe Business Platform.] </p>
>
>   <p>Anweisungen zum Hinzufügen eines Benutzers zu einer Organisation, die in die [!DNL Adobe Business Platform], siehe <a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Fügen Sie einen Benutzer zu einer Organisation hinzu, die in die [!DNL Adobe Business Platform]</a></p>

Der Benutzer erhält eine Einladungs-E-Mail, in der er die Einladung annehmen kann.
