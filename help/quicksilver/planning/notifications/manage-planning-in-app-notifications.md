---
title: Verwalten von Adobe Workfront Planning-In-App-Benachrichtigungen
description: Wenn Sie in einem Datensatzkommentar getaggt werden, erhalten Sie eine E-Mail-Benachrichtigung für dieses Tag.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: a6eb8c7c-a34d-4c84-a45c-7e7f050a4302
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 1%

---


# Verwalten von In-App-Benachrichtigungen in Adobe Workfront Planning

{{planning-important-intro}}

In-App-Benachrichtigungen von Workfront Planning können empfangen werden, wenn die folgenden Szenarien vorliegen:

* Jemand versieht Sie mit Tags in einem Datensatzkommentar

  Informationen zum Tagging anderer Personen in einem Datensatzkommentar finden Sie unter [Verwalten von Datensatzkommentaren](/help/quicksilver/planning/records/manage-record-comments.md).
* Jemand fragt nach Ihrer Berechtigung für den Zugriff auf eine Ansicht oder einen Arbeitsbereich
* Jemand bestätigt, dass Ihr Zugriff für eine Ansicht oder einen <!--Isk confirmed there is no notification for denying permissions - did not test--> gewährt wurde

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

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
<p>Einer der folgenden Workfront-Pläne:</p> 
<ul><li>Auswählen</li> 
<li>Erstklassig</li> 
<li>Ultimativ</li></ul> 
<p>Workfront Planning ist nicht für ältere Workfront-Pläne verfügbar</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Planungspaket*</p></td> 
   <td> 
<p>Beliebig </p> 
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen erhalten Sie von Ihrem Workfront Account Manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Die Workfront-Instanz Ihres Unternehmens muss in das einheitliche Adobe-Erlebnis integriert werden.</p> 
<p>Die Benutzenden in Ihrem Unternehmen erhalten nur dann Benachrichtigungen von Workfront Planning, wenn Ihr Unternehmen zum einheitlichen Adobe-Erlebnis hinzugefügt wird. </p>
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard, Licht oder Mitwirkende</p>
   <p>Workfront Planning ist nicht für ältere Workfront-Lizenzen verfügbar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Anzeigen oder Erweitern von Berechtigungen für einen Arbeitsbereich</a> </p>  
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout-Vorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

## Verwalten von In-App-Benachrichtigungen, wenn jemand Sie in einem Kommentar taggt

1. (Bedingt) Nachdem Sie in einem Kommentar zu einem Datensatz getaggt wurden, navigieren Sie zum In-App **Benachrichtigungssymbol** Experience Cloud![Benachrichtigungssymbol](assets/experience-cloud-notifications-icon.png) in Adobe Experience Cloud.

   ![Beispiel für In-App-Benachrichtigung](assets/in-app-notification-example.png)

1. Klicken Sie auf die Benachrichtigung.

   Die Seite mit den Datensatzdetails wird in Workfront Planning geöffnet. Sie können Aktualisierungen am Datensatz vornehmen oder auf den Kommentar antworten.

1. (Optional) Klicken Sie auf **Alle als gelesen markieren** um anzugeben, dass Sie alle Benachrichtigungen gelesen haben.
1. (Optional) Klicken Sie auf **Alle anzeigen**, um die Seite **Benachrichtigungen** in Adobe Experience Cloud aufzurufen.

## Verwalten von In-App-Benachrichtigungen beim Anfordern und Gewähren von Berechtigungen

Sie erhalten In-App-Benachrichtigungen, wenn jemand Sie um Berechtigungen für eine Ansicht oder einen Arbeitsbereich bittet oder Ihnen Berechtigungen erteilt.

Informationen zum Anfordern, Gewähren oder Verweigern von Berechtigungen für eine Ansicht oder einen Arbeitsbereich finden Sie [Berechtigungen für eine Ansicht oder einen Arbeitsbereich anfordern](/help/quicksilver/planning/access/request-permissions.md).

Informationen zum Verwalten Ihrer Workfront Planning-Benachrichtigungen finden Sie unter [Verwalten von Adobe Workfront Planning-Benachrichtigungseinstellungen](/help/quicksilver/planning/notifications/manage-notification-preferences.md).
