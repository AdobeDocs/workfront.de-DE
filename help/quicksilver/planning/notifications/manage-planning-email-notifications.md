---
title: Verwalten von Adobe Workfront Planning-E-Mail-Benachrichtigungen
description: Wenn Sie oder Ihre Teams in einem Datensatzkommentar in Adobe Workfront Planning getaggt werden, erhalten Sie eine E-Mail-Benachrichtigung für dieses Tag.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 3c505b3a-cda7-4e7b-b497-28b820e9bb8f
last-update: 2026-04-01T18:23:03.000Z
git-commit-file: c04fc32836179ccbd80a7de3978493caf8ba8670
TQID: https://experienceleague.adobe.com/4MvX3EX6KfcXwk5lrq6bRU7HC6gzAI1Zgi49TMZbP7M
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 614b25d3255b27f09f2624afd8691e08cfb7ddf4
workflow-type: tm+mt
source-wordcount: 614
ht-degree: 2%

---

# Verwalten von E-Mail-Benachrichtigungen in Adobe Workfront-Planung

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Sie können E-Mail-Benachrichtigungen von Workfront Planning erhalten, wenn die folgenden Szenarien vorliegen:

* Jemand versieht Sie oder Ihre Teams in einem Datensatzkommentar mit Tags

  Informationen zum Tagging anderer Personen in einem Datensatzkommentar finden Sie unter [Verwalten von Datensatzkommentaren](/help/quicksilver/planning/records/manage-record-comments.md).
* Jemand fragt nach Ihrer Berechtigung für den Zugriff auf eine Ansicht, einen Arbeitsbereich, einen Datensatztyp oder einen Datensatz
* Jemand bestätigt, dass Ihr Zugriff für eine Ansicht, einen Arbeitsbereich, einen Datensatztyp oder einen Datensatz gewährt wurde.
* Sie senden eine Workfront Planning-Anfrage. Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* Jemand genehmigt oder lehnt eine von Ihnen gesendete Workfront Planning-Anfrage ab. Weitere Informationen finden Sie unter [Genehmigen einer Anfrage in Adobe Workfront Planning](/help/quicksilver/planning/requests/approve-request.md)
* Der Status ändert sich in eine von Ihnen gesendete Workfront Planning-Anfrage.

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
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
  
</td>
  </tr>

</tbody> 
</table>
-->


## Verwalten von E-Mail-Benachrichtigungen, wenn jemand Sie in einem Kommentar taggt

1. (Bedingt und optional) Nachdem jemand Sie oder Ihr Team in einem Kommentar zu einem Datensatz getaggt hat, wechseln Sie zu der E-Mail-Benachrichtigung, die Sie über das Tag und den Kommentar informiert. Der Absender der E-Mail ist Adobe Experience Cloud.

   ![Beispiel für E-Mail-Benachrichtigungen](assets/email-notification-example.png)

1. (Optional) Klicken Sie auf die Nachricht im Feld **Workfront** in der E-Mail.

   Die Seite mit den Datensatzdetails wird in Workfront geöffnet. Sie können Aktualisierungen am Datensatz vornehmen oder auf den Kommentar antworten.

1. (Bedingt) Klicken Sie, falls verfügbar, auf **Alle Benachrichtigungen anzeigen**. <!--check with Lilit - do non-IMS users have this button??-->
Die **Benachrichtigungen** wird in Adobe Experience Cloud geöffnet. Alle Benachrichtigungen aus allen Adobe Experience Cloud-Programmen werden angezeigt.

## Verwalten von E-Mail-Benachrichtigungen beim Anfordern und Gewähren von Berechtigungen

1. (Bedingt und optional) Nachdem Sie von einer Person um Zugriff auf ein Planning-Objekt gebeten oder ihm Berechtigungen erteilt wurden, wechseln Sie zu der E-Mail, in der Sie über die Berechtigungsanfrage informiert werden. Der Absender der E-Mail ist Adobe Experience Cloud.

1. (Optional) Klicken Sie auf die Nachricht im Feld **Workfront** in der E-Mail.

   Das Objekt, für das Sie Berechtigungen angefordert haben, wird in Workfront geöffnet.

1. (Bedingt) Klicken Sie, falls verfügbar, auf **Alle Benachrichtigungen anzeigen**.
Die **Benachrichtigungen** wird in Adobe Experience Cloud geöffnet. Alle Benachrichtigungen aus allen Adobe Experience Cloud-Programmen werden angezeigt.


Informationen zum Anfordern, Gewähren oder Ablehnen von Berechtigungen finden Sie [Anfordern von Berechtigungen für eine Ansicht oder einen Arbeitsbereich](/help/quicksilver/planning/access/request-permissions.md).

Informationen zum Verwalten Ihrer Workfront Planning-Benachrichtigungen finden Sie unter [Verwalten von Adobe Workfront Planning-Benachrichtigungseinstellungen](/help/quicksilver/planning/notifications/manage-notification-preferences.md).

## Verwalten von E-Mail-Benachrichtigungen zum Senden, Genehmigen oder Ablehnen von Workfront Planning-Anfragen

1. (Optional) Gehen Sie zu der E-Mail, die Workfront Ihnen sendet, nachdem Sie eine Anfrage gesendet haben oder nachdem eine von Ihnen gesendete Anfrage genehmigt oder abgelehnt wurde. Der Absender der E-Mail ist Adobe Workfront.

1. (Optional) Klicken Sie auf **Anfrage öffnen**. Dadurch wird die Anfrage in Workfront Planning geöffnet.

1. Klicken Sie oben rechts in der Anfrage auf die Schaltfläche **Überprüfen und genehmigen** und dann auf eine der folgenden Aktionen:

   * **Genehmigen**, um die Anfrage zu genehmigen. Wenn Sie eine Planungsanfrage genehmigen, wird ein Datensatz erstellt.
   * **Ablehnen**, um die Anfrage abzulehnen. Wenn Sie eine Anfrage in Workfront Planning ablehnen, wird kein Datensatz erstellt. Die Anfrage wird im Bereich Anfragen mit dem Status &quot;**&quot;**.

   ![Schaltfläche „Überprüfen und genehmigen“ auf Planungsanfrage](assets/review-approval-button-with-drop-down-expanded.png)

1. Klicken Sie auf **Benachrichtigungen**-Symbol ![Benachrichtigungsbereichssymbol Unified Shell](assets/notifications-area-icon-unified-shell.png) in der rechten oberen Ecke des Bildschirms, um auf die Seite **Benachrichtigungen** zuzugreifen.

   Informationen zum Verwalten Ihrer Workfront Planning-Benachrichtigungen finden Sie unter [Verwalten von Adobe Workfront Planning-Benachrichtigungseinstellungen](/help/quicksilver/planning/notifications/manage-notification-preferences.md).
