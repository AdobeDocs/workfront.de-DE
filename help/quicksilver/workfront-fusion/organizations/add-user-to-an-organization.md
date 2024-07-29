---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Hinzufügen eines Benutzers zu einer Organisation in Adobe Workfront Fusion
description: Sie können in Adobe Workfront Fusion Organisationen Benutzer hinzufügen.
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 1b4a6d2b2ad57ddf1afd5dadf8b1fed358f95b61
workflow-type: tm+mt
source-wordcount: '623'
ht-degree: 0%

---

# Hinzufügen eines Benutzers zu einer Organisation oder einem Team in Adobe Workfront Fusion

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in den [!DNL Adobe Admin Console] integriert wurden. Wenn Ihr Unternehmen in die [!DNL Adobe Admin Console] integriert wurde, müssen Sie diese Aktion über die [!DNL Adobe Admin Console] durchführen.
>
>Anweisungen zum Hinzufügen eines Benutzers, nachdem Ihr Unternehmen in den Ordner &quot;[!DNL  Adobe Admin Console]&quot;und das Adobe &quot;Einheitliches Erlebnis&quot;verschoben wurde, finden Sie unter [Hinzufügen von Benutzern zu  [!DNL Adobe Workfront Fusion]  über den Abschnitt &quot; [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md)&quot;.
>
>Eine Liste der Verfahren, die sich je nachdem, ob Ihr Unternehmen in die Adobe Admin Console integriert wurde, unterscheiden, finden Sie unter [Plattformbasierte Verwaltungsunterschiede (Adobe Workfront Fusion/Adobe Business Platform)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

## Zugriffsanforderungen

Sie müssen über den folgenden Zugriff verfügen, um die Funktionalität in diesem Artikel verwenden zu können:

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
    <td> <p>[!UICONTROL Plan], [!UICONTROL Arbeit]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion]-Lizenz*</td> 
   <td>
   <p>Aktuelle Lizenzanforderungen: Keine [!DNL Workfront Fusion] Lizenzanforderungen.</p>
   <p>Oder</p>
   <p>Alte Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung und -integration], [!UICONTROL [!DNL Workfront Fusion] für die Arbeitsautomatisierung]</p>
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
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> 
     <p>Sie müssen ein [!DNL Workfront Fusion] -Administrator für Ihre Organisation sein.</p>
     <p>Sie müssen ein [!DNL Workfront Fusion] -Administrator für Ihr Team sein.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront] -Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

Informationen zu [!DNL Adobe Workfront Fusion] -Lizenzen finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Hinzufügen von Benutzern zu einer Organisation


<!--
<p>The procedure to add a user to your Fusion organization differs based on whether your organization has been onboarded to the Adobe Business Platform. </p>
<ul>
<li> <p><a href="#add-a-user-to-an-organization-that-has-been-onboarded-to-the-adobe-business-platform" class="MCXref xref">Add a user to an organization that has been onboarded to the Adobe Business Platform</a> </p> </li>
<li> <p><a href="#add-a-user-to-an-organization-that-has-not-been-onboarded-to-the-adobe-business-console" class="MCXref xref">Add a user to an organization that has not been onboarded to the Adobe Business Console</a> </p> </li>
</ul>
<div>
<p><strong>Add a user to an organization that has been onboarded to the Adobe Business Platform</strong></p>
<p>If your organization has been onboarded to the Adobe Business Platform, you must perform this action through the Adobe Admin Console.</p>
<p>For instructions on adding a user in the Adobe Admin Console:</p>
<ul>
<li> <p>See <a href="../../administration-and-setup/add-users/create-and-manage-users/admin-console.md#create" class="MCXref xref">Create users in Workfront with the Adobe Admin Console</a></p> </li>
<li> <p>See the section "Add users" in the article <a href="https://helpx.adobe.com/enterprise/using/manage-users-individually.html">Manage users individually</a></p> </li>
<li> <p>Contact your Adobe Admin Console Administrator.</p> </li>
</ul>
<p>For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Business Platform, see <a href="../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md" class="MCXref xref">Platform-based administration differences (Adobe Workfront/Adobe Business Platform)</a>.</p>
</div>
<p><strong>Add a user to an organization that has not been onboarded to the Adobe Business Console</strong></p>

-->

Um Benutzer zur Organisation hinzuzufügen, müssen Sie Administrator der Organisation sein, der Sie Benutzer hinzufügen möchten. Informationen zu Rollen finden Sie unter [Organisationsrollen in  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

So fügen Sie einen Benutzer zur Organisation hinzu:

1. Navigieren Sie im Menü zu **[!UICONTROL Organisationen]** und wählen Sie die Organisation aus, der Sie einen Benutzer hinzufügen möchten.
1. Öffnen Sie die Registerkarte **[!UICONTROL Benutzer]** in Ihrem Dashboard.
1. Klicken Sie auf **[!UICONTROL Einladen eines neuen Benutzers]**.und senden Sie die Einladung durch Klicken auf **[!UICONTROL Senden]**.

   >[!NOTE]
   >
   >   
   >Wenn die Schaltfläche [!UICONTROL Neuen Benutzer einladen] nicht angezeigt wird, wurde Ihr Unternehmen in den Bereich [!DNL Adobe Business Platform.] integriert
   >
   >  Anweisungen zum Hinzufügen eines Benutzers zu einer Organisation, die in den [!DNL Adobe Business Platform] integriert wurde, finden Sie unter [Hinzufügen von Benutzern zu  [!DNL Adobe Workfront Fusion] über den Abschnitt  [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md)

1. Füllen Sie das Formular aus.

   <table style="table-layout:auto">
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL E-Mail-Adresse]</td>
      <td>
        E-Mail-Adresse des Benutzers eingeben
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name]</td>
      <td>
        <p>Vollständigen Namen des Benutzers eingeben</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Rolle] </td>
      <td>Wählen Sie die Benutzerrolle aus. Eine Erläuterung der Rollen finden Sie unter <a href="/help/quicksilver/workfront-fusion/organizations/organization-roles.md">Organisations- und Teamrollen.</a></p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Teams</td>
      <td>Wählen Sie alle Teams aus, denen der Benutzer angehören soll.</td>
    </tr>
    <tr>
      <td role="rowheader">Notiz</td>
      <td>Geben Sie eine Notiz für den Benutzer ein. Dieser Hinweis wird in der Einladungs-E-Mail des Benutzers angezeigt.</td>
    </tr>
  </tbody>
</table>

Der Benutzer erhält eine Einladungs-E-Mail, in der er die Einladung annehmen kann.

## Hinzufügen eines Benutzers zu einem Team

Ihre Benutzer werden Teams zugewiesen, wenn Sie sie erstellen. Wenn ein bestehender Benutzer einem Team hinzugefügt werden muss, können Sie ihn auf der Seite &quot;Benutzer&quot;des Teams hinzufügen.

Das Hinzufügen eines Benutzers zu einem Team erfolgt über die Seite für dieses Team.

1. Wechseln Sie zu dem Team, dem Sie den Benutzer hinzufügen möchten, indem Sie im linken Bereich die Option **Organisationen** auswählen, auf die Registerkarte **Teams** auf der Organisationsseite klicken und das Team auswählen.

   Oder

   Wenn Sie sich auf der Seite für ein anderes Team befinden, klicken Sie auf das Team-Dropdown-Menü oben auf der Seite.

1. Wählen Sie auf der Seite des Teams (mit dem Teamnamen oben auf der Seite) die Registerkarte **Benutzer** aus.
1. Suchen Sie den Benutzer auf der Seite. Benutzer in Ihrer Organisation werden auf dieser Seite angezeigt, auch wenn sie nicht Mitglied des Teams sind.
1. Klicken Sie rechts neben dem Namen des Benutzers auf **Keine** und wählen Sie dann die Rolle aus, die ihm im Team zugewiesen werden soll.

Der Benutzer wird dem Team hinzugefügt.