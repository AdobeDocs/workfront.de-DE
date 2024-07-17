---
product-area: resource-management
navigation-topic: resource-planning
title: Suchen Sie den Ressourcen-Planer .
description: '(Dieser Artikel ist von diesem Artikel ausgegangen: Entwurf des Inhalts im Artikel, wenn er live kommt: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)'
author: Alina
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Suchen Sie den Ressourcen-Planer .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

Sie können den Ressourcen-Planer verwenden, um die Zuweisung Ihrer Ressourcen zu Projekten zu verwalten. Sie können auf den Ressourcen-Planer für mehrere Projekte gleichzeitig oder für ein Projekt über den Geschäftsfallbereich des Projekts zugreifen.

## Zugriffsanforderungen

Sie müssen über Folgendes verfügen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Plan*</td> 
   <td> <p>Pro und höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz*</td> 
   <td> <p>Überprüfen oder höher<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> <p>Planen oder höher, um den Ressourcenplaner im globalen Bereich zu finden</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene*</td> 
   <td> <p>Zugriff oder höher auf die Ressourcenverwaltung anzeigen</p> <p><b>NOTIZ</b>

Wenn Sie immer noch keinen Zugriff haben, fragen Sie Ihren Workfront-Administrator, ob er zusätzliche Zugriffsbeschränkungen für Ihre Zugriffsebene festlegt. Informationen dazu, wie ein Workfront-Administrator Ihre Zugriffsebene ändern kann, finden Sie unter <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Benutzerdefinierte Zugriffsebenen erstellen oder ändern</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für Projekte und Benutzer anzeigen </p> <p>Weitere Informationen zum Anfordern von zusätzlichem Zugriff finden Sie unter <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Anfordern des Zugriffs auf Objekte </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Wenden Sie sich an Ihren Workfront-Administrator, um zu erfahren, welchen Plan, welchen Lizenztyp oder welchen Zugriff Sie haben.

## Voraussetzungen

Stellen Sie sicher, dass alle Voraussetzungen für den Zugriff auf den Ressourcen-Planer und dessen Verwendung erfüllt sind, bevor Sie mit der Verwendung beginnen. Auf diese Weise stellen Sie sicher, dass der Ressourcen-Planer die richtigen Informationen anzeigt, bevor Sie mit der Budgetierung Ihrer Ressourcen beginnen.

Informationen zu den Voraussetzungen für den Ressourcenplaner finden Sie unter [Erste Schritte mit der Ressourcenplanung](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## Suchen Sie den Ressourcen-Planer .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this was moved from the get-started-resource-planner article)</p>
-->

Sie können den Ressourcenplaner in zwei Bereichen von Workfront finden, je nachdem, ob Sie Ihre Ressourcen für mehrere Projekte oder nur für ein Projekt einsetzen möchten.

* [Verwenden Sie den Ressourcenplaner für mehrere Projekte](#use-the-resource-planner-for-multiple-projects)
* [Verwenden des Ressourcen-Planers für ein Projekt](#use-the-resource-planner-for-one-project)

### Verwenden des Ressourcen-Planers für mehrere Projekte {#use-the-resource-planner-for-multiple-projects}

Wenn Sie den Ressourcenplaner für mehrere Projekte verwenden, stellen die Zuordnungsnummern für Ihre Ressourcen Zahlen für mehrere Projekte dar.

So greifen Sie auf den Abschnitt &quot;Planer&quot;im Bereich &quot;Ressourcen&quot;zu:

1. Klicken Sie oben rechts in Adobe Workfront auf das Symbol **Hauptmenü** ![](assets/main-menu-icon.png).

1. Klicken Sie auf **Ressourcen**. Der Planer wird standardmäßig angezeigt.  Weitere Informationen zu Budgeteinträgen im Ressourcenplaner finden Sie im Artikel [Budgetressourcen im Ressourcenplaner unter Verwendung der Projekt- und Rollenansichten](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   ![](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. Bewegen Sie den Mauszeiger über den linken Bereich und klicken Sie auf **Ressourcenpools**.\
   Informationen zum Erstellen von Ressourcen-Pools finden Sie unter [Erstellen von Ressourcen-Pools](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

### Verwenden des Ressourcen-Planers für ein Projekt {#use-the-resource-planner-for-one-project}

Wenn Sie den Ressourcenplaner für ein Projekt verwenden, stellen die Zuordnungsnummern für Ihre Ressourcen Zahlen für das ausgewählte Projekt dar.

1. Gehen Sie zu einem Projekt, für das Sie Ressourcen planen möchten.
1. Klicken Sie im linken Bereich auf **Geschäftsszenario** .
1. Scrollen Sie zum Abschnitt **Ressourcenbudgeting** des Geschäftsfalls.
1. Klicken Sie auf **Ressourcen-Budgetierung bearbeiten** , um Ressourcen-Pools zu Ihrem Projekt hinzuzufügen und mit der Budgetierung Ihrer Ressourcen zu beginnen.

   >[!TIP]
   >
   >Sie können einen Ressourcenpool nur im Bereich Ressourcenbudgetierung des Geschäftsfalls hinzufügen, wenn dem Projekt keine Ressourcenpools zugeordnet sind. Wenn das Projekt bereits über einen Ressourcen-Pool verfügt, werden die Benutzer im Pool und ihre Arbeitsplatzrollen standardmäßig im Bereich Ressourcenbudgetierung angezeigt.

   ![](assets/resource-budgeting-area-on-project-350x70.png)

   Informationen zu Budgeteinträgen für ein Projekt finden Sie im Artikel [Budgetressourcen im Geschäftsfall](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
