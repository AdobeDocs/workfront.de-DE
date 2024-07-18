---
product-area: projects
navigation-topic: approvals
title: Anzeigen von Genehmigungen
description: Genehmigungsprozesse bieten die Flexibilität, mehrstufige Genehmigungen für Projekte, Aufgaben und Probleme zu erstellen. Adobe Workfront-Administratoren definieren Validierungsprozesse, die im gesamten System konsistent sind.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 1071e456-f111-4c52-b13a-ac1113f69cec
source-git-commit: c6e3e3d8d4fd6b6916c8fd49983bc3572949acaa
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 0%

---

# Anzeigen von Genehmigungen

Genehmigungsprozesse bieten die Flexibilität, mehrstufige Genehmigungen für Projekte, Aufgaben und Probleme zu erstellen. Adobe Workfront-Administratoren definieren Validierungsprozesse, die im gesamten System konsistent sind.

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

Sie können Genehmigungen in verschiedenen Bereichen von Workfront anzeigen oder verwalten. Informationen zum Verwalten von Genehmigungen in verschiedenen Bereichen finden Sie unter [Arbeiten genehmigen](../../review-and-approve-work/manage-approvals/approving-work.md).

Sie können Genehmigungen in den folgenden Bereichen anzeigen oder verwalten:

* Im Startbereich

   * Alle Projekte, Aufgaben, Probleme, Timesheets, Dokumente und Zugriffe, die auf Ihre Genehmigung warten, werden im Bereich Startseite angezeigt, wenn Sie Alle oder Genehmigungen anzeigen.
   * Genehmigungen, die Sie selbst eingereicht haben, werden auch im Bereich &quot;Startseite&quot;im Abschnitt &quot;Von mir gesendete Genehmigungen&quot;der Arbeitsliste angezeigt. Weitere Informationen finden Sie im Abschnitt [Arbeiten zur Überprüfung, die Sie zur Genehmigung im Startbereich einreichen](#review-work-you-submit-for-approval-in-the-home-area) in diesem Artikel.
   * Genehmigungen werden aus dem Startbereich entfernt, wenn das zugehörige Projekt, die Aufgabe oder das Problem mit &quot;Gelöst&quot;, &quot;Auf Halten&quot;, &quot;Geschlossen&quot;oder &quot;Abgebrochen&quot;markiert ist.

  Informationen zur Verwendung von Home finden Sie unter [Erste Schritte mit Home](../../workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

* In der Kopfzeile eines Projekts, einer Aufgabe, eines Problems, eines Dokuments oder eines Testversands
* Im Abschnitt Genehmigungen eines Projekts, einer Aufgabe oder eines Problems
* In einem Bericht

  >[!NOTE]
  >
  >Sie können keine Entscheidung über eine Genehmigung aus einem Bericht treffen.

  Sie können einen Projekt-, Aufgaben-, Problem- oder Dokumentgenehmigungsbericht erstellen, der Validierungsinformationen enthält.

  Informationen zum Erstellen von Berichten finden Sie unter [Benutzerdefinierten Bericht erstellen](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Überprüfen Sie die Arbeit, die Sie zur Genehmigung im Startbereich einreichen. {#review-work-you-submit-for-approval-in-the-home-area}

1. Klicken Sie oben links in Adobe Workfront auf das Symbol **Startseite** ![](assets/home-icon-30x29.png) .

   >[!NOTE]
   >
   >Ihr Workfront-Administrator kann die folgenden Änderungen am Startseiten-Symbol in Ihrer Umgebung vornehmen:
   >
   >* Ersetzen Sie sie durch ein Bild, das zur Veranschaulichung Ihrer Organisation angepasst wurde. In diesem Fall sieht das Symbol anders aus als in diesem Artikel.
   >* Ersetzen Sie die verknüpfte Seite durch eine andere Seite. Klicken Sie in diesem Fall auf das **Hauptmenü** ![](assets/main-menu-icon.png) in der oberen rechten Ecke der Seite und klicken Sie dann auf **Startseite**.

1. Wählen Sie **Arbeitsliste**, klicken Sie dann auf das Dropdown-Menü **Filter** und wählen Sie **Genehmigungen** aus.
1. Erweitern Sie den Abschnitt **Gesendete Genehmigungen** und suchen Sie nach den von Ihnen gesendeten Genehmigungen.

   ![](assets/approvals-submitted-section-in-home-nwe-350x401.png)

## Genehmigungsstatus eines Objekts anzeigen

Sie können den Genehmigungsstatus eines Objekts in den folgenden Abschnitten des Objekts anzeigen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Updates </td> 
   <td> <p>Zeigt alle Genehmigungsstatus an, wenn sie auftreten. Der Genehmigungsstatus wird entsprechend den anderen Status angezeigt, die im Abschnitt <strong>Aktualisierungen</strong> angezeigt werden.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Genehmigungen</td> 
   <td> <p>Enthält detailliertere Informationen zum Genehmigungsprozess, z. B. zu den einzelnen Phasen des Genehmigungsprozesses und dazu, ob Genehmiger die Genehmigung erteilt haben.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Im Bereich Updates können Sie einen Genehmigungsstatus anzeigen. {#use-the-updates-area-to-view-an-approval-status}

Wenn eine Genehmigung für ein Projekt, eine Aufgabe oder ein Problem eingeleitet wird, wird auf der Registerkarte **Aktualisierungen** des Objekts ein Status angezeigt, der den Genehmigungsstatus angibt. Ein neuer Status wird immer dann angezeigt, wenn das Objekt durch den Genehmigungsprozess wechselt. Dazu gehören die folgenden Ereignisse:

* Ein Genehmigungsprozess wird für ein Objekt eingeleitet. Der Validierungsprozess wird bei Änderung des Status eingeleitet.
* Das Objekt wird zurückgewiesen
* Das Objekt wird genehmigt

>[!TIP]
>
>Wenn eine Validierung auf eine Aufgabe angewendet wird, werden die Validierungsaktualisierungen auf dem Tab Aktualisierungen der Aufgabe und nicht auf dem Tab Aktualisierungen des Projekts angezeigt, in dem sich die Aufgabe befindet.

### Verwenden Sie den Bereich Genehmigungen , um einen Genehmigungsstatus anzuzeigen. {#use-the-approvals-area-to-view-an-approval-status}

Sie können sehen, wo sich eine Aufgabe oder ein Problem, an der Sie derzeit arbeiten, im Genehmigungsprozess befindet. Sie können die folgenden Informationen sehen:

* Phase des Genehmigungsverfahrens
* Welche Genehmiger haben sie bereits genehmigt?
* Welche Genehmiger haben sie noch nicht genehmigt?

So zeigen Sie den aktuellen Status an, an dem sich eine Aufgabe oder ein Problem im Genehmigungsprozess befindet:

1. Gehen Sie zum Projekt, zur Aufgabe oder zum Problem, mit dem die Genehmigung verknüpft ist.
1. Klicken Sie im linken Bereich auf **Genehmigungen**. Möglicherweise müssen Sie zuerst auf **Mehr anzeigen** klicken.

   Auf der Registerkarte Genehmigungen werden alle Informationen zu allen bisherigen Genehmigungspfaden und -phasen angezeigt. Sie können genau sehen, wer eine Entscheidung über die Genehmigung getroffen hat oder ob die Genehmigung für ein Team, eine Rolle oder einen Benutzer festgelegt wurde.

   ![](assets/approvals-tab-expanded-on-issue-nwe-350x320.png)

   Informationen zum Erstellen eines Genehmigungsprozesses finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
