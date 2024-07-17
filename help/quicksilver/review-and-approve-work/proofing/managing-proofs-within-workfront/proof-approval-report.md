---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Validierungsbericht für Testsendungen verwenden
description: Im Validierungsbericht für Testsendungen erhalten Sie Informationen zu Testsendungen in Ihrer Umgebung.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 1%

---

# Validierungsbericht für Testsendungen verwenden

Im Validierungsbericht für Testsendungen erhalten Sie Informationen zu Testsendungen in Ihrer Umgebung.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Workfront-Plan*</p> </td> 
   <td>Alle</td> 
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
     <li> <p>Erstellen von Filtern, Ansichten und Gruppen</p> </li> 
    </ul> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Validierungsbericht für Testsendungen verwenden

1. Klicken Sie auf das Symbol **Hauptmenü** oben rechts in Adobe Workfront und klicken Sie dann auf **Berichte**.![](assets/main-menu-icon.png)
1. Klicken Sie auf &quot;**Neuer Bericht**&quot;und scrollen Sie dann zu &quot;**Bestätigung der Genehmigung prüfen**&quot;.

   ![](assets/proof-approval-report.png)

1. (Optional) Fügen Sie weitere Felder hinzu.
1. Klicken Sie auf **Speichern + schließen**.

## Zusätzliche Felder

Folgende Felder können in den Validierungsbericht für Testsendungen eingefügt werden:

* **Entscheidungsdatum**: Zeigt das Datum an, an dem ein Genehmiger eine Entscheidung über einen Testversand trifft. Dieses Datum finden Sie auch in der Druckzusammenfassung des Testversands.
* **Phase &quot;Genehmiger&quot;**: Zeigt die aktuellen Informationen zur Bühne an.
* **Workflow-Vorlage**: Zeigt alle an den Testversand angehängten Workflow-Vorlagen an. Wenn keine Vorlage angehängt ist, ist die Spalte leer.
* **Warten auf Entscheidung**: Zeigt &quot;true&quot;an, um zu signalisieren, dass eine Entscheidung in der neuesten Version nicht getroffen wurde, wenn Folgendes zutrifft:

   * Der Nachweis wurde nicht archiviert
   * Die Phase, in der der Genehmiger aktiv ist
   * Der Testversand steht noch aus.

* **Testversand-Deadline**: Zeigt die Deadline des Testversands an. Für jede Phase muss eine Frist zugewiesen sein, damit dieses Feld ausgefüllt werden kann. Im Feld wird der Termin für die zuletzt aktivierte Phase angezeigt.

 
