---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Erstellen eines statischen Korrekturabzugs für eine Website oder andere Web-Inhalte
description: Sie können für Web-Inhalte einen neuen statischen Korrekturabzug oder eine neue Version eines vorhandenen statischen Korrekturabzugs erstellen. Web-Inhalte können Dinge wie Anzeigen mit Streaming-Videos, HTML-Animationen oder interaktiven Bannern enthalten, sie werden jedoch in mehrere Screenshots zerlegt, um ein statisches Proofing zu ermöglichen.
author: Courtney
feature: Digital Content and Documents
exl-id: 1c0511f6-c60b-4a81-bfff-55b6f866add6
source-git-commit: 0a7cdf217d3c8227c569831b16f09c0b1d9c7111
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Erstellen eines statischen Korrekturabzugs für eine Website oder andere Web-Inhalte

Sie können für Web-Inhalte einen neuen statischen Korrekturabzug oder eine neue Version eines vorhandenen statischen Korrekturabzugs erstellen. Web-Inhalte können Dinge wie Anzeigen mit Streaming-Videos, HTML-Animationen oder interaktiven Bannern enthalten, sie werden jedoch in mehrere Screenshots zerlegt, um ein statisches Proofing zu ermöglichen.

Beachten Sie beim Erstellen statischer Korrekturabzüge für eine Website oder andere Web-Inhalte Folgendes:

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
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront Proof-Administrator, um herauszufinden, über welchen Plan, welche Rolle oder welches Proof-Berechtigungsprofil Sie verfügen.

+++

## Erstellen eines statischen Korrekturabzugs für eine Website oder andere Web-Inhalte

Um einen statischen Korrekturabzug zu erstellen, muss die Website öffentlich zugänglich sein (nicht hinter einer Firewall). Andernfalls muss die Zulassungsliste Ihres Unternehmens die Workfront-Domain enthalten. Workfront kann keine kennwortgeschützte Website als statischen Korrekturabzug erfassen.

>[!TIP]
>
>Wir empfehlen interaktives Proofing anstelle von statischem Proofing für interne Seiten, die eine Autorisierung und kennwortgeschützte Seiten erfordern. Weitere Informationen finden Sie unter [Übersicht über Korrekturabzüge für interaktive Inhalte](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Wechseln Sie zum Projekt, zur Aufgabe oder zum Problem, in dem bzw. dem Sie einen neuen Website-Korrekturabzug oder eine neue Version eines vorhandenen Korrekturabzugs erstellen möchten.
1. Klicken Sie **linken** auf Dokumente .
1. (Bedingt) Wenn Sie einen neuen Korrekturabzug erstellen, klicken Sie auf **Neu hinzufügen** und klicken Sie dann im **angezeigten Menü auf** Korrekturabzug.
1. (Bedingt) Wenn Sie eine neue Version eines vorhandenen Korrekturabzugs erstellen:

   1. Bewegen Sie den Mauszeiger über den URL-Korrekturabzug, für den Sie eine neue Version erstellen möchten, und wählen Sie ihn aus, indem Sie in den hellblauen Hintergrund klicken, der ihn umgibt.

      ![Select_proof_by_selector_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)

   1. Klicken Sie **Neu hinzufügen** > **Version** > **Testversand**.

1. Geben Sie die URL der Website, die Sie prüfen möchten, im Bereich **Dateien hinzufügen** ein und drücken Sie dann die **Eingabetaste**.

   >[!NOTE]
   >
   > Die URL darf höchstens 2.000 Zeichen enthalten.

1. Klicken Sie auf die hinzugefügte URL.

   Es werden Optionen zum Konfigurieren des Website-Korrekturabzugs angezeigt.

   ![](assets/interactive-proof-radio-btn-area-350x199.png)

1. (Optional) Wenn Sie den Namen des Korrekturabzugs von der Website-URL in etwas Anderes ändern möchten, geben Sie einen **Korrekturabzugsnamen“**
1. Stellen Sie sicher **dass &quot;**&quot; ausgewählt ist, und verwenden Sie eine der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Auflösung des Screenshots</strong> </td> 
      <td> <p>Passen Sie die Auflösung Ihrer Inhalte an, wenn Prüfer den Korrekturabzug anzeigen, sodass sie sehen können, wie er auf Geräten mit unterschiedlichen Größen wie Smartphones, Tablets und Monitoren angezeigt wird.</p> <p>Wenn Sie mehrere Auflösungen auswählen, wird für jede ausgewählte Auflösung ein separater Korrekturabzug erstellt.</p> <p>Hinweis: Wenn ein Prüfer den Korrekturabzug kommentiert, enthält der Kommentar die Auflösung, aus der hervorgeht, wann der Kommentar abgegeben wurde, sodass andere Prüfer wissen, welche Lösung mit dem Kommentar verbunden ist. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Suchen Sie nach Unterseiten</strong> </td> 
      <td> <p>Erfassen Sie die Unterseiten der Website sowie ihre Hauptseiten. Sie können auf Alle auswählen klicken, um alle Seiten einzubeziehen, oder Sie können nur auf bestimmte Seiten klicken, die einbezogen werden sollen. Mit den Schaltflächen Plus und Minus können Sie die Unterseitenbereiche auf der Website erweitern und schließen.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!IMPORTANT]
   >
   >Sie können die Einstellung „Screenshot erfassen“ für nachfolgende Versionen des von Ihnen erstellten Korrekturabzugs nicht ändern.

1. Klicken Sie **Fertig**.

   Wenn Sie in Schritt 8 mehrere Screenshot-Auflösungen ausgewählt haben, enthält die Liste für jede Auflösung einen Satz von Screenshots. Sie können diese Screenshots als separate Korrekturabzüge generieren oder zu einem einzigen Korrekturabzug kombinieren (siehe  in .). Es wird empfohlen, sie zu kombinieren, insbesondere wenn Sie einen statischen Website-Korrekturabzug erstellen.

   >[!NOTE]
   >
   >Wenn Sie eine neue Version zu einem vorhandenen URL-Korrekturabzug hinzufügen, werden alle Optionen, die für den ursprünglichen Korrekturabzug oder die vorherige Version konfiguriert wurden, in dieser Version beibehalten.

1. Klicken Sie **Korrekturabzug erstellen**, um einen einfachen Korrekturabzug ohne Prüfungsprozess zu erstellen.\
   oder\
   Fahren Sie mit der Konfiguration eines erweiterten Korrekturabzugs fort:

   * [Erstellen eines erweiterten Korrekturabzugs mit einem einfachen Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Erstellen eines erweiterten Korrekturabzugs mit einem automatisierten Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
