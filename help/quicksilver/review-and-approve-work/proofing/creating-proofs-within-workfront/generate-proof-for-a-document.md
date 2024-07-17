---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Erstellen eines Testversands für ein Dokument
description: Sie können zum Zeitpunkt des Hochladens auf Workfront einen Testversand für ein Dokument erstellen. Sie können auch einen Testversand für ein bereits in Adobe Workfront hochgeladenes Dokument oder für eine neue Testversion erstellen, die bereits in Workfront verfügbar ist.
author: Courtney
feature: Digital Content and Documents
exl-id: 609e95fa-1fb3-4cc4-9ee8-403fd2f30e10
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 0%

---

# Erstellen eines Testversands für ein Dokument

<!-- Audited: 1/2024 -->

Sie können zum Zeitpunkt des Hochladens auf Workfront einen Testversand für ein Dokument erstellen.

Sie können auch einen Testversand für ein bereits in Adobe Workfront hochgeladenes Dokument oder für eine neue Testversion erstellen, die bereits in Workfront verfügbar ist.

<!--
If a proof fails to generate after following the steps described in the following sections, see [Troubleshoot proof creation failures](../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/troubleshooting-proof-creation-failures.md).
-->

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td> 
   <p>Neu: Beliebig </p>
   <p>Aktuell: Pro oder höher</p> <p>Veralteter Plan: Wählen Sie oder Premium</p> <p>Weitere Informationen zum Testen des Zugriffs mit den verschiedenen Plänen finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testfunktion in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Neu: Standard</p>
   <p>Aktuell : Arbeit oder Plan</p> <p>Veralteter Plan: Beliebig (Sie müssen die Testfunktion für den Benutzer aktiviert haben)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Hochladen eines Dokuments und Erstellen eines Testversands

1. Gehen Sie zum Projekt, zur Aufgabe oder zur Ausgabe, in dem/der Sie einen neuen Testversand erstellen möchten.
1. Klicken Sie auf die Registerkarte **Dokumente**.
1. Klicken Sie im linken Bereich auf Dokumente ![](assets/document-icon.png) .
1. Klicken Sie auf **Neu hinzufügen** und dann im angezeigten Menü auf **Testversand** .

   >[!TIP]
   >
   >Sie können die Einstellung **Testsendungen beim Hochladen von Dokumenten automatisch generieren** in Ihrem Benutzerprofil aktivieren, um diesen Prozess zu automatisieren. Weitere Informationen finden Sie unter [Meine Einstellungen konfigurieren](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md) .

1. Auf der angezeigten Seite **Neuer Testversand** können Sie

   * [Erstellen eines erweiterten Testversands mit einem einfachen Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Erstellen eines erweiterten Testversands mit einem automatisierten Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Hochladen eines Dokuments und Erstellen einer neuen Version eines Testversands

1. Gehen Sie zum Projekt, zur Aufgabe oder zur Ausgabe, in der Sie eine neue Version eines vorhandenen Testversands erstellen möchten.
1. Klicken Sie auf die Registerkarte **Dokumente**.
1. Wählen Sie das Dokument aus, dem Sie eine neue Version hinzufügen möchten.
1. Klicken Sie auf **Neu hinzufügen** > **Version** > **Testversand**.
1. Auf der Seite **Neue Testversion** können Sie

   * [Erstellen eines erweiterten Testversands mit einem einfachen Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Erstellen eines erweiterten Testversands mit einem automatisierten Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Verwenden Sie Drag &amp; Drop, um einen einfachen Testversand für eine neue Version zu erstellen

Sie können ein Dokument aus Ihrem Dateisystem (z. B. Ihrem Desktop) ziehen und ablegen, um einen neuen Testversand oder eine neue Version eines vorhandenen Testversands zu erstellen. Der Testversand enthält die folgenden Einstellungen, je nachdem, ob Sie einen neuen Testversand oder eine neue Version erstellen:

* **Neuer Testversand:** Erstellt einen einfachen Testversand, der nur für Sie freigegeben ist. Sie können die Freigabeeinstellungen ändern, nachdem der Testversand erstellt wurde, wie unter [Testversandeinstellungen bearbeiten](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md) beschrieben.

* **Neue Version des vorhandenen Testversands:** Erstellt eine neue Version mit denselben Testversandeinstellungen wie die vorherige Version.

So erstellen Sie mit Drag &amp; Drop eine neue Testversand- oder Testversion:

1. Stellen Sie sicher, dass Testsendungen so konfiguriert sind, dass sie automatisch generiert werden, wie in beschrieben.
1. Fahren Sie mit  [Dokumente aus Ihrem Dateisystem zu Adobe Workfront hinzufügen](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md), was die Drag-and-Drop-Methode zum Hinzufügen von Dokumenten erklärt. 

## Erstellen eines Testversands für ein vorhandenes Dokument

1. Wechseln Sie zum Projekt, zur Aufgabe oder zur Ausgabe, an der Sie den Testversand durchführen möchten, und klicken Sie dann auf den Abschnitt **Dokumente** .
1. Bewegen Sie den Mauszeiger über das Dokument und klicken Sie dann auf den Link **Testversand erstellen** , der unter dem Dokumentnamen angezeigt wird.

   >[!NOTE]
   >
   >Wenn Sie in Ihrem Benutzerprofil **Testsendungen beim Hochladen von Dokumenten automatisch generieren** aktiviert haben, erstellt das System automatisch einen einfachen Testversand.

1. Wählen Sie eine der folgenden Optionen aus:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Einfacher Testversand</td> 
      <td>Diese Option erstellt einen Testversand ohne angehängten Workflow und wendet die standardmäßigen Testversandeinstellungen an. Sie können die standardmäßigen Testversandeinstellungen aktualisieren oder einen Workflow hinzufügen, nachdem Sie den Testversand erstellt haben. Weitere Informationen zu den Testversandeinstellungen finden Sie unter <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Testversandeinstellungen bearbeiten</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Erweiterter Testversand</td> 
      <td> <p>Mit dieser Option können Sie einen einfachen oder erweiterten Workflow konfigurieren und die Testversandeinstellungen für den von Ihnen erstellten Testversand ändern. Weitere Informationen finden Sie unter </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Erstellen eines erweiterten Testversands mit einem einfachen Workflow</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Erstellen eines erweiterten Testversands mit einem automatisierten Workflow</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
