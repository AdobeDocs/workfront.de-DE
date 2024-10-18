---
product-area: projects
navigation-topic: approvals
title: Validierung der Arbeit
description: Validierung der Arbeit
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 216bf9ea9cb58294b42cc41d70ca0ab99b6dc827
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 1%

---

# Validierung der Arbeit

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

Wenn Sie als Genehmiger festgelegt sind, sollten Sie regelmäßig überprüfen, welche Arbeit auf Ihre Genehmigung wartet.

Informationen zum Erstellen von Genehmigungsprozessen finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Informationen zum Verknüpfen von Genehmigungen mit Arbeiten in Workfront finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Alle</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Objekte, die Genehmigungen zugeordnet sind, anzeigen oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für die Objekte, die mit Genehmigungen verknüpft sind</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

+++

## Suchen von Genehmigungen in Adobe Workfront

Sie können Genehmigungen in verschiedenen Bereichen von Workfront anzeigen und verwalten.

Weitere Informationen zum Anzeigen von Elementen, die auf Genehmigungen warten, oder von Elementen, die Sie selbst zur Genehmigung eingereicht haben, finden Sie unter [Genehmigungen anzeigen](../../review-and-approve-work/manage-approvals/view-approvals.md).

## Genehmigen Sie die Arbeit vom Startbereich aus.

1. Klicken Sie oben rechts auf das Hauptmenü ]**![](assets/main-menu-icon.png) und dann auf**[!UICONTROL  Startseite ]**.**[!UICONTROL 
1. (Bedingt) Klicken Sie auf **Anpassen** , um das Widget **Meine Genehmigungen** hinzuzufügen.
1. (Bedingt) Klicken Sie auf das Dropdown-Menü **Filter** und wählen Sie dann **Alle** aus, um die Ihnen zugewiesenen und zugewiesenen Genehmigungen anzuzeigen.

   >[!NOTE]
   >
   >Genehmigungen, die Auftragsrollen oder Gruppen zugewiesen sind, werden nicht auf der Startseite angezeigt. Die den Teams zugewiesenen Validierungen werden im Widget Meine Validierungen für jedes Teammitglied angezeigt.


1. Wählen Sie das Element aus, für das Sie eine Genehmigungsentscheidung treffen möchten.

   ![](assets/my-approvals-widget.png)

1. Klicken Sie im rechten Bereich auf eine der verfügbaren Optionen, wenn Sie eine Genehmigungsentscheidung treffen. Je nach Typ des zu genehmigenden Elements werden in der rechten oberen Ecke der Seite die folgenden Optionen angezeigt:

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
      <li>Zuschuss</li>
      <li>Ignorieren</li>
      </ul>
      Sie können die Zugriffsebene im Dropdown-Menü <b>Zugriff ändern</b> nach Bedarf anpassen.
      </td>
      <td>
         <ul>
         <li>Genehmigen</li>
         <li>Ablehnen</li>
         </ul>
      Sie können einen Kommentar zu Ihrer Entscheidung hinterlassen, indem Sie auf das Dropdown-Menü in der Entscheidungsschaltfläche klicken.
      </td>
      <td>
   Als Genehmiger zugewiesen
         <ul>
         <li>Genehmigen</li>
         <li>Mit Änderungen genehmigt</li>
         <li>Muss bearbeitet werden</li>
         </ul>
   Als Validierer zugewiesen
         <ul>
         <li>Überprüfung abschließen</li>
         </ul>
      Die Optionen in dieser Spalte gelten nur für neue Dokumentgenehmigungen. Genehmigungen veralteter Dokumente erscheinen genauso wie Genehmigungen für Arbeitselemente. 
      </td>
      <td>
         <ul>
         <li>Testversand durchführen</li>
         </ul>
         Sie treffen Ihre Entscheidung im Testversand-Viewer. Informationen zum Überprüfen eines Testversands finden Sie unter <a href="../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md">Testsendungen in Adobe Workfront überprüfen</a>.
      </td>
   </tr>
   </table>

Nachdem Sie eine Entscheidung getroffen haben, wird die Genehmigung aus dem Widget Meine Genehmigung entfernt.


## Direkte Genehmigung der Arbeit über ein Projekt, eine Aufgabe oder ein Problem

Wenn die Genehmigung eines Projekts, einer Aufgabe oder eines Problems aussteht, können Sie die Genehmigung direkt über das Projekt, die Aufgabe oder das Problem genehmigen oder ablehnen. Sie können auch Details zum Validierungsprozess anzeigen.

So genehmigen Sie Arbeiten direkt über ein Projekt, eine Aufgabe oder ein Problem:

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, für das eine Genehmigung erforderlich ist.

   Genehmigungsinformationen zum aktuellen Genehmigungsprozess eines Projekts, einer Aufgabe oder eines Problems werden in der Kopfzeile des Elements angezeigt.

   ![](assets/current-approval-process-in-project-header-with-stages-nwe-350x92.png)

   Die folgenden Validierungsinformationen sind verfügbar:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td>Der aktuelle Status des Projekts, der Aufgabe oder des Problems. Dies ist der aktuelle Status des Elements, das auf die Genehmigung wartet. Der Status wird genehmigt, nachdem jede Phase im Genehmigungsprozess genehmigt wurde.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Validierungsphasen</td> 
      <td>Die Etappen des Validierungsprozesses. <br>Die aktuelle Phase, in der die Genehmigung aussteht, wird als Ausstehend angezeigt. Bereits genehmigte Phasen werden als Genehmigt angezeigt. Etappen, die noch nicht genehmigt wurden, werden als Nicht gestartet angezeigt.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Genehmigen** oder **Ablehnen**, je nachdem, ob Sie den Genehmigungsprozess genehmigen oder ablehnen möchten.\
   Die Validierungsphase, für die die Genehmigung ausstand, wird nun genehmigt und der Genehmigungsprozess wird in die nächste Phase verschoben. Der Status wird genehmigt, nachdem alle Phasen genehmigt wurden.

## Dokument direkt aus einem Dokument genehmigen 

1. Markieren Sie den Dokumentbereich, der das Dokument enthält, für das Sie eine Genehmigung benötigen.
1. Wählen Sie das Dokument aus und klicken Sie dann auf **Genehmigen**, **Änderungen** oder **Ablehnen**.\
   ![](assets/approval-approve-document-350x215.png)\
   ![](assets/document-approval-350x199.png)

1. (Optional) Wenn ein Testversand für das Dokument generiert wurde, können Sie das Dokument in der Testversandschnittstelle genehmigen, wie unter [Dokument anhand eines Testversands genehmigen](#approve-a-document-from-a-proof) beschrieben.

## Dokument aus einer Validierungs-E-Mail validieren

Abhängig von Ihren Benachrichtigungseinstellungen erhalten Sie E-Mails, die Sie über Dokumente informieren, für die andere Benutzer eine Validierungsentscheidung treffen müssen. Wenn Sie eine E-Mail mit der Schaltfläche **Genehmigungsentscheidung treffen** erhalten, können Sie den Genehmigungsprozess direkt über die E-Mail starten:

1. Klicken Sie in der E-Mail auf **Genehmigungsentscheidung treffen** , um die Seite &quot;Dokumentdetails&quot;für den Testversand zu öffnen.
1. Führen Sie einen der folgenden Schritte aus, um das Dokument zu überprüfen:

   * Anzeigen der Metadaten zum Dokument.
   * Wenn ein Testversand zur Überprüfung des Dokuments mit Markup und Kommentaren erstellt wurde, klicken Sie oben rechts auf **Testversand öffnen** ![](assets/open-proof-icon-qs.png) und überprüfen Sie den Testversand.

     <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

     Informationen zur Überprüfung von Testsendungen finden Sie unter [Testsendungen in Adobe Workfront überprüfen](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Klicken Sie oben rechts auf die Option **Entscheidung** , um das Dokument zu genehmigen, mit Änderungen zu genehmigen oder abzulehnen.

## Dokument anhand eines Testversands genehmigen {#approve-a-document-from-a-proof}

Sie können ein Dokument im Testversand-Viewer genehmigen. Weitere Informationen finden Sie unter [Entscheidungsfindung über einen Testversand im Testversand-Viewer](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) im Artikel [Entscheidungsfindung über einen Testversand im Testversand-Viewer](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).
