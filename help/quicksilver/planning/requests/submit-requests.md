---
title: Adobe Workfront-Planungsanfragen senden
description: Nachdem in Adobe Workfront Planning von einer Datensatztypseite aus ein Link zu einem Anforderungsformular für Sie freigegeben wurde, können Sie eine Anforderung hinzufügen, um Datensätze für den Datensatztyp zu erstellen, der mit dem Anforderungsformular verknüpft ist.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: f171db8474df703fddbf63a673f9bfbd2ab2db27
workflow-type: tm+mt
source-wordcount: '1875'
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

  In diesem Artikel wird beschrieben, wie Sie eine Anfrage zum Hinzufügen neuer Datensätze zu einem Datensatztyp über den Bereich Anfragen in Workfront oder über einen freigegebenen Link senden können.
* Auf der Seite „Datensatztyp“, wenn Sie einen neuen Datensatz hinzufügen oder anfordern. Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).

Workfront-Benutzende und externe Benutzende können Anfragen an Planning-Datensatztypen senden und Datensätze erstellen. <!--double check on the external users-->

Informationen dazu, wie ein Workspace-Manager ein Anfrageformular erstellen und mit einem Datensatztyp verknüpfen kann, finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
<p>Weitere Informationen zu den einzelnen Workfront-Planungsplänen erhalten Sie von Ihrem Workfront Account Manager. </td>
<tr>
   <td role="rowheader"><p>Adobe Workfront-Plattform</p></td>
   <td>
<p>Um auf alle Funktionen von Workfront zugreifen zu können, muss die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert sein.</p>
<p>Weitere Informationen finden Sie unter <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront-Lizenz*</p></td>
   <td>
   <p>Externe, Mitwirkende, Light- oder Standardlizenz</p>
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
   <td>
   <p>Zeigen Sie Berechtigungen oder höhere Berechtigungen für einen Arbeitsbereich (<span class="preview"> Datensatztyp) an</span> wenn Sie ein Workfront-Benutzer sind</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout-Vorlage</p></td>
   <td> <p>Für den Zugriff auf den Planungsbereich in Workfront muss Ihnen eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p>
   <p> Der Zugriff auf den Bereich Planung ist jedoch nicht erforderlich, um Anfragen an Workfront Planning zu senden. </p>  
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--replace the layout template info in the table with this at release: 

<div class="preview">
<p> Users with a Light or Contributor license must be assigned a layout template that includes the Planning option  in the following areas:</p>
   <ul><li>Main Menu</li>
   <li>Left panel of projects, portfolios, and programs</li>
   <li>Landing page</li>
   <li>Pins</li></ul>
   <p>For more information, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md">Create and manage layout templates</a>.</p>
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div>
   <p><b>NOTE</b></p>
   <p>In the Production environment, all users including the System administrators must be assigned to a layout template that includes the Planning areas.</p>

-->

## Voraussetzungen

Folgendes muss vorhanden sein, bevor Sie eine Anfrage an ein Workfront Planning-Anfrageformular senden können:

* In Workfront Planning muss Folgendes vorhanden sein:

   * Ein Arbeitsbereich
   * Ein Datensatztyp.
   * Ein mit einem Datensatztyp verknüpftes Anforderungsformular.

     Weitere Informationen finden Sie unter [Erstellen eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* Das Anfrageformular muss so freigegeben werden, dass Sie darauf zugreifen können. Die folgenden Szenarien sind vorhanden:

   * Intern muss das Formular für Benutzende freigegeben werden, die über die Berechtigung zum Anzeigen oder eine höhere Berechtigung für den Arbeitsbereich verfügen.

     Workfront-Benutzer können entweder über einen Link auf das Formular zugreifen oder das Anfrageformular im Bereich Anfragen von Workfront suchen.

   * Wenn Sie kein Workfront-Konto haben, wurde ein Link zum Formular für externe Personen freigegeben.

     Benutzende von Workfront können auch auf einen Link zugreifen, der für externe Personen freigegeben ist.

* Der Link zum Formular darf nicht abgelaufen sein.

## Überlegungen zum Senden von Anfragen an Workfront Planning

* Eine Anfrage kann nach dem Senden nicht mehr in Workfront bearbeitet werden.
* Jede gesendete Anfrage erstellt einen Datensatz für den Datensatztyp, der mit dem von Ihnen verwendeten Formular verknüpft ist, wenn das Formular nicht mit einer Genehmigung verknüpft ist oder wenn die Genehmigung von allen genehmigenden Personen erteilt wurde.
* Datensätze, die durch das Übermitteln von Anfrageformularen erstellt wurden, können nicht von Datensätzen unterschieden werden, die über eine andere Methode in Workfront Planning hinzugefügt wurden.

  Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).
* Gesendete Anfragen werden in Workfront im Bereich Anfragen auf der Registerkarte Planung des Abschnitts Gesendet angezeigt.
* Die Anzeige bestimmter Feldtypen in einem Anfrageformular oder auf der Seite mit den Anfragedetails nach dem Senden eines Formulars ist eingeschränkt.

  Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Senden einer Anfrage an Workfront Planning im Bereich „Anfragen“ von Workfront

{{step1-to-requests}}

1. Aktivieren Sie **Einstellung „Zu einem neuen Erlebnis**&quot; in der rechten oberen Ecke des Bildschirms.
Durch Aktivierung dieser Einstellung werden die Workfront Planning-Anfrageformulare im Bereich **Anfragen** von Workfront verfügbar.

   >[!TIP]
   >
   >Diese Einstellung ist nur verfügbar, wenn Folgendes zutrifft:
   >
   >* Ihr Unternehmen hat ein Workfront Planning-Paket erworben.
   >* Ihre Workfront-Instanz wird in das einheitliche Adobe-Erlebnis integriert.
   >* Sie haben Zugriff, um mindestens einen Arbeitsbereich anzuzeigen.
   >

1. Klicken Sie auf **Neue Anfrage**.

   ![Neues Anfragefeld mit einheitlichen Workfront- und Planungskarten](assets/new-request-box-with-unified-workfront-and-planning-cards.png)

   Das **Neue Anfrage** wird mit den folgenden Informationen geöffnet:

   * Die 6 zuletzt aufgerufenen Workfront-Anfragewarteschlangen und Planungsanfrageformulare werden im Abschnitt Letzte angezeigt.
   * 50 zusätzliche Workfront-Anfragewarteschlangen und Planungsanfrageformulare werden im Abschnitt **Alle Anfrageformulare** in alphabetischer Reihenfolge angezeigt. Sie können nach einer Anfrage-Warteschlange suchen, die standardmäßig nicht angezeigt wird.

1. Führen Sie einen der folgenden Schritte aus:

   * Klicken Sie in den Abschnitten „Letzte“ oder „Alle Anfrageformulare“ auf die Karte für eines der Planungsanfrageformulare
   * Geben Sie zunächst den Namen eines Planungsanfrageformulars in das Suchfeld ein und klicken Sie dann auf die Karte, wenn sie in der Liste angezeigt wird.

   Das Anfrageformular wird geöffnet.

1. Aktualisieren Sie die im Anfrageformular verfügbaren Felder. Felder mit einem roten Sternchen sind Pflichtfelder.
1. Klicken Sie **Senden**.

   Das Anfrageformular wird geschlossen und Sie kehren zum Bereich **Anfragen** zurück.

   Ihr Formular wird übermittelt und Folgendes geschieht:

   * Wenn das Anfrageformular nicht mit einer Genehmigung verknüpft war, wird die Anfrage auf der Registerkarte Planung im Bereich Gesendet im Bereich Workfront-Anfragen hinzugefügt und ein neuer Datensatz wird zu dem Datensatztyp hinzugefügt, der mit dem Formular verknüpft ist.

   * Wenn das Anfrageformular mit einer Genehmigung verknüpft war, wird die Anfrage auf der Registerkarte Planung im Abschnitt Gesendet im Bereich Workfront-Anfragen hinzugefügt. Ein neuer Datensatz wird der Seite „Datensatztyp“ erst hinzugefügt, nachdem alle genehmigenden Personen ihn genehmigt haben.

     Weitere Informationen finden Sie unter [Hinzufügen einer Genehmigung zu einem Anfrageformular](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

     ![Bereich „Anfragen“ mit Umschalter für die Registerkarte „Einheitliche Workflow-Planung“](assets/requests-area-with-toggle-for-unified-workflow-planning-tab-open.png)

     >[!IMPORTANT]
     >
     >Alle Benutzer, die Zugriff auf mindestens einen Arbeitsbereich haben, können die Registerkarte Planung im Bereich Anfragen anzeigen. Sie können nur die Anfragen anzeigen, die von Ihnen oder einer anderen Person an die Arbeitsbereiche gesendet wurden, für die Sie zumindest über die Berechtigung zum Anzeigen verfügen. Workfront-Admins können alle Anfragen anzeigen, die an einen beliebigen Arbeitsbereich im System gesendet wurden.

   * Die Anfrage ist nur für den Eigentümer, die genehmigende Person und die Personen sichtbar, die zumindest über Anzeigeberechtigungen für den Arbeitsbereich verfügen.

   * Sie erhalten eine In-App- und eine E-Mail-Benachrichtigung, dass die Anfrage entweder erfolgreich übermittelt wurde oder zur Überprüfung gesendet wurde.
   * Wenn das Anfrageformular mit einer Genehmigung verknüpft war, erhalten die genehmigenden Personen eine In-App- und eine E-Mail-Benachrichtigung, um die Anfrage zu überprüfen und zu genehmigen.

     >[!NOTE]
     >
     >Die E-Mail- und In-App-Benachrichtigungen sind nur sichtbar, wenn die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert wird.
     >
     >In der Bestätigungs- oder Validierungsbenachrichtigung per E-Mail ist ein Link zur Anfrage vorhanden.

   1. (Optional) Klicken Sie in **Bestätigungsmeldung auf** Anforderung anzeigen“, um die Anforderung zu öffnen, oder klicken Sie auf das Symbol **X**, um die Bestätigung zu schließen.

1. (Optional) Klicken Sie auf die **Planung** im Bereich Anfragen , um Ihre Anfrage anzuzeigen, und klicken Sie dann auf den Namen der Anfrage.

   Die Seite mit den Anfragedetails wird geöffnet.

   ![Seite mit Anforderungsdetails](assets/request-details-page.png)

1. (Bedingt) Wenn das Anfrageformular nicht mit einer Genehmigung verknüpft ist oder die Anforderung genehmigt wurde, klicken Sie auf den Namen der Anforderung und anschließend auf den Namen des Datensatzes **Feld &quot;**&quot;.

   Die Seite des Datensatzes wird in Workfront Planning geöffnet.

   >[!TIP]
   >
   >* Wenn das Primärfeld des Datensatzes im Anfrageformular nicht aktualisiert wurde, wird der Name des Datensatzes im Datensatzfeld der Anfrage als „Nicht **&quot;**.
   >
   >* Wenn das Anfrageformular mit einer Genehmigung verknüpft ist, muss die Genehmigung erteilt werden, bevor Sie auf den Datensatz auf der Anfrageseite zugreifen können.

1. (Optional) Klicken Sie auf den Namen des **Datensatztyps**.

   Die Seite „Datensatztyp“ wird in Workfront Planning geöffnet.

## Senden einer Anfrage an Workfront Planning über einen freigegebenen Link in ein Anfrageformular

1. Navigieren Sie zu dem Link, der von einem Workfront Planning-Datensatztyp für Sie freigegeben wurde.

1. Aktualisieren Sie die im Formular verfügbaren Felder. Felder mit einem Sternchen sind Pflichtfelder.

   >[!TIP]
   >
   >   Wenn das Feld **Betreff** verfügbar ist, wird es nach dem Senden der Anfrage in Workfront Planning nicht angezeigt.
   >
   >Es wird empfohlen, so viele Felder wie möglich in Ihrer Anfrage zu aktualisieren, damit der neue Datensatz identifizierbar wird, wenn er zum Datensatztyp in Workfront Planning hinzugefügt wird.

1. Klicken Sie **Senden**.

   Ihr Formular wird übermittelt und Folgendes geschieht:

   * Wenn das Anfrageformular nicht mit einer Genehmigung verknüpft war, wird die Anfrage auf der Registerkarte Planung im Bereich Gesendet im Bereich Workfront-Anfragen hinzugefügt und ein neuer Datensatz wird zu dem Datensatztyp hinzugefügt, der mit dem Formular verknüpft ist.

   * Wenn das Anfrageformular mit einer Genehmigung verknüpft war, wird die Anfrage auf der Registerkarte Planung im Abschnitt Gesendet im Bereich Workfront-Anfragen hinzugefügt. Ein neuer Datensatz wird der Seite „Datensatztyp“ erst hinzugefügt, nachdem alle genehmigenden Personen ihn genehmigt haben.

     Weitere Informationen finden Sie unter [Hinzufügen einer Genehmigung zu einem Anfrageformular](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

     ![Registerkarte „Planung“ in Anfragen](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     >Alle Benutzer, die Zugriff auf mindestens einen Arbeitsbereich haben, können die Registerkarte Planung im Bereich Anfragen anzeigen. Sie können nur die Anfragen anzeigen, die von Ihnen oder einer anderen Person an die Arbeitsbereiche gesendet wurden, für die Sie zumindest über die Berechtigung zum Anzeigen verfügen. Workfront-Admins können alle Anfragen anzeigen, die an einen beliebigen Arbeitsbereich im System gesendet wurden. <!--ensure this is correct; asking team in slack-->

   * Sie erhalten eine In-App- und eine E-Mail-Benachrichtigung, dass die Anfrage entweder erfolgreich übermittelt wurde oder zur Überprüfung gesendet wurde.
   * Wenn das Anfrageformular mit einer Genehmigung verknüpft war, erhalten die genehmigenden Personen eine In-App- und eine E-Mail-Benachrichtigung, um die Anfrage zu überprüfen und zu genehmigen.

     >[!NOTE]
     >
     >Die E-Mail- und In-App-Benachrichtigungen sind nur sichtbar, wenn die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert wird.

1. (Optional) Klicken Sie auf **Ihre Anfrage anzeigen**, um die Anfrage in Workfront zu öffnen.

   <!--Or-->

   <!--Click [Submit another request](https://pulsar.devtest.workfront-dev.com/intake/6740a1ff44bf3a5600cf4481/request) to open the request form and add a new request.-->

1. (Optional) Klicken Sie auf **Hauptmenü** > **Anfragen** > die **Planung**, um Ihre Anfrage anzuzeigen, und klicken Sie dann auf den Namen der Anfrage.

   Die Seite mit den Anfragedetails wird geöffnet.

   ![Seite mit Anforderungsdetails](assets/request-details-page.png)

1. (Bedingt) Wenn das Anfrageformular nicht mit einer Genehmigung verknüpft ist oder die Anforderung genehmigt wurde, klicken Sie auf den Namen der Anforderung und anschließend auf den Namen des Datensatzes **Feld &quot;**&quot;.

   Die Seite des Datensatzes wird in Workfront Planning geöffnet.

   >[!TIP]
   >
   >* Wenn der Datensatzname nicht zum Anfrageformular hinzugefügt wurde, wird der Name des Datensatzes im Datensatzfeld der Anfrage als „Nicht **&quot;**.
   >
   >* Wenn das Anfrageformular mit einer Genehmigung verknüpft ist, muss die Genehmigung erteilt werden, bevor Sie auf den Datensatz auf der Anfrageseite zugreifen können.

1. (Optional) Klicken Sie auf den Namen des **Datensatztyps**.

   Die Seite „Datensatztyp“ wird in Workfront Planning geöffnet.




