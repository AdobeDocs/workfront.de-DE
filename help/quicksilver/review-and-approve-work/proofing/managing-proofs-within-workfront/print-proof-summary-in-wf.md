---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Testversandzusammenfassung in Adobe Workfront drucken
description: Sie können eine Testversand-Zusammenfassung drucken, als PDF speichern oder als XLS-Datei oder PDF-Datei exportieren, die für Adobe Reader optimiert ist.
author: Courtney
feature: Digital Content and Documents
exl-id: 129c8e6b-5c66-445b-a5d0-7b1460aeabd6
source-git-commit: 1b85267e811f5832480316be5322ee819abaf190
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 1%

---

# Testversandzusammenfassung in Adobe Workfront drucken

Sie können eine Testversand-Zusammenfassung drucken, als PDF speichern oder als XLS-Datei oder PDF-Datei exportieren, die für Adobe Reader optimiert ist.

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

## Testversand-Zusammenfassung drucken oder als PDF-Datei speichern

Sie können eine Testversand-Zusammenfassung direkt aus der Dokumentliste drucken.

>[!NOTE]
>
>Sie können nicht mehrere Testversand-Zusammenfassungen gleichzeitig aus der Dokumentliste drucken.

1. Halten Sie in der Dokumentliste, die den Testversand enthält, den Mauszeiger über die das Dokument enthaltende Zeile und klicken Sie dann auf **Zusammenfassung drucken** .

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

   Oder

   Klicken Sie beim Anzeigen des Testversands im Testversand-Viewer in der linken Symbolleiste auf das Symbol **Drucken** ![](assets/print-icon-in-pv.png) . (Wenn die linke Symbolleiste nicht angezeigt wird, klicken Sie in der oberen linken Ecke des Testversand-Viewers auf das Menüsymbol ![](assets/menu-icon-in-pv.png) .)

1. Verwenden Sie eine der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anzeigen</td> 
      <td> <p>Geben Sie an, was Sie drucken möchten:</p> 
       <ul> 
        <li>Die <strong>aktuelle Version</strong> oder <strong>Alle Versionen</strong> des Testversands</li> 
        <li>Nur die <strong>Seiten mit Kommentaren</strong> oder <strong>Alle Seiten</strong></li> 
        <li>Nur die <strong>Seiten-Miniaturansichten</strong> (eine kleine Darstellung jeder Seite) oder <strong>Vollseiten</strong> (eine vollständige Darstellung des Testversands)<br></li> 
        <p>Hinweis: Um die Pin-Zahlen auf dem Markup in Ihrer gedruckten Ausgabe anzuzeigen, müssen Sie Vollseiten und nicht Seiten-Miniaturansichten auswählen. </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sortieren von Kommentaren nach</td> 
      <td> <p>(Nur verfügbar, wenn Sie die Option Seitenminiaturansichten oben ausgewählt haben) Geben Sie die Reihenfolge an, in der die Kommentare des Testversands gedruckt werden sollen:</p> 
       <ul> 
        <li><strong>Oldest</strong>: Vom ersten Kommentar zum letzten</li> 
        <li><strong>Latest</strong>: Vom letzten Kommentar zum ersten</li> 
        <li><strong>Seite</strong>: Nach Seite, von der ersten Seite zur letzten oder von der letzten Seite zur ersten</li> 
        <li><strong>Ersteller</strong>: Nach den Namen der Benutzer, die sie hinzugefügt haben, von A-Z oder Z-A</li> 
       </ul> <p>Diese Optionen wirken sich nicht auf die Ausgabe aus, die Sie als XLS- oder PDF-Datei exportieren.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Filtern von Kommentaren nach</td> 
      <td> <p>Sie können eine beliebige Kombination dieser Optionen verwenden, um nur bestimmte Kommentare in die Ausgabe einzuschließen, die Sie als XLS- oder PDF-Datei drucken oder exportieren:</p> 
       <ul> 
        <li>Von Ihnen ausgewählte Autoren (Standard)</li> 
        <li>Aktionen, die Sie auswählen</li> 
        <li>Status <strong>Unresolved</strong></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Workflow</td> 
      <td> <p>(Nur verfügbar, wenn der Testversand einen automatisierten Workflow aufweist) Sie können auf <strong>Diagramm anzeigen</strong> klicken, um ein Diagramm in die gedruckte Ausgabe einzuschließen, in dem die Phasen des Testversands und die auf jeder Stufe getroffenen Entscheidungen dargestellt werden. Im angezeigten Diagramm stellen die Farben die auf einer Bühne getroffenen Entscheidungen dar:</p> <p><strong>Grün</strong>: Genehmigt</p> <p><strong>Blau</strong>: Entscheidung ausstehend</p> <p><strong>Rot</strong>: Erforderliche Entscheidung für Änderungen</p> <p><strong>Gray</strong>: Noch nicht gestartet</p> <p><strong>Gelb</strong>: Genehmigt mit Änderungen</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie auf **Drucken**.
1. Klicken Sie im rechten Bereich des angezeigten Fensters, wenn Sie die Zusammenfassung drucken möchten, auf das Menü **Ziel** und dann auf **Mehr anzeigen**. Klicken Sie in der angezeigten Liste auf den Drucker, den Sie verwenden möchten, und klicken Sie dann auf **Drucken**.

   Oder

   Wenn Sie die Zusammenfassung als PDF-Datei speichern möchten, klicken Sie auf das Menü **Ziel**, klicken Sie auf **Als PDF speichern** und dann auf **Speichern**.

## Testversand-Zusammenfassung als XLS oder PDF exportieren

Sie können eine Testversand-Zusammenfassung für statischen Inhalt als XLS-Datei oder als PDF-Datei exportieren. Der Testversand umfasst nur den Testversand-Inhalt.

1. Halten Sie in der Dokumentliste, die den Testversand enthält, den Mauszeiger über die das Dokument enthaltende Zeile und klicken Sie dann auf **Zusammenfassung drucken** .

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

1. Klicken Sie auf das XLS-Symbol oder PDF-Symbol oben rechts auf der Seite.

   ![](assets/xls-pdf-icons-350x136.png)

Wenn die exportierte Datei fertig ist, erhalten Sie eine E-Mail, aus der Sie die Datei herunterladen können.

Wenn Sie die Zusammenfassung als PDF-Datei exportiert haben, erscheinen im PDF-Reader Kommentare zum Testversand. Wenn einem Kommentar mehrere Markups zugeordnet sind, wird der Kommentar mehrmals in der Kommentarliste angezeigt (einmal pro Markup).
