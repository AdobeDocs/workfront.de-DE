---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Testversandzusammenfassung in Adobe Workfront drucken
description: Sie können eine Testversand-Zusammenfassung drucken, als PDF speichern oder als XLS-Datei oder PDF-Datei exportieren, die für Adobe Reader optimiert ist.
author: Courtney
feature: Digital Content and Documents
exl-id: 129c8e6b-5c66-445b-a5d0-7b1460aeabd6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '749'
ht-degree: 1%

---

# Testversandzusammenfassung in Adobe Workfront drucken

Sie können eine Testversand-Zusammenfassung drucken, als PDF speichern oder als XLS-Datei oder PDF-Datei exportieren, die für Adobe Reader optimiert ist.

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
   <td> <p>Zugriff auf Dokumente bearbeiten</p> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront- oder Workfront-Testversandadministrator, um zu erfahren, welchen Plan, welche Rolle oder welches Profil für die Testberechtigung Sie haben.

## Testversand-Zusammenfassung drucken oder als PDF-Datei speichern

Sie können eine Testversand-Zusammenfassung direkt aus der Dokumentliste drucken.

>[!NOTE]
>
>Sie können nicht mehrere Testversand-Zusammenfassungen gleichzeitig aus der Dokumentliste drucken.

1. Halten Sie in der Dokumentliste, die den Testversand enthält, den Mauszeiger über die das Dokument enthaltende Zeile und klicken Sie auf **Druckzusammenfassung**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

   Oder

   Klicken Sie beim Anzeigen des Testversands im Testversand-Viewer auf die Schaltfläche **Drucken** icon ![](assets/print-icon-in-pv.png) in der linken Symbolleiste. (Wenn die linke Symbolleiste nicht sichtbar ist, klicken Sie auf das Menüsymbol ![](assets/menu-icon-in-pv.png) in der linken oberen Ecke des Testversand-Viewers.)

1. Verwenden Sie eine der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anzeigen</td> 
      <td> <p>Geben Sie an, was Sie drucken möchten:</p> 
       <ul> 
        <li>Die <strong>Aktuelle Version</strong> oder <strong>Alle Versionen</strong> des Nachweises</li> 
        <li>Nur die <strong>Seiten mit Kommentaren</strong> oder <strong>Alle Seiten</strong></li> 
        <li>Nur die <strong>Seitenminiaturen</strong> (kleines Rendering jeder Seite) oder <strong>Vollständige Seiten</strong> (vollständige Darstellung des Testversands)<br></li> 
        <p>Hinweis: Um die Pin-Zahlen auf dem Markup in Ihrer gedruckten Ausgabe anzuzeigen, müssen Sie Vollseiten und nicht Seiten-Miniaturansichten auswählen. </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sortieren von Kommentaren nach</td> 
      <td> <p>(Nur verfügbar, wenn Sie die Option Seitenminiaturansichten oben ausgewählt haben) Geben Sie die Reihenfolge an, in der die Kommentare des Testversands gedruckt werden sollen:</p> 
       <ul> 
        <li><strong>Oldest</strong>: Aus dem ersten Kommentar zum letzten</li> 
        <li><strong>Neueste</strong>: Aus dem letzten Kommentar, der zum ersten</li> 
        <li><strong>Seite</strong>: Nach Seite, von der ersten Seite zur letzten oder von der letzten Seite zur ersten</li> 
        <li><strong>Ersteller</strong>: Nach den Namen der Benutzer, die sie hinzugefügt haben, von A-Z oder von Z-A</li> 
       </ul> <p>Diese Optionen wirken sich nicht auf die Ausgabe aus, die Sie als XLS- oder PDF-Datei exportieren.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Filtern von Kommentaren nach</td> 
      <td> <p>Sie können eine beliebige Kombination dieser Optionen verwenden, um nur bestimmte Kommentare in die Ausgabe einzuschließen, die Sie als XLS- oder PDF-Datei drucken oder exportieren:</p> 
       <ul> 
        <li>Von Ihnen ausgewählte Autoren (Standard)</li> 
        <li>Aktionen, die Sie auswählen</li> 
        <li><strong>Ungelöst</strong> status</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Workflow</td> 
      <td> <p>(Nur verfügbar, wenn der Testversand einen automatisierten Workflow aufweist) Klicken Sie auf <strong>Diagramm anzeigen</strong> in gedruckter Ausgabe ein Diagramm mit den Phasen des Testversands und den auf jeder Stufe getroffenen Entscheidungen anzuzeigen. Im angezeigten Diagramm stellen die Farben die auf einer Bühne getroffenen Entscheidungen dar:</p> <p><strong>Grün</strong>: Genehmigt</p> <p><strong>Blau</strong>: Ausstehende Entscheidung</p> <p><strong>Rot</strong>: Erforderliche Entscheidung ändern</p> <p><strong>Grau</strong>: Noch nicht gestartet</p> <p><strong>Gelb</strong>: Genehmigt mit Änderungen</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken **Drucken**.
1. Wenn Sie die Zusammenfassung im rechten Bereich des angezeigten Fensters drucken möchten, klicken Sie auf die Schaltfläche **Ziel** Menü und klicken Sie auf **Weitere Informationen**. Klicken Sie in der angezeigten Liste auf den Drucker, den Sie verwenden möchten, und klicken Sie dann auf **Drucken**.

   Oder

   Wenn Sie die Zusammenfassung als PDF-Datei speichern möchten, klicken Sie auf die **Ziel** Menü, klicken Sie **Als PDF speichern** Klicken Sie auf **Speichern**.

## Testversand-Zusammenfassung als XLS oder PDF exportieren

Sie können eine Testversand-Zusammenfassung für statischen Inhalt als XLS-Datei oder als PDF-Datei exportieren. Der Testversand umfasst nur den Testversand-Inhalt.

1. Halten Sie in der Dokumentliste, die den Testversand enthält, den Mauszeiger über die das Dokument enthaltende Zeile und klicken Sie auf **Druckzusammenfassung**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

1. Klicken Sie auf das XLS-Symbol oder PDF-Symbol oben rechts auf der Seite.

   ![](assets/xls-pdf-icons-350x136.png)

Wenn die exportierte Datei fertig ist, erhalten Sie eine E-Mail, aus der Sie die Datei herunterladen können.

Wenn Sie die Zusammenfassung als PDF-Datei exportiert haben, erscheinen im PDF-Reader Kommentare zum Testversand. Wenn einem Kommentar mehrere Markups zugeordnet sind, wird der Kommentar mehrmals in der Kommentarliste angezeigt (einmal pro Markup).
