---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Verwenden des Validierungsberichts
description: Im Validierungsbericht für Testsendungen erhalten Sie Informationen zu Testsendungen in Ihrer Umgebung.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 1%

---

# Verwenden des Validierungsberichts

Im Validierungsbericht für Testsendungen erhalten Sie Informationen zu Testsendungen in Ihrer Umgebung.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Workfront-Plan*</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Übersicht über Adobe Workfront-Lizenzen*</p> </td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Zugriffsebene*</strong> </td> 
   <td> <p>Zugriff bearbeiten auf:</p> 
    <ul> 
     <li> <p>Erstellen von Berichten, Dashboards und Kalendern</p> </li> 
     <li> <p>Erstellen von Filtern, Ansichten und Gruppierungen</p> </li> 
    </ul> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsstufe ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Verwenden des Validierungsberichts

1. Klicken Sie auf **Hauptmenü** icon ![](assets/main-menu-icon.png) Klicken Sie oben rechts in Adobe Workfront auf **Berichte**.
1. Klicken **Neuer Bericht**, dann scrollen Sie zu **Validierung des Testversands**.

   ![](assets/proof-approval-report.png)

1. (Optional) Fügen Sie weitere Felder hinzu.
1. Klicken **Speichern und schließen**.

## Zusätzliche Felder

Folgende Felder können in den Validierungsbericht für Testsendungen eingefügt werden:

* **Entscheidungsdatum**: Zeigt das Datum an, an dem ein Genehmiger eine Entscheidung über einen Testversand trifft. Dieses Datum finden Sie auch in der Druckzusammenfassung des Testversands.
* **Stufe des Genehmigers**: Zeigt die aktuellen Informationen zur Bühne an.
* **Workflow-Vorlage**: Zeigt alle an den Testversand angehängten Workflow-Vorlagen an. Wenn keine Vorlage angehängt ist, ist die Spalte leer.
* **Entscheidung warten**: Zeigt &quot;true&quot;an, um zu signalisieren, dass eine Entscheidung in der neuesten Version nicht getroffen wurde, wenn Folgendes zutrifft:

   * Der Testversand wurde nicht archiviert
   * Die Phase, in der der Genehmiger aktiv ist
   * Der Testversand steht noch aus.

* **Testversand-Deadline**: Zeigt den Stichtag des Testversands an. Für jede Phase muss eine Frist zugewiesen sein, damit dieses Feld ausgefüllt werden kann. Im Feld wird der Termin für die zuletzt aktivierte Phase angezeigt.

 
