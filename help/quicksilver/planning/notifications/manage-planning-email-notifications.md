---
title: Verwalten von Adobe Workfront Planning-E-Mail-Benachrichtigungen
description: Wenn Sie in Adobe Workfront Planning in einem Datensatzkommentar getaggt werden, erhalten Sie eine E-Mail-Benachrichtigung für dieses Tag.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 1%

---


# Verwalten von Adobe Workfront Planning-E-Mail-Benachrichtigungen

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Sie können E-Mail-Benachrichtigungen von Workfront Planning erhalten, wenn die folgenden Szenarien vorliegen:

* Jemand versieht Sie mit Tags in einem Datensatzkommentar

  Informationen zum Tagging anderer Personen in einem Datensatzkommentar finden Sie unter [Verwalten von Datensatzkommentaren](/help/quicksilver/planning/records/manage-record-comments.md).
* Jemand fragt nach Ihrer Berechtigung für den Zugriff auf eine Ansicht oder einen Arbeitsbereich
* Jemand bestätigt, dass Ihr Zugriff für eine Ansicht oder einen <!--Isk confirmed that there is nno email for denying access but did not test--> gewährt wurde
* Sie senden eine Workfront Planning-Anfrage. Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* Jemand genehmigt oder lehnt eine von Ihnen gesendete Workfront Planning-Anfrage ab. Weitere Informationen finden Sie unter [Genehmigen einer Anfrage in Adobe Workfront Planning](/help/quicksilver/planning/requests/approve-request.md)
* Der Status ändert sich in eine von Ihnen gesendete Workfront Planning-Anfrage.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

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
   <p>Systemadministratoren haben Berechtigungen für alle Arbeitsbereiche, einschließlich der nicht erstellten</p> </td> 
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


## Verwalten von E-Mail-Benachrichtigungen, wenn jemand Sie in einem Kommentar taggt

1. (Bedingt und optional) Nachdem Sie in einem Kommentar zu einem Datensatz getaggt wurden, wechseln Sie zu der E-Mail-Benachrichtigung, die Sie über das Tag und den Kommentar informiert. Der Absender der E-Mail ist Adobe Experience Cloud.

   ![Beispiel für E-Mail-Benachrichtigungen](assets/email-notification-example.png)

1. (Optional) Klicken Sie auf die Nachricht im Feld **Workfront** in der E-Mail.

   Die Seite mit den Datensatzdetails wird in Workfront geöffnet. Sie können Aktualisierungen am Datensatz vornehmen oder auf den Kommentar antworten.

1. (Bedingt) Klicken Sie, falls verfügbar, auf **Alle Benachrichtigungen anzeigen**. <!--check with Lilit - do non-IMS users have this button??-->
Die **Benachrichtigungen** wird in Adobe Experience Cloud geöffnet. Alle Benachrichtigungen von allen Adobe Experience Cloud-Programmen werden angezeigt.

## Verwalten von E-Mail-Benachrichtigungen beim Anfordern und Gewähren von Berechtigungen

1. (Bedingt und optional) Nachdem Sie von einer Person aufgefordert oder Ihnen Berechtigungen für den Zugriff auf eine Ansicht oder einen Arbeitsbereich erteilt wurden, wechseln Sie zu der E-Mail, in der Sie über die Berechtigungsanfrage informiert werden. Der Absender der E-Mail ist Adobe Experience Cloud.

1. (Optional) Klicken Sie auf die Nachricht im Feld **Workfront** in der E-Mail.

   Die Seite mit den Datensatzdetails wird in Workfront geöffnet. Sie können Aktualisierungen am Datensatz vornehmen oder auf den Kommentar antworten.

1. (Bedingt) Klicken Sie, falls verfügbar, auf **Alle Benachrichtigungen anzeigen**.
Die **Benachrichtigungen** wird in Adobe Experience Cloud geöffnet. Alle Benachrichtigungen von allen Adobe Experience Cloud-Programmen werden angezeigt.


Informationen zum Anfordern, Gewähren oder Verweigern von Berechtigungen für eine Ansicht oder einen Arbeitsbereich finden Sie [Berechtigungen für eine Ansicht oder einen Arbeitsbereich anfordern](/help/quicksilver/planning/access/request-permissions.md).

Informationen zum Verwalten Ihrer Workfront Planning-Benachrichtigungen finden Sie unter [Verwalten von Adobe Workfront Planning-Benachrichtigungseinstellungen](/help/quicksilver/planning/notifications/manage-notification-preferences.md).

## Verwalten von E-Mail-Benachrichtigungen zum Senden, Genehmigen oder Ablehnen von Workfront Planning-Anfragen

1. (Optional) Wechseln Sie zu der E-Mail, die Workfront Ihnen sendet
nachdem Sie eine Anforderung gesendet haben oder nachdem eine von Ihnen gesendete Anforderung genehmigt oder abgelehnt wurde. Der Absender der E-Mail ist Adobe Workfront.

1. (Optional) Klicken Sie auf **Anfrage öffnen**. Dadurch wird die Anfrage in Workfront Planning geöffnet.

1. Klicken Sie auf **Benachrichtigungen**-Symbol ![Benachrichtigungsbereichssymbol Unified Shell](assets/notifications-area-icon-unified-shell.png) in der rechten oberen Ecke des Bildschirms, um auf die Seite **Benachrichtigungen** zuzugreifen.

   Informationen zum Verwalten Ihrer Workfront Planning-Benachrichtigungen finden Sie unter [Verwalten von Adobe Workfront Planning-Benachrichtigungseinstellungen](/help/quicksilver/planning/notifications/manage-notification-preferences.md).
