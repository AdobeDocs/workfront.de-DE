---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Erstellen eines interaktiven Testversands für eine Website oder einen anderen Webinhalt
description: Sie können einen neuen interaktiven Testversand oder eine neue Version eines vorhandenen interaktiven Testversands für Webinhalte erstellen. Dabei kann es sich um eine Website oder andere interaktive Inhalte handeln, z. B. Anzeigen mit Streaming-Video oder -Audio, HTML-Animationen und interaktive Banner.
author: Courtney
feature: Digital Content and Documents
exl-id: 56e5eeea-1ab9-43c8-bc84-d10638171871
source-git-commit: 35d76d3cb06c9e9b449844f304f1443e24a221d4
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# Erstellen eines interaktiven Testversands für eine Website oder einen anderen Webinhalt

Sie können einen neuen interaktiven Testversand oder eine neue Version eines vorhandenen interaktiven Testversands für Webinhalte erstellen. Dabei kann es sich um eine Website oder andere interaktive Inhalte handeln, z. B. Anzeigen mit Streaming-Video oder -Audio, HTML-Animationen und interaktive Banner.

In einem interaktiven Testversand können Prüfer wie gewohnt mit der Website oder anderen Webinhalten navigieren und interagieren.

>[!IMPORTANT]
>
>Stellen Sie sicher, dass die Website oder der interaktive Inhalt für die Personen zugänglich ist, die ihn überprüfen werden. Sie können nur dann im Testversand darauf zugreifen, wenn sie auch über das Internet darauf zugreifen können.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Veralteter Plan: Premium</p> <p>Weitere Informationen zum Testen des Zugriffs mit den verschiedenen Plänen finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testfunktion in Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Aktueller Plan: Arbeit oder Plan</p> <p>Veralteter Plan: Beliebig (Sie müssen die Testfunktion für den Benutzer aktiviert haben)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Testberechtigung Sie haben.

## Erstellen eines interaktiven Testversands für eine Website oder einen anderen Webinhalt

1. Gehen Sie zum Projekt, zur Aufgabe oder zur Ausgabe, in der Sie einen neuen Website-Testversand oder eine neue Version eines vorhandenen erstellen möchten.
1. Klicken Sie im linken Bereich auf **Dokumente** .
1. (Bedingt) Wenn Sie einen neuen Testversand erstellen, klicken Sie auf **Neu hinzufügen** und dann im angezeigten Menü auf **Testversand** .

1. (Bedingt) Wenn Sie eine neue Version eines vorhandenen Testversands erstellen, wird auf der Seite **Neuer Testversand** angezeigt:

   1. Bewegen Sie den Mauszeiger über den URL-Testversand, für den Sie eine neue Version erstellen möchten, und wählen Sie ihn aus, indem Sie im hellblauen Hintergrund darauf klicken.

      ![Select_proof_by_selection_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)


   1. Klicken Sie in der Dropdown-Liste **Neu hinzufügen** auf **Version** > **Testversand**.

1. Geben Sie im Abschnitt **Dateien hinzufügen** die URL der Website ein, die Sie testen möchten, und drücken Sie dann die Eingabetaste **3}.**  Sie können diesen Vorgang wiederholen, um mehrere Websites hinzuzufügen, die getestet werden sollen.

   ![proof_website.png](assets/proof-website-350x65.png)


   >[!NOTE]
   >
   > Die URL darf maximal 1.000 Zeichen enthalten.

1. Klicken Sie auf die von Ihnen hinzugefügte URL.

   ![](assets/click-url-350x137.png)

1. (Optional) Wenn Sie den Namen des Testversands aus der Website-URL in etwas Anderes ändern möchten, geben Sie einen **Testversand-Namen** ein.
1. Wählen Sie **Interaktiv** und klicken Sie dann auf **Fertig**.

   >[!NOTE]
   >
   >Wenn Sie eine neue Version zu einem vorhandenen URL-Testversand hinzufügen, werden alle Optionen, die für den ursprünglichen Testversand oder die vorherige Version konfiguriert wurden, in dieser Version beibehalten.

1. Klicken Sie auf **Testversand erstellen** , um einen einfachen Testversand ohne Überprüfungsprozess zu erstellen.\
   oder\
   Fahren Sie mit der Konfiguration eines erweiterten Testversands fort:

   * [Erstellen eines erweiterten Testversands mit einem einfachen Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Erstellen eines erweiterten Testversands mit einem automatisierten Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
