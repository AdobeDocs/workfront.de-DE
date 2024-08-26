---
title: E-Mail-Benachrichtigungen für die Adobe Workfront-Planung verwalten
description: Wenn Sie in der Adobe Workfront-Planung mit einem Kommentar versehen werden, erhalten Sie eine E-Mail-Benachrichtigung zu diesem Tag.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
source-git-commit: f8ad026582be5b4c89939af8f135151ffaabccfe
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 1%

---


# Verwalten von Adobe Workfront-Planungs-E-Mail-Benachrichtigungen

{{planning-important-intro}}

Sie können E-Mail-Benachrichtigungen von der Workfront-Planung erhalten, wenn die folgenden Szenarien vorliegen:

* Jemand markiert Sie in einem Datensatz-Kommentar
<!--
* Someone asks for your permission to access a view or a workspace
* Someone confirms your access has been granted for a view or a workspace
* Someone has denied your access for a view or a workspace. -->


>[!IMPORTANT]
>
>Ihr Unternehmen muss Adobe Unified Experience-Kunde sein, um Benachrichtigungen von der Workfront-Planung erhalten zu können.
>
>Weitere Informationen finden Sie unter [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

Weitere Informationen zum Tagging anderer Kommentare in einem Datensatzkommentar finden Sie unter [Verwalten von Datensatzkommentaren](/help/quicksilver/planning/records/manage-record-comments.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Workfront-Planung anzuzeigen.

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
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen finden Sie unter <a href="https://business.adobe.com/products/workfront/pricing.html">Preise und Verpackung für Adobe Workfront</a>. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td> 
   <td> 
<p>Die Workfront-Instanz Ihres Unternehmens muss in das Adobe Unified Experience integriert sein, damit Sie auf alle Funktionen der Workfront-Planung zugreifen können.</p> 
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
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich derjenigen, die sie nicht erstellt haben</p> </td> 
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
   <p>In order to receive notifications from Workfront Planning and manage notification preferences, your organization's instance of Workfront must be onboarded to the Adobe Unified Experience. For information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>.</p></td>
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
-->


## Verwalten von E-Mail-Benachrichtigungen <!--when someone tags you in a comment-->

1. (Bedingt) Nachdem jemand Sie in einem Kommentar zu einem Datensatz getaggt hat, gehen Sie zur E-Mail-Benachrichtigung, die Sie über das Tag und den Kommentar informiert. Der Absender der E-Mail ist Adobe Experience Cloud.

   ![](assets/email-notification-example.png)

1. Klicken Sie auf die Meldung im Feld **Workfront**.

   Die Seite mit den Datensatzdetails wird in Workfront geöffnet. Sie können den Datensatz aktualisieren oder auf den Kommentar antworten.

1. (Bedingt) Wenn verfügbar, klicken Sie auf **Alle Benachrichtigungen anzeigen**. <!--check with Lilit - do non-IMS users have this button??-->
Die Seite **Benachrichtigungen** wird in Adobe Experience Cloud geöffnet. Alle Benachrichtigungen aus allen Adobe Experience Cloud-Anwendungen werden angezeigt.

<!--
## Manage email notifications when requesting, granting, or denying permissions to a view or a workspace

For information about requesting, granting, or denying permissions to a view or a workspace, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). 
-->