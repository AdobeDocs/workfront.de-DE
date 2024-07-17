---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Erforderlicher Zugriff auf Budgetressourcen in Adobe Workfront
description: Sie können Informationen zur Ressourcenplanung für die Projekte, auf die Sie Zugriff haben, anzeigen und verwalten, wenn Sie über bestimmte Einstellungen für die Zugriffsstufe und über die Berechtigungen für Ihre Arbeitselemente, Benutzer, Rollen und Teams verfügen.
author: Alina
feature: Resource Management
exl-id: d2bfc411-188a-4f8b-8180-0e984f01b5ab
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Erforderlicher Zugriff auf Budgetressourcen in Adobe Workfront

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><b>(LINKED TO PRODUCT</b>: This is also linked to the product, in two different tooltips in the RP:</p>
<p>- the tooltip for the View-only mode of the Budgeted Hours boxes. You gave this link to Vazgen and the team for the tooltip and documented this in this sheet:https://docs.google.com/spreadsheets/d/1zKjNVw_TyfQ474jbY7JorSWTkptMNb5RFCck2IficYs/edit#gid=0</p>
<p>- Also in the tooltip from this issue: https://hub.workfront.com/issue/view?ID=5ca708d00024a39e58b5dbeaceb00939)</p>
<p>This might need to be moved to Resource Management overview and title needs to be changed to "Acces needed to manage resources" when the res manager prerequisite will drop for resource scheduling and the field goes away.</p>
<p>This should be linked from Planning in the Resource Planner - in the Budgeting Resources in the RP area)</p>
</div>
-->

Wenn Ihr Unternehmen eine Adobe Workfront-Lizenz erworben hat, die die Ressourcenplanung enthält, können Sie Ressourcenbudgeting-Informationen für die Projekte anzeigen, für die Sie über Berechtigungen verfügen. Sie können Budgetierungsinformationen im Ressourcen-Planer anzeigen.

Weitere Informationen zu den Voraussetzungen für die Verwendung der Budgetierungs-Tools in Workfront finden Sie unter [Erste Schritte mit der Ressourcenplanung](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

Um Ressourcen zu finanzieren, Ressourcen-Pools zu verwalten und Kosteninformationen in den Tools für die Ressourcenplanung anzuzeigen, müssen Ihr Unternehmen und Sie über den folgenden Zugriff verfügen: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Pro oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> 
    <ul> 
     <li> <p>Bearbeiten Sie den Zugriff auf die Ressourcenverwaltung in Ihrer Zugriffsebene, einschließlich:</p> 
      <ul> 
       <li> <p>Zugriff auf die Bearbeitung von Projektprioritäten und Budgetzeiten. </p> </li> 
       <li> <p>Zugriff auf die Verwaltung von Ressourcen-Pools, wenn Sie Ressourcen-Pool verwalten müssen.</p> </li> 
      </ul> <p>Weitere Informationen zur Zugriffsebene für die Ressourcenverwaltung finden Sie im Artikel <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Zugriff auf die Ressourcenverwaltung gewähren</a>.</p> </li> 
     <li> <p>Bearbeiten Sie den Zugriff auf Projekte und Benutzer. </p> </li> 
     <li> <p> Bearbeiten Sie den Zugriff auf Finanzdaten in Ihrer Zugriffsebene, wenn Sie Informationen nach Kosten anzeigen oder verwalten möchten.</p> <p>Weitere Informationen zur Zugriffsebene für Finanzdaten finden Sie im Artikel <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Zugriff auf Finanzdaten gewähren</a>.</p> </li> 
    </ul>

<p><b>NOTE</b> </p>

<p> Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Verwalten Sie Berechtigungen für das Projekt, die Berechtigungen für die Verwaltung von Finanzen enthalten.</p> <p>Weitere Informationen zu Projektberechtigungen finden Sie im Artikel <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Projekt in Adobe Workfront freigeben</a> .</p> <p>Weitere Informationen zu finanziellen Berechtigungen für ein Projekt finden Sie im Artikel <a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Finanzberechtigungen für ein Objekt freigeben</a></a>.</p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md">Anfordern des Zugriffs auf Objekte </a>.</p>

<p><b>NOTIZ</b>

Wenn Sie bei der Budgetierung von Ressourcen in der Rollenansicht weniger als Verwaltungsberechtigungen für mindestens ein unter der Rolle aufgelistetes Projekt haben, können Sie keine Stunden, FTE oder Kosten für die Rolle einplanen. Sie können nur Projekte mit Verwaltungsberechtigungen für Ihre Projekte einplanen.</p> </td>
</tr> 
 </tbody> 
</table>

*Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.
