---
title: Adobe Workfront-Planungsanfragen senden
description: Nachdem in Adobe Workfront Planning von einer Datensatztypseite aus ein Link zu einem Anforderungsformular für Sie freigegeben wurde, können Sie eine Anforderung hinzufügen, um Datensätze für den Datensatztyp zu erstellen, der mit dem Anforderungsformular verknüpft ist.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 5510f99e9e5c8c4c5f85953e19563f9ab18b0fae
workflow-type: tm+mt
source-wordcount: '1089'
ht-degree: 0%

---

# Senden von Adobe Workfront-Planungsanfragen zum Erstellen von Datensätzen

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Nachdem in Adobe Workfront Planning von einer Datensatztypseite aus ein Link zu einem Anforderungsformular für Sie freigegeben wurde, können Sie eine Anforderung hinzufügen, um Datensätze für den Datensatztyp zu erstellen, der mit dem Anforderungsformular verknüpft ist.

Workfront-Benutzende und externe Benutzende können Anfragen an Planning-Datensatztypen senden und Datensätze erstellen. <!--double check on the external users-->

In diesem Artikel wird beschrieben, wie Sie eine Anfrage zum Hinzufügen neuer Datensätze zu einem Datensatztyp senden können.

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
   <p>Anzeigen von oder höhere Berechtigungen für einen Arbeitsbereich, wenn Sie Workfront-Benutzer sind</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Layoutvorlage</p></td>
   <td> <p>Für den Zugriff auf den Planungsbereich in Workfront muss Ihnen eine Layoutvorlage zugewiesen werden, die den Planungsbereich im Hauptmenü enthält. </p>
   <p> Der Zugriff auf den Bereich Planung ist jedoch nicht erforderlich, um Anfragen an Workfront Planning zu senden. </p>  
</td>
  </tr>
 </tbody>
</table>

*Weitere Informationen zu Zugriffsanforderungen für Workfront finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Voraussetzungen

Folgendes muss vorhanden sein, bevor Sie eine Anfrage an ein Workfront Planning-Anfrageformular senden können:

* In Workfront Planning muss Folgendes vorhanden sein:

   * Ein Arbeitsbereich
   * Ein mit einem Anfrageformular verknüpfter Datensatztyp. Weitere Informationen finden Sie unter [Erstellen eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* Das Anfrageformular muss für einen Link freigegeben werden, sodass Sie darauf zugreifen können. Die folgenden Szenarien sind vorhanden:

   * Wenn Sie über ein Workfront-Konto verfügen, wurde der Link nur für interne Personen freigegeben, und Sie haben Zugriff auf den Arbeitsbereich, der Ihnen zur Verfügung steht, oder darüber hinaus. Personen außerhalb von Workfront können nicht auf einen intern freigegebenen Link zugreifen.
   * Wenn Sie kein Workfront-Konto haben, wurde der Link für externe Personen freigegeben. Benutzende von Workfront können auch auf einen Link zugreifen, der für externe Personen freigegeben ist.

* Der Link zum Formular darf nicht abgelaufen sein.

## Überlegungen zum Senden von Anfragen an Workfront Planning

* Der Zugriff auf ein Anforderungsformular für Workfront Planning-Anforderungen ist nur über einen bestimmten Link zum Formular möglich.
* Eine Anforderung kann nicht in Workfront bearbeitet werden, nachdem sie an Workfront Planning übermittelt wurde.
* Jede gesendete Anfrage erstellt einen Datensatz für den Datensatztyp, der mit dem von Ihnen verwendeten Formular verknüpft ist, wenn das Formular nicht mit einer Genehmigung verknüpft ist oder wenn die Genehmigung von allen genehmigenden Personen erteilt wurde.
* Datensätze, die durch das Übermitteln von Anfrageformularen erstellt wurden, können nicht von Datensätzen unterschieden werden, die über eine andere Methode hinzugefügt wurden. Weitere Informationen finden Sie unter [Erstellen von Datensätzen](/help/quicksilver/planning/records/create-records.md).
* Gesendete Anfragen werden in Workfront im Bereich Anfragen auf der Registerkarte Planung des Abschnitts Gesendet angezeigt.
* Die Anzeige bestimmter Feldtypen in einem Anfrageformular oder auf der Seite mit den Anfragedetails nach dem Senden eines Formulars ist eingeschränkt. Weitere Informationen finden Sie unter [Erstellen und Verwalten eines Anfrageformulars in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Anforderung an Workfront Planning senden

<!--
<div class="preview">

Submitting requests to Workfront Planning differs depending on what environment you use. 

### Submit a request to Workfront Planning in the Preview Environment

>[!NOTE]
>
>After the monthly releases to Production, the features described in this section are also available in the Production environment for customers who enabled fast releases.

{{step1-to-requests}}

1. Enable the **Switch to a new experience** setting, in the upper-right corner of he screen. 
   Enabling this setting makes the Workfront Planning request forms available in the **Requests** area of Workfront.

   >[!TIP]
   >
   >This setting is available only when the following are in place:
   >
   >* Your company has purchased a Workfront Planning package. 
   >* Your Workfront instance is onboarded to the Adobe Unified Experience. 
   >* You have access to view at least one workspace. 
   >

1. Click **New request**. (********* update screen shot at release ********)

   ![New request box with unified Workfront and Planning cards](assets/new-request-box-with-unified-workfront-and-planning-cards.png)

   The New request area opens with the following information: 

   * The 6 most recently accessed Workfront request queues and Planning request forms display in the Recent section. 
   * 50 additional Workfront request queues and Planning request forms display in alphabetical order in the **All request forms** section. You can search for a request queue that does not display by default. 

1. Do one of the following:

   * Click the card for one of the Planning request forms in the Recent or All request forms sections
   * Start typing the name of a Planning request form in the search box, then click the card when it displays in the list. 

   The request form opens.

1. Update the fields available in the request form. Fields with a red asterisk are required. 
1. Click **Submit**.
    
   The request form closes and you return to the **Requests** area. 

   Your form is submitted and the following things occur:

   * If the request form was not associated with an approval, the request is added to the Planning tab of the Submitted section of the Workfront Requests area and a new record is added to the record type associated with the form.
   
   * If the request form was associated with an approval, the request is added to the Planning tab of the Submitted section of the Workfront Requests area. A new record is added to the record type page only after all the approvers have approved it.
   
      For information, see [Add an approval to a request form](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

      ![](assets/requests-area-with-toggle-for-unified-workflow-planning-tab-open.png)

      >[!IMPORTANT]
      >
      >All users who have access to at least one workspace can view the Planning tab in the Requests area. You can view only the requests submitted by you or anyone else to the workspaces that you have at least permissions to View. Workfront administrators can view all requests submitted to any workspace in the system. (******** ensure this is correct; asking team in slack **************)

   * You receive an in-app and an email notification that the request has either been submitted successfully or has been sent for review.
   * If the request form was associated with an approval, the approvers receive an in-app and an email notification to review and approve the request.

      >[!NOTE]
      >
      >The email and in-app notifications are visible only when your organization's instance of Workfront is onboarded to the Adobe Unified Experience.

1. (Optional) Click the **Planning** tab in the Requests area to view your request, then click the name of the request. 

   The request details page opens. 

   ![Request details page](assets/request-details-page.png)

1. (Conditional) If the request form is not associated with an approval, or if the request has been approved, click the name of the request, then click the name of the record in the **Record** field. 

   The record's page opens in Workfront Planning. 

   >[!TIP]
   >
   >* If the record name was not added to the request form, the name of the record in the Record field of the request displays as **Untitled**. 
   >
   >* If the request form is associated with an approval, the approval must be granted before you can access the record from the request page. 

1. (Optional) Click the name of the **Record type**. 

   The record type page opens in Workfront Planning. 

</div>

### Submit a request to Workfront Planning in the Production environment

-->

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

     ![](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     >Alle Benutzer, die Zugriff auf mindestens einen Arbeitsbereich haben, können die Registerkarte Planung im Bereich Anfragen anzeigen. Sie können nur die Anfragen anzeigen, die von Ihnen oder einer anderen Person an die Arbeitsbereiche gesendet wurden, für die Sie zumindest über die Berechtigung zum Anzeigen verfügen. Workfront-Admins können alle Anfragen anzeigen, die an einen beliebigen Arbeitsbereich im System gesendet wurden. <!--ensure this is correct; asking team in slack-->

   * Sie erhalten eine In-App- und eine E-Mail-Benachrichtigung, dass die Anfrage entweder erfolgreich übermittelt wurde oder zur Überprüfung gesendet wurde.
   * Wenn das Anfrageformular mit einer Genehmigung verknüpft war, erhalten die genehmigenden Personen eine In-App- und eine E-Mail-Benachrichtigung, um die Anfrage zu überprüfen und zu genehmigen.

     >[!NOTE]
     >
     >Die E-Mail- und In-App-Benachrichtigungen sind nur sichtbar, wenn die Workfront-Instanz Ihres Unternehmens in das einheitliche Adobe-Erlebnis integriert wird.

1. (Optional) Klicken Sie auf die **Planung** im Bereich Anfragen , um Ihre Anfrage anzuzeigen, und klicken Sie dann auf den Namen der Anfrage.

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




