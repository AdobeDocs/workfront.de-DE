---
title: Verwalten von Adobe Workfront Planning-In-App-Benachrichtigungen
description: Wenn Sie oder Ihre Teams in einem Datensatzkommentar getaggt werden, erhalten Sie eine E-Mail-Benachrichtigung für dieses Tag.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: a6eb8c7c-a34d-4c84-a45c-7e7f050a4302
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---


# Verwalten von In-App-Benachrichtigungen in Adobe Workfront Planning

{{planning-important-intro}}

In-App-Benachrichtigungen von Workfront Planning können empfangen werden, wenn die folgenden Szenarien vorliegen:

* Jemand versieht Sie oder Ihre Teams in einem Datensatzkommentar mit Tags

  Informationen zum Tagging anderer Personen in einem Datensatzkommentar finden Sie unter [Verwalten von Datensatzkommentaren](/help/quicksilver/planning/records/manage-record-comments.md).
* Jemand fragt nach Ihrer Berechtigung für den Zugriff auf eine Ansicht oder einen Arbeitsbereich
* Jemand bestätigt, dass Ihr Zugriff für eine Ansicht oder einen <!--Isk confirmed there is no notification for denying permissions - did not test--> gewährt wurde

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktion in diesem Artikel anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<p>Beliebiges Workfront und beliebiges Planungspaket</p> <p>Beliebiger Workflow und beliebiges Planungspaket</p>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Licht oder höher</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Anzeigen oder Erweitern von Berechtigungen für einen Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> Benutzenden mit einer Light- oder Contributor-Lizenz muss eine Layout-Vorlage zugewiesen werden, die Planning enthält.
   <p>Für Standardbenutzer und Systemadministratoren sind die Planungsbereiche standardmäßig aktiviert.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


<!--
OLD:

+++ Expand to view access requirements. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience.</p> 
<p>The users in your organization receive notifications from Workfront Planning only when your organization is onboarded to the Adobe Unified Experience. </p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard, Light, or Contributor</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table> 

+++
-->

## Verwalten von In-App-Benachrichtigungen, wenn jemand Sie in einem Kommentar taggt

1. (Bedingt) Nachdem Sie oder Ihre Teams in einem Kommentar zu einem Datensatz getaggt wurden, navigieren Sie zum In-App-Symbol **Benachrichtigungen** (Symbol ![Experience Cloud-Benachrichtigungen](assets/experience-cloud-notifications-icon.png) in Adobe Experience Cloud.

   ![Beispiel für In-App-Benachrichtigung](assets/in-app-notification-example.png)

1. Klicken Sie auf die Benachrichtigung.

   Die Seite mit den Datensatzdetails wird in Workfront Planning geöffnet. Sie können Aktualisierungen am Datensatz vornehmen oder auf den Kommentar antworten.

1. (Optional) Klicken Sie auf **Alle als gelesen markieren** um anzugeben, dass Sie alle Benachrichtigungen gelesen haben.
1. (Optional) Klicken Sie auf **Alle anzeigen**, um die Seite **Benachrichtigungen** in Adobe Experience Cloud aufzurufen.

## Verwalten von In-App-Benachrichtigungen beim Anfordern und Gewähren von Berechtigungen

Sie erhalten In-App-Benachrichtigungen, wenn jemand Sie um Berechtigungen für eine Ansicht oder einen Arbeitsbereich bittet oder Ihnen Berechtigungen erteilt.

Informationen zum Anfordern, Gewähren oder Verweigern von Berechtigungen für eine Ansicht oder einen Arbeitsbereich finden Sie [Berechtigungen für eine Ansicht oder einen Arbeitsbereich anfordern](/help/quicksilver/planning/access/request-permissions.md).

Informationen zum Verwalten Ihrer Workfront Planning-Benachrichtigungen finden Sie unter [Verwalten von Adobe Workfront Planning-Benachrichtigungseinstellungen](/help/quicksilver/planning/notifications/manage-notification-preferences.md).
