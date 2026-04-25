---
content-type: reference
product-area: documents
navigation-topic: documents-navigation-topic
title: Massenbearbeitung von Dokumenten
description: Im Bereich „Dokumente“ können Sie mehrere Dokumente gleichzeitig bearbeiten.
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: e8badce6-86f5-416c-a238-f9b7f19cdd2d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 90eb99fa46e706a53427f995d484e2fb42e9c293
workflow-type: tm+mt
source-wordcount: '925'
ht-degree: 76%

---

# Massenbearbeitung von Dokumenten

Sie können die Beschreibung bearbeiten, benutzerdefinierte Formulare hinzufügen und benutzerdefinierte Formulare in mehreren Dokumenten gleichzeitig bearbeiten.

## Überlegungen beim Bearbeiten benutzerdefinierter Formulare

Beachten Sie Folgendes, wenn Sie benutzerdefinierte Formulare für Dokumente stapelweise bearbeiten:

* Die Informationen, die Sie für alle ausgewählten Dokumente ändern, überschreiben die vorhandenen Informationen in den einzelnen Dokumenten.
* Wenn Sie Dokumente mit unterschiedlichen Werten für dasselbe Feld auswählen, wird für das Feld ein Indikator für „Mehrere Werte“ angezeigt. Bei Feldern, die Kontrollkästchen, Optionsfelder und Umschalter sind, wird neben diesen ein Indikator für „Mehrere Werte“ angezeigt.
* Wenn Sie eine Option in einem Feld mit mehreren Optionen aktualisieren (z. B. in einem Feld, das als eine Reihe von Umschaltern oder Kontrollkästchen angezeigt wird), müssen alle anderen Optionen zwischen den ausgewählten Dokumenten übereinstimmen.

>[!BEGINSHADEBOX]

**Example**
You might have a custom form with a checkbox field with three checkboxes (Option1, Option 2, and Option 3) and Option 1 is unchecked for all selected documents, and Option 2 and 3 are checked for some and unchecked for other documents that you selected. Wenn Sie Option 1 für alle Dokumente aktivieren möchten, müssen Sie auch die Optionen 2 und 3 für alle ausgewählten Projekte anpassen, bevor Sie Ihre Änderungen speichern können. Daher müssen Sie sie entweder aktivieren oder deaktivieren, damit sie mit allen ausgewählten Projekten übereinstimmen können. Wenn Sie keine der Optionen ändern, können Sie das Feld unverändert speichern, und die Dokumente behalten ihre aktuelle Auswahl für alle Optionen bei.

>[!ENDSHADEBOX]

## Zugriffsanforderungen

+++ Erweitern, um die Zugriffsanforderungen für die in diesem Artikel beschriebene Funktionalität anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Paket</td> 
   <td> <p>Jedes Workfront-Paket zum Verwalten von Dokumenten unter Verwendung des alten Workfront-Speichers</p>
<p>Beliebiges Workflow-Paket zum Verwalten von Dokumenten mit Adobe Enterprise Storage</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenzen*</td> 
   <td><p>Mitwirkende oder höher</p> 
   <p>Anfragende oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> <p>Zugriffrecht „Bearbeiten“ für Dokumente</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Zugriffsrecht „Verwalten“ für das Dokument</p></td> 
  </tr> 
 </tbody> 
</table>

Weitere Details zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Edit documents in bulk in the legacy documents area

Wenn sich Ihr Unternehmen im alten Workfront-Speicher befindet, wird der Bereich für ältere Dokumente angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Workfront Storage finden Sie unter [Unterschiede zwischen Adobe Enterprise Storage und Legacy Workfront Storage](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-enterprise-storage-and-legacy-workfront-storage).

So bearbeiten Sie Dokumente stapelweise:

1. Navigieren Sie zur Registerkarte „Dokumente“ eines Projekts oder zum Bereich „Dokumente“ im Hauptmenü.
1. Drücken Sie die Strg- oder Befehlstaste auf der Tastatur und wählen Sie die Dokumente aus, die Sie bearbeiten möchten.
1. Klicken Sie auf das Symbol „Bearbeiten“ ![Symbol „Bearbeiten“](assets/edit-icon.png).
   ![Position des Bearbeitungssymbols auf der Seite](assets/edit-multiple-documents.png)
1. (Optional) Fügen Sie eine **Beschreibung** hinzu oder bearbeiten Sie sie. Wenn die Beschreibung für jedes Dokument unterschiedlich ist, wird _Mehrere Werte_ im Beschreibungsfeld angezeigt. Sie können dieselbe Beschreibung für alle Dokumente hinzufügen, aber Sie können einzelne Dokumentbeschreibungen nicht gleichzeitig bearbeiten.
1. Nehmen Sie bei benutzerdefinierten Formularen die folgenden Änderungen vor:

   <table>
    <tr>
    <td><strong>Formulare hinzufügen</strong></td>
    <td>Im Feld <strong>Benutzerdefiniertes Formular hinzufügen</strong> können Sie zwischen angehängten Formularen und Formularen wählen, die hinzugefügt werden sollen. Angehängte Formulare sind für einige der ausgewählten Dokumente verfügbar, jedoch nicht für alle. Ein Formular, das an alle ausgewählten Dokumente angehängt ist, wird automatisch im Bearbeitungsfenster angezeigt.  </td>
    </tr>
    <tr>
    <td><strong>Formulare bearbeiten</strong></td>
    <td>Bearbeiten Sie alle angehängten benutzerdefinierten Formulare. Die von Ihnen geänderten Informationen überschreiben die vorhandenen Informationen in den einzelnen Dokumenten. Felder mit unterschiedlichen Werten in allen Dokumenten werden als „Mehrere Werte“ angezeigt. </td>
    </tr>
    <tr>
    <td><strong>Formulare neu anordnen</strong></td>
    <td>Klicken Sie auf das benutzerdefinierte Formular und ziehen Sie es, um es neu anzuordnen.</td>
    </tr>
    </table>
1. Klicken Sie auf **Speichern**.

## Edit documents in bulk in the new documents area


Wenn Ihr Unternehmen Enterprise-Speicher verwendet, wird der Bereich „Neue Dokumente“ angezeigt, wenn Sie auf Dokumente in Workfront zugreifen. Weitere Informationen zu Massenspeicher für Unternehmen finden Sie unter [Übersicht über Speicher für Unternehmen in Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

So bearbeiten Sie Dokumente stapelweise:

1. Gehen Sie zu dem Projekt, der Aufgabe oder dem Problem, das/das das Dokument enthält, und wählen Sie dann **Dokumente**.
1. Drücken Sie die Strg- oder Befehlstaste auf der Tastatur und wählen Sie die Dokumente aus, die Sie bearbeiten möchten.
1. Click Edit at the bottom of the page.
   ![edit multiple documents](assets/bulk-edit-documents.png)
1. (Optional) Fügen Sie eine **Beschreibung** hinzu oder bearbeiten Sie sie. Wenn die Beschreibung für jedes Dokument unterschiedlich ist, wird _Mehrere Werte_ im Beschreibungsfeld angezeigt. Sie können dieselbe Beschreibung für alle Dokumente hinzufügen, aber Sie können einzelne Dokumentbeschreibungen nicht gleichzeitig bearbeiten.
1. Nehmen Sie bei benutzerdefinierten Formularen die folgenden Änderungen vor:

   <table>
    <tr>
    <td><strong>Formulare hinzufügen</strong></td>
    <td>In the <strong>Custom form</strong> section, you can add a new custom form to the selected documents. Custom forms attached to all selected documents display in the <strong>Custom forms in common</strong> section.  </td>
    </tr>
    <tr>
    <td><strong>Formulare bearbeiten</strong></td>
    <td>Bearbeiten Sie alle angehängten benutzerdefinierten Formulare. Die von Ihnen geänderten Informationen überschreiben die vorhandenen Informationen in den einzelnen Dokumenten. Felder mit unterschiedlichen Werten in allen Dokumenten werden als „Mehrere Werte“ angezeigt. </td>
    </tr>
    </table>
1. Klicken Sie auf **Speichern**.

## Stapelweises Bearbeiten von Dokumenten in einem Dokumentbericht

1. Navigieren Sie zu einem vorhandenen Dokumentbericht.
oder
Create a document report as described in [Create a custom report](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Wählen Sie die Dokumente aus, die Sie bearbeiten möchten.
1. Klicken Sie auf das Symbol „Bearbeiten“ ![Symbol „Bearbeiten“](assets/edit-icon.png).
1. (Optional) Fügen Sie eine **Beschreibung** hinzu oder bearbeiten Sie sie. Wenn die Beschreibung für jedes Dokument unterschiedlich ist, wird _Mehrere Werte_ im Beschreibungsfeld angezeigt. Sie können dieselbe Beschreibung für alle Dokumente hinzufügen, aber Sie können einzelne Dokumentbeschreibungen nicht gleichzeitig bearbeiten.
1. Nehmen Sie bei benutzerdefinierten Formularen die folgenden Änderungen vor:

   <table>
    <tr>
    <td><strong>Formulare hinzufügen</strong></td>
    <td>Im Feld <strong>Benutzerdefiniertes Formular hinzufügen</strong> können Sie zwischen angehängten Formularen und Formularen wählen, die hinzugefügt werden sollen. Angehängte Formulare sind für einige der ausgewählten Dokumente verfügbar, jedoch nicht für alle. Ein Formular, das an alle ausgewählten Dokumente angehängt ist, wird automatisch im Bearbeitungsfenster angezeigt.  </td>
    </tr>
    <tr>
    <td><strong>Formulare bearbeiten</strong></td>
    <td>Bearbeiten Sie alle angehängten benutzerdefinierten Formulare. Die von Ihnen geänderten Informationen überschreiben die vorhandenen Informationen in den einzelnen Dokumenten. Felder mit unterschiedlichen Werten in allen Dokumenten werden als „Mehrere Werte“ angezeigt. </td>
    </tr>
    <tr>
    <td><strong>Formulare neu anordnen</strong></td>
    <td>Klicken Sie auf das benutzerdefinierte Formular und ziehen Sie es, um es neu anzuordnen.</td>
    </tr>
    </table>
1. Klicken Sie auf **Speichern**.
