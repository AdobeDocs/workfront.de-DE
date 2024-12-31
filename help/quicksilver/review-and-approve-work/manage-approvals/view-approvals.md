---
product-area: projects
navigation-topic: approvals
title: Genehmigungen anzeigen
description: Genehmigungsprozesse bieten die Flexibilität, mehrstufige Genehmigungen für Projekte, Aufgaben und Probleme zu erstellen. Adobe Workfront-Administratoren definieren Genehmigungsprozesse, um im gesamten System für Konsistenz zu sorgen.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 1071e456-f111-4c52-b13a-ac1113f69cec
source-git-commit: b0b83e8a8a2a076ec20691183605e3d25d10129d
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Genehmigungen anzeigen

Genehmigungsprozesse bieten die Flexibilität, mehrstufige Genehmigungen für Projekte, Aufgaben und Probleme zu erstellen. Adobe Workfront-Administratoren definieren Genehmigungsprozesse, um im gesamten System für Konsistenz zu sorgen.

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

Sie können Validierungen aus verschiedenen Bereichen von Workfront anzeigen oder verwalten. Informationen zum Verwalten von Validierungen in verschiedenen Bereichen finden Sie unter [Genehmigen von ](../../review-and-approve-work/manage-approvals/approving-work.md).

Sie können Validierungen aus den folgenden Bereichen anzeigen oder verwalten:

* Im Bereich Home

   * Alle Projekte, Aufgaben, Probleme, Arbeitszeittabellen, Dokumente und Zugriffsberechtigungen, die auf Ihre Genehmigung warten, werden im Widget Meine Genehmigungen im Bereich Startseite angezeigt.
   * Genehmigungen, die Sie selbst gesendet haben, werden auch im Widget Meine Genehmigungen im Bereich Startseite angezeigt, wenn Sie die Filteroption Von mir gesendete Genehmigungen auswählen. Weitere Informationen finden Sie im Abschnitt [Prüfungsarbeit, die Sie im Bereich Startseite zur Genehmigung einreichen](#review-work-you-submit-for-approval-in-the-home-area) dieses Artikels.
   * Genehmigungen werden aus dem Widget Meine Genehmigungen im Bereich Startseite entfernt, wenn das zugehörige Projekt, die zugehörige Aufgabe oder das zugehörige Problem als „Gelöst“, „Gesperrt“, „Geschlossen“ oder „Abgebrochen“ gekennzeichnet ist.

  Informationen zur Verwendung der Startseite finden Sie unter [Erste Schritte mit der Startseite](../../workfront-basics/using-home/using-the-home-area/get-started-with-home.md).

* In der Kopfzeile eines Projekts, einer Aufgabe, eines Problems, eines Dokuments oder eines Korrekturabzugs
* Im Abschnitt Genehmigungen eines Projekts, einer Aufgabe oder eines Problems
* In einem Bericht

  >[!NOTE]
  >
  >Sie können keine Entscheidung über eine Genehmigung anhand eines Berichts treffen.

  Sie können einen Projekt-, Aufgaben-, Problem- oder Dokumentgenehmigungsbericht erstellen, der Genehmigungsinformationen enthält.

  Informationen zum Erstellen von Berichten finden Sie [Erstellen eines benutzerdefinierten Berichts](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Prüfungsarbeit, die zur Genehmigung im Bereich Startseite eingereicht wird {#review-work-you-submit-for-approval-in-the-home-area}

1. Klicken Sie oben rechts auf **[!UICONTROL Hauptmenü]** ![](assets/main-menu-icon.png) und dann auf **[!UICONTROL Home]**.
1. (Bedingt) Klicken Sie auf **Anpassen**, um das Widget **Meine Genehmigungen** hinzuzufügen.
1. (Bedingt) Klicken Sie auf das **Filter** Dropdown-Menü und wählen Sie **Von mir gesendete Genehmigungen** aus, um die von Ihnen gesendeten Genehmigungen anzuzeigen.


## Anzeigen des Genehmigungsstatus eines Objekts

Sie können den Genehmigungsstatus eines Objekts in den folgenden Abschnitten des Objekts einsehen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Updates </td> 
   <td> <p>Zeigt alle Genehmigungsstatus an, wenn sie auftreten. Der Genehmigungsstatus wird zusammen mit anderen Status im Abschnitt <strong>Updates</strong> angezeigt.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Genehmigungen</td> 
   <td> <p>Zeigt detailliertere Informationen zum Genehmigungsprozess an, z. B. jede Phase des Genehmigungsprozesses und ob die genehmigenden Personen die Genehmigung erteilt haben.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Im Bereich Aktualisierungen können Sie einen Genehmigungsstatus anzeigen {#use-the-updates-area-to-view-an-approval-status}

Wenn eine Genehmigung für ein Projekt, eine Aufgabe oder ein Problem initiiert wird, wird auf der Registerkarte **Aktualisierungen** des Objekts ein Status angezeigt, der den Genehmigungsstatus angibt. Ein neuer Status wird immer dann angezeigt, wenn das Objekt den Genehmigungsprozess durchläuft. Dazu gehören die folgenden Ereignisse:

* Für ein Objekt wird ein Genehmigungsprozess gestartet. Der Genehmigungsprozess wird gestartet, wenn der Status geändert wird.
* Das Objekt wird abgelehnt
* Das Objekt wurde genehmigt

>[!TIP]
>
>Wenn eine Genehmigung auf eine Aufgabe angewendet wird, werden die Genehmigungsaktualisierungen auf der Registerkarte Aktualisierungen der Aufgabe angezeigt und nicht auf der Registerkarte Aktualisierungen des Projekts, in dem sich die Aufgabe befindet.

### Im Bereich Genehmigungen können Sie einen Genehmigungsstatus anzeigen. {#use-the-approvals-area-to-view-an-approval-status}

Sie erhalten Einblick in die Position einer Aufgabe oder eines Problems, an der bzw. dem Sie gerade arbeiten, im Genehmigungsprozess. Sie können die folgenden Informationen anzeigen:

* Die Phase des Genehmigungsprozesses
* Welche genehmigenden Personen haben es bereits genehmigt?
* Welche genehmigenden Personen haben es noch nicht genehmigt?

So zeigen Sie den aktuellen Status an, in dem sich eine Aufgabe oder ein Problem im Genehmigungsprozess befindet:

1. Zu dem Projekt, der Aufgabe oder dem Problem gehen, mit dem/dem die Genehmigung verknüpft ist.
1. Klicken Sie im linken Bedienfeld auf **Genehmigungen**. Möglicherweise müssen Sie zunächst auf &quot;**anzeigen“**.

   Die Registerkarte Genehmigungen enthält vollständige Informationen zu allen früheren Genehmigungspfaden und -schritten. Sie können genau sehen, wer eine Entscheidung über die Genehmigung getroffen hat oder ob die Genehmigung für ein Team, ein Aufgabengebiet oder einen Benutzer festgelegt ist.

   ![](assets/approvals-tab-expanded-on-issue-nwe-350x320.png)

   Weitere Informationen zum Erstellen eines Genehmigungsprozesses finden Sie unter [Erstellen eines Genehmigungsprozesses für Arbeitselemente](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
