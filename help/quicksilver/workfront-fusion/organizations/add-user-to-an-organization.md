---
product-previous: workfront-fusion
product-area: workfront-integrations;user-management
navigation-topic: organizations
title: Hinzufügen eines Benutzers zu einer Organisation in Adobe Workfront Fusion
description: Die Dokumentation zu Adobe Workfront Fusion wurde an einen neuen Speicherort verschoben. Dieser Artikel ist veraltet, enthält jedoch einen Link zum neuen Artikel, der diese Funktion behandelt.
author: Becky
feature: Workfront Fusion
exl-id: 98248cca-98f5-4eb5-b203-67e261df33f1
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 0%

---

# Hinzufügen von Benutzenden zu einer Organisation oder einem Team in Adobe Workfront Fusion

>[!IMPORTANT]
>
>Dieser Artikel wird in naher Zukunft entfernt, da alle Organisationen in die Adobe Admin Console verschoben werden.

>[!IMPORTANT]
>
>Das auf dieser Seite beschriebene Verfahren gilt nur für Organisationen, die noch nicht in das [!DNL Adobe Admin Console] integriert wurden. Wenn Ihre Organisation in die [!DNL Adobe Admin Console] integriert wurde, müssen Sie diese Aktion über die [!DNL Adobe Admin Console] durchführen.
>
>Anweisungen zum Hinzufügen eines Benutzers, nachdem Ihr Unternehmen in das [!DNL  Adobe Admin Console] verschoben wurde, und zum einheitlichen Adobe-Erlebnis finden Sie unter [Hinzufügen von Benutzern zu [!DNL Adobe Workfront Fusion] über die [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md).
>
>Eine Liste der Verfahren, die sich je nachdem unterscheiden, ob Ihr Unternehmen Adobe Admin Console verwendet hat, finden Sie unter [Plattformbasierte Administrationsunterschiede (Adobe Workfront Fusion/Adobe Business Platform)](../../../quicksilver/workfront-fusion/fusion-in-admin-console/fusion-in-admin-console.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Funktion in diesem Artikel verwenden zu können:

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
    <td> <p>[!UICONTROL-Plan], [!UICONTROL-Arbeit]</p> </td> 
   </tr>
   <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] Lizenz**</td> 
   <td>
   <p>Aktuelle Lizenzanforderung: Keine [!DNL Workfront Fusion].</p>
   <p>Oder</p>
   <p>Legacy-Lizenzanforderung: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration], [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuelle Produktanforderung: Wenn Sie über den [!DNL Adobe Workfront] [!UICONTROL Select] oder [!UICONTROL Prime] verfügen, muss Ihr Unternehmen [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu nutzen. [!DNL Workfront Fusion] ist im [!DNL Workfront] [!UICONTROL Ultimate] enthalten.</p>
   <p>Oder</p>
   <p>Legacy-Produktanforderung: Ihr Unternehmen muss [!DNL Adobe Workfront Fusion] erwerben und [!DNL Adobe Workfront], die in diesem Artikel beschriebenen Funktionen zu verwenden.</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> 
     <p>Sie müssen ein [!DNL Workfront Fusion]-Administrator für Ihre Organisation sein.</p>
     <p>Sie müssen [!DNL Workfront Fusion] für Ihr Team sein.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren [!DNL Workfront], um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

Informationen zu [!DNL Adobe Workfront Fusion] finden Sie unter [[!DNL Adobe Workfront Fusion] Lizenzen](../../workfront-fusion/get-started/license-automation-vs-integration.md).

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
>[!NOTE]
>
>Wenn Ihr Unternehmen derzeit zur Adobe Admin Console wechselt, können Sie in Workfront keine Benutzenden verwalten (Benutzende hinzufügen oder löschen). Sie können diese Aktionen nach Abschluss der Migration in der Adobe Admin Console ausführen.

Um Benutzer zur Organisation hinzuzufügen, müssen Sie Administrator der Organisation sein, der Benutzer hinzugefügt werden sollen. Informationen zu Rollen finden Sie unter [Organisationsrollen in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/organizations/organization-roles.md).

So fügen Sie einen Benutzer zur Organisation hinzu:

1. Navigieren Sie **[!UICONTROL Menü zu]** und wählen Sie die Organisation aus, der Sie einen Benutzer hinzufügen möchten.
1. Öffnen Sie die **[!UICONTROL Benutzer]** in Ihrem Dashboard.
1. Klicken Sie **[!UICONTROL Neuen Benutzer einladen]** und senden Sie die Einladung durch Klicken auf **[!UICONTROL Senden]**.

   >[!NOTE]
   >
   >   
   >Wenn die Schaltfläche [!UICONTROL Neuen Benutzer einladen] nicht angezeigt wird, wurde Ihr Unternehmen in das [!DNL Adobe Business Platform.] integriert
   >
   >  Anweisungen zum Hinzufügen eines Benutzers zu einer Organisation, die in die [!DNL Adobe Business Platform] integriert wurde, finden Sie unter [Hinzufügen von Benutzern zu [!DNL Adobe Workfront Fusion]  über die  [!DNL Adobe Admin Console]](/help/quicksilver/workfront-fusion/fusion-in-admin-console/add-fusion-users-admin-console.md)

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
        <p>Den vollständigen Namen des Benutzers eingeben</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Role] </td>
      <td>Wählen Sie die Rolle des Benutzers aus. Erläuterungen zu Rollen finden Sie unter <a href="/help/quicksilver/workfront-fusion/organizations/organization-roles.md">Organisations- und Teamrollen.</a></p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Teams</td>
      <td>Wählen Sie alle Teams aus, denen der Benutzer als Mitglied angehören soll.</td>
    </tr>
    <tr>
      <td role="rowheader">Notiz</td>
      <td>Geben Sie eine Notiz für den Benutzer ein. Diese Anmerkung wird in der Einladungs-E-Mail des Benutzers angezeigt.</td>
    </tr>
  </tbody>
</table>

Der Benutzer erhält eine Einladungs-E-Mail, über die er die Einladung annehmen kann.

## Hinzufügen eines Benutzers zu einem Team

Ihre Benutzer werden Teams zugewiesen, wenn Sie sie erstellen. Wenn ein vorhandener Benutzer einem Team hinzugefügt werden muss, können Sie ihn auf der Seite Benutzer des Teams hinzufügen.

Das Hinzufügen eines Benutzers zu einem Team wird von der Seite aus für dieses Team vorgenommen.

1. Gehen Sie zu dem Team, dem Sie den Benutzer hinzufügen möchten, indem Sie **Organisationen** im linken Bereich auswählen, auf die Registerkarte **Teams** auf der Seite Organisation klicken und das Team auswählen.

   Oder

   Wenn Sie sich auf der Seite für ein anderes Team befinden, klicken Sie auf das Dropdown-Menü Team oben auf der Seite.

1. Wählen Sie auf der Seite „Team“ (mit dem Team-Namen oben auf der Seite) die Registerkarte **Benutzer** aus.
1. Suchen Sie den Benutzer auf der Seite. Benutzer in Ihrer Organisation werden auf dieser Seite angezeigt, auch wenn sie kein Mitglied des Teams sind.
1. Klicken Sie **rechts neben** Namen des Benutzers auf „Ohne“ und wählen Sie dann die Rolle aus, die er im Team haben soll.

Der Benutzer wird dem Team hinzugefügt.