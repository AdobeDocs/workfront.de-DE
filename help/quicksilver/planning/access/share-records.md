---
title: Freigeben von Datensätzen
description: Sie können Datensätze mithilfe der Schaltfläche Freigeben freigeben, um die Zusammenarbeit bei der Adobe Workfront-Planung zu verbessern.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 66dd7354f3723e266b77cb2f367b09c022e8c95e
workflow-type: tm+mt
source-wordcount: '1838'
ht-degree: 2%

---


<!--update metadata with real information at release-->

# Freigeben von Datensätzen

<!--this will NOT be available in Preview ever - find a way to add this in this article that is prominent-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->


{{planning-important-intro}}

Sie können die Berechtigungen von Personen für einzelne Datensätze in einem Datensatztyp anpassen.

Sie können einen Adobe Workfront Planning-Datensatz wie folgt freigeben:

* Freigeben eines Links zum Datensatz.

  Weitere Informationen finden Sie unter [Freigeben von Datensätzen über einen Link](/help/quicksilver/planning/records/share-records.md).

* Geben Sie alle Datensätze in einem Arbeitsbereich für andere Benutzer frei, indem Sie den Arbeitsbereich und den Datensatztyp freigeben.

  Weitere Informationen finden Sie in den folgenden Artikeln:

   * [Freigeben eines Arbeitsbereichs](/help/quicksilver/planning/access/share-workspaces.md)

   * [Datensatztyp freigeben](/help/quicksilver/planning/access/share-record-types.md)

* Freigeben eines Datensatzes mithilfe der Option **Freigeben**.

  In diesem Artikel wird beschrieben, wie Sie einen Datensatz mit der Option **Freigeben** freigeben können.

>[!IMPORTANT]
>
>Benutzende mit Zugriff auf einen Arbeitsbereich erhalten automatisch mindestens die Berechtigung Anzeigen für alle Datensätze im Arbeitsbereich.
>Bei der Freigabe von Ansichten erhalten Benutzende keine Berechtigungen für Datensätze. Nur freigegebene Arbeitsbereiche können Benutzern Berechtigungen für Datensatztypen und Datensätze gewähren.
>
>Allgemeine Informationen zum Freigeben von Objekten in Workfront Planning finden Sie auch unter [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).


## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

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
ODER
<p>Beliebiges Workflow- und Planungspaket</p> 
 </tr>

<tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Beliebig</p> 
   <p><b>NOTIZ</b></p>
   <p>Nur Personen mit einer Standardlizenz können Berechtigungen zum Verwalten von Datensätzen erhalten. Alle anderen Lizenzen können nur über Anzeigeberechtigungen verfügen und die Option Verwalten ist für sie abgeblendet.</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfiguration der Zugriffsebene</p></td> 
   <td> <p>Es gibt keine Zugriffssteuerungsebenen für Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>  <p>Verwalten von Berechtigungen für einen Arbeitsbereich, einen Datensatztyp und den Datensatz</p>  
   <p><b>WICHTIG</b></p>
   <p>Nur Benutzer mit der Berechtigung Verwalten für einen Arbeitsbereich können einen Datensatz freigeben</p></td> 
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

## Überlegungen zur Freigabe von Datensätzen

<!--maybe use the Share record types as example here and touch on the same points: help/quicksilver/planning/access/share-record-types.md; in addition to using Lilit's information-->

<!--checking on the below with Lilit-->

* Sie können Datensätze für die folgenden Entitäten freigeben: Personen, Gruppen, Teams, Unternehmen oder Aufgabengebiete.
* Wenn Sie einen Datensatz freigeben, haben Benutzer überall dort, wo dieser Datensatz im System erscheint, denselben Zugriff.
* Wenn Sie die Berechtigungen auf einen Datensatz beschränken, können Benutzer diesen Datensatz und die Werte für die Suchfelder an keiner Stelle des Systems mehr anzeigen, an der dieser Datensatz hinzugefügt wird.
* Workfront überprüft Datensatzberechtigungen in Verbindungen mit bis zu fünf Datensätzen, um sicherzustellen, dass Benutzende nur die für sie freigegebenen Datensätze sehen.
* Sie können einem Datensatz die folgenden Berechtigungsebenen gewähren:

   * Ansicht
   * Verwalten
* Wenn Sie einen Arbeitsbereich und einen Datensatztyp für Benutzende freigeben, erhalten diese standardmäßig auch dieselben Berechtigungen für die Datensätze im Arbeitsbereich.
Wenn Benutzende die Berechtigung Beitragen für einen Arbeitsbereich oder Datensatztyp haben, erhalten sie Verwaltungsberechtigungen für die Datensätze dieses Datensatztyps.
* Wenn Sie eine Entität aus einem Arbeitsbereich entfernen, werden alle Freigabeberechtigungen aus den Datensatztypen und allen darin enthaltenen Datensätzen entfernt.
* Der Zugriff eines Benutzers auf den Datensatz wird durch die Kombination der folgenden drei Einstellungen bestimmt:

   * Berechtigungen, die vom Datensatztyp und Arbeitsbereich übernommen wurden
   * Im Dialogfeld zur Datensatzfreigabe individuell hinzugefügte Berechtigungen
   * Die folgenden Berechtigungen:

      * **Jeder Benutzer im Arbeitsbereich kann Folgendes anzeigen**: Dadurch kann der Datensatz für alle Benutzer im Arbeitsbereich-<!-- is this OK to say "workspace? should it be "record"??--> angezeigt werden
      * **Nur eingeladene Personen können zugreifen**: Dies ist standardmäßig ausgewählt und ermöglicht die Einschränkung des Zugriffs auf den Datensatz auf bestimmte Personen.

     >[!NOTE]
     >
     >Wenn Sie die Berechtigung **Alle im Arbeitsbereich können anzeigen** für einen Datensatztyp oder einen Datensatz gewähren, verfügen alle in der Freigabeliste der Arbeitsbereichsberechtigungen aufgeführten Personen über dieselben Berechtigungen für den Datensatztyp und den Datensatz, auch wenn die geerbten Berechtigungen deaktiviert sind.


* Wenn Sie einen Datensatz für einen Benutzer freigeben, werden diese standardmäßig mit derselben Berechtigung hinzugefügt, die sie für den Datensatztyp haben.

  Beispiel:

   * Wenn sie über Anzeigeberechtigungen für den Datensatztyp verfügen, erhalten sie Anzeigeberechtigungen für den Datensatz
   * Wenn sie die Berechtigungen Beitragen oder Verwalten für den Datensatztyp besitzen, erhalten sie die Berechtigung Verwalten für den Datensatz

* Als Workspace-Manager können Sie einen Datensatz für Benutzende freigeben, die nicht über die Berechtigungen für den Datensatztyp oder den Arbeitsbereich verfügen. In diesem Fall gibt es eine Warnung neben der hinzugefügten Entität, die darauf hinweist, dass sie keinen Zugriff auf den Arbeitsbereich oder den Datensatztyp haben. <!--ensure this is this way, because in devtest the warning only shows record type, but logged a bug to add "workspace" to the warning too--> Sie können den Benutzer weiterhin zum Datensatz hinzufügen, wodurch er auch zum Datensatztyp und Arbeitsbereich hinzugefügt wird, oder die Freigabe abbrechen.

* Wenn ein(e) Benutzende(r) über die Berechtigungen Verwalten oder Beitragen für den Arbeitsbereich und den Datensatztyp verfügt und Sie sie zu den Datensatzberechtigungen hinzufügen, sind die Anzeigeberechtigungen abgeblendet. Sie behalten dieselben Berechtigungen für den Datensatz wie für den Datensatztyp, und Sie können ihnen keine niedrigeren Berechtigungen für den Datensatz erteilen. <!--Lilit is checking on this, it is not working correctly-->

  Wenn sie über Anzeigeberechtigungen für den Arbeitsbereich oder den Datensatztyp verfügen, behalten sie die Anzeigeberechtigungen für die Datensätze bei. Sie können ihnen Berechtigungen zum Verwalten des Datensatzes erteilen, indem Sie die geerbten Berechtigungen deaktivieren und die Einstellung Nur eingeladene Personen können Zugriff haben auswählen. <!-- I think this is right, but because of the above not working, I can't test-->

<!-- not sure what this means, confusing, hiding for now: * If you don't have permissions to add people to the workspace, you will only see and add users, teams, groups, roles, and companies that are already added to the workspace. You cannot add any other entity that is not already part of the workspace.-->

* Sie können geerbte Berechtigungen für einen einzelnen Datensatz deaktivieren. In diesem Fall können Sie ihnen Berechtigungen für einzelne Datensätze erteilen. Alternativ können sie Berechtigungen erlangen, wenn sie zur Option **Alle im Arbeitsbereich können anzeigen** gehören.

* Wenn für denselben Benutzer mehrere Freigabeberechtigungen gelten, erhalten diese die höchste Berechtigung dieser Berechtigungen.

  Wenn beispielsweise ein Datensatz für einen Benutzer mit Ansichtsberechtigungen und dessen Gruppe mit Verwaltungszugriff freigegeben wird, erhält dieser Benutzer Verwaltungsberechtigungen für den Datensatz.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* Wenn ein Formelfeld oder ein Nachschlagefeld aus einem verbundenen Datensatz auf einem Feld für einen Datensatz basiert, für den Sie keine Berechtigungen haben, wird die richtige Berechnung angezeigt, auf welche Faktoren im Datensatz Sie sonst nicht zugreifen können.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## Datensatzberechtigungen freigeben

Als Workspace-Manager können Sie Berechtigungen an einzelne Datensätze anpassen.

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Datensätze Sie freigeben möchten.
1. Klicken Sie auf den Datensatztyp, dessen Datensätze Sie freigeben möchten.

1. Führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie in der Tabellenansicht den Mauszeiger über den Namen eines Datensatzes und klicken Sie auf das Menü **Mehr** ![Mehr ](assets/more-menu.png) dann auf **Freigeben**.
   * Wählen Sie in der Tabellenansicht einen Datensatz aus und klicken Sie dann unten **der Liste auf** Freigeben“ in der blauen Symbolleiste.
   * Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes und dann **Freigeben** in der oberen rechten Ecke der Detailseite des Datensatzes.

   Das Feld **Freigeben** wird geöffnet.

   ![Berechtigungen für Datensätze mit geerbten Berechtigungen für](assets/permissions-for-records-with-inherited-permissions-on.png)

1. (Optional) Im Bereich **Wer Zugriff hat** ist die Option **Jeder Benutzer im Arbeitsbereich kann** anzeigen) standardmäßig ausgewählt.  Alle Benutzer mit **Anzeigen** oder höheren Berechtigungen für den Arbeitsbereich und den Datensatztyp haben dieselben Berechtigungen für den Datensatz.

1. (Optional) Klicken Sie unter der Option **Vererbte Berechtigungen** auf die Anzahl der Benutzer, um Benutzer, Teams, Gruppen, Unternehmen oder Aufgabengebiete anzuzeigen, die Berechtigungen vom Arbeitsbereich erben.

   >[!TIP]
   >
   >Sie können keine einzelnen Entitäten aus der Liste „Geerbte Berechtigungen“ entfernen.

1. (Optional und bedingt) Wenn Sie den Datensatz für bestimmte Entitäten freigeben und ihnen einen anderen Zugriff auf den Datensatztyp gewähren möchten, als sie bereits für den Arbeitsbereich haben, gehen Sie wie folgt vor:

   1. Wählen **Deaktivieren** aus dem Dropdown **Menü „Übernommene Berechtigungen** aus.

   >[!TIP]
   >
   >Workspace-Manager verfügen weiterhin über Verwaltungsberechtigungen für den Datensatztyp und den Datensatz.

   1. (Optional) Wählen Sie **Nur eingeladene Personen können zugreifen** im Bereich **Wer hat Zugriff** aus.

   1. Fügen Sie im Feld **Zugriff auf diesen Datensatztyp gewähren** die Benutzer, Teams, Gruppen, Unternehmen oder Aufgabengebiete hinzu, denen Sie eine andere Berechtigungsstufe gewähren möchten als für den Arbeitsbereich oder den Datensatztyp.
   1. Wählen Sie eine der folgenden Berechtigungsebenen aus:

      * Ansicht
      * Verwalten

      <!--checking on the below with Lilit-->

   >[!IMPORTANT]
   >
   >* Zusätzlich zu Teams, Gruppen, Unternehmen und Aufgabengebieten können Sie nur für Benutzende freigeben, die der Adobe Admin Console hinzugefügt wurden. Benutzende, die nur Workfront unterstützen, können nicht hinzugefügt werden. Weitere Informationen finden Sie unter [Verwalten von Benutzern in der Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).
   >* Wenn Benutzende über die Berechtigungen Beitragen oder Verwalten für den Arbeitsbereich und den Datensatztyp verfügen, behalten sie die Berechtigung Verwalten für den Datensatz bei. Die Berechtigung zum Anzeigen ist abgeblendet. <!--this is not dimmed at this time, Lilit to check-->
   >* Benutzenden, die den Datensatztyp Contribute oder höher haben, können keine geringere Berechtigung für den Datensatz erteilt werden.
   > Weitere Informationen finden Sie unter [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

1. Um Benutzern, die keine Berechtigungen zum Anzeigen eines Datensatzes haben, Zugriff auf den Arbeitsbereich zu gewähren, geben Sie im Feld **Zugriff auf diese Ansicht gewähren** zunächst den Namen eines Benutzers, einer Gruppe, eines Teams, eines Unternehmens oder eines Aufgabengebiets ein. Klicken Sie dann auf den Namen, wenn er in der Liste angezeigt wird.

   Die ausgewählte Entität wird dem Datensatz hinzugefügt sowie dem Datensatztyp und dem Arbeitsbereich mit „Anzeigen **-**.

   Systemadministratoren erhalten immer Verwaltungsberechtigungen für Datensätze, die für sie freigegeben wurden, und es gibt einen Hinweis darauf, dass ein Benutzer Systemadministrator ist.

1. (Optional) Klicken Sie auf **Link kopieren**, um einen Link zum Datensatz in die Zwischenablage zu kopieren und für andere freizugeben. Durch Klicken auf diesen Link wird die Detailseite des Datensatzes geöffnet.
1. Klicken Sie auf **Speichern**.

   Der Datensatz wird jetzt für andere Benutzer freigegeben.

   Die Benutzer, für die Sie den Datensatz freigegeben haben, erhalten sowohl eine In-App- als auch eine E-Mail-Benachrichtigung darüber, dass sie den folgenden Entitäten Berechtigungen erteilt haben:

   * Der Datensatz
   * Der Datensatztyp, wenn er zuvor noch keine Berechtigungen hatte
   * den Arbeitsbereich, wenn er vor der Freigabe des Datensatzes keine Berechtigungen für den Arbeitsbereich hatte.

   Weitere Informationen finden Sie unter [Adobe Workfront-Planungsbenachrichtigungen: Artikelindex](/help/quicksilver/planning/notifications/notifications-information.md).

1. Geben Sie den kopierten Link für andere frei. Benutzer, die den Link erhalten, müssen aktive Benutzer sein und sich bei Workfront anmelden, um auf die Seite für den Datensatztyp zugreifen und sie in der ausgewählten Ansicht anzeigen zu können. Sie müssen über Berechtigungen für den Datensatztyp verfügen, um ihn anzeigen zu können. Weitere Informationen finden Sie auch unter [Freigeben von Datensätzen über einen Link](/help/quicksilver/planning/records/share-records.md).

## Entfernen von Berechtigungen für einen Datensatz

Sie können Benutzerberechtigungen aus einem Datensatz entfernen. Sie behalten jedoch mindestens die Berechtigung Anzeigen für den Arbeitsbereich bei, wodurch sie mindestens die Berechtigung Anzeigen für den Datensatztyp erhalten. Sie müssen ihren Zugriff aus dem Arbeitsbereich entfernen, wenn sie keine Berechtigungen für die Datensatztypen oder Datensätze im Arbeitsbereich haben sollen.

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Datensätze Sie nicht mehr freigeben möchten, und klicken Sie dann auf eine Karte vom Typ Datensatz. Dadurch wird die Seite „Datensatztyp“ geöffnet.
1. Führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie in der Tabellenansicht den Mauszeiger über den Namen eines Datensatzes und klicken Sie auf das Menü **Mehr** ![Mehr ](assets/more-menu.png) dann auf **Freigeben**.
   * Wählen Sie in der Tabellenansicht einen Datensatz aus und klicken Sie dann unten **der Liste auf** Freigeben“ in der blauen Symbolleiste.
   * Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes und dann **Freigeben** in der oberen rechten Ecke der Detailseite des Datensatzes.

   Das Feld **Freigeben** wird geöffnet.
1. Suchen Sie die Person, Gruppe, Team, Firma oder Aufgabengebiet, deren Berechtigungen Sie entfernen möchten, erweitern Sie das Dropdown-Menü Berechtigungen rechts neben ihrem Namen und klicken Sie auf **Entfernen**. <!--check the screen shot below - the UI text for View might not be accurate-->

   ![Berechtigungen für Eintrag entfernen](assets/remove-option-on-record-sharing-drop-down.png)

1. Klicken Sie auf **Speichern**.

   Die Personen verfügen nicht mehr über die angegebenen Berechtigungen für den Datensatz. Sie haben jedoch weiterhin Berechtigungen für den Datensatztyp und den Arbeitsbereich, es sei denn, Sie entfernen sie auch aus diesen Berechtigungen.

   Die Benutzer, die vom Zugriff auf den Datensatz entfernt wurden, erhalten keine Benachrichtigung, dass sie nicht mehr über diese Berechtigungen verfügen.
