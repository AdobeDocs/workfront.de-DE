---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Korrekturabzugs-Genehmigungs-Bericht verwenden
description: Sie können den Bericht zu Korrekturabzugsgenehmigungen verwenden, um Informationen zu Korrekturabzügen in Ihrer Umgebung anzuzeigen.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 2%

---

# Korrekturabzugs-Genehmigungs-Bericht verwenden

Sie können den Bericht zu Korrekturabzugsgenehmigungen verwenden, um Informationen zu Korrekturabzügen in Ihrer Umgebung anzuzeigen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Workfront-Paket</p> </td> 
   <td>Beliebig</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront-Lizenz</p> </td> 
   <td> 
   <p>Standard</p>
   <p>Plan</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Konfiguration der Zugriffsebene</strong> </td> 
   <td> <p>Zugriff bearbeiten auf:</p> 
    <ul> 
     <li> <p>Berichte, Dashboards und Kalender erstellen</p> </li> 
     <li> <p>Filter, Ansichten und Gruppierungen erstellen</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen in der Dokumentation zu Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Korrekturabzugs-Genehmigungs-Bericht verwenden

{{step1-to-reports}}

1. Klicken Sie **Neuer Bericht** und blättern Sie zur Auswahl **Korrekturabzugsgenehmigung**.

   ![Bericht zur Korrekturabzugsgenehmigung](assets/proof-approval-report.png)

1. (Optional) Fügen Sie weitere Felder hinzu.
1. Klicken Sie auf **Speichern + schließen**.

## Zusätzliche Felder

Sie können die folgenden Felder zum Bericht über Korrekturabzugsgenehmigungen hinzufügen:

* **Entscheidungsdatum**: Zeigt das Datum an, an dem eine genehmigende Person eine Entscheidung über einen Korrekturabzug trifft. Dieses Datum finden Sie auch in der Druckzusammenfassung des Testversands.
* **Genehmiger-Phase**: Zeigt die Informationen zum aktuellen Schritt an.
* **Workflow-**: Zeigt alle Workflow-Vorlagen an, die an den Korrekturabzug angehängt sind. Wenn keine Vorlage angehängt ist, ist die Spalte leer.
* **Entscheidung ausstehend**: Zeigt „true“ an, um anzuzeigen, dass eine Entscheidung auf der neuesten Version nicht erfüllt wurde, wenn Folgendes zutrifft:

   * Der Korrekturabzug wurde nicht archiviert
   * Die Phase, in der sich die genehmigende Person befindet, ist aktiv
   * Die Genehmigung des Korrekturabzugs steht aus

* **Testversand-Frist**: Zeigt die Frist für den Testversand an. Jeder Phase muss eine Frist zugewiesen sein, damit dieses Feld ausgefüllt werden kann. Das Feld zeigt den Termin für die zuletzt aktivierte Phase an.

 
