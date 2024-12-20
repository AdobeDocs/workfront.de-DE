---
product-area: projects
navigation-topic: approvals
title: Genehmigende Arbeit
description: Genehmigende Arbeit
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 7366e3dd37b686a3566ca6d39e28eb6762c6d1ff
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 1%

---

# Genehmigende Arbeit

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

Wenn Sie als genehmigende Person festgelegt sind, sollten Sie regelmäßig überprüfen, welche Arbeiten von Ihnen genehmigt werden müssen.

Informationen zum Erstellen von Genehmigungsprozessen finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Informationen zum Verknüpfen von Genehmigungen mit Arbeiten in Workfront finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit Arbeiten](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Objekte, die mit Genehmigungen verknüpft sind, anzeigen oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für die Objekte, die mit Genehmigungen verbunden sind</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

## Suchen von Validierungen in Adobe Workfront

Sie können Validierungen in verschiedenen Bereichen von Workfront anzeigen und verwalten.

Weitere Informationen zum Anzeigen von Elementen, die auf Genehmigungen warten, oder von Elementen, die Sie selbst zur Genehmigung eingereicht haben, finden Sie unter [Anzeigen von Genehmigungen](../../review-and-approve-work/manage-approvals/view-approvals.md).

## Genehmigen von Arbeit im Bereich „Startseite“

1. Klicken Sie oben rechts auf **[!UICONTROL Hauptmenü]** ![](assets/main-menu-icon.png) und dann auf **[!UICONTROL Home]**.
1. (Bedingt) Klicken Sie auf **Anpassen**, um das Widget **Meine Genehmigungen** hinzuzufügen.
1. (Bedingt) Klicken Sie auf das **Filter** Dropdown-Menü und wählen Sie **Alle**, um die Ihnen zugewiesenen und delegierten Genehmigungen anzuzeigen.

   >[!NOTE]
   >
   >Genehmigungen, die Aufgabengebieten oder Gruppen zugewiesen wurden, werden nicht auf der Startseite angezeigt. Genehmigungen, die Teams zugewiesen wurden, werden für jedes Teammitglied im Widget Meine Genehmigungen angezeigt.


1. Wählen Sie das Element aus, für das Sie eine Genehmigungsentscheidung treffen möchten.

   ![](assets/my-approvals-widget.png)

1. Klicken Sie im rechten Bedienfeld auf eine der verfügbaren Optionen, wenn Sie eine Genehmigungsentscheidung treffen. Die folgenden Optionen werden je nach Art des zu genehmigenden Elements in der rechten oberen Ecke der Seite angezeigt:

   <table>
   <tr>
      <td>
      <p><strong>Zugriff</strong></p>
      </td>
      <td>
      <p><strong>Arbeitselemente</strong></p>
      </td>
      <td>
      <p><strong>Dokumente</strong></p>
      </td>
      <td>
      <p><strong>Korrekturabzüge</strong></p>
      </td>
   </tr>
   <tr>
      <td>
       <ul>
      <li>erteilen</li>
      <li>Ignorieren</li>
      </ul>
      Sie können die Zugriffsebene bei Bedarf im Dropdown-Menü <b>Zugriff ändern</b> anpassen.
      </td>
      <td>
         <ul>
         <li>Genehmigen</li>
         <li>Ablehnen</li>
         </ul>
      Sie können eine Entscheidung kommentieren, indem Sie auf das Dropdown-Menü in der Entscheidungsschaltfläche klicken.
      </td>
      <td>
   Als genehmigende Person zugewiesen
         <ul>
         <li>Genehmigen</li>
         <li>Mit Änderungen genehmigt</li>
         <li>Muss bearbeitet werden</li>
         </ul>
   Als Prüfer zugewiesen
         <ul>
         <li>Überprüfung abschließen</li>
         </ul>
      Die Optionen in dieser Spalte gelten nur für neue Dokumentgenehmigungen. Legacy-Dokumentgenehmigungen erscheinen genauso wie Arbeitselementgenehmigungen. 
      </td>
      <td>
         <ul>
         <li>Zum Korrekturabzug gehen</li>
         </ul>
         Sie treffen Ihre Entscheidung in der Korrekturabzugsansicht. Informationen zur Überprüfung eines Korrekturabzugs finden Sie unter <a href="../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md">Testsendungen in Adobe Workfront </a>.
      </td>
   </tr>
   </table>

Nachdem Sie eine Entscheidung getroffen haben, wird die Genehmigung aus dem Widget Meine Genehmigung entfernt.


## Arbeit direkt aus einem Projekt, einer Aufgabe oder einem Problem genehmigen

Wenn für ein Projekt, eine Aufgabe oder ein Problem die Genehmigung aussteht, können Sie die Genehmigung direkt über das Projekt, die Aufgabe oder das Problem genehmigen oder ablehnen. Sie können auch Details zum Genehmigungsprozess anzeigen.

So genehmigen Sie Arbeiten direkt aus einem Projekt, einer Aufgabe oder einem Problem:

1. Wechseln Sie zu dem Projekt, der Aufgabe oder dem Problem, das bzw. das Ihre Genehmigung erfordert.

   Genehmigungsinformationen zum aktuellen Genehmigungsprozess eines Projekts, einer Aufgabe oder eines Problems werden in der Kopfzeile des Elements angezeigt.

   ![](assets/current-approval-process-in-project-header-with-stages-nwe-350x92.png)

   Folgende Validierungsinformationen stehen zur Verfügung:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td>Der aktuelle Status des Projekts, der Aufgabe oder des Problems. Dies ist der aktuelle Status des Elements, das noch nicht genehmigt wurde. Der Status wird nach jeder Phase im Genehmigungsprozess genehmigt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Genehmigungsphasen</td> 
      <td>Die Phasen des Genehmigungsprozesses. <br>Die aktuelle Phase, für die die Genehmigung aussteht, wird als Ausstehend angezeigt. Phasen, die bereits genehmigt wurden, werden als genehmigt angezeigt. Phasen, die noch nicht genehmigt wurden, werden als Nicht gestartet angezeigt.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Genehmigen** oder **Ablehnen**, je nachdem, ob Sie den Genehmigungsprozess genehmigen oder ablehnen möchten.\
   Die Genehmigungsphase, für die die Genehmigung ausstand, wird jetzt genehmigt und der Genehmigungsprozess geht zur nächsten Phase über. Der Status wird genehmigt, nachdem alle Phasen genehmigt wurden.

## Genehmigen eines Dokuments direkt aus einem Dokument

1. Wechseln Sie zum Bereich Dokumente , der das Dokument enthält, das Ihre Genehmigung erfordert.
1. Wählen Sie das Dokument aus und klicken Sie dann auf **Genehmigen**, **Änderungen** oder **Ablehnen**.\
   ![](assets/approval-approve-document-350x215.png)\
   ![](assets/document-approval-350x199.png)

1. (Optional) Wenn ein Korrekturabzug für das Dokument generiert wurde, können Sie das Dokument innerhalb der Proofing-Oberfläche genehmigen, wie in [Genehmigen eines Dokuments aus einem Korrekturabzug](#approve-a-document-from-a-proof) beschrieben.

## Genehmigen eines Dokuments über eine Genehmigungsbenachrichtigungs-E-Mail

Abhängig von Ihren Benachrichtigungseinstellungen erhalten Sie möglicherweise E-Mails, die Sie über Dokumente informieren, für die andere Benutzer eine Genehmigungsentscheidung treffen müssen. Wenn Sie eine E-Mail mit der Schaltfläche **Genehmigungsentscheidung treffen** erhalten, können Sie den Genehmigungsprozess direkt aus der E-Mail heraus starten:

1. Klicken Sie in der E **Mail auf Genehmigungsentscheidung**, um die Dokumentdetailseite für den Korrekturabzug zu öffnen.
1. Führen Sie einen der folgenden Schritte aus, um das Dokument zu überprüfen:

   * Anzeigen der Metadaten zum Dokument.
   * Wenn ein Korrekturabzug zur Überprüfung des Dokuments mit Markup und Kommentaren erstellt wurde, klicken Sie auf **Korrekturabzug öffnen** ![](assets/open-proof-icon-qs.png) in der oberen rechten Ecke und prüfen Sie den Korrekturabzug.

     <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

     Informationen zur Überprüfung von Testsendungen finden Sie unter [Testsendungen in Adobe Workfront ](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Klicken Sie **oben rechts auf** Option „Entscheidung“, um das Dokument zu genehmigen, mit Änderungen zu genehmigen oder abzulehnen.

## Genehmigen eines Dokuments aus einem Korrekturabzug {#approve-a-document-from-a-proof}

Sie können ein Dokument in der Proofing-Anzeige genehmigen. Weitere Informationen finden Sie unter [Entscheidung über einen Korrekturabzug in der Korrekturabzugsansicht treffen](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) im Artikel [Entscheidung über einen Korrekturabzug in der Korrekturabzugsansicht treffen](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).
