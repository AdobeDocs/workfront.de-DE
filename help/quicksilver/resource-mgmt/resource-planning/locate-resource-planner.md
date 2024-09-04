---
product-area: resource-management
navigation-topic: resource-planning
title: Suchen Sie den Ressourcen-Planer .
description: Sie können den Ressourcen-Planer verwenden, um die Zuweisung Ihrer Ressourcen zu Projekten zu verwalten. Sie können auf den Ressourcen-Planer für mehrere Projekte gleichzeitig oder für ein Projekt über den Geschäftsfallbereich des Projekts zugreifen.
author: Lisa
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Suchen Sie den Ressourcen-Planer .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

Sie können den Ressourcen-Planer verwenden, um die Zuweisung Ihrer Ressourcen zu Projekten zu verwalten. Sie können auf den Ressourcen-Planer für mehrere Projekte gleichzeitig oder für ein Projekt über den Geschäftsfallbereich des Projekts zugreifen.

## Zugriffsanforderungen

+++ Erweitern Sie , um die Zugriffsanforderungen für die Funktionalität in diesem Artikel anzuzeigen.

Sie müssen über folgenden Zugriff verfügen, um die Schritte in diesem Artikel ausführen zu können:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Abo</td> 
   <td><p>Neu: Beliebig</p>
       <p>oder</p>
       <p>Aktuell: Pro oder höher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-Lizenz</td> 
   <td><p>Neu: Licht oder höher;</br>
          Standard zum Suchen des Ressourcen-Planers im Hauptmenü</p>
       <p>oder</p>
       <p>Aktuell: Überprüfen oder höher;</br>
       Planen Sie, den Ressourcen-Planer im Hauptmenü zu finden.</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationen auf Zugriffsebene</td> 
   <td> <p>Zugriff oder höher auf die Ressourcenverwaltung anzeigen</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektberechtigungen</td> 
   <td> <p>Berechtigungen für Projekte und Benutzer anzeigen </p> </td> 
  </tr> 
 </tbody> 
</table>

Weitere Informationen zu den Informationen in dieser Tabelle finden Sie unter [Zugriffsanforderungen in der Workfront-Dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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

{{step1-to-resourcing}}

Der Planer wird standardmäßig angezeigt.  Weitere Informationen zu Budgeteinträgen im Ressourcenplaner finden Sie im Artikel [Budgetressourcen im Ressourcenplaner unter Verwendung der Projekt- und Rollenansichten](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

![](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. Klicken Sie im linken Bereich auf **Ressourcenpools** .
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
