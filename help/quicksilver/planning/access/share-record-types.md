---
title: Datensatztypen freigeben
description: Sie können einen Datensatztyp für andere freigeben, um die Zusammenarbeit bei der Verwendung von Adobe Workfront Planning sicherzustellen.
hide: true
hidefromtoc: true
exl-id: bf49db73-09f1-417e-836b-16c6062740d4
source-git-commit: 5005493bb98b63f4c463f424be43a9d422744846
workflow-type: tm+mt
source-wordcount: '1188'
ht-degree: 0%

---

<!-- add these to metadata on release:

author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog-->

# Datensatztypen freigeben

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Sie können einen Datensatztyp für andere freigeben, um die Zusammenarbeit beim Arbeiten mit Datensätzen in Adobe Workfront Planning sicherzustellen.

>[!IMPORTANT]
>
>* Durch das Gewähren von Berechtigungen für einen Arbeitsbereich erhalten Benutzerinnen und Benutzer standardmäßig dieselben Berechtigungen für die Datensatztypen im Arbeitsbereich.
>* Sie können Berechtigungen für einzelne Datensatztypen anpassen.
>* Sie können Personen keinen höheren Zugriff auf einen Datensatztyp gewähren als Personen, die Zugriff auf den Arbeitsbereich haben.
> Weitere Informationen finden Sie im Abschnitt [Überlegungen bei der Freigabe ](#considerations-when-sharing-record-types) Datensatztypen“ in diesem Artikel.

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
<p>Um auf alle Funktionen von Workfront zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p> 
<p>Das Unternehmen muss in das einheitliche Adobe-Erlebnis integriert sein, damit Benutzer Berechtigungen für eine Ansicht über eine Berechtigungsanfrage anfordern und erteilen können. </p>
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
<tr> 
   <td role="rowheader"><p>Layoutvorlage</p></td> 
   <td> <p>Allen Benutzern, einschließlich Workfront-Administratoren, muss eine Layoutvorlage zugewiesen werden, die den Bereich Planung im Hauptmenü enthält. </p> </td> 
  </tr> 
</tbody> 
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Überlegungen zur Freigabe von Datensatztypen

* Allgemeine Informationen zum Freigeben von Objekten in Workfront Planning finden Sie auch unter [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
* Sie können einen Datensatztyp intern für die folgenden Entitäten freigeben:

   * Workfront-Benutzende, -Gruppen, -Teams, -Unternehmen und -Aufgabengebiete
* Datensatztypen können nicht extern für Benutzende außerhalb von Workfront freigegeben werden.
* Automatisch erben Benutzende die Berechtigungen für den Datensatztyp vom Arbeitsbereich.
* Sie können Benutzern manuell Ansichtsberechtigungen für einen Datensatztyp erteilen oder die geerbten Berechtigungen aus dem Arbeitsbereich entfernen.

* Benutzende, die zum Freigabefeld für Datensatztypen hinzugefügt wurden und keine Arbeitsbereich-Berechtigungen haben, werden automatisch zur Arbeitsbereich-Freigabe mit Ansichtsberechtigungen hinzugefügt.

  Wenn Sie einem Benutzer, der keine Workspace-Berechtigungen hat, höhere Berechtigungen als Anzeigen für einen Datensatztyp gewähren möchten, müssen Sie den Workspace zunächst für ihn freigeben. Wenn Sie nur den Datensatztyp freigeben, können diese nur Anzeigeberechtigungen für den Datensatztyp erhalten. Außerdem werden sie zum Arbeitsbereich mit Anzeigeberechtigungen hinzugefügt. Da Sie dem Datensatztyp Berechtigungen erteilen, gibt es im Freigabefeld einen Hinweis darauf, dass er auch zum Arbeitsbereich hinzugefügt wird.

* Es können niemandem höhere Berechtigungen für den Datensatztyp erteilt werden als jemandem für einen Arbeitsbereich.

  Sie können beispielsweise niemandem die Berechtigung Anzeigen für einen Arbeitsbereich und die Berechtigung Verwalten für einen Datensatztyp erteilen.


## Freigeben von Berechtigungen für einen Datensatztyp

Sie können Berechtigungen an einzelne Datensatztypen eines Arbeitsbereichs anpassen, wenn Sie über Verwaltungsberechtigungen für den Arbeitsbereich verfügen.

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Datensatztypen Sie freigeben möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz .

   Dadurch wird die Seite „Datensatztyp“ geöffnet.

1. Klicken Sie auf der Registerkarte einer beliebigen Ansicht **Freigeben** in der oberen rechten Ecke des Datensatztyps.

   Das Feld **Freigeben** wird geöffnet.

   ![Berechtigungen für Datensatztypen mit geerbten Berechtigungen für](assets/permissions-for-record-types-with-inherited-permissions-on.png)

1. (Optional) Wählen Sie im Bereich **Wer hat Zugriff** eine der folgenden Optionen aus: <!--the Only invited people is supposed to be removed - rewrite this - according to Vahan-->

   * **Nur eingeladene Personen können zugreifen**: Sie müssen Benutzer, Gruppen, Teams, Unternehmen oder Aufgabengebiete angeben, für die Sie die Ansicht freigeben möchten.
   * **Jeder im Arbeitsbereich kann Folgendes anzeigen**: Alle Benutzer mit der Berechtigung „Anzeigen“ oder einer höheren Berechtigung für den Arbeitsbereich können auf die Ansicht zugreifen. Dies ist die Standardoption. <!--rewrite this based on what Lilit says in the proof: At this point, once the inherited permissions are disabled, everyone in the workspace except workspace managers will have View permission to the record type because the "Everyone in the workspace can view"  setting cannot be changed. -->

1. (Optional) Erweitern Sie die Option **Vererbte Berechtigungen**, um Benutzer, Teams, Gruppen, Unternehmen oder Aufgabengebiete anzuzeigen, die Berechtigungen vom Arbeitsbereich erben.

   >[!TIP]
   >
   >Sie können keine einzelnen Entitäten aus der Liste „Geerbte Berechtigungen“ entfernen.

1. (Optional und bedingt) Wenn Sie den Datensatztyp für bestimmte Entitäten freigeben und ihnen einen anderen Zugriff auf den Datensatztyp gewähren möchten, als sie bereits für den Arbeitsbereich haben, gehen Sie wie folgt vor:

   1. Deaktivieren von geerbten Berechtigungen.
   1. Fügen Sie im Feld **Zugriff auf diesen Datensatztyp gewähren** die Benutzer, Teams, Gruppen, Unternehmen oder Aufgabengebiete hinzu, denen Sie eine andere Berechtigungsstufe gewähren möchten.
   1. Berechtigungsstufe wählen.

   >[!IMPORTANT]
   >
   >* Sie können Benutzenden nie größere Berechtigungen für einen Datensatztyp erteilen als für einen Arbeitsbereich.
   >* Benutzenden mit der Berechtigung Verwalten für einen Datensatztyp kann keine geringere Berechtigung erteilt werden, wenn sie über Verwaltungsberechtigungen für den Arbeitsbereich verfügen.
   >* Sie können Benutzenden eine geringere Berechtigung für den Datensatztyp erteilen, wenn sie über die Berechtigung Beitragen für den Arbeitsbereich verfügen.
   > Weitere Informationen finden Sie unter [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

1. Um Benutzern, die keine Berechtigungen für den Arbeitsbereich haben, Zugriff zum Anzeigen des Datensatztyps zu gewähren, geben Sie im Feld **Zugriff auf diese Ansicht gewähren** zunächst den Namen eines Benutzers, einer Gruppe, eines Teams, eines Unternehmens oder eines Aufgabengebiets ein. Klicken Sie dann auf den Namen, wenn er in der Liste angezeigt wird.

   Die ausgewählte Entität wird dem Datensatztyp und dem Arbeitsbereich mit „Anzeigen **-** hinzugefügt.

   Systemadministratoren erhalten immer Verwaltungsberechtigungen für Aufzeichnungstypen, die für sie freigegeben wurden, und es gibt einen Hinweis darauf, dass ein Benutzer Systemadministrator ist.

1. Klicken Sie **Link kopieren**, um einen Link zum Datensatztyp in die Zwischenablage zu kopieren.
1. Klicken Sie auf **Speichern**.

   Der Datensatztyp wird jetzt für andere Benutzer freigegeben.

1. Geben Sie den kopierten Link für andere frei. Benutzer, die den Link erhalten, müssen aktive Benutzer sein und sich bei Workfront anmelden, um auf die Seite für den Datensatztyp zugreifen und sie in der ausgewählten Ansicht anzeigen zu können.

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

## Entfernen von Berechtigungen für einen Datensatztyp

<!-- take this section out - this is what Lilit said: Because of "Everyone in the workspace can view" wildcard, currently it's not possible to entirely remove access to a record type. Let's take out this section. -->

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Datensatztypen Sie nicht mehr freigeben möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz . Dadurch wird die Seite „Datensatztyp“ geöffnet.

1. Klicken Sie auf der Registerkarte einer beliebigen Ansicht **Freigeben** in der oberen rechten Ecke des Datensatztyps.

   Das Feld **Freigeben** wird geöffnet.
1. Suchen Sie die Person, Gruppe, Team, Firma oder Aufgabengebiet, deren Berechtigungen Sie entfernen möchten, erweitern Sie das Dropdown-Menü Berechtigungen rechts neben ihrem Namen und klicken Sie auf **Entfernen**. <!--check the screen shot below - the UI text for View might not be accurate-->

   ![Entfernen Sie die Option aus der Dropdown-Liste für die Freigabe des Datensatztyps](assets/remove-option-on-record-type-sharing-drop-down.png)

1. Klicken Sie auf **Speichern**.

   Die Benutzer haben keinen Zugriff mehr auf den Datensatztyp. Sie könnten weiterhin Berechtigungen für den Arbeitsbereich haben, es sei denn, Sie entfernen sie auch aus den Arbeitsbereich-Berechtigungen.

   Es gibt keine Benachrichtigung für die Benutzer, die vom Zugriff auf entfernt wurden, dass sie diesen Zugriff nicht mehr haben.
