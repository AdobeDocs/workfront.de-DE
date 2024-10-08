---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Erstellen eines statischen Testversands für eine Website oder andere Webinhalte
description: Sie können einen neuen statischen Testversand oder eine neue Version eines vorhandenen statischen Testversands für Webinhalte erstellen. Webinhalte können Dinge wie Anzeigen mit Streaming-Videos, HTML-Animationen oder interaktiven Bannern enthalten, sie werden jedoch in mehrere Screenshots unterteilt, um statische Testsendungen zu ermöglichen.
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: 0a7cdf217d3c8227c569831b16f09c0b1d9c7111
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Erstellen eines statischen Testversands für eine Website oder andere Webinhalte

Sie können einen neuen statischen Testversand oder eine neue Version eines vorhandenen statischen Testversands für Webinhalte erstellen. Webinhalte können Dinge wie Anzeigen mit Streaming-Videos, HTML-Animationen oder interaktiven Bannern enthalten, sie werden jedoch in mehrere Screenshots unterteilt, um statische Testsendungen zu ermöglichen.

Beachten Sie beim Erstellen von statischen Testsendungen für eine Website oder andere Webinhalte Folgendes:

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Veralteter Plan: Wählen Sie oder Premium</p> <p>Weitere Informationen zum Testen des Zugriffs mit den verschiedenen Plänen finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testfunktion in Workfront</a>.</p> </td> 
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

+++

## Erstellen eines statischen Testversands für eine Website oder andere Webinhalte

Um einen statischen Testversand zu erstellen, muss die Website öffentlich zugänglich sein (nicht hinter einer Firewall) oder die Zulassungsliste Ihres Unternehmens muss die Workfront-Domäne enthalten. Workfront kann eine kennwortgeschützte Website nicht als statischen Testversand erfassen.

>[!TIP]
>
>Für interne Seiten, für die eine Autorisierung und kennwortgeschützte Seiten erforderlich sind, empfehlen wir interaktive Testsendungen anstelle statischer Testsendungen. Weitere Informationen finden Sie unter [Übersicht über interaktive Inhaltsanalysen](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Gehen Sie zum Projekt, zur Aufgabe oder zur Ausgabe, in der Sie einen neuen Website-Testversand oder eine neue Version eines vorhandenen erstellen möchten.
1. Klicken Sie im linken Bereich auf **Dokumente** .
1. (Bedingt) Wenn Sie einen neuen Testversand erstellen, klicken Sie auf **Neu hinzufügen** und dann im angezeigten Menü auf **Testversand** .
1. (Bedingt) Wenn Sie eine neue Version eines vorhandenen Testversands erstellen:

   1. Bewegen Sie den Mauszeiger über den URL-Testversand, für den Sie eine neue Version erstellen möchten, und wählen Sie ihn aus, indem Sie im hellblauen Hintergrund darauf klicken.

      ![Select_proof_by_selection_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. Klicken Sie auf **Neu hinzufügen** > **Version** > **Testversand**.

1. Geben Sie die URL der Website, die Sie testen möchten, in den Bereich **Dateien hinzufügen** ein und drücken Sie dann die Eingabetaste **3}.**

   >[!NOTE]
   >
   > Die URL darf maximal 2.000 Zeichen enthalten.

1. Klicken Sie auf die von Ihnen hinzugefügte URL.

   Optionen zum Konfigurieren des Website-Testversands werden angezeigt.

   ![](assets/interactive-proof-radio-btn-area-350x199.png)

1. (Optional) Wenn Sie den Namen des Testversands aus der Website-URL in einen anderen Namen ändern möchten, geben Sie einen **Testversand-Namen** ein.
1. Stellen Sie sicher, dass **Screenshot &quot;Aufnahme&quot;** ausgewählt ist, und verwenden Sie eine der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Screenshot-Auflösung</strong> </td> 
      <td> <p>Passen Sie die Auflösung Ihres Inhalts an, wenn die Prüfer den Testversand anzeigen. So können sie sehen, wie er auf Geräten unterschiedlicher Größe wie Smartphones, Tablets und Monitoren angezeigt wird.</p> <p>Wenn Sie mehrere Auflösungen auswählen, wird für jede ausgewählte Auflösung ein separater Testversand erstellt.</p> <p>Hinweis: Wenn ein Validierer den Testversand kommentiert, enthält der Kommentar die Auflösung, die anzeigt, wann der Kommentar abgegeben wurde, damit andere Validierer wissen, welche Auflösung mit dem Kommentar verknüpft ist. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Suchen nach Unterseiten</strong> </td> 
      <td> <p>Erfassen Sie die Unterseiten der Website sowie deren Hauptseiten. Sie können auf Alle auswählen klicken, um alle Seiten einzuschließen, oder Sie können nur auf bestimmte Seiten klicken, die eingeschlossen werden sollen. Mit den Plus- und Minusschaltflächen können Sie die Unterseitenbereiche auf der Website erweitern und schließen.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Sie können die Screenshot-Einstellung &quot;Aufnahme&quot;für keine nachfolgenden Versionen des von Ihnen erstellten Testversands ändern.

1. Klicken Sie auf **Fertig**.

   Wenn Sie in Schritt 8 mehrere Screenshot-Auflösungen ausgewählt haben, enthält die Liste eine Reihe von Screenshots für jede Auflösung. Sie können diese Screenshots als separate Testsendungen erstellen oder sie zu einem Testversand zusammenführen (siehe  in .). Es wird empfohlen, diese zu kombinieren, insbesondere wenn Sie einen statischen Website-Testversand erstellen.

   >[!NOTE]
   >
   >Wenn Sie eine neue Version zu einem vorhandenen URL-Testversand hinzufügen, werden alle Optionen, die für den ursprünglichen Testversand oder die vorherige Version konfiguriert wurden, in dieser Version beibehalten.

1. Klicken Sie auf **Testversand erstellen** , um einen einfachen Testversand ohne Überprüfungsprozess zu erstellen.\
   oder\
   Fahren Sie mit der Konfiguration eines erweiterten Testversands fort:

   * [Erstellen eines erweiterten Testversands mit einem einfachen Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Erstellen eines erweiterten Testversands mit einem automatisierten Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
