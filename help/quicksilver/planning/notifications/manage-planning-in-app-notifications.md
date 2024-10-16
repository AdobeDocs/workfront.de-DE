---
title: Verwalten von In-App-Benachrichtigungen zur Adobe Workfront-Planung
description: Wenn Sie von jemandem in einem Datensatz-Kommentar markiert werden, erhalten Sie eine E-Mail-Benachrichtigung für dieses Tag.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: a6eb8c7c-a34d-4c84-a45c-7e7f050a4302
source-git-commit: 9debb7c6d9df0f9f4962f3e66f146e5f605d20f0
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 1%

---


# Verwalten von Adobe Workfront-Planungs-In-App-Benachrichtigungen

{{planning-important-intro}}

Sie können In-App-Benachrichtigungen von der Workfront-Planung erhalten, wenn die folgenden Szenarien vorliegen:

* Jemand markiert Sie in einem Datensatz-Kommentar

  Weitere Informationen zum Tagging anderer Kommentare in einem Datensatzkommentar finden Sie unter [Verwalten von Datensatzkommentaren](/help/quicksilver/planning/records/manage-record-comments.md).
* Jemand bittet um Ihre Erlaubnis, auf eine Ansicht oder einen Arbeitsbereich zuzugreifen
* Jemand bestätigt, dass Ihr Zugriff für eine Ansicht oder einen Arbeitsbereich gewährt wurde <!--Isk confirmed there is no notification for denying permissions - did not test-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Workfront-Planung anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produkte</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront-Planung<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Plan*</p></td> 
   <td> 
<p>Die folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Erstklassig</li> 
<li>Ultimativ</li></ul> 
<p>Die Workfront-Planung ist für veraltete Workfront-Pläne nicht verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungsplan*</p></td> 
   <td> 
<p>Alle </p> 
<p>Weitere Informationen zu den Funktionen der einzelnen Workfront-Planungspläne erhalten Sie von Ihrem Workfront-Kundenbetreuer. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Die Workfront-Instanz Ihres Unternehmens muss in das Adobe Unified Experience integriert sein.</p> 
<p>Die Benutzer in Ihrem Unternehmen erhalten nur Benachrichtigungen von Workfront Planning, wenn Ihr Unternehmen mit dem Adobe Unified Experience integriert ist. </p>
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard, Light oder Contributor</p>
   <p>Für ältere Workfront-Lizenzen ist die Workfront-Planung nicht verfügbar.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Für die Adobe Workfront-Planung gibt es keine Zugriffssteuerungselemente</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Anzeigen oder höherer Berechtigungen für einen Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu den Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


<!--
OLD:

+++ Expand to view access requirements for Workfront Planning. 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> 
   <p>In order to receive notifications from Workfront Planning, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls in Workfront Planning. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

+++
-->

## In-App-Benachrichtigungen verwalten, wenn Sie von einem Benutzer mit einem Kommentar markiert werden

1. (Bedingt) Nachdem ein Benutzer einen Kommentar zu einem Datensatz mit einem Tags versehen hat, gehen Sie zum In-App-Symbol **Benachrichtigungen** ![](assets/experience-cloud-notifications-icon.png) in Adobe Experience Cloud.

   ![](assets/in-app-notification-example.png)

1. Klicken Sie auf die Benachrichtigung.

   Die Seite mit den Datensatzdetails wird in der Workfront-Planung geöffnet. Sie können den Datensatz aktualisieren oder auf den Kommentar antworten.

1. (Optional) Klicken Sie auf **Alle als gelesen markieren** , um anzugeben, dass Sie alle Benachrichtigungen gelesen haben.
1. (Optional) Klicken Sie auf **Alle anzeigen** , um zur Seite **Benachrichtigungen** in Adobe Experience Cloud zu wechseln.

## In-App-Benachrichtigungen beim Anfordern und Gewähren von Berechtigungen verwalten

Sie erhalten In-App-Benachrichtigungen, wenn jemand Ihnen Berechtigungen für eine Ansicht oder einen Arbeitsbereich erteilt.

Informationen zum Anfordern, Gewähren oder Ablehnen von Berechtigungen für eine Ansicht oder einen Arbeitsbereich finden Sie unter [Anfordern von Berechtigungen für eine Ansicht oder einen Arbeitsbereich](/help/quicksilver/planning/access/request-permissions.md).

Informationen zum Verwalten von Workfront-Planungs-Benachrichtigungen finden Sie unter [Voreinstellungen für Adobe Workfront-Planungs-Benachrichtigungen verwalten](/help/quicksilver/planning/notifications/manage-notification-preferences.md).