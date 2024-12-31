---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Anzeigen von automatisierten Workflow-Phasen für einen Korrekturabzug
description: Sie können den Fortschritt eines Korrekturabzugs, der mit einem automatisierten Workflow konfiguriert wurde, bequem verfolgen. Sie können die bereits in Phasen des Korrekturabzugs durchgeführten Arbeiten anzeigen, ändern, hinzufügen, starten und sperren.
author: Courtney
feature: Digital Content and Documents
exl-id: 71df1445-c64c-4de2-a9b8-23bd47898b6d
source-git-commit: f252e3562b8ea73486d407138251b3d15d4b9f3a
workflow-type: tm+mt
source-wordcount: '537'
ht-degree: 0%

---

# Anzeigen von automatisierten Workflow-Phasen für einen Korrekturabzug

Sie können den Fortschritt eines Korrekturabzugs, der mit einem automatisierten Workflow konfiguriert wurde, bequem verfolgen. Sie können die bereits in Phasen des Korrekturabzugs durchgeführten Arbeiten anzeigen, ändern, hinzufügen, starten und sperren.

Informationen zum Hinzufügen von Phasen und Benutzern zu einem Korrekturabzug mit einem automatisierten Workflow finden Sie unter [Hinzufügen von Phasen und Benutzern zu einem automatisierten Workflow mit einem Korrekturabzug](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/add-stages-users-to-automated-workflow-proof.md).

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Legacy-Plan: Auswählen oder Premium</p> <p>Weitere Informationen zum Proofing-Zugriff für die verschiedenen Pläne finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Proofing-Funktionalität in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeits- oder Plan</p> <p>Legacy-Plan: Beliebig (Proofing muss für den Benutzer aktiviert sein)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Informationen zum Anfordern zusätzlicher Zugriffsberechtigungen finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern von Zugriffsberechtigungen für Objekte </a>.</p> </td> 
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

   Sie können den Mauszeiger über eine Phase im Diagramm bewegen, um deren Fortschritt anzuzeigen. Wenn die Phase nicht aktiv ist und Sie über Bearbeitungsrechte für die Phase verfügen, können Sie auf die Schaltfläche Phase aktivieren ![](assets/activate-stage-btn.png) klicken, um die Phase zu starten. Wenn die Phase aktiv ist und Sie über Bearbeitungsrechte für die Phase verfügen, können Sie sie sperren. ![](assets/lock-stage-btn.png) Weitere Informationen über die Fortschrittsleiste (S, O, C, D) finden Sie unter  [Fortschritt und Status eines Korrekturabzugs in Workfront Proof anzeigen](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

## Stadium anzeigen

1. Bewegen Sie in einer Dokumentliste, die das Dokument enthält, den Mauszeiger über die Zeile, die das Dokument enthält, und klicken Sie dann auf **Proofing-Workflow**.
1. Klicken Sie im Diagramm auf die Phase, die Sie anzeigen möchten.

   ![](assets/view-stage-diagram-350x204.png)

1. Um die Details für eine Phase zu erweitern, klicken Sie auf den Pfeil nach der Seite unter dem Namen.

   ![](assets/stage-details-caret-350x167.png)

## Alle Stadien anzeigen

So zeigen Sie alle Phasen eines automatisierten Workflows an:

1. Klicken Sie oben auf der ![](assets/change-view-btn.png) auf die Schaltfläche Ansicht ändern und dann auf **Alle Stadien anzeigen**.

   Alle Phasen des automatisierten Workflows werden im Abschnitt aufgelistet, die Details sind jedoch ausgeblendet.

1. Um die Details eines Schritts zu erweitern, klicken Sie auf den Pfeil nach der Seite unter dem Namen.

## Alle Stadien im Detail anzeigen

So zeigen Sie alle Phasen Ihres automatisierten Workflows mit erweiterten Details an:

1. Klicken Sie oben auf der ![](assets/change-view-btn.png) auf die Schaltfläche Ansicht ändern und dann auf **Alle Stadien im Detail anzeigen**.
1. Um die Details eines Schritts anzuzeigen, klicken Sie auf den Abwärtspfeil unter dem Namen.
