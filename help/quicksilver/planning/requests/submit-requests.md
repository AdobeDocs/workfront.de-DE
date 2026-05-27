---
title: Adobe Workfront-Planungsanfragen senden
description: Nachdem in Adobe Workfront Planning von einer Datensatztypseite aus ein Link zu einem Anforderungsformular für Sie freigegeben wurde, können Sie eine Anforderung hinzufügen, um Datensätze für den Datensatztyp zu erstellen, der mit dem Anforderungsformular verknüpft ist.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453dbf1c7598858e99d963f7a3806355a8cc80a9
workflow-type: tm+mt
source-wordcount: '2352'
ht-degree: 1%

---

# Senden von Anfragen zum Erstellen von Einträgen in Adobe Workfront-Planung

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Nachdem ein Workspace-Manager ein Anfrageformular für einen Datensatztyp in Adobe Workfront Planning erstellt hat, können Sie das Formular zum Senden von Anfragen verwenden, die Datensätze für den mit dem Formular verknüpften Datensatztyp erstellen.

Sie können eine Workfront-Planungsanfrage aus den folgenden Bereichen senden:

* Vom Bereich Anfragen in Workfront oder vom Widget Meine Anfragen auf der Startseite.
* Von einem direkten Link zum freigegebenen Anfrageformular.
* Auf der Seite „Datensatztyp“, wenn Sie einen neuen Datensatz hinzufügen, indem Sie eine Anfrage senden. Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).

In diesem Artikel wird beschrieben, wie Sie eine Anfrage zum Hinzufügen neuer Datensätze zu einem Datensatztyp über den Bereich Anfragen in Workfront oder über einen freigegebenen Link senden können.

Workspace-Manager können Anfrageformulare erstellen, mit denen Sie als Benutzer oder externe Person Anfragen an Datensatztypen in Planning senden können. Die Anfragen erstellen Datensätze für den Datensatztyp, der mit dem Anfrageformular verknüpft ist.

Informationen dazu, wie ein Workspace-Manager ein Anfrageformular erstellen und mit einem Datensatztyp verknüpfen kann, finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront-Pakete</p></td> 
   <td> 
<p>Beliebiges Workfront- oder Workflow-Paket</p>
<p>Beliebiges Workfront-Planungspaket</p>
<p>Weitere Informationen zu den einzelnen Workfront-Planungspaketen erhalten Sie von Ihrem Workfront-Kundenbetreuer.</p>
   </td> </tr>
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront-Lizenz</p></td> 
   <td><p>Beliebig</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Objektberechtigungen</p></td> 
   <td>   <p>Anzeigen oder Erweitern der Berechtigungen für einen Arbeitsbereich und einen Datensatztyp, wenn Sie Workfront-Benutzer sind</p>  </td> 
  </tr>  
</tbody> 
</table>

Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Folgendes muss vorhanden sein, bevor Sie eine Anfrage an ein Workfront Planning-Anfrageformular senden können:

* In Workfront Planning muss Folgendes vorhanden sein:

   * Ein Arbeitsbereich
   * Ein Datensatztyp
   * Ein mit einem Datensatztyp verknüpftes Anforderungsformular.

     Weitere Informationen finden Sie unter [Erstellen eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* Das Anfrageformular muss so freigegeben werden, dass Sie darauf zugreifen können. Die folgenden Szenarien sind vorhanden:

   * Intern muss das Formular für Benutzende freigegeben werden, die über die Berechtigung zum Anzeigen oder eine höhere Berechtigung für den Arbeitsbereich verfügen.

     Workfront-Benutzer können entweder über einen Link auf das Formular zugreifen oder das Anfrageformular im Bereich Anfragen von Workfront suchen.

   * Extern, indem Sie einen Link zum Datensatzformular für externe Personen freigeben, die kein Workfront-Konto haben.

     Benutzende von Workfront können auch auf den Link zugreifen, der für externe Personen freigegeben wurde.

* Bei Freigabe über einen Link darf der Link zum Formular nicht abgelaufen sein.

## Überlegungen zum Senden von Anfragen an Workfront Planning

* Eine Anfrage kann nach dem Senden nicht mehr in Workfront bearbeitet werden.
* Jede gesendete Anfrage erstellt einen Datensatz für den Datensatztyp, der mit dem von Ihnen verwendeten Formular verknüpft ist, wenn das Formular nicht mit einer Genehmigung verknüpft ist oder wenn die Genehmigung von allen genehmigenden Personen erteilt wurde.
* Durch das Übermitteln von Anfrageformularen erstellte Datensätze sind mit den Datensätzen identisch, die über eine andere Methode in Workfront Planning hinzugefügt wurden.

  Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).
* Durch das Übermitteln von Anfrageformularen erstellte Datensätze sind mit der ursprünglichen Anfrage verbunden. Diese Verbindung kann nicht entfernt werden.
* Sie können sowohl die erstellten Einträge als auch die zu ihrer Erstellung verwendeten Anfragen in den folgenden Bereichen anzeigen:
   * Bereich „Anfragen“ in Workfront.
   * In einem verbundenen Feld eines Datensatztyps in Workfront Planning, wenn Sie die Anfrage als verbundenen Datensatz hinzufügen.
   * Wenn Sie die Anfrage als verbundenen Datensatz hinzufügen, wird in Workfront Planning im Bereich „Details“ eines Datensatzes ein verknüpftes Feld angezeigt.

  >[!TIP]
  >
  >Sie können den Namen der Anfrage im Feld „Betreff“ im Bereich „Anfragen“ von Workfront oder im Feld „Ausgangsanfrageverbindung“ in Workfront Planning anzeigen.

* Gesendete Planungsanfragen sind nur in der neuen anfordernden -Version sichtbar. In der Legacy-Anfrageerfahrung werden keine Planungsanfragen angezeigt.

  Weitere Informationen finden Sie unter [Erstellen und Senden von Anfragen](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).
* Die Anzeige bestimmter Feldtypen in einem Anfrageformular oder auf der Seite mit den Anfragedetails nach dem Senden eines Formulars ist eingeschränkt.

  Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

<!--
Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.
-->


## Senden einer Anfrage an Workfront Planning im Bereich „Anfragen“ von Workfront

{{step1-to-requests}}

1. Aktivieren Sie **Einstellung**&#x200B;Neues Erlebnis verwenden“ in der rechten oberen Ecke des Bildschirms.
Durch Aktivieren dieser Einstellung werden die Workfront Planning-Anfrageformulare im Bereich **Anfragen** von Workfront verfügbar.

   >[!TIP]
   >
   >
   >Um Workfront-Planungsanfragen in diesem Bereich senden zu können, müssen Sie die folgenden Bedingungen erfüllen:
   >
   >* Ihr Unternehmen hat eine Workfront Planning-Lizenz erworben.
   >
   >* Sie haben Zugriff, um mindestens einen Arbeitsbereich anzuzeigen.

1. Klicken Sie in die **Welche Anfrage möchten Sie senden?** Leiste zum Öffnen einer Liste von Anfrageformularen.
1. Wählen Sie ein Anfrageformular aus der Liste aus oder geben Sie den Namen des Anfrageformulars ein und wählen Sie es aus, wenn es in der Liste angezeigt wird.

   Ein Fenster mit dem Namen des Anforderungsformulars wird oben geöffnet.

   >[!TIP]
   >
   >Workfront-Anfrage-Warteschlangen enthalten den Namen der Warteschlange und den Namen des Formulars in der Liste der Anfragen. In den Formularen für Planungsanfragen wird nur der Formularname in der Anfrageliste angezeigt.

1. Aktualisieren Sie das Feld **Betreff**. Dies ist der Name der Anfrage. Dies ist ein Pflichtfeld.
1. Aktualisieren Sie das Feld **Name**. Dies ist der Name des zukünftigen Datensatzes.

   >[!TIP]
   >
   >Das **Name** ist für Ihr Unternehmen eindeutig und zeigt in Ihrer Workfront-Instanz möglicherweise eine andere Bezeichnung an. Das Feld ist das primäre Feld des Datensatzes.

1. Aktualisieren Sie die verbleibenden Felder im Anfrageformular. Felder mit einem roten Sternchen sind Pflichtfelder.
1. (Bedingt) Wenn Ihr Unternehmen das Ausfüllen **Formulare** KI zulässt, können Sie Dokumente bei Bedarf hochladen. KI verwendet diese Dokumente, um das Formular auszufüllen, und Sie können die KI-Vorschläge akzeptieren oder ablehnen, bevor Sie die Anfrage senden.


   Anweisungen finden Sie unter [Verwenden von Formularausfüllen mit KI zum Ausfüllen einer Anfrage mithilfe von Eingabeaufforderungen oder Dokumenten](/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md).
1. Klicken Sie auf **Senden**.

   Das Anfrageformular wird geschlossen und Sie kehren zum Bereich **Anfragen** zurück.

   Ihr Formular wird übermittelt und Folgendes geschieht:

   * Wenn das Anfrageformular nicht mit einer Genehmigung verknüpft war, wird die Anfrage der Liste Anfragen im Bereich Workfront-Anfragen und im Widget Meine Anfragen auf der Startseite hinzugefügt und ein neuer Datensatz wird zu dem mit dem Formular verknüpften Datensatztyp hinzugefügt.

     In den folgenden Feldern werden Anfrage- und Datensatzinformationen im Bereich Anfragen und im Widget Meine Anfragen auf der Startseite angezeigt:

      * **Betreff**: Der Name der ursprünglichen Anfrage, wie im Bereich „Anfragen“ hinzugefügt. Sie können das Feld **Betreff** nicht aus der Anfrageliste ausblenden oder entfernen. Der Name enthält einen Link, der die Anfrageseite in Planning öffnet.
      * **Erstelltes Objekt**: Der Name des Datensatzes, der aus der Anforderung erstellt wurde und in Planning angezeigt wird. Der erstellte Objektname enthält einen Link, der den aus der Anfrage erstellten Datensatz öffnet.
      * **Objekttyp**: Der Name des Arbeitsbereichs und der Datensatztyp, in dem aufgrund der Anforderung in Planning Datensätze erstellt wurden.
      * **Status**: Der Status des Anfrageobjekts.
      * **Anfrageformular**: Der Name des Anfrageformulars, das mit dem Datensatztyp in Planning verknüpft ist.
      * **Erstellter Objektstatus**: Der Status des erstellten Datensatzes.

   * Wenn das Anfrageformular mit einer Genehmigung verknüpft war, wird die Anfrage zur Anfragenliste im Bereich &quot;Workfront-Anfragen“ und zum Widget „Meine Anfragen“ mit dem Status &quot;**Überprüfung** hinzugefügt. Ein neuer Datensatz wird der Seite „Datensatztyp“ erst hinzugefügt, nachdem ihn die genehmigenden Personen genehmigt haben.

     Weitere Informationen finden Sie unter [Hinzufügen einer Genehmigung zu einem Anfrageformular](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

   * Sie können das Verbindungsfeld **Ursprüngliche Anfrage** zu einem Datensatztyp in Planning hinzufügen, um den Namen der ursprünglichen Anfrage anzuzeigen, die einen Datensatz erstellt hat. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md).
   * Die Anfrage ist nur für den Eigentümer, die genehmigende Person und die Personen sichtbar, die zumindest über Anzeigeberechtigungen für den Arbeitsbereich verfügen. Workfront-Admins können alle Anfragen anzeigen, die an einen beliebigen Arbeitsbereich im System gesendet wurden.
   * Sie erhalten eine In-App- und eine E-Mail-Benachrichtigung, dass die Anfrage entweder erfolgreich übermittelt wurde oder zur Überprüfung gesendet wurde.
   * Wenn das Anfrageformular mit einer Genehmigung verknüpft war, erhalten die genehmigenden Personen eine In-App- und eine E-Mail-Benachrichtigung, um die Anfrage zu überprüfen und zu genehmigen.

     In der Bestätigungs- oder Validierungsbenachrichtigung per E-Mail ist ein Link zur Anfrage vorhanden.

1. (Optional) Klicken Sie in **Bestätigungsmeldung auf** Anforderung anzeigen“, um die Anforderung zu öffnen, oder klicken Sie auf das Symbol **X**, um die Bestätigung zu schließen.
1. (Optional) Um zu verwalten, wie die Informationen in der Anfragenliste angezeigt werden, aktualisieren Sie die folgenden Ansichtselemente für die Liste:

   * Ansicht
   * Filter
   * Spalten
   * Gruppierung
   * Zellen formatieren
   * Zeilenhöhe

   Weitere Informationen finden Sie unter [Verwenden erweiterter Listen](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

   <!-- 
   Removing this as this is covered at a higher level in the Use enhanced lists article: 
   1. (Optional) From the requests list, do any of the following:
      * Click **Filters** and start adding conditions for what requests you want to view in the Requests list. 
         ![Editing filters in the Requests area](assets/filters-editing-box-in-requests-planning-tab.png)
         You can filter by the following fields:  
         * **Workspace**: The workspace the request form is associated with.
         * **Object type**: The record type the request form is associated with.
         * **Entry date**: The date when the request was submitted.
         * **Request form**: The name of the request form used to submit the request.
         * **Status**: The status of the request.
         * **Entered by**: The name of the user who added the request. If the request was added by someone outside of Workfront, the **Entered by** field shows `N/A`.
        You can have multiple filters joined by either **And** or **Or**.
         The request list is filtered automatically, as you add the filter conditions. 
      * Click **Columns** to open the **Fields visibility and order** box, then hide, show, or rearrange the columns in the request list. 
         >[!TIP]
         >
         >You cannot add any more columns. 
         ![Columns editing box in Requests area](assets/columns-editing-box-in-requests-planning-tab.png)
      * Click the **+** icon in the upper-right corner of the request list to open the **Column manager** and add or remove columns in the requests list. 
   -->

1. Klicken Sie auf den Namen einer Anfrage in der Liste.

   Die Seite mit den Anfragedetails wird geöffnet.

   ![Seite mit Kommentar anfordern](assets/new-request-page-with-comment.png)

1. (Optional) Geben Sie einen Kommentar im Bereich **Kommentare** ein.
1. (Bedingt) Wenn das Anfrageformular nicht mit einer Genehmigung verknüpft ist oder die Anfrage genehmigt wurde, klicken Sie auf den Namen der Anfrage und dann auf den Namen des Datensatzes im Feld **Erstelltes** Objekt“.

   Die Seite des Datensatzes wird in Workfront Planning geöffnet.

   >[!TIP]
   >
   >* Wenn das Primärfeld des Datensatzes im Anfrageformular nicht aktualisiert wurde, wird der Name des Datensatzes im Datensatzfeld der Anfrage als „Nicht **&quot;**.
   >
   >* Wenn das Anfrageformular mit einer Genehmigung verknüpft ist, muss die Genehmigung erteilt werden, bevor Sie auf den Datensatz auf der Anfrageseite zugreifen können. Der Datensatz wird erst erstellt, wenn die Genehmigung erteilt wurde.

1. (Optional) Klicken Sie auf den Namen des **Datensatztyps**.

   Die Seite „Datensatztyp“ wird in Workfront Planning geöffnet.

## Senden einer Anfrage an Workfront Planning über einen freigegebenen Link in ein Anfrageformular

Die Informationen in diesem Abschnitt gelten nur für Personen, die eine Anfrage über einen freigegebenen Link senden und möglicherweise kein Workfront-Konto haben.

Externe Personen können nicht auf interne Bereiche von Workfront zugreifen, z **B. &quot;**&quot; oder **Startseite**.

1. Navigieren Sie zu dem Link, der von einem Workfront Planning-Datensatztyp für Sie freigegeben wurde.

1. Aktualisieren Sie die im Formular verfügbaren Felder. Felder mit einem Sternchen sind Pflichtfelder.

   >[!TIP]
   >
   >   Wenn das Feld **Betreff** verfügbar ist, wird es nach dem Senden der Anfrage in Workfront Planning nicht angezeigt.
   >
   >Es wird empfohlen, so viele Felder wie möglich in Ihrer Anfrage zu aktualisieren, damit der neue Datensatz identifizierbar wird, wenn er zum Datensatztyp in Workfront Planning hinzugefügt wird.

1. Klicken Sie auf **Senden**.

   Ihr Formular wird gesendet und Sie erhalten eine Bestätigung.

   Wenn das Formular mit einer Genehmigung verknüpft ist, muss es genehmigt werden, bevor ein Datensatz erstellt werden kann.

1. (Optional) Klicken Sie auf **Weitere Anfrage senden**, um über denselben freigegebenen Link eine weitere Anfrage hinzuzufügen.

   * Wenn das Anfrageformular nicht mit einer Genehmigung verknüpft war, wird die Anfrage der Liste Anfragen im Bereich Workfront-Anfragen und im Widget Meine Anfragen auf der Startseite hinzugefügt und ein neuer Datensatz wird zu dem mit dem Formular verknüpften Datensatztyp hinzugefügt. Dies ist nur verfügbar, wenn Sie sich bei Workfront anmelden.

   * Wenn das Anfrageformular mit einer Genehmigung verknüpft war, wird die Anfrage zur Anfragenliste im Bereich &quot;Workfront-Anfragen“ hinzugefügt und verfügt über das Widget „Meine Anfragen“ mit dem Status „Prüfung ausstehend“. Ein neuer Datensatz wird der Seite „Datensatztyp“ erst hinzugefügt, nachdem alle genehmigenden Personen ihn genehmigt haben. Dies ist nur verfügbar, wenn Sie sich bei Workfront anmelden.

     Weitere Informationen finden Sie unter [Hinzufügen einer Genehmigung zu einem Anfrageformular](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

     >[!IMPORTANT]
     >
     >Sie können nur die Anfragen anzeigen, die von Ihnen oder einer anderen Person an die Arbeitsbereiche gesendet wurden, für die Sie zumindest über die Berechtigung zum Anzeigen verfügen. Workfront-Admins können alle Anfragen anzeigen, die an einen beliebigen Arbeitsbereich im System gesendet wurden.

   * Sie erhalten eine In-App- und eine E-Mail-Benachrichtigung, dass die Anfrage entweder erfolgreich übermittelt wurde oder zur Überprüfung gesendet wurde.
   * Wenn das Anfrageformular mit einer Genehmigung verknüpft war, erhalten die genehmigenden Personen eine In-App- und eine E-Mail-Benachrichtigung, um die Anfrage zu überprüfen und zu genehmigen.

     Nachdem die Anfrage genehmigt und der Datensatz erstellt wurde, zeigen die Felder Genehmigt von und Genehmigt Datum Informationen zur Genehmigung des Datensatzes an.

1. (Optional) Klicken Sie auf **Ihre Anfrage anzeigen**, um die Anfrage in Workfront zu öffnen.

ODER

Klicken Sie [Weitere Anfrage senden](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request), um das Anfrageformular zu öffnen und eine neue Anfrage hinzuzufügen.

Die Seite mit den Anfragedetails wird geöffnet.

![Seite mit Kommentar anfordern](assets/new-request-page-with-comment.png)

1. (Optional) Geben Sie einen Kommentar im Bereich **Kommentare** ein.
1. (Bedingt) Wenn das Anfrageformular nicht mit einer Genehmigung verknüpft ist oder die Anfrage genehmigt wurde, klicken Sie auf den Namen der Anfrage und dann auf den Namen des Datensatzes im Feld **Erstelltes** Objekt“.

   Die Seite des Datensatzes wird in Workfront Planning geöffnet.

   >[!TIP]
   >
   >* Wenn der Datensatzname nicht zum Anfrageformular hinzugefügt wurde, wird der Name des Datensatzes im Datensatzfeld der Anfrage als „Nicht **&quot;**.
   >
   >* Wenn das Anfrageformular mit einer Genehmigung verknüpft ist, muss die Genehmigung erteilt werden, bevor Sie auf den Datensatz auf der Anfrageseite zugreifen können.

1. (Optional) Klicken Sie auf den Namen **Objekttyp**.

   Die Seite „Datensatztyp“ wird in Workfront Planning geöffnet.

## Erstellen einer Anfrage durch Kopieren einer vorhandenen Anfrage

Sie können eine Anfrage in der Anfragenliste in Workfront kopieren, dann die Details bearbeiten und als neue Anfrage senden.

Dies ist nur in der neuen anfragenden -Version verfügbar.

Das Kopieren einer bestehenden Planungsanfrage und das Senden als neue Anfrage ähnelt dem Kopieren einer bestehenden Workfront-Anfrage.

Weitere Informationen finden Sie unter [Kopieren und Senden von Anfragen](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Entwürfe und Anfragen aus vorhandenen Entwürfen erstellen

Sie können einen Entwurf einer Anfrage erstellen, dann zum Entwurf zurückkehren und ihn später als Anfrage übermitteln.

Dies ist nur in der neuen anfragenden -Version verfügbar. Das Erstellen von Entwürfen und Anfragen aus bestehenden Entwürfen in Workfront Planning ist identisch mit dem Erstellen aus Adobe Workfront.

Weitere Informationen finden Sie unter [Erstellen von Anfragen aus Entwürfen](/help/quicksilver/manage-work/requests/create-requests/create-requests-from-drafts.md).

## Entwürfe oder gesendete Anfragen löschen

Sie können gesendete Anfragen oder deren Entwürfe löschen, wenn Sie das neue Anfrageerlebnis verwenden.

Wenn Sie eine Planungsanfrage löschen, treten folgende Dinge auf:

* Die Anfrage kann nicht wiederhergestellt werden.
* Der aus der Anfrage erstellte Datensatz wird nicht gelöscht.
* Gelöschte Entwürfe können nicht wiederhergestellt werden. Es sind keine Datensätze mit Entwürfen verknüpft.

Das Löschen von Planungsanfragen ähnelt dem Löschen von Workfront-Anfragen.

Weitere Informationen finden Sie [Löschen einer gesendeten Anfrage oder eines Anfrageentwurfs](/help/quicksilver/manage-work/requests/create-requests/delete-request-draft.md).







