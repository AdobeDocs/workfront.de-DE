---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Erstellen eines Korrekturabzugs für interaktive Inhalte in einer ZIP-Datei
description: Sie können einen Korrekturabzug für nicht auf der Website interaktive Inhalte generieren, die in einer ZIP-Datei gespeichert sind. Beispiele für diese Art von Web-Inhalten sind Anzeigen mit Streaming-Video oder Audio, HTML-Animationen, interaktive Banner.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: ac908d52d1538b1ffe7d9bfca94cb9921445633d
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 1%

---

# Erstellen eines Korrekturabzugs für interaktive Inhalte in einer ZIP-Datei

Sie können einen Korrekturabzug für nicht auf der Website interaktive Inhalte generieren, die in einer ZIP-Datei gespeichert sind. Beispiele für diese Art von Web-Inhalten sind Anzeigen mit Streaming-Video oder Audio, HTML-Animationen, interaktive Banner.

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

## Erstellen eines Korrekturabzugs für interaktive Inhalte in einer ZIP-Datei

Nachdem Sie interaktiven Inhalt in einer ZIP-Datei zu einem Korrekturabzug hinzugefügt haben, erstellt Adobe Workfront einen Korrekturabzug der komprimierten Dokumente. Je nach Dateigröße kann die Ladezeit variieren. Die Erstellung größerer Dateien dauert länger. Wenn Sie die Seite verlassen möchten, erstellt Workfront weiterhin die Datei. Die maximale Größe des Datei-Uploads beträgt 4 GB. 

1. Bereiten Sie Ihren Inhalt vor, indem Sie eine ZIP-Datei im Bundle erstellen.

   Die ZIP-Datei muss die folgenden Anforderungen erfüllen:

   * Alle Assets wie CSS, JavaScript, Videos, Sounds und Bilder sollten in der Bundle-Datei enthalten sein.
   * Stellen Sie sicher, dass sich die Hauptdatei (z. B. index.html, index.htm) im Stammordner befindet und dass es sich dabei um die einzige HTML/HTML.htm-Datei handelt, die dort gespeichert ist.

     Wenn die Hauptdatei nicht im Stammordner abgelegt ist, durchsucht Workfront den Ordner nach der Hauptdatei.

   * Die maximale Bundle-Größe beträgt 500 MB.
   * Bei in iOS erstellten ZIP-Dateien erkennt das Tool automatisch den richtigen Ordner, in dem der Inhalt platziert wird.

1. Gehen Sie zum Projekt, zur Aufgabe oder zum Problem, in das bzw. in das Sie die ZIP-Datei hochladen möchten.
1. Klicken Sie **linken** auf Dokumente .
1. Klicken Sie **Neu hinzufügen** und klicken Sie dann **angezeigten Menü auf** Testversand“.
1. Ziehen Sie **Abschnitt „Dateien**&quot; per Drag-and-Drop oder suchen Sie nach der benötigten ZIP-Datei.
1. Klicken Sie **Korrekturabzug erstellen**, um einen einfachen Korrekturabzug ohne Prüfungsprozess zu erstellen.\
   oder\
   Fahren Sie mit der Konfiguration eines erweiterten Korrekturabzugs fort:

   * [Erstellen eines erweiterten Korrekturabzugs mit einem einfachen Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Erstellen eines erweiterten Korrekturabzugs mit einem automatisierten Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
