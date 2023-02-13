---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Anzeigen von automatisierten Workflow-Phasen auf einem Testversand
description: Sie können den Fortschritt eines mit einem automatisierten Workflow konfigurierten Testversands bequem verfolgen. Sie können die bereits auf Bühnen des Testversands durchgeführten Arbeiten anzeigen, ändern, hinzufügen, starten und sperren.
author: Courtney
feature: Digital Content and Documents
exl-id: 71df1445-c64c-4de2-a9b8-23bd47898b6d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# Anzeigen von automatisierten Workflow-Phasen auf einem Testversand

Sie können den Fortschritt eines mit einem automatisierten Workflow konfigurierten Testversands bequem verfolgen. Sie können die bereits auf Bühnen des Testversands durchgeführten Arbeiten anzeigen, ändern, hinzufügen, starten und sperren.

Informationen zum Hinzufügen von Bühnen und Benutzern zu einem Testversand mit einem automatisierten Workflow finden Sie unter [Hinzufügen von Bühnen und Benutzern zu einem automatisierten Workflow auf einem Testversand](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/add-stages-users-to-automated-workflow-proof.md).

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Veralteter Plan: Select oder Premium</p> <p>Weitere Informationen zum Testzugang für die verschiedenen Pläne finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testversandfunktion in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeit oder Plan</p> <p>Veralteter Plan: Beliebig (Sie müssen die Testversandfunktion für den Benutzer aktiviert haben)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Zugriff auf Objekte anfordern </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront-Testversandadministrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Testberechtigung Sie haben.

## Anzeigen des Diagramms &quot;Automatisierter Workflow&quot;

1. Bewegen Sie in einer Dokumentliste, die das Dokument enthält, den Mauszeiger über die das Dokument enthaltende Zeile und klicken Sie auf **Testversand-Workflow**.

   Das Diagramm für den automatisierten Workflow wird direkt unter dem Workflow-Titel angezeigt.

   Die Phasen im Diagramm sind wie folgt gekennzeichnet:

   ![dot.png](assets/dot.png) Aktive Phase

   ![gray_dot.png](assets/grey-dot.png) Inaktive Phase\
   ![sbw-key-icon.png](assets/sbw-key-icon.png)  Private Bühne

   ![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)  Gesperrte Phase

   Die Linien zwischen den Bühnen zeigen die Abhängigkeiten zwischen den Bühnen an. Die Linien, die zu inaktiven Bühnen führen, werden gepunktet, bis die Bühne aktiviert ist.

   Sie können den Mauszeiger über eine Phase im Diagramm bewegen, um den Fortschritt anzuzeigen. Wenn die Bühne nicht aktiv ist und Sie Bearbeitungsrechte auf der Bühne haben, können Sie auf die Schaltfläche &quot;Bühne aktivieren&quot;klicken ![](assets/activate-stage-btn.png) um die Bühne zu starten. Wenn die Bühne aktiv ist und Sie Bearbeitungsrechte auf der Bühne haben, können Sie sie sperren. ![](assets/lock-stage-btn.png) Weitere Informationen zur Fortschrittsleiste (S, O, C, D) finden Sie unter  [Anzeigen von Fortschritt und Status eines Testversands in Workfront Testversand](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

## Bühne anzeigen

1. Bewegen Sie in einer Dokumentliste, die das Dokument enthält, den Mauszeiger über die das Dokument enthaltende Zeile und klicken Sie auf **Testversand-Workflow**.
1. Klicken Sie im Diagramm auf die Bühne, die Sie anzeigen möchten.

   ![](assets/view-stage-diagram-350x204.png)

1. Um die Details für eine Bühne zu erweitern, klicken Sie auf den Seitenpfeil unter ihrem Namen.

   ![](assets/stage-details-caret-350x167.png)

## Alle Phasen anzeigen

So zeigen Sie alle Phasen in einem automatisierten Workflow an:

1. Klicken Sie oben auf der Seite auf die Schaltfläche Ansicht ändern . ![](assets/change-view-btn.png)Klicken Sie auf **Alle Phasen anzeigen**.

   Alle Phasen des automatisierten Workflows werden im Abschnitt aufgelistet, die Details sind jedoch ausgeblendet.

1. Um die Details einer Bühne zu erweitern, klicken Sie auf den Seitenpfeil unter ihrem Namen.

## Detailansicht aller Bühnen

So zeigen Sie alle Phasen Ihres automatisierten Workflows mit erweiterten Details an:

1. Klicken Sie oben auf der Seite auf die Schaltfläche Ansicht ändern . ![](assets/change-view-btn.png)Klicken Sie auf **Detailansicht aller Bühnen**.
1. Um die Details einer Bühne anzuzeigen, klicken Sie auf den Pfeil nach unten unter ihrem Namen.
