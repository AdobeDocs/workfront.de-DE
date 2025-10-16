---
title: Datensatztypen freigeben
description: Sie können einen Datensatztyp für andere freigeben, um die Zusammenarbeit bei der Verwendung von Adobe Workfront Planning sicherzustellen.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: bf49db73-09f1-417e-836b-16c6062740d4
source-git-commit: 2fb95d37c32984e248767993c4858038d27e0590
workflow-type: tm+mt
source-wordcount: '1513'
ht-degree: 0%

---


<!-- take the Remove permissions section out, at the end - this is what Lilit said: Because of "Everyone in the workspace can view" wildcard, currently it's not possible to entirely remove access to a record type. Let's take out this section. -->

# Datensatztypen freigeben

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

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

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen. 

<!--at GA, check that the Workfront plans article linked below has Planning info-->



<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Paket</p></td> 
   <td> 
<p>Beliebiges Workfront- und Planungspaket</p> 
Oder
<p>Beliebiges Workflow- und Planungspaket</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Beliebig</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>  <p>Verwalten von Berechtigungen für einen Arbeitsbereich und einen Datensatztyp</p>  
   <p><b>WICHTIG</b></p>
   <p>Nur Benutzer mit der Berechtigung Verwalten für einen Arbeitsbereich können die Berechtigung Verwalten für einen Datensatztyp freigeben.</p></td> 
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

<!--Old:

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
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>Users must be added to the Adobe Admin Console in order to gain permissions to Workfront Planning views.</p>
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
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
   <td>  <p>Manage permissions to a record type</p>  
   <p>Only users with Manage permissions to a workspace can share Manage permissions to a record type</p></td> 
  </tr> 
 
</tbody> 
</table>-->

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

<div class="preview">

* Bei der Freigabe globaler Datensatztypen gibt es die folgenden Szenarien:

   * Sie können globale Datensatztypen über ihren ursprünglichen Arbeitsbereich freigeben.
   * Globale Datensatztypen können nicht freigegeben werden, nachdem sie einem sekundären Arbeitsbereich hinzugefügt wurden.

  Weitere Informationen finden Sie [Übersicht über Workspace-übergreifende Datensatztypen](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

</div>

## Freigeben von Berechtigungen für einen Datensatztyp

Sie können Berechtigungen an einzelne Datensatztypen eines Arbeitsbereichs anpassen, wenn Sie über Verwaltungsberechtigungen für den Arbeitsbereich verfügen.

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Datensatztypen Sie freigeben möchten.

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie auf der Karte Datensatztyp auf das Menü **Mehr** > **Freigeben**.
   * Klicken Sie auf eine Karte für den Datensatztyp, um die Seite des Datensatztyps zu öffnen, und klicken Sie dann in einer beliebigen Datensatztypansicht auf **Freigeben** > **Datensatztyp** Freigeben).

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
   >* Zusätzlich zu Teams, Gruppen, Unternehmen und Aufgabengebieten können Sie nur für Benutzende freigeben, die der Adobe Admin Console hinzugefügt wurden. Benutzende, die nur Workfront unterstützen, können nicht hinzugefügt werden. Weitere Informationen finden Sie unter [Verwalten von Benutzern in der Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
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

