---
title: Datensatztypen freigeben
description: Sie können einen Datensatztyp für andere freigeben, um die Zusammenarbeit bei der Verwendung von Adobe Workfront Planning sicherzustellen.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: bf49db73-09f1-417e-836b-16c6062740d4
source-git-commit: b27b01e1efacc3fc459cec0a53b2c11cbe5e132b
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 0%

---


<!-- take the Remove permissions section out, at the end - this is what Lilit said: Because of "Everyone in the workspace can view" wildcard, currently it's not possible to entirely remove access to a record type. Let's take out this section. -->

# Datensatztypen freigeben

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Sie können einen Datensatztyp für andere freigeben, um die Zusammenarbeit beim Arbeiten mit Datensätzen in Adobe Workfront Planning sicherzustellen.

>[!IMPORTANT]
>
>Benutzende mit Zugriff auf einen Arbeitsbereich erhalten automatisch mindestens die Berechtigung Anzeigen für alle Datensatztypen im Arbeitsbereich.
>>Bei der Freigabe von Ansichten erhalten Benutzende keine Berechtigungen für Datensatztypen. Nur freigegebene Arbeitsbereiche können Benutzern Berechtigungen für Datensatztypen erteilen.
>
>* Allgemeine Informationen zum Freigeben von Objekten in Workfront Planning finden Sie auch unter [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
>* Weitere Informationen finden Sie im Abschnitt [Überlegungen bei der Freigabe ](#considerations-when-sharing-record-types) Datensatztypen“ in diesem Artikel.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen anzuzeigen.

<!--at GA, check that the Workfront plans article linked below has Planning info-->

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
<p>Um auf Workfront Planning zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Benutzende müssen zur Adobe Admin Console hinzugefügt werden, um Berechtigungen für Workfront Planning-Ansichten zu erhalten.</p>
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td> 
   <td><p> Standard</p>
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
   <td>  <p>Verwalten der Berechtigungen für einen Datensatztyp</p>  
   <p>Nur Benutzer mit der Berechtigung Verwalten für einen Arbeitsbereich können die Berechtigung Verwalten für einen Datensatztyp freigeben.</p></td> 
  </tr>

</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zur Freigabe von Datensatztypen

* Durch das Gewähren von Berechtigungen für einen Arbeitsbereich erhalten Benutzerinnen und Benutzer standardmäßig dieselben Berechtigungen für die Datensatztypen im Arbeitsbereich.

  Darüber hinaus können Sie die Berechtigungen für einzelne Datensatztypen anpassen.

  Sie können Personen jedoch keine Berechtigungen erteilen, die höher sind als die Berechtigungen, die sie für den Arbeitsbereich haben.
* Sie können Benutzern niedrigere Berechtigungen für den Datensatztyp gewähren, als sie für den Arbeitsbereich haben. Sie können beispielsweise über die Berechtigungen Beitragen zum -Arbeitsbereich und Anzeigen für einen Datensatztyp verfügen.
* Personen mit der Berechtigung Verwalten für den Arbeitsbereich behalten immer ihren Verwaltungszugriff auf alle Datensatztypen im Arbeitsbereich. Ihre Berechtigungen können für Datensatztypen nicht herabgesetzt werden, auch wenn die geerbten Berechtigungen deaktiviert sind.

* Derzeit können Sie beim Freigeben von Datensatztypen Folgendes erreichen:

   * Erteilen Sie Benutzern Anzeigeberechtigungen für einen Arbeitsbereich, wenn Sie einen Datensatztyp zum ersten Mal für sie freigeben und sie keine Berechtigungen für den Arbeitsbereich haben.

     Dadurch erhalten sie auch Ansichtsberechtigungen für alle Datensatztypen im Arbeitsbereich.

     Da Sie dem Datensatztyp Berechtigungen erteilen, gibt es im Freigabefeld einen Hinweis darauf, dass er auch zum Arbeitsbereich hinzugefügt wird.
   * Wenn Sie die geerbten Berechtigungen deaktivieren, ist der Datensatztyp nur für alle Personen im Arbeitsbereich sichtbar (mit Ausnahme von Arbeitsbereich-Managern).

     Personen mit der Berechtigung Verwalten für den Arbeitsbereich verfügen immer über die Berechtigung Verwalten für die Datensatztypen, auch wenn Sie geerbte Berechtigungen für den Datensatztyp deaktivieren.
   * Berechtigung von Benutzern für einen Datensatztyp herabsetzen. Es ist nicht möglich, die Berechtigung einer Person auf einen Datensatztyp zu erhöhen, verglichen mit dem, was diese Person im Arbeitsbereich hat.

     Wenn beispielsweise jemand die Berechtigung Beitragen für den Arbeitsbereich hat, können Sie seine Berechtigung für die Anzeige in einen bestimmten Datensatztyp ändern. Wenn er/sie jedoch über die Berechtigung Anzeigen für den Arbeitsbereich verfügt, können Sie ihm/ihr keine Beitragsberechtigung für einen Datensatztyp erteilen.

* Es ist nicht möglich, den Zugriff auf einen Datensatztyp für Personen im Arbeitsbereich zu entfernen. Jeder hat immer mindestens die Berechtigung Anzeigen für alle Datensatztypen, wenn er mindestens die Berechtigung Anzeigen für den Arbeitsbereich hat.

* Sie können einen Datensatztyp intern für die folgenden Entitäten freigeben:

  Workfront-Benutzende, -Gruppen, -Teams, -Unternehmen und -Aufgabengebiete
* Datensatztypen können nicht extern für Benutzende außerhalb von Workfront freigegeben werden.
* Wenn Sie einem Benutzer, der keine Workspace-Berechtigungen hat, höhere als die Anzeigeberechtigungen für einen Datensatztyp gewähren möchten, müssen Sie zunächst den Workspace für ihn mit einer höheren Berechtigung als „Anzeigen“ freigeben. Die höheren Berechtigungen für den Arbeitsbereich gelten dann für die Datensatztypen.

## Freigeben von Berechtigungen für einen Datensatztyp

Sie können Berechtigungen an einzelne Datensatztypen eines Arbeitsbereichs anpassen, wenn Sie über Verwaltungsberechtigungen für den Arbeitsbereich verfügen.

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Datensatztypen Sie freigeben möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz .

   Dadurch wird die Seite „Datensatztyp“ geöffnet.

1. Klicken Sie auf der Registerkarte einer beliebigen Ansicht **Freigeben** in der oberen rechten Ecke des Datensatztyps.
1. Klicken Sie **Datensatztyp freigeben**.

   Das Feld **Freigeben** wird geöffnet.

   ![Berechtigungen für Datensatztypen mit geerbten Berechtigungen für](assets/permissions-for-record-types-with-inherited-permissions-on.png)

1. (Optional) Im Bereich **Wer Zugriff hat** ist die Option **Jeder Benutzer im Arbeitsbereich kann** anzeigen) standardmäßig ausgewählt.  Alle Benutzenden mit Ansichts- oder höheren Berechtigungen für den Arbeitsbereich können den Datensatztyp anzeigen.

1. (Optional) Klicken Sie unter der Option **Vererbte Berechtigungen** auf die Anzahl der Benutzer, um Benutzer, Teams, Gruppen, Unternehmen oder Aufgabengebiete anzuzeigen, die Berechtigungen vom Arbeitsbereich erben.

   >[!TIP]
   >
   >Sie können keine einzelnen Entitäten aus der Liste „Geerbte Berechtigungen“ entfernen.


1. (Optional und bedingt) Wenn Sie den Datensatztyp für bestimmte Entitäten freigeben und ihnen einen anderen Zugriff auf den Datensatztyp gewähren möchten, als sie bereits für den Arbeitsbereich haben, gehen Sie wie folgt vor:

   1. Wählen **Deaktivieren** aus dem Dropdown **Menü „Übernommene Berechtigungen** aus.

   >[!TIP]
   >
   >Workspace-Manager verfügen weiterhin über Verwaltungsberechtigungen für den Datensatztyp.

   1. Fügen Sie im Feld **Zugriff auf diesen Datensatztyp gewähren** die Benutzer, Teams, Gruppen, Unternehmen oder Aufgabengebiete hinzu, denen Sie eine andere Berechtigungsstufe gewähren möchten als für den Arbeitsbereich.
   1. Berechtigungsstufe wählen.

   >[!IMPORTANT]
   >
   >* Zusätzlich zu Teams, Gruppen, Unternehmen und Aufgabengebieten können Sie nur für Benutzende freigeben, die der Adobe Admin Console hinzugefügt wurden.
   >* Sie können Benutzenden nie größere Berechtigungen für einen Datensatztyp erteilen als für einen Arbeitsbereich.
   >* Sie können Benutzenden keine geringere Berechtigung als „Verwalten“ für einen Datensatztyp erteilen, wenn sie über Verwaltungsberechtigungen für den Arbeitsbereich verfügen.
   >* Sie können Benutzenden eine geringere Berechtigung für den Datensatztyp erteilen, wenn sie über die Berechtigung Beitragen für den Arbeitsbereich verfügen.
   > Weitere Informationen finden Sie unter [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

1. Wenn Sie Benutzenden, die keine Berechtigung zum Anzeigen eines Datensatztyps haben, Zugriff auf den Arbeitsbereich gewähren möchten, geben Sie im Feld **Zugriff auf diese Ansicht gewähren** zunächst den Namen eines Benutzers, einer Gruppe, eines Teams, eines Unternehmens oder eines Aufgabengebiets ein. Klicken Sie dann auf den Namen, wenn er in der Liste angezeigt wird.

   Die ausgewählte Entität wird dem Datensatztyp und dem Arbeitsbereich mit „Anzeigen **-** hinzugefügt.

   Systemadministratoren erhalten immer Verwaltungsberechtigungen für Aufzeichnungstypen, die für sie freigegeben wurden, und es gibt einen Hinweis darauf, dass ein Benutzer Systemadministrator ist.

1. (Optional) Klicken Sie auf **Link kopieren**, um einen Link zum Datensatztyp in die Zwischenablage zu kopieren und für andere freizugeben.
1. Klicken Sie auf **Speichern**.

   Der Datensatztyp wird jetzt für andere Benutzer freigegeben.
Die Benutzer, für die Sie den Datensatztyp freigegeben haben, erhalten sowohl eine In-App- als auch eine E-Mail-Benachrichtigung über Berechtigungen für die folgenden Entitäten:

   * Der Datensatztyp
   * den Arbeitsbereich, wenn sie keine Berechtigungen für den Arbeitsbereich hatten, bevor der Datensatztyp für sie freigegeben wurde.

1. Geben Sie den kopierten Link für andere frei. Benutzer, die den Link erhalten, müssen aktive Benutzer sein und sich bei Workfront anmelden, um auf die Seite für den Datensatztyp zugreifen und sie in der ausgewählten Ansicht anzeigen zu können. Sie müssen über Berechtigungen für den Datensatztyp verfügen, um ihn anzeigen zu können.

## Entfernen von Berechtigungen für einen Datensatztyp

Sie können Benutzerberechtigungen von einem Datensatztyp entfernen. Sie behalten jedoch mindestens die Berechtigung Anzeigen für den Arbeitsbereich bei, wodurch sie mindestens die Berechtigung Anzeigen für den Datensatztyp erhalten. Sie müssen ihren Zugriff aus dem Arbeitsbereich entfernen, wenn sie keine Berechtigungen für die Datensatztypen im Arbeitsbereich haben sollen.

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Datensatztypen Sie nicht mehr freigeben möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz . Dadurch wird die Seite „Datensatztyp“ geöffnet.

1. Klicken Sie auf der Registerkarte einer beliebigen Ansicht **Freigeben** in der oberen rechten Ecke des Datensatztyps.
1. Klicken Sie **Datensatztyp freigeben**.

   Das Feld **Freigeben** wird geöffnet.
1. Suchen Sie die Person, Gruppe, Team, Firma oder Aufgabengebiet, deren Berechtigungen Sie entfernen möchten, erweitern Sie das Dropdown-Menü Berechtigungen rechts neben ihrem Namen und klicken Sie auf **Entfernen**. <!--check the screen shot below - the UI text for View might not be accurate-->

   ![Entfernen Sie die Option aus der Dropdown-Liste für die Freigabe des Datensatztyps](assets/remove-option-on-record-type-sharing-drop-down.png)

1. Klicken Sie auf **Speichern**.

   Die Personen verfügen nicht mehr über die angegebenen Berechtigungen für den Datensatztyp. Sie haben jedoch weiterhin Berechtigungen für den Arbeitsbereich, es sei denn, Sie entfernen sie auch aus den Arbeitsbereich-Berechtigungen.

   Es gibt keine Benachrichtigung für die Benutzer, die vom Zugriff auf entfernt wurden, dass sie diesen Zugriff nicht mehr haben.

<!-- This is not working yet: *************************** edit this before publishing, because this was not tested with record types - this section came from sharing views *******************: 

## Grant permissions to a record type from a permission request

Users who access a link to a record type to which they do not have permissions can request permissions to the record type. All users with Manage permissions to the view receive the permission request and can grant or deny the permissions. 

1. (Conditional) If you are are the manager of a view, you might receive a request from another user to access the view in the following areas:
   
   * An in-app notification
      ![In-app notification for access request for view](assets/in-app-notification-for-access-request-for-view.png)
   * An email notification
      ![In-app notification for access request for view](assets/in-app-notification-for-access-request-for-view.png)
1. (Conditional) From the notification area in Workfront, click the in-app notification
   Or
   From the email notification, click **View all notifications**, then click the notification in the list.

   The **Pending access requests** box displays. 

      ![Notifications list approval box](assets/notifications-list-approval-box.png)
1. (Optional) For the user whose permissions you want to approve, select one of the following options from the drop-down menu to the right of the user's name: 
   * **View**
   * **Manage**
1. Select the user for whom you want to approve or deny the permission, then click **Approve all** or **Deny all**. 
1. Click the left-pointing arrow to the left of **Pending access requests**, then click **Save**.

   If you approved the request, the users are added to the sharing box of the view. The user requesting the permission receives an email confirmation that their request was approved. <!--will they also get an in-app notification??-->

