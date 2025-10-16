---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Erstellen eines Korrekturabzugs für interaktive Inhalte in einer ZIP-Datei
description: Sie können einen Korrekturabzug für nicht auf der Website interaktive Inhalte generieren, die in einer ZIP-Datei gespeichert sind. Beispiele für diese Art von Web-Inhalten sind Anzeigen mit Streaming-Video oder Audio, HTML-Animationen, interaktive Banner.
author: Courtney
feature: Digital Content and Documents
exl-id: 2ab00d17-a3a3-4417-a958-ac3d95cb8fc8
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---

# Erstellen eines Korrekturabzugs für interaktive Inhalte in einer ZIP-Datei

Sie können einen Korrekturabzug für nicht auf der Website interaktive Inhalte generieren, die in einer ZIP-Datei gespeichert sind. Beispiele für diese Art von Web-Inhalten sind Anzeigen mit Streaming-Video oder Audio, HTML-Animationen, interaktive Banner.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Beliebig</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td> 
   <p>Standard</p>
   <p>Arbeit oder Plan</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Proof-Berechtigungsprofil </td> 
   <td>Manager oder höher</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriff auf Dokumente bearbeiten</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
