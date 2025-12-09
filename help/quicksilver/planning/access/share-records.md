---
title: Freigeben von Datensätzen
description: Sie können Datensätze mithilfe der Schaltfläche Freigeben freigeben, um die Zusammenarbeit bei der Adobe Workfront-Planung zu verbessern.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: e6fc6def1553df3faa8e1200f7ec2ca2bb97eb04
workflow-type: tm+mt
source-wordcount: '1620'
ht-degree: 2%

---


<!--update metadata with real information at release-->

# Freigeben von Datensätzen

<span class="preview">Die Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


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
* Wenn Sie einen Arbeitsbereich für Benutzende freigeben, erhalten diese standardmäßig dieselben Berechtigungen für die Datensätze im Arbeitsbereich.
* Wenn Sie eine Entität aus einem Arbeitsbereich entfernen, werden alle Freigabeberechtigungen aus den Datensatztypen und allen darin enthaltenen Datensätzen entfernt.
* Der Zugriff eines Benutzers auf den Datensatz wird durch die Kombination der folgenden drei Einstellungen bestimmt:

   * Berechtigungen, die vom Datensatztyp und Arbeitsbereich übernommen wurden
   * Im Dialogfeld zur Datensatzfreigabe individuell hinzugefügte Berechtigungen
   * Die folgenden Berechtigungen:

      * **Jeder Benutzer im Arbeitsbereich kann Folgendes anzeigen**: Dadurch kann der Datensatz für alle Benutzer im Arbeitsbereich-<!-- is this OK to say "workspace? should it be "record"??--> angezeigt werden
      * **Nur eingeladene Personen können zugreifen**: Dies ist standardmäßig ausgewählt und ermöglicht die Einschränkung des Zugriffs auf den Datensatz auf bestimmte Personen.

* Sie können einem Datensatz die folgenden Berechtigungsebenen gewähren:

   * Ansicht
   * Verwalten

* Wenn Sie einen Datensatz für einen Benutzer freigeben, werden diese standardmäßig mit derselben Berechtigung hinzugefügt, die sie für den Datensatztyp haben.

  Beispiel:

   * Wenn sie über Anzeigeberechtigungen für den Datensatztyp verfügen, erhalten sie Anzeigeberechtigungen für den Datensatz
   * Wenn sie die Berechtigungen Beitragen oder Verwalten für den Datensatztyp besitzen, erhalten sie die Berechtigung Verwalten für den Datensatz

* Als Workspace-Manager können Sie einen Datensatz für Benutzende freigeben, die nicht zum Workspace gehören. In diesem Fall wird neben der hinzugefügten Entität eine Warnung angezeigt, die besagt, dass sie keinen Zugriff auf den Arbeitsbereich haben. Sie können den Benutzer weiterhin zum Datensatz hinzufügen, wodurch er auch zum Arbeitsbereich hinzugefügt wird, oder aufhören, ihn zum Datensatz hinzuzufügen, wodurch er ihn auch nicht zum Arbeitsbereich hinzufügt.

* Wenn Sie einen Datensatz für Benutzende freigeben, die über Verwaltungsberechtigungen für den Arbeitsbereich verfügen, erhalten diese standardmäßig auch Verwaltungsberechtigungen für den Datensatz. Die Berechtigung zum Anzeigen ist abgeblendet.

* Wenn Sie nicht über die Berechtigung zum Hinzufügen von Personen zum Arbeitsbereich verfügen, sehen und fügen Sie nur Benutzer, Teams, Gruppen, Rollen und Unternehmen hinzu, die bereits zum Arbeitsbereich hinzugefügt wurden. Sie können keine anderen Entitäten hinzufügen, die noch nicht Teil des Arbeitsbereichs sind.

* Sie können geerbte Berechtigungen für einen einzelnen Datensatz deaktivieren. In diesem Fall können Sie ihnen Berechtigungen für einzelne Datensätze erteilen. Alternativ können sie Berechtigungen erlangen, wenn sie zur Option **Alle im Arbeitsbereich können anzeigen** gehören. <!-- is this OK to say "workspace? should it be "record"??-->

* Wenn für denselben Benutzer mehrere Freigabeberechtigungen gelten, erhalten diese die höchste Berechtigung dieser Berechtigungen.

  Wenn beispielsweise ein Datensatz für einen Benutzer mit Ansichtsberechtigungen und dessen Gruppe mit Verwaltungszugriff freigegeben wird, erhält dieser Benutzer Verwaltungsberechtigungen für den Datensatz.

<!--Too granular??

If the inheritance has not been disabled, the user gets the maximum of inherited+individual+wildcard access 

If the inherited permissions are disabled, the user gets the maximum of wildcard+individual permissions -->

* Wenn ein Formelfeld oder ein Nachschlagefeld aus einem verbundenen Datensatz auf einem Feld für einen Datensatz basiert, für den Sie keine Berechtigungen haben, wird die richtige Berechnung angezeigt, auf welche Faktoren im Datensatz Sie sonst nicht zugreifen können.

<!-- not sure if any of the Share record types points might match here - ask Lilit??-->


## Datensatzberechtigungen freigeben

Sie können Berechtigungen für einzelne Datensätze anpassen, wenn Sie über Verwaltungsberechtigungen für den Arbeitsbereich verfügen.

{{step1-to-planning}}

1. Öffnen Sie den Arbeitsbereich, dessen Datensätze Sie freigeben möchten.
1. Klicken Sie auf den Datensatztyp, dessen Datensätze Sie freigeben möchten.

1. Führen Sie einen der folgenden Schritte aus:

   * Bewegen Sie in der Tabellenansicht den Mauszeiger über den Namen eines Datensatzes und klicken Sie auf das Menü **Mehr** ![Mehr &#x200B;](assets/more-menu.png) dann auf **Freigeben**.
   * Klicken Sie in einer beliebigen Ansicht auf den Namen eines Datensatzes und dann **Freigeben** in der oberen rechten Ecke der Detailseite des Datensatzes.

   Das Feld **Freigeben** wird geöffnet.

   ![Berechtigungen für Datensätze mit geerbten Berechtigungen für](assets/permissions-for-records-with-inherited-permissions-on.png)

1. (Optional) Im Bereich **Wer Zugriff hat** ist die Option **Jeder Benutzer im Arbeitsbereich kann** anzeigen) standardmäßig ausgewählt.  Alle Benutzenden mit Ansichts- oder höheren Berechtigungen für den Arbeitsbereich und den Datensatztyp können den Datensatz anzeigen.

1. (Optional) Klicken Sie unter der Option **Vererbte Berechtigungen** auf die Anzahl der Benutzer, um Benutzer, Teams, Gruppen, Unternehmen oder Aufgabengebiete anzuzeigen, die Berechtigungen vom Arbeitsbereich erben.

   >[!TIP]
   >
   >Sie können keine einzelnen Entitäten aus der Liste „Geerbte Berechtigungen“ entfernen.

1. (Optional und bedingt) Wenn Sie den Datensatztyp für bestimmte Entitäten freigeben und ihnen einen anderen Zugriff auf den Datensatztyp gewähren möchten, als sie bereits für den Arbeitsbereich haben, gehen Sie wie folgt vor:

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
   >* Wenn Benutzende über die Berechtigungen Beitragen oder Verwalten für den Arbeitsbereich und den Datensatztyp verfügen, behalten sie die Berechtigung Verwalten für den Datensatz bei. Die Berechtigung zum Anzeigen ist abgeblendet
   >* Sie können Benutzenden keine geringere Berechtigung für den Datensatz erteilen, wenn sie „Beitragen“ oder höher haben.
   > Weitere Informationen finden Sie unter [Übersicht über Freigabeberechtigungen in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

1. Um Benutzern, die keine Berechtigungen zum Anzeigen eines Datensatzes haben, Zugriff auf den Arbeitsbereich zu gewähren, geben Sie im Feld **Zugriff auf diese Ansicht gewähren** zunächst den Namen eines Benutzers, einer Gruppe, eines Teams, eines Unternehmens oder eines Aufgabengebiets ein. Klicken Sie dann auf den Namen, wenn er in der Liste angezeigt wird.

   Die ausgewählte Entität wird dem Datensatz und dem Arbeitsbereich mit „Anzeigen **-** hinzugefügt.

   Systemadministratoren erhalten immer Verwaltungsberechtigungen für Datensätze, die für sie freigegeben wurden, und es gibt einen Hinweis darauf, dass ein Benutzer Systemadministrator ist.

1. (Optional) Klicken Sie auf **Link kopieren**, um einen Link zum Datensatz in die Zwischenablage zu kopieren und für andere freizugeben. Durch Klicken auf diesen Link wird die Detailseite des Datensatzes geöffnet.
1. Klicken Sie auf **Speichern**.

   Der Datensatz wird jetzt für andere Benutzer freigegeben.
   <!--Checking with Lilit on this: The users you shared the record with receive both an in-app and email notification about having given permissions to the following entities:

   * The record
   * The record type, if they never had permissions before
   * The workspace, if they had not had permissions to the workspace before the record was shared with them. -->

1. Geben Sie den kopierten Link für andere frei. Benutzer, die den Link erhalten, müssen aktive Benutzer sein und sich bei Workfront anmelden, um auf die Seite für den Datensatztyp zugreifen und sie in der ausgewählten Ansicht anzeigen zu können. Sie müssen über Berechtigungen für den Datensatztyp verfügen, um ihn anzeigen zu können. Weitere Informationen finden Sie auch unter [Freigeben von Datensätzen über einen Link](/help/quicksilver/planning/records/share-records.md).

## Entfernen von Berechtigungen für einen Datensatz (**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B; DIES WURDE AUS DATENSATZTYPEN KOPIERT, MUSS FÜR DATENSÄTZE BEARBEITET WERDEN, ABER WARTEN AUF LILITS SLACK-ANTWORT &#x200B;**&#x200B;**&#x200B;**&#x200B;**&#x200B;**)

Sie können Benutzerberechtigungen aus einem Datensatz entfernen. Sie behalten jedoch mindestens Anzeigeberechtigungen für den Arbeitsbereich „Datensatz“ bei, wodurch sie auch mindestens Anzeigeberechtigungen für den Datensatztyp erhalten. Sie müssen ihren Zugriff aus dem Arbeitsbereich entfernen, wenn sie keine Berechtigungen für die Datensatztypen im Arbeitsbereich haben sollen.

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
