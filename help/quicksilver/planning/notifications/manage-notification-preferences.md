---
title: Adobe Workfront Planning-Benachrichtigungseinstellungen verwalten
description: Möglicherweise können Sie auch Ihre Benachrichtigungseinstellungen für Adobe Workfront Planning verwalten. In diesem Artikel wird beschrieben, wie Sie Ihre Benachrichtigungseinstellungen konfigurieren können.
author: Alina
feature: Workfront Planning
role: User
recommendations: noDisplay, noCatalog
exl-id: ec549a61-095c-433f-80e2-1be5c0a05180
source-git-commit: 60f2890e431065d0eb034a9254680e43a51ecab8
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 1%

---


# Adobe Workfront Planning-Benachrichtigungseinstellungen verwalten

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Sie erhalten möglicherweise In-App- oder E-Mail-Benachrichtigungen, wenn in Workfront Planning die folgenden Aktionen ausgeführt werden:

* Jemand fügt Sie zu einem Kommentar auf der Datensatzseite hinzu.
* Jemand fragt nach der Berechtigung für den Zugriff auf eine Ansicht oder einen Arbeitsbereich
* Jemand gewährt Ihnen die Berechtigung, auf eine Ansicht oder einen <!--I could not test this but Isk confirmed--> zuzugreifen
* Sie senden eine Workfront Planning-Anfrage.
* Jemand genehmigt oder lehnt eine von Ihnen gesendete Workfront Planning-Anfrage ab.
* Der Status ändert sich in eine von Ihnen gesendete Workfront Planning-Anfrage.

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
   <td><p><p>Standard, Licht oder Mitwirkende
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

Weitere Informationen zu Workfront Planning-Benachrichtigungen finden Sie in den folgenden Artikeln:

* Weitere Informationen zu Kommentaren zu Datensätzen finden Sie unter [Verwalten von Datensatzkommentaren](/help/quicksilver/planning/records/manage-record-comments.md).
* Informationen zu In-App-Benachrichtigungen von Workfront Planning finden Sie unter [Verwalten von In-App-Benachrichtigungen für Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-planning-in-app-notifications.md).
* Weitere Informationen zu E-Mail-Benachrichtigungen von Workfront Planning finden Sie unter [Verwalten von E-Mail-Benachrichtigungen für Adobe Workfront Planning](/help/quicksilver/planning/notifications/manage-planning-email-notifications.md).


## Benachrichtigungseinstellungen verwalten

1. Melden Sie sich mit Ihren Adobe Experience Cloud-Anmeldeinformationen bei Workfront an.
1. Klicken Sie auf **Kontomenü**-Symbol ![Kontomenüsymbol in Experience Cloud](assets/account-menu-icon-on-experience-cloud.png) oben rechts im Bildschirm und dann auf **Voreinstellungen**.
1. Klicken **im Abschnitt** auf **Workfront**.
1. Wählen Sie die Benachrichtigungen aus, die Sie erhalten möchten.
oder
Heben Sie die Markierung der Benachrichtigungen auf, die Sie nicht mehr erhalten möchten.

   ![Adobe Experience Cloud-Benachrichtigungsbereich für Workfront Planning](assets/adobe-experience-cloud-notifications-panel-for-workfront-planning.png)
1. Die folgenden Benachrichtigungen sind für Workfront verfügbar:

   * **Erwähnungen**: Sie erhalten eine Benachrichtigung, wenn Sie oder Ihr Team in Workfront Planning in einem Kommentar getaggt werden
   * **Anfragen**: Sie erhalten eine Benachrichtigung, wenn jemand einen der folgenden Schritte ausgeführt hat:

      * Fordert ein Workfront Planning-Objekt an oder gewährt Ihnen die Berechtigung dafür
      * Sie haben eine Workfront Planning-Anfrage gesendet
      * Der Status einer von Ihnen gesendeten Workfront-Planungsanfrage ändert sich
      * Genehmigungen für Workfront Planning-Anfragen anfordern, gewähren oder ablehnen

   Weitere Informationen zum Verwalten von Benachrichtigungen finden Sie unter [Kontoeinstellungen und Benachrichtigungen](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

<!--OLD: notifications are not available to non-IMS customers: 

When someone adds you to a comment in the record page, you may receive an in-app as well as an email notification about the comment. 

The following scenarios exist:   

* Adobe Unified Experience customers receive both an in-app notification and an email notification. They can manage their in-app and email notification preferences in the Preferences area of their Adobe Experience Cloud profile for the Workfront product. 

    For more information, see [Account preferences and notifications](https://experienceleague.adobe.com/en/docs/core-services/interface/features/account-preferences).

* Customers who are not on the Adobe Unified Experience receive only an email notification. They cannot manage their email notifications preferences and will always receive an email when someone adds them to a comment on a record in Workfront Planning.   

-->
