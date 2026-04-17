---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Zum Budgetieren von Ressourcen in Workfront erforderliche Zugriffsrechte
description: Sie können Informationen zur Ressourcenplanung für die Projekte, auf die Sie Zugriff haben, anzeigen und verwalten, wenn Sie über bestimmte Zugriffsebenen-Einstellungen und -Berechtigungen für Ihre Arbeitselemente, Benutzer, Aufgabengebiete und Teams verfügen.
author: Lisa
feature: Resource Management
exl-id: d2bfc411-188a-4f8b-8180-0e984f01b5ab
source-git-commit: b78b86806e5c3c1e6d0662fea0e1a11f97ef032e
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 10%

---

# Zum Budgetieren von Ressourcen in Workfront erforderliche Zugriffsrechte

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><b>(LINKED TO PRODUCT</b>: This is also linked to the product, in two different tooltips in the RP:</p>
<p>- the tooltip for the View-only mode of the Budgeted Hours boxes. You gave this link to Vazgen and the team for the tooltip and documented this in this sheet:https://docs.google.com/spreadsheets/d/1zKjNVw_TyfQ474jbY7JorSWTkptMNb5RFCck2IficYs/edit#gid=0</p>
<p>- Also in the tooltip from this issue: https://hub.workfront.com/issue/view?ID=5ca708d00024a39e58b5dbeaceb00939)</p>
<p>This might need to be moved to Resource Management overview and title needs to be changed to "Acces needed to manage resources" when the res manager prerequisite will drop for resource scheduling and the field goes away.</p>
<p>This should be linked from Planning in the Resource Planner - in the Budgeting Resources in the RP area)</p>
</div>
-->

Wenn Ihr Unternehmen eine Adobe Workfront-Lizenz mit Ressourcenplanung erworben hat, können Sie Informationen zur Ressourcenbudgetierung für die Projekte anzeigen, für die Sie berechtigt sind. Sie können Budgetinformationen im Ressourcenplaner anzeigen.

Weitere Informationen zu den Voraussetzungen für die Verwendung der Budgetierungs-Tools in Workfront finden Sie [Erste Schritte mit der Ressourcenplanung](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

Um Ressourcen zu budgetieren, Ressourcenpools zu verwalten und Kosteninformationen in den Ressourcenplanungs-Tools anzuzeigen, benötigen Ihr Unternehmen und Sie die folgenden Zugriffsrechte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront-Paket</td> 
   <td><p>Beliebig</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-Lizenz</td> 
   <td><p>Standard</p>
       <p>Abo</p></td>
  </tr>  
  <tr> 
   <td role="rowheader">Konfigurationen der Zugriffsebene</td> 
   <td> 
    <ul> 
     <li> <p>Bearbeiten Sie den Zugriff auf die Ressourcenverwaltung in Ihrer Zugriffsebene, indem Sie Folgendes beinhalten:</p> 
      <ul> 
       <li> <p>Zugriff auf die Bearbeitung von Projektprioritäten und Budgetstunden. </p> </li> 
       <li> <p>Zugriff auf die Verwaltung von Ressourcenpools, wenn Sie Ressourcenpools verwalten müssen.</p> </li> 
      </ul> <p>Informationen zur Zugriffsebene für das Ressourcen-Management finden Sie im Artikel <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Zugriff auf das Ressourcen-Management gewähren</a>.</p> </li> 
     <li> <p>Zugriff auf Projekte und Benutzer bearbeiten. </p> </li> 
     <li> <p> Bearbeiten Sie den Zugriff auf Finanzdaten auf Ihrer Zugriffsebene, einschließlich des Zugriffs zum Anzeigen oder Bearbeiten von Kostensätzen und zum Anzeigen oder Bearbeiten der allgemeinen Finanzen, wenn Sie Informationen nach Kosten anzeigen oder verwalten müssen.</p> <p>Weitere Informationen zur Zugriffsebene „Finanzdaten“ finden Sie im Artikel <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Zugriff auf Finanzdaten gewähren</a>.</p> </li> 
    </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten Sie Berechtigungen für das Projekt, einschließlich der Berechtigungen Kostensätze bearbeiten und Allgemeine Finanzen bearbeiten .</p> <p>Informationen zu Projektberechtigungen finden Sie im Artikel <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Freigeben eines Projekts in Adobe Workfront</a>.</p> <p>Informationen zu Finanzberechtigungen für ein Projekt finden Sie im Artikel <a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Freigeben von Finanzberechtigungen für ein Objekt</a></a>.</p>

<p><b>HINWEIS:</b> Wenn Sie bei der Budgetierung von Ressourcen in der Rollenansicht für mindestens ein unter der Rolle aufgeführtes Projekt weniger als Verwaltungsberechtigungen haben, können Sie für die Rolle keine Stunden, FTE oder Kosten budgetieren. Sie können nur die Projekte budgetieren, für die Sie über Verwaltungsberechtigungen verfügen.</p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen finden Sie unter [Zugriffsanforderungen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) in der Dokumentation zu Workfront.
