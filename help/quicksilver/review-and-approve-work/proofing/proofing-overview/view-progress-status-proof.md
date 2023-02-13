---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Fortschritt und Status des Testversands - Übersicht
description: Sie können Informationen darüber anzeigen, wie ein Testversand während des Überprüfungsprozesses durchgeführt wird, und eine Zusammenfassung des Entscheidungsstatus des Testversands im Bereich Dokumente anzeigen.
author: Courtney
feature: Digital Content and Documents
exl-id: 78e81070-ff82-4d82-90a3-6e0cd176b290
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 2%

---

# Fortschritt und Status des Testversands - Übersicht

Sie können Informationen darüber anzeigen, wie ein Testversand während des Überprüfungsprozesses durchgeführt wird, und eine Zusammenfassung des Entscheidungsstatus des Testversands im Bereich Dokumente anzeigen.

## Übersicht über den Fortschritt des Testversands

Der Fortschritt des Testversands gibt an, welche Arbeit an einem Testversand von dem Zeitpunkt an, an dem Sie den Testversand an die Empfänger senden, bis zu dem Zeitpunkt, an dem sie über den Testversand entscheiden. Die Fortschrittssymbole S, O, C und D erscheinen neben dem Testversandnamen und geben Informationen zum Fortschritt des Testversands an.

![](assets/proof-edit-existing-progress-350x62.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>Fortschrittssymbol</strong> </p> </td> 
   <td> <p><strong>Beschreibung</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-sent-icon.png" alt=""> </p> <p><strong>Gesendet</strong> </p> </td> 
   <td> <p>Der Testversand wurde an zugewiesene Empfänger gesendet.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>Geöffnet</strong> </p> </td> 
   <td> <p>Alle zugewiesenen Empfänger öffnen die Seite mit den Testversand- oder Testversanddetails .</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>Stellungnahmen</strong> </p> </td> 
   <td> <p>Alle zugewiesenen Empfänger geben mindestens einen Kommentar zum Testversand ab.</p> <p>Wenn dem Testversand keine Validierungsverantwortlichen zugewiesen sind, wird die <strong>C</strong> in der Fortschrittsleiste nicht angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-decision-icon.png" alt=""> </p> <p><strong>Entscheidung</strong> </p> </td> 
   <td> <p>Alle zugewiesenen Genehmiger treffen eine Entscheidung über den Testversand, alle zugewiesenen Genehmiger treffen eine Entscheidung über den Testversand, es sei denn, der Ersteller des Testversands gibt nur eine Entscheidung an.</p> <p>Wenn für den Testversand keine Genehmiger (Entscheidungsträger) bestimmt sind, wird die <strong>D</strong> in der Fortschrittsleiste nicht angezeigt. </p> </td> 
  </tr> 
 </tbody> 
</table>

Die Fortschrittssymbole können in den folgenden Farben angezeigt werden, um bestimmte Informationen über den Fortschritt des Testversands anzuzeigen:

* **Grün**: Abgeschlossen.
* **weiß**: Nicht abgeschlossen.
* **Orange**: Unvollständig und Abgabetermin ist weniger als 24 Stunden.
* **Rot**: Nicht abgeschlossen und die Frist verstrichen.

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Levels of proof progress</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront Proof uses the progress icons to track a proof's progress at each of the following levels:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each reviewer, based on that person's activity on the proof.&nbsp;</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each stage, based on the progress the reviewer on the stage who is most behind in the proofing process.&nbsp;To learn more about stages, see <a href="../../../review-and-approve-work/proofing/proofing-overview/stages.md" class="MCXref xref">Automated Workflow Stages overview</a>.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For the proof, based on the progress of the stage (group of reviewers) who is the most behind in the proofing process.</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For an example of how Workfront Proof determines progress using the reviewer or stage that is most behind,&nbsp;suppose three reviewers on a proof need to make a&nbsp;decision. If two of them have made their&nbsp;decision&nbsp;but the third has not, the progress bar for the proof does not show&nbsp;the D in green because of the outstanding&nbsp;decision.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If the Primary Decision Maker setting is selected on a proof and the primary decision maker submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Similarly, if the Only One Decision Required setting is selected on a proof and any reviewer submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

## Übersicht über den Teststatus

Der Status des Testversands zeigt den Status der Entscheidungen an, die für den Testversand erforderlich sind. Der Status des Testversands wird durch den Teilnehmer &quot;Schlimmster Fall&quot; bestimmt. Angenommen, es gibt drei Entscheidungen zum Testversand: zwei haben den Status **Akzeptiert** und hat den Status **Zurückgewiesen**. Die Entscheidung des &quot;schlimmsten Falls&quot; **Zurückgewiesen** überregelt die anderen Entscheidungen und der Gesamtstatus des Testversands wird wie folgt angezeigt: **Zurückgewiesen**. 

![](assets/proof-edit-existing-progress-350x62.png)

Die Standardstatusoptionen lauten wie folgt:

* Ausstehend
* Genehmigt
* Genehmigt mit Änderungen
* Erforderliche Änderungen
* Nicht relevant

Wenn benutzerdefinierte Entscheidungen in Ihrem Konto konfiguriert sind, spiegeln die Statusoptionen Ihre benutzerdefinierten Entscheidungseinstellungen wider.

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Viewing proof progress and status</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> You can view the progress and status of proofs for individual documents. </p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-progress-and-status-for-a-document" class="MCXref xref">View proof progress and status&nbsp;for a document</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-approval-information-in-home" class="MCXref xref">View proof approval information&nbsp;in Home</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-progress-and-status-for-a-document">View proof progress and status&nbsp;for a document</h3>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">If a proof has not already been generated for the document in Adobe Workfront, generate it, as described in the articles.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Documents area, under the proof's name, click <strong>Proof Details</strong>.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Proofing Details</strong> box that appears, the proof's progress for each stage, then click <strong>Done</strong>.</li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Under the proof's name, click <strong>Proofing Workflow</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <img src="assets/click-proofing-workflow-qs-350x149.png" style="width: 350;height: 149;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
   -->
<!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   These screenshots will need to change with new terminology ("Review Workflow" for this one?)
   </MadCap:conditionalText>
   <br> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Workflow information that appears, scroll down to see the proof's progress for each stage:</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/scroll-to-see-socd-for-stages-qs-350x152.png" style="width: 350;height: 152;"> </p>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-approval-information-in-home">View proof approval information&nbsp;in Home</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can view information about proofs that you have submitted for approval. Proof approval information is displayed in the Home area only while the proof is pending approval.&nbsp;For information about how to view information about proof approvals in the Home area, see&nbsp;<a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">View approvals </a>.</p>
-->
