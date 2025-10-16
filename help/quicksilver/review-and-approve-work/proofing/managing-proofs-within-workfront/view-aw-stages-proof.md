---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Anzeigen von automatisierten Workflow-Phasen für einen Korrekturabzug
description: Sie können den Fortschritt eines Korrekturabzugs, der mit einem automatisierten Workflow konfiguriert wurde, bequem verfolgen. Sie können die bereits in Phasen des Korrekturabzugs durchgeführten Arbeiten anzeigen, ändern, hinzufügen, starten und sperren.
author: Courtney
feature: Digital Content and Documents
exl-id: 71df1445-c64c-4de2-a9b8-23bd47898b6d
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 1%

---

# Anzeigen von automatisierten Workflow-Phasen für einen Korrekturabzug

Sie können den Fortschritt eines Korrekturabzugs, der mit einem automatisierten Workflow konfiguriert wurde, bequem verfolgen. Sie können die bereits in Phasen des Korrekturabzugs durchgeführten Arbeiten anzeigen, ändern, hinzufügen, starten und sperren.

Informationen zum Hinzufügen von Phasen und Benutzern zu einem Korrekturabzug mit einem automatisierten Workflow finden Sie unter [Hinzufügen von Phasen und Benutzern zu einem automatisierten Workflow mit einem Korrekturabzug](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/add-stages-users-to-automated-workflow-proof.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td>
   <p>Beliebig</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td>
   <p>Standard</p >
   <p>Arbeit oder Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p></td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um herauszufinden, über welchen Plan, welche Rolle oder welches Proof-Berechtigungsprofil Sie verfügen.

+++

## Anzeigen des Diagramms eines automatisierten Workflows

1. Bewegen Sie in einer Dokumentliste, die das Dokument enthält, den Mauszeiger über die Zeile, die das Dokument enthält, und klicken Sie dann auf **Proofing-Workflow**.

   Das Diagramm für den automatisierten Workflow wird direkt unter dem Workflow-Titel angezeigt.

   Die Schritte im Diagramm sind wie folgt gekennzeichnet:

   ![dot.png](assets/dot.png) Aktives Stadium

   ![gray_dot.png](assets/grey-dot.png) Inaktives Stadium\
   ![sbw-key-icon.png](assets/sbw-key-icon.png)  Private Bühne

   ![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)  Gesperrte Phase

   Die Linien zwischen den Stadien stellen die Abhängigkeiten zwischen den Stadien dar. Die Linien, die zu inaktiven Stufen führen, sind gepunktet, bis die Stufe aktiviert ist.

   Sie können den Mauszeiger über eine Phase im Diagramm bewegen, um deren Fortschritt anzuzeigen. Wenn die Phase nicht aktiv ist und Sie Bearbeitungsrechte für die Phase haben, können Sie auf die Schaltfläche Phase aktivieren ![Phase aktivieren](assets/activate-stage-btn.png) klicken, um die Phase zu starten. Wenn die Phase aktiv ist und Sie über Bearbeitungsrechte für die Phase verfügen, können Sie sie sperren. ![Phase sperren](assets/lock-stage-btn.png) Weitere Informationen zur Fortschrittsleiste (S, O, C, D) finden Sie unter  [Fortschritt und Status eines Korrekturabzugs in Workfront Proof anzeigen](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

## Stadium anzeigen

1. Bewegen Sie in einer Dokumentliste, die das Dokument enthält, den Mauszeiger über die Zeile, die das Dokument enthält, und klicken Sie dann auf **Proofing-Workflow**.
1. Klicken Sie im Diagramm auf die Phase, die Sie anzeigen möchten.

   ![Anzeigen des Stadiendiagramms](assets/view-stage-diagram-350x204.png)

1. Um die Details für eine Phase zu erweitern, klicken Sie auf den Pfeil nach der Seite unter dem Namen.

   ![Staging-Details](assets/stage-details-caret-350x167.png)

## Alle Stadien anzeigen

So zeigen Sie alle Phasen eines automatisierten Workflows an:

1. Klicken Sie oben auf der Seite auf die Schaltfläche Ansicht ändern ![Ansicht ändern](assets/change-view-btn.png) und klicken Sie dann auf **Alle Stadien anzeigen**.

   Alle Phasen des automatisierten Workflows werden im Abschnitt aufgelistet, die Details sind jedoch ausgeblendet.

1. Um die Details eines Schritts zu erweitern, klicken Sie auf den Pfeil nach der Seite unter dem Namen.

## Alle Stadien im Detail anzeigen

So zeigen Sie alle Phasen Ihres automatisierten Workflows mit erweiterten Details an:

1. Klicken Sie oben auf der Seite auf die Schaltfläche Ansicht ändern ![Ansicht ändern](assets/change-view-btn.png) und klicken Sie dann auf **Alle Stadien im Detail anzeigen**.
1. Um die Details eines Schritts anzuzeigen, klicken Sie auf den Abwärtspfeil unter dem Namen.
