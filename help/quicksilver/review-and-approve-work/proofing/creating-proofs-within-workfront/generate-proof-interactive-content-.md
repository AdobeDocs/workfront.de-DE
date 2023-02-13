---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Erstellen eines Testversands für interaktive Inhalte in einer ZIP-Datei
description: Sie können einen Testversand für interaktive Inhalte erstellen, die nicht auf einer Website gespeichert sind und in einer ZIP-Datei gespeichert sind. Beispiele für diese Art von Webinhalt sind Anzeigen mit Streaming-Video oder -Audio, HTML-Animationen und interaktive Banner.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 1%

---

# Erstellen eines Testversands für interaktive Inhalte in einer ZIP-Datei

Sie können einen Testversand für interaktive Inhalte erstellen, die nicht auf einer Website gespeichert sind und in einer ZIP-Datei gespeichert sind. Beispiele für diese Art von Webinhalt sind Anzeigen mit Streaming-Video oder -Audio, HTML-Animationen und interaktive Banner.

## Zugriffsanforderungen

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Aktueller Plan: Pro oder höher</p> <p>oder</p> <p>Veralteter Plan: Premium</p> <p>Weitere Informationen zum Testzugang für die verschiedenen Pläne finden Sie unter <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Zugriff auf die Testversandfunktion in Workfront</a>.</p> </td> 
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
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront-Testversandadministrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Testberechtigung Sie haben.

## Erstellen eines Testversands für interaktive Inhalte in einer ZIP-Datei

Nachdem Sie interaktive Inhalte in einer ZIP-Datei zu einem Testversand hinzugefügt haben, erstellt Adobe Workfront einen Testversand der komprimierten Dokumente. Je nach Dateigröße kann die Ladezeit für den Upload variieren. Die Erstellung größerer Dateien dauert länger. Sie können von der Seite weg navigieren und Workfront erstellt Ihre Datei weiterhin. Die maximale Größe für den Datei-Upload beträgt 4 GB. 

1. Bereiten Sie Ihren Inhalt vor, indem Sie eine ZIP-Bundle-Datei erstellen.

   Die ZIP-Datei muss die folgenden Anforderungen erfüllen:

   * Alle Assets wie CSS, JavaScript, Videos, Sounds und Bilder sollten in die Bundle-Datei aufgenommen werden.
   * Stellen Sie sicher, dass sich die Hauptdatei (z. B. index.html, index.htm) im Stammordner befindet und dass es sich um die einzige dort gespeicherte .html/.htm-Datei handelt.

      Wenn die Hauptdatei nicht im Stammordner abgelegt ist, sucht Workfront im Ordner nach der Hauptdatei.

   * Die maximale Bundle-Größe beträgt 500 MB.
   * Bei in iOS erstellten ZIP-Dateien identifiziert das Tool automatisch den richtigen Ordner, in dem der Inhalt abgelegt wird.

1. Gehen Sie zum Projekt, zur Aufgabe oder zum Problem, in das Sie die ZIP-Datei hochladen möchten.
1. Klicken **Dokumente** im linken Bereich .
1. Klicken **Neu hinzufügen** Klicken Sie auf **Testversand** im angezeigten Menü.
1. Im **Dateien hinzufügen** -Abschnitt, ziehen Sie die gewünschte ZIP-Datei per Drag-and-Drop oder suchen Sie nach der gewünschten ZIP-Datei.
1. Klicken **Testversand erstellen** , um einen einfachen Testversand ohne Überprüfungsprozess zu erstellen.\
   oder\
   Fahren Sie mit der Konfiguration eines erweiterten Testversands fort:

   * [Erstellen eines erweiterten Testversands mit einem einfachen Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Erstellen eines erweiterten Testversands mit einem automatisierten Workflow](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
