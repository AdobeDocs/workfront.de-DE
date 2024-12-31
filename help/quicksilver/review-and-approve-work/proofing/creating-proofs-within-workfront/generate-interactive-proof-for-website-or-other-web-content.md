---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Erstellen eines interaktiven Korrekturabzugs für eine Website oder andere Web-Inhalte
description: Sie können für Web-Inhalte einen neuen interaktiven Korrekturabzug oder eine neue Version eines vorhandenen interaktiven Korrekturabzugs erstellen. Dabei kann es sich um eine Website oder andere Arten interaktiver Inhalte handeln, z. B. Anzeigen mit Streaming-Video oder Audio, HTML-Animationen und interaktiven Bannern.
author: Courtney
feature: Digital Content and Documents
exl-id: 56e5eeea-1ab9-43c8-bc84-d10638171871
source-git-commit: ac908d52d1538b1ffe7d9bfca94cb9921445633d
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

# Erstellen eines interaktiven Korrekturabzugs für eine Website oder andere Web-Inhalte

Sie können für Web-Inhalte einen neuen interaktiven Korrekturabzug oder eine neue Version eines vorhandenen interaktiven Korrekturabzugs erstellen. Dabei kann es sich um eine Website oder andere Arten interaktiver Inhalte handeln, z. B. Anzeigen mit Streaming-Video oder Audio, HTML-Animationen und interaktiven Bannern.

Bei einem interaktiven Korrekturabzug können Reviewer wie gewohnt mit der Website oder anderen Web-Inhalten navigieren und interagieren.

>[!IMPORTANT]
>
>Stellen Sie sicher, dass die Website oder der interaktive Inhalt für die Personen zugänglich ist, die sie überprüfen werden. Sie können beim Proofing nur darauf zugreifen, wenn sie auch im Internet darauf zugreifen können.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Legacy-Plan: Premium</p> <p>Weitere Informationen zum Proofing-Zugriff für die verschiedenen Pläne finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Proofing-Funktionalität in Workfront</a>.</p> </td> 
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
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um herauszufinden, über welchen Plan, welche Rolle oder welches Proof-Berechtigungsprofil Sie verfügen.

+++

## Erstellen eines interaktiven Korrekturabzugs für eine Website oder andere Web-Inhalte

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, in dem bzw. dem Sie einen neuen Website-Korrekturabzug oder eine neue Version eines vorhandenen Korrekturabzugs erstellen möchten.
1. Klicken Sie **linken** auf „Dokumente“.
1. (Bedingt) Wenn Sie einen neuen Korrekturabzug erstellen, klicken Sie auf **Neu hinzufügen** und klicken Sie dann im **angezeigten Menü auf** Korrekturabzug.

1. (Bedingt) Auf der Seite **Neuer Korrekturabzug** wird angezeigt, wenn Sie eine neue Version eines vorhandenen Korrekturabzugs erstellen:

   1. Bewegen Sie den Mauszeiger über den URL-Korrekturabzug, für den Sie eine neue Version erstellen möchten, und wählen Sie ihn aus, indem Sie in den hellblauen Hintergrund klicken, der ihn umgibt.

      ![Select_proof_by_selector_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)


   1. Klicken **in der Dropdown** Liste Neu hinzufügen“ auf **Version** > **Testversand**.

1. Geben **im Abschnitt „Dateien hinzufügen** die URL der Website ein, die Sie prüfen möchten, und drücken Sie dann die **Eingabetaste**.  Sie können diesen Vorgang wiederholen, um mehrere Websites zum Testversand hinzuzufügen.

   ![proof_website.png](assets/proof-website-350x65.png)


   >[!NOTE]
   >
   > Die URL darf höchstens 1.000 Zeichen enthalten.

1. Klicken Sie auf die hinzugefügte URL.

   ![](assets/click-url-350x137.png)

1. (Optional) Wenn Sie den Namen des Korrekturabzugs von der Website-URL in etwas Anderes ändern möchten, geben Sie einen **Korrekturabzugsnamen“**.
1. Wählen Sie **Interaktiv** aus und klicken Sie dann auf **Fertig**.

   >[!NOTE]
   >
   >Wenn Sie eine neue Version zu einem vorhandenen URL-Korrekturabzug hinzufügen, werden alle Optionen, die für den ursprünglichen Korrekturabzug oder die vorherige Version konfiguriert wurden, in dieser Version beibehalten.

1. Klicken Sie **Korrekturabzug erstellen**, um einen einfachen Korrekturabzug ohne Prüfungsprozess zu erstellen.\
   oder\
   Fahren Sie mit der Konfiguration eines erweiterten Korrekturabzugs fort:

   * [Erstellen eines erweiterten Korrekturabzugs mit einem einfachen Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Erstellen eines erweiterten Korrekturabzugs mit einem automatisierten Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
