---
product-area: projects
navigation-topic: approvals
title: Validierung der Arbeit
description: Validierung der Arbeit
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 0%

---

# Validierung der Arbeit

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

Wenn Sie als Genehmiger festgelegt sind, sollten Sie regelmäßig überprüfen, welche Arbeit auf Ihre Genehmigung wartet.

Informationen zum Erstellen von Genehmigungsprozessen finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Informationen zum Verknüpfen von Genehmigungen mit Arbeiten in Workfront finden Sie unter [Verknüpfen eines neuen oder vorhandenen Genehmigungsprozesses mit der Arbeit](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Zugriffsanforderungen

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
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Objekte, die Genehmigungen zugeordnet sind, anzeigen oder höher</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Anzeigen von oder höheren Berechtigungen für die Objekte, die mit Genehmigungen verknüpft sind</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Suchen von Genehmigungen in Adobe Workfront

Sie können Genehmigungen in verschiedenen Bereichen von Workfront anzeigen und verwalten.

Weitere Informationen zum Anzeigen von Elementen, die auf Genehmigungen warten, oder von Elementen, die Sie selbst zur Genehmigung eingereicht haben, finden Sie unter [Anzeigen von Genehmigungen](../../review-and-approve-work/manage-approvals/view-approvals.md).

## Genehmigen Sie die Arbeit vom Startbereich aus.

1. Klicken Sie auf **Startseite** icon ![](assets/home-icon-30x29.png) in der linken oberen Ecke von Adobe Workfront.

   >[!NOTE]
   >
   >Ihr Workfront-Administrator kann die folgenden Änderungen am Startseiten-Symbol in Ihrer Umgebung vornehmen:
   >
   >   
   >* Ersetzen Sie sie durch ein Bild, das zur Veranschaulichung Ihrer Organisation angepasst wurde. In diesem Fall sieht das Symbol anders aus als in diesem Artikel.
   >* Ersetzen Sie die verknüpfte Seite durch eine andere Seite. Klicken Sie in diesem Fall auf die **Hauptmenü** ![](assets/main-menu-icon.png) in der rechten oberen Ecke der Seite klicken Sie auf **Startseite**.

1. Klicken Sie auf **Filter** Dropdown-Menü.

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. Auswählen **Genehmigungen**.\
   Alle Arbeitselemente, für die Ihre Genehmigung erforderlich ist, werden angezeigt. 

   >[!NOTE]
   >
   >Genehmigungen, die Auftragsrollen oder Gruppen zugewiesen sind, werden nicht auf der Startseite angezeigt. Für Teams zugewiesene Validierungen werden in der Gruppe Teamanfrage in der Arbeitsliste angezeigt.

1. (Optional) Ändern Sie die Reihenfolge, in der die Genehmigungen angezeigt werden, wie im Artikel &quot;Gruppieren und nach Datum, Projekt oder Priorität sortieren&quot;beschrieben. [Anzeigen von Elementen in der Arbeitsliste im Startbereich](../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).
1. Wählen Sie das Element aus, für das Sie eine Genehmigungsentscheidung treffen möchten.

   ![](assets/task-approval-home-350x127.png)

1. Klicken Sie im rechten Bereich auf eine der verfügbaren Optionen, wenn Sie eine Genehmigungsentscheidung treffen. Je nach Typ des zu genehmigenden Elements werden in der rechten oberen Ecke der Seite die folgenden Optionen angezeigt:

   * **Projekte:** Klicks **Genehmigen** oder **Ablehnen**.

   * **Aufgaben:** Klicks **Genehmigen** oder **Ablehnen** .

   * **Probleme:** Klicks **Genehmigen** oder **Ablehnen** .

   * **Timesheets:** Klicks **Genehmigen** oder **Ablehnen** .

   * **Dokumente:** Klicks **Genehmigen**, **Ablehnen** oder **Änderungen**.\
      Beachten Sie beim Anzeigen von Genehmigungen Folgendes:

      * Hier werden die Testversandgenehmigungen angezeigt, wenn ein Benutzer einen Testversand für Sie freigegeben hat, wie im Artikel unter &quot;Link zum Testversand freigeben&quot;beschrieben. [Freigeben eines Testversands in Adobe Workfront](../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
      * Testversandgenehmigungen werden nur dann im Startbereich angezeigt, wenn Ihre Workfront-Umgebung in ein Workfront Testversand Premium-Konto integriert ist. Wenden Sie sich an Ihren Workfront-Administrator, wenn Sie die Proofing-Funktion nicht wie hier beschrieben verwenden können.
      * Sie erhalten eine In-App-Benachrichtigung, in der Sie über die Genehmigung des Testversands informiert werden.\
        Weitere Informationen zu In-App-Benachrichtigungen finden Sie unter [Anzeigen und Verwalten von In-App-Benachrichtigungen](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

      * Der Name des Benutzers, der die Genehmigung angefordert hat, wird neben dem Miniaturbild im Startbereich mit folgendem Text angezeigt:\
        &quot;*Benutzer A* Ihre Genehmigung soll...&quot;

        <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE:&nbsp;From&nbsp;Courtney: Is this true?)      
        </MadCap:conditionalText>      
        -->

        Wenn der Benutzername nicht verfügbar ist, wird der folgende Text angezeigt:\
        &quot;Eine neue Version eines Testversands kann angezeigt werden.&quot;
      * Um eine Validierungsentscheidung für den Testversand zu treffen, klicken Sie auf **Gehe zu Testversand** klicken **Finish-Überprüfung** und klicken Sie dann auf eine der verfügbaren Optionen. Folgende Optionen stehen bei der Validierung eines Testversands zur Verfügung: **Genehmigt**, **Genehmigt mit Änderungen**, **Erforderliche Änderungen**, und **Nicht zutreffend**.

      * Nachdem eine Entscheidung über den Testversand getroffen wurde, bleibt der Testversand im Tab Meine Genehmigungen mit dem Text &quot;Entscheidung getroffen&quot;, bis Sie auf die Schaltfläche **Aktualisieren** oder bis Sie die Browser-Seite aktualisieren.

        Informationen zur Überprüfung eines Testversands finden Sie unter [Überprüfen von Testsendungen in Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

   * **Zugriff:** Wählen Sie die Zugriffsstufe aus, die im **Zugriff ändern** Dropdown-Menü, und klicken Sie auf **Zugriff gewähren**. Oder klicken Sie auf **Ignorieren**.

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

1. Klicks **Genehmigen** oder **Ablehnen**, je nachdem, ob Sie den Validierungsprozess genehmigen oder ablehnen möchten.\
   Die Validierungsphase, für die die Genehmigung ausstand, wird nun genehmigt und der Genehmigungsprozess wird in die nächste Phase verschoben. Der Status wird genehmigt, nachdem alle Phasen genehmigt wurden.

## Dokument direkt aus einem Dokument genehmigen 

1. Markieren Sie den Dokumentbereich, der das Dokument enthält, für das Sie eine Genehmigung benötigen.
1. Wählen Sie das Dokument aus und klicken Sie auf **Genehmigen**, **Änderungen** oder **Ablehnen**.\
   ![](assets/approval-approve-document-350x215.png)\
   ![](assets/document-approval-350x199.png)

1. (Optional) Wenn ein Testversand für das Dokument generiert wurde, können Sie das Dokument in der Testversandschnittstelle genehmigen, wie hier beschrieben: [Dokument anhand eines Testversands genehmigen](#approve-a-document-from-a-proof).

## Dokument aus einer Validierungs-E-Mail validieren

Abhängig von Ihren Benachrichtigungseinstellungen erhalten Sie E-Mails, die Sie über Dokumente informieren, für die andere Benutzer eine Validierungsentscheidung treffen müssen. Wenn Sie eine E-Mail mit einer **Genehmigungsentscheidung treffen** können Sie den Validierungsprozess direkt über die E-Mail starten:

1. Klicken Sie in der E-Mail auf **Genehmigungsentscheidung treffen** , um die Seite Dokumentdetails für den Testversand zu öffnen.
1. Führen Sie einen der folgenden Schritte aus, um das Dokument zu überprüfen:

   * Anzeigen der Metadaten zum Dokument.
   * Wenn ein Testversand zur Überprüfung des Dokuments mit Markup und Kommentaren erstellt wurde, klicken Sie auf **Offener Testversand** ![](assets/open-proof-icon-qs.png) in der Nähe der oberen rechten Ecke und überprüfen Sie den Testversand.

     <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

     Informationen zur Überprüfung von Testsendungen finden Sie unter [Überprüfen von Testsendungen in Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Klicken Sie auf **Entscheidung** in der oberen rechten Ecke die Option zum Genehmigen, Genehmigen mit Änderungen oder Ablehnen des Dokuments.

## Dokument anhand eines Testversands genehmigen {#approve-a-document-from-a-proof}

Sie können ein Dokument im Testversand-Viewer genehmigen. Weitere Informationen finden Sie unter [Entscheidungsfindung über einen Testversand im Testversand-Viewer](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) im Artikel [Entscheidungsfindung über einen Testversand im Testversand-Viewer](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).
