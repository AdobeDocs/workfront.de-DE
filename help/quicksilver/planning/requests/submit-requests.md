---
title: Adobe Workfront-Planungsanfragen senden
description: Nachdem in Adobe Workfront Planning von einer Datensatztypseite aus ein Link zu einem Anforderungsformular für Sie freigegeben wurde, können Sie eine Anforderung hinzufügen, um Datensätze für den Datensatztyp zu erstellen, der mit dem Anforderungsformular verknüpft ist.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '2200'
ht-degree: 0%

---

# Senden von Adobe Workfront-Planungsanfragen zum Erstellen von Datensätzen

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<span class="preview">Die hervorgehobenen Informationen auf dieser Seite beziehen sich auf Funktionen, die noch nicht allgemein verfügbar sind. Sie ist nur in der Vorschau -Umgebung für alle Kunden verfügbar. Nach den monatlichen Releases in der Produktion stehen dieselben Funktionen auch in der Produktionsumgebung für Kunden zur Verfügung, die schnelle Releases aktiviert haben. </span>

<span class="preview">Informationen zu Schnellversionen finden Sie unter [Aktivieren oder Deaktivieren von Schnellversionen für Ihre Organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Nachdem ein Workspace-Manager ein Anfrageformular für einen Datensatztyp in Adobe Workfront Planning erstellt hat, können Sie das Formular zum Senden von Anfragen verwenden, die Datensätze für den mit dem Formular verknüpften Datensatztyp erstellen.

Sie können eine Workfront-Planungsanfrage aus den folgenden Bereichen senden:

* Aus dem Bereich Anfragen von Workfront.
* Von einem direkten Link zum freigegebenen Anfrageformular.
* Auf der Seite „Datensatztyp“, wenn Sie einen neuen Datensatz hinzufügen oder anfordern. Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).

In diesem Artikel wird beschrieben, wie Sie eine Anfrage zum Hinzufügen neuer Datensätze zu einem Datensatztyp über den Bereich Anfragen in Workfront oder über einen freigegebenen Link senden können.

Workfront-Benutzende und externe Benutzende können Anfragen an Planungs-Datensatztypen senden. Die Anfragen erstellen Datensätze für den Datensatztyp, der mit dem Anfrageformular verknüpft ist. <!--double check on the external users-->

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
<p>Jedes Workfront-Paket und jedes Planungspaket</p>
ODER
<p>Beliebiges Workflow-Paket und beliebiges Planungspaket</p>
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
   * Anfragebereich in Workfront

  <div class="preview">

   * Datensatztypseiten in Workfront Planning
   * Detailbereich eines Datensatzes in Workfront Planning

  </div>

  >[!TIP]
  >
  ><span class="preview">Sie können den Namen der Anfrage im Feld „Betreff“ im Bereich „Anfragen“ von Workfront oder im Feld „Ausgangsanfrageverbindung“ in Workfront Planning einsehen. </span>



* Gesendete Anfragen werden im Bereich Anfragen von Workfront angezeigt.
* Gesendete Planungsanfragen sind nur in der neuen anfordernden -Version sichtbar. In der Legacy-Anfrageerfahrung werden keine Planungsanfragen angezeigt.
Weitere Informationen finden Sie unter [Erstellen und Senden von Anfragen](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).
* Die Anzeige bestimmter Feldtypen in einem Anfrageformular oder auf der Seite mit den Anfragedetails nach dem Senden eines Formulars ist eingeschränkt.

  Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Senden einer Anfrage an Workfront Planning im Bereich „Anfragen“ von Workfront

{{step1-to-requests}}

1. Aktivieren Sie **Einstellung „Zu einem neuen Erlebnis**&quot; in der rechten oberen Ecke des Bildschirms.
Durch Aktivierung dieser Einstellung werden die Workfront Planning-Anfrageformulare im Bereich **Anfragen** von Workfront verfügbar.

   >[!TIP]
   >
   >Diese Einstellung ist nur verfügbar, wenn Ihre Workfront-Instanz in das einheitliche Adobe-Erlebnis integriert ist.
   >
   >Um Workfront-Planungsanfragen in diesem Bereich senden zu können, müssen Sie die folgenden Bedingungen erfüllen:
   >
   >* Ihr Unternehmen hat eine Workfront Planning-Lizenz erworben.
   >
   >* Sie haben Zugriff, um mindestens einen Arbeitsbereich anzuzeigen.

1. Klicken Sie in die **Welche Anfrage möchten Sie senden**, um eine Liste von Anfrageformularen zu öffnen.
1. Wählen Sie ein Anfrageformular aus der Liste aus oder geben Sie den Namen des Anfrageformulars ein und wählen Sie es aus, wenn es in der Liste angezeigt wird.

   Ein Fenster mit dem Namen des Anforderungsformulars wird oben geöffnet.
1. Aktualisieren Sie die im Anfrageformular verfügbaren Felder. Felder mit einem roten Sternchen sind Pflichtfelder.
1. Klicken Sie auf **Senden**.

   Das Anfrageformular wird geschlossen und Sie kehren zum Bereich **Anfragen** zurück.

   Ihr Formular wird übermittelt und Folgendes geschieht:

   * Wenn das Anfrageformular nicht mit einer Genehmigung verknüpft war, wird die Anfrage der Liste Anfragen im Bereich Workfront-Anfragen und im Widget Meine Anfragen auf der Startseite hinzugefügt und ein neuer Datensatz wird zu dem mit dem Formular verknüpften Datensatztyp hinzugefügt.

     In den folgenden Feldern werden Anfrage- und Datensatzinformationen im Bereich Anfragen und im Widget Meine Anfragen auf der Startseite angezeigt:

      * **Betreff**: Der Name der ursprünglichen Anfrage, wie im Bereich „Anfragen“ hinzugefügt. Sie können das Feld **Betreff** nicht aus der Anfrageliste ausblenden oder entfernen.
      * **Erstelltes Objekt**: Der Name des Datensatzes, der aus der Anforderung erstellt wurde und in Planning angezeigt wird.
      * **Objekttyp**: Der Name des Arbeitsbereichs und der Datensatztyp, in dem aufgrund der Anforderung in Planning Datensätze erstellt wurden.
      * **Status**: Der Status des Anfrageobjekts.
      * **Anfrageformular**: Der Name des Anfrageformulars, das mit dem Datensatztyp in Planning verknüpft ist.

   * Wenn das Anfrageformular mit einer Genehmigung verknüpft war, wird die Anfrage zur Anfragenliste im Bereich &quot;Workfront-Anfragen“ hinzugefügt und verfügt über das Widget „Meine Anfragen“ mit dem Status „Prüfung ausstehend“. Ein neuer Datensatz wird der Seite „Datensatztyp“ erst hinzugefügt, nachdem ihn die genehmigenden Personen genehmigt haben.

     Weitere Informationen finden Sie unter [Hinzufügen einer Genehmigung zu einem Anfrageformular](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

   * <span class="preview">In Planning können Sie das Feld „Ursprüngliche Anfrageverbindung“ zu einem Datensatztyp hinzufügen, um den Namen der ursprünglichen Anfrage anzuzeigen, die einen Datensatz erstellt hat. Weitere Informationen finden Sie unter [Verbinden von Datensatztypen](/help/quicksilver/planning/architecture/connect-record-types.md). </span>
   * Die Anfrage ist nur für den Eigentümer, die genehmigende Person und die Personen sichtbar, die zumindest über Anzeigeberechtigungen für den Arbeitsbereich verfügen. Workfront-Admins können alle Anfragen anzeigen, die an einen beliebigen Arbeitsbereich im System gesendet wurden.

   * Sie erhalten eine In-App- und eine E-Mail-Benachrichtigung, dass die Anfrage entweder erfolgreich übermittelt wurde oder zur Überprüfung gesendet wurde.
   * Wenn das Anfrageformular mit einer Genehmigung verknüpft war, erhalten die genehmigenden Personen eine In-App- und eine E-Mail-Benachrichtigung, um die Anfrage zu überprüfen und zu genehmigen.

     >[!NOTE]
     >
     >Die E-Mail- und In-App-Benachrichtigungen sind nur sichtbar, wenn die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert wird.
     >
     >In der Bestätigungs- oder Validierungsbenachrichtigung per E-Mail ist ein Link zur Anfrage vorhanden.

1. (Optional) Klicken Sie in **Bestätigungsmeldung auf** Anforderung anzeigen“, um die Anforderung zu öffnen, oder klicken Sie auf das Symbol **X**, um die Bestätigung zu schließen.
1. (Optional) Führen Sie einen der folgenden Schritte aus der Anfragenliste aus:

   * Klicken Sie **Filter** und beginnen Sie mit dem Hinzufügen von Bedingungen für die Anfragen, die Sie in der Anfragenliste anzeigen möchten.

     ![Bearbeiten von Filtern im Bereich Anfragen](assets/filters-editing-box-in-requests-planning-tab.png)

     Sie können nach den folgenden Feldern filtern:

      * **Workspace**: Der Arbeitsbereich, mit dem das Anfrageformular verknüpft ist.
      * **Datensatztyp**: Der Datensatztyp, mit dem das Anfrageformular verknüpft ist.
      * **Eingabedatum** Das Datum, an dem die Anfrage gesendet wurde.
      * **Anfrageformular**: Der Name des Anfrageformulars, das zum Senden der Anfrage verwendet wird.
      * **Status**: Der Status der Anfrage.
      * **Eingegeben von**: Der Name des Benutzers, der die Anfrage hinzugefügt hat. Wenn die Anfrage von einer Person außerhalb von Workfront hinzugefügt wurde, wird im Feld **Eingegeben von** `N/A` angezeigt.
      * **Erstellter Objektstatus**: Der Status des erstellten Datensatzes.

     Es können mehrere Filter entweder durch „Und **oder** Oder **verbunden**.
Die Anfrageliste wird automatisch gefiltert, wenn Sie die Filterbedingungen hinzufügen.

   * Klicken Sie auf **Spalten**, um das Feld **Sichtbarkeit und Reihenfolge der Felder** zu öffnen, und blenden Sie die Spalten in der Anfrageliste aus, zeigen oder neu an.

     >[!TIP]
     >
     >Es können keine weiteren Spalten hinzugefügt werden.

     ![Bearbeitungsfeld „Spalten“ im Bereich „Anfragen“](assets/columns-editing-box-in-requests-planning-tab.png)
   * Klicken Sie auf das Symbol **+** in der oberen rechten Ecke der Anfrageliste, um den **Spalten-Manager** zu öffnen und Spalten in der Anfrageliste hinzuzufügen oder zu entfernen.

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
   >* Wenn das Anfrageformular mit einer Genehmigung verknüpft ist, muss die Genehmigung erteilt werden, bevor Sie auf den Datensatz auf der Anfrageseite zugreifen können.

1. (Optional) Klicken Sie auf den Namen des **Datensatztyps**.

   Die Seite „Datensatztyp“ wird in Workfront Planning geöffnet.

## Senden einer Anfrage an Workfront Planning über einen freigegebenen Link in ein Anfrageformular

Die Informationen in diesem Abschnitt gelten nur für Workfront-Benutzer, die eine Anfrage über einen freigegebenen Link senden. Externe Personen können nicht auf interne Bereiche von Workfront zugreifen, z. B. Anfragen oder Startseite.

1. Navigieren Sie zu dem Link, der von einem Workfront Planning-Datensatztyp für Sie freigegeben wurde.

1. Aktualisieren Sie die im Formular verfügbaren Felder. Felder mit einem Sternchen sind Pflichtfelder.

   >[!TIP]
   >
   >   Wenn das Feld **Betreff** verfügbar ist, wird es nach dem Senden der Anfrage in Workfront Planning nicht angezeigt.
   >
   >Es wird empfohlen, so viele Felder wie möglich in Ihrer Anfrage zu aktualisieren, damit der neue Datensatz identifizierbar wird, wenn er zum Datensatztyp in Workfront Planning hinzugefügt wird.

1. Klicken Sie auf **Senden**.

   Ihr Formular wird übermittelt und Folgendes geschieht:

   * Wenn das Anfrageformular nicht mit einer Genehmigung verknüpft war, wird die Anfrage der Liste Anfragen im Bereich Workfront-Anfragen und im Widget Meine Anfragen auf der Startseite hinzugefügt und ein neuer Datensatz wird zu dem mit dem Formular verknüpften Datensatztyp hinzugefügt.

   * Wenn das Anfrageformular mit einer Genehmigung verknüpft war, wird die Anfrage der Liste Anfragen im Bereich Workfront-Anfragen und im Widget Meine Anfragen hinzugefügt. Ein neuer Datensatz wird der Seite „Datensatztyp“ erst hinzugefügt, nachdem alle genehmigenden Personen ihn genehmigt haben.

     Weitere Informationen finden Sie unter [Hinzufügen einer Genehmigung zu einem Anfrageformular](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

     >[!IMPORTANT]
     >
     >Sie können nur die Anfragen anzeigen, die von Ihnen oder einer anderen Person an die Arbeitsbereiche gesendet wurden, für die Sie zumindest über die Berechtigung zum Anzeigen verfügen. Workfront-Admins können alle Anfragen anzeigen, die an einen beliebigen Arbeitsbereich im System gesendet wurden. <!--ensure this is correct; asking team in slack-->

   * Sie erhalten eine In-App- und eine E-Mail-Benachrichtigung, dass die Anfrage entweder erfolgreich übermittelt wurde oder zur Überprüfung gesendet wurde.
   * Wenn das Anfrageformular mit einer Genehmigung verknüpft war, erhalten die genehmigenden Personen eine In-App- und eine E-Mail-Benachrichtigung, um die Anfrage zu überprüfen und zu genehmigen.

     >[!NOTE]
     >
     >Die E-Mail- und In-App-Benachrichtigungen sind nur sichtbar, wenn die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert wird.

   <!-- <span class="preview"> After the request was approved and the record was created, the Approved by and Approved date fields display information about the approval on the record.</span>-->

1. (Optional) Klicken Sie auf **Ihre Anfrage anzeigen**, um die Anfrage in Workfront zu öffnen.

   <!--Or-->

   <!--Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.-->

1. (Optional) Klicken Sie auf **Hauptmenü** > **Anfragen**, um Ihre Anfrage anzuzeigen, und klicken Sie dann auf den Namen der Anfrage.

   Die Seite mit den Anfragedetails wird geöffnet.

   ![Seite mit Kommentar anfordern](assets/new-request-page-with-comment.png)

1. (Optional) Geben Sie im Bereich „Kommentare“ einen Kommentar ein.
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

Anweisungen finden Sie unter [Kopieren und Senden von Anfragen](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Entwürfe und Anfragen aus vorhandenen Entwürfen erstellen

Sie können einen Entwurf einer Anfrage erstellen, dann zum Entwurf zurückkehren und ihn später als Anfrage übermitteln.

Dies ist nur in der neuen anfragenden -Version verfügbar.

Anweisungen finden Sie unter [Erstellen von Anfragen aus Entwürfen](/help/quicksilver/manage-work/requests/create-requests/create-requests-from-drafts.md).



