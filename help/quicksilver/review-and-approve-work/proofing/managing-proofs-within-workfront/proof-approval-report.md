---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Korrekturabzugs-Genehmigungs-Bericht verwenden
description: Sie können den Bericht zu Korrekturabzugsgenehmigungen verwenden, um Informationen zu Korrekturabzügen in Ihrer Umgebung anzuzeigen.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
source-git-commit: 8a388ffa2d30683c08637a4273f628c553e55fdb
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 1%

---

# Korrekturabzugs-Genehmigungs-Bericht verwenden

Sie können den Bericht zu Korrekturabzugsgenehmigungen verwenden, um Informationen zu Korrekturabzügen in Ihrer Umgebung anzuzeigen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die -Funktion in diesem Artikel anzuzeigen.

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
     <li> <p>Berichte, Dashboards und Kalender erstellen</p> </li> 
     <li> <p>Filter, Ansichten und Gruppierungen erstellen</p> </li> 
    </ul> <p>Hinweis: Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Einschränkungen in Ihrer Zugriffsebene festgelegt hat. Informationen dazu, wie Workfront-Admins Ihre Zugriffsebene ändern können, finden Sie unter <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Erstellen oder Ändern benutzerdefinierter Zugriffsebenen</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um herauszufinden, über welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie verfügen.

+++

## Korrekturabzugs-Genehmigungs-Bericht verwenden

{{step1-to-reports}}

1. Klicken Sie **Neuer Bericht** und blättern Sie zur Auswahl **Korrekturabzugsgenehmigung**.

   ![](assets/proof-approval-report.png)

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

 
