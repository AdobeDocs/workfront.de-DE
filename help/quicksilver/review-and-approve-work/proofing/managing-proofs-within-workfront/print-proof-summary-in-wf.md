---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Drucken einer Zusammenfassung eines Korrekturabzugs in Adobe Workfront
description: Sie können eine Korrekturabzugszusammenfassung drucken, als PDF speichern oder als XLS- oder PDF-Datei exportieren, die für Adobe Reader optimiert ist.
author: Courtney
feature: Digital Content and Documents
exl-id: 129c8e6b-5c66-445b-a5d0-7b1460aeabd6
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 1%

---

# Drucken einer Zusammenfassung eines Korrekturabzugs in Adobe Workfront

Sie können eine Korrekturabzugszusammenfassung drucken, als PDF speichern oder als XLS- oder PDF-Datei exportieren, die für Adobe Reader optimiert ist.

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

## Drucken Sie eine Korrekturabzugszusammenfassung oder speichern Sie sie als PDF-Datei

Sie können eine Zusammenfassung eines Korrekturabzugs direkt aus der Dokumentliste drucken.

>[!NOTE]
>
>* Zusammenfassungen, die größer als 1 GB sind, werden nicht unterstützt.
>* Sie können nicht mehrere Korrekturabzugszusammenfassungen gleichzeitig aus der Dokumentliste drucken.

1. Bewegen Sie in der Dokumentliste, die den Korrekturabzug enthält, den Mauszeiger über die Zeile, die das Dokument enthält, und klicken Sie dann auf **Druckzusammenfassung**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

   Oder

   Klicken Sie während der Anzeige des Korrekturabzugs in der Korrekturabzugsansicht auf das Symbol **Drucken** (![) ](assets/print-icon-in-pv.png) der linken Symbolleiste. (Wenn die linke Symbolleiste nicht sichtbar ist, klicken Sie auf das Menüsymbol ![Menüsymbol](assets/menu-icon-in-pv.png) in der linken oberen Ecke der Korrekturabzugsanzeige.)

1. Verwenden Sie eine der folgenden Optionen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anzeigen</td> 
      <td> <p>Geben Sie an, was Sie drucken möchten:</p> 
       <ul> 
        <li>Die <strong>Aktuelle Version</strong> oder <strong>Alle Versionen</strong> des Korrekturabzugs</li> 
        <li>Nur die <strong>Seiten mit Kommentaren</strong> oder <strong>Alle Seiten</strong></li> 
        <li>Nur die <strong>Seitenminiaturen</strong> (ein kleines Rendering jeder Seite) oder <strong>Vollständige Seiten</strong> (ein vollständiges Rendering des Korrekturabzugs)<br></li> 
        <p>Hinweis: Um Pin-Nummern auf dem Markup in der gedruckten Ausgabe anzuzeigen, müssen Sie Vollständige Seiten und nicht Miniaturansichten auswählen. </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kommentare sortieren nach</td> 
      <td> <p>(Nur verfügbar, wenn Sie oben „Seitenminiaturansichten“ ausgewählt haben.) Geben Sie die Reihenfolge an, in der die Kommentare des Korrekturabzugs gedruckt werden sollen:</p> 
       <ul> 
        <li><strong>Älteste</strong>: Vom ersten Kommentar bis zum letzten</li> 
        <li><strong>Letzte</strong>: Vom letzten Kommentar zum ersten</li> 
        <li><strong>Seite</strong>: Nach Seite, von der ersten Seite zur letzten oder von der letzten Seite zur ersten</li> 
        <li><strong>Creator</strong>: Nach den Namen der Benutzer, die sie hinzugefügt haben, von A-Z oder von Z-A</li> 
       </ul> <p>Diese Optionen wirken sich nicht auf die Ausgabe aus, die Sie als XLS- oder PDF-Datei exportieren.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kommentare filtern nach</td> 
      <td> <p>Sie können eine beliebige Kombination dieser Optionen verwenden, um nur bestimmte Kommentare in die Ausgabe einzuschließen, die Sie als XLS- oder PDF-Datei drucken oder exportieren:</p> 
       <ul> 
        <li>Von Ihnen ausgewählte Autoren (Standard)</li> 
        <li>Ausgewählte Aktionen</li> 
        <li><strong>Nicht aufgelöster</strong> Status</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Workflow</td> 
      <td> <p>(Nur verfügbar, wenn der Korrekturabzug über einen automatisierten Workflow verfügt) Sie können auf <strong>Diagramm anzeigen</strong> klicken, um ein Diagramm in die gedruckte Ausgabe aufzunehmen, das die Phasen des Korrekturabzugs und die auf den einzelnen Phasen getroffenen Entscheidungen anzeigt. In dem angezeigten Diagramm stellen die Farben die auf einer Bühne getroffenen Entscheidungen dar:</p> <p><strong>grün</strong>: Genehmigt</p> <p><strong>Blue</strong>: Entscheidung steht aus</p> <p><strong>Rot</strong>: Änderungen für Entscheidung erforderlich</p> <p><strong>Grau</strong>: Noch nicht gestartet</p> <p><strong>Gelb</strong>: Mit Änderungen genehmigt</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicken Sie **Drucken**.
1. Wenn Sie die Zusammenfassung drucken möchten, klicken Sie im rechten Bedienfeld des angezeigten Fensters auf das Menü **Ziel** und dann auf **Weitere Informationen**. Klicken Sie in der angezeigten Liste auf den Drucker, den Sie verwenden möchten, und dann auf **Drucken**.

   Oder

   Wenn Sie die Zusammenfassung als PDF-Datei speichern möchten, klicken Sie auf das Menü **Ziel**, klicken Sie auf **Als PDF speichern** und dann auf **Speichern**.

## Exportieren einer Zusammenfassung eines Korrekturabzugs als XLS oder PDF

Sie können eine Korrekturabzugszusammenfassung für statische Inhalte als XLS- oder als PDF-Datei exportieren. Testversand-Exporte umfassen nur den Inhalt des Testversands.

1. Bewegen Sie in der Dokumentliste, die den Korrekturabzug enthält, den Mauszeiger über die Zeile, die das Dokument enthält, und klicken Sie dann auf **Druckzusammenfassung**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

1. Klicken Sie oben rechts auf der Seite auf das XLS- oder PDF-Symbol.

   ![XLS-PDF-Symbol](assets/xls-pdf-icons-350x136.png)

Wenn die exportierte Datei fertig ist, erhalten Sie eine E-Mail, aus der Sie die Datei herunterladen können.

Wenn Sie die Zusammenfassung als PDF-Datei exportiert haben, werden Kommentare zum Korrekturabzug im PDF-Reader angezeigt. Wenn einem Kommentar mehrere Markierungen zugeordnet sind, wird der Kommentar mehrmals in der Liste Kommentare angezeigt (einmal für jedes Markup).
